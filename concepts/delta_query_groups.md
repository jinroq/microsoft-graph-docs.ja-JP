# <a name="get-incremental-changes-for-groups-preview"></a>グループに対する増分の変更を取得する (プレビュー)

[デルタ クエリ](./delta_query_overview.md)では、一連の[デルタ](../api-reference/beta/api/group_delta.md)関数呼び出しを使用して、グループへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からグループのセット全体をフェッチして、変更を比較せずに、グループへの変更を検出できます。

デルタ クエリでは、テナント内のすべてのグループを取得する完全な同期と、最後の同期以降に変更されたグループのみを取得する増分同期の両方がサポートされています。通常は、テナント内のすべてのグループの最初の完全同期を実行して、その後、グループへの増分の変更を定期的に取得します。 

## <a name="tracking-group-changes"></a>グループ変更の追跡

グループ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。GET 要求は、次を含めることを除き、[グループの一覧表示](../api-reference/beta/api/group_list.md)とほぼ同じ方法で実行します。

- **デルタ**関数。
- 以前の GET **デルタ**関数呼び出しからの[状態トークン](./delta_query_overview.md) (_deltaToken_ または _skipToken_)。

## <a name="example"></a>例

次の例は、グループへの変更を追跡するための一連の要求を示しています。

1. [最初の要求](#initial-request)と[応答](#initial-response)
2. [nextLink 要求](#nextlink-request)と[応答](#nextlink-response)
3. [最後の nextLink 要求](#final-nextlink-request)と[応答](#final-nextlink-response)
4. [deltaLink 要求](#deltalink-request)と [deltaLink 応答](#deltalink-response)

## <a name="initial-request"></a>最初の要求

グループ リソースの変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。 

以下の点に注意してください。

- オプションの $Select クエリ パラメーターは、クエリ パラメーターが将来の要求に自動的に含まれる方法をデモンストレーションする要求に含まれています。
- 最初の要求には、状態トークンは含まれません。状態トークンはそれ以降の要求で使用されます。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description
```

### <a name="initial-response"></a>最初の応答

成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で[グループ](../api-reference/beta/resources/group.md) コレクション オブジェクトを返します。グループのセット全体が大きすぎると仮定した場合、応答には nextLink 状態トークンも含まれます。

この例では、セッションで取得するデータの追加ページがあることを示す nextLink URL が返されます。最初の要求からの $select クエリ パラメーターは、nextLink URL にエンコードされます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink 要求

2 番目の要求は、前の応答から返された `skipToken` を指定します。`$select` パラメーターは、`skipToken` によってエンコードされ含まれるため必須ではないことに注意してください。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink 応答

応答には `nextLink` および `skipToken` が含まれ、利用可能な他のグループがあることを示しています。deltaLink URL が応答で返されるまで、nextLink URL を使用して要求を実行し続けます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最後の nextLink 要求

3 番目の要求は、最後の同期要求から返された最新の `skipToken` を引き続き使用します。 

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>最後の nextLink 応答

deltaLink URL が返されると、返されるリソースの既存の状態に関するデータはなくなります。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点について説明します。`deltaToken` を保存して、グループへの変更を検出するために要求 URL で使用します。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink 要求

[最後の応答](#final-nextlink-response)からの `deltaToken` を使用すると、最後の要求以降に (追加、削除、または更新によって) 変更されたグループを取得できます。

``` http
GET https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink 応答

変更が行われなかった場合は、結果のない同じ `deltatoken` が返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

変更が行われた場合は、変更されたグループのコレクションを含み、同じ `deltatoken` が返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a>関連項目
[Microsoft Graph デルタ クエリ](../concepts/delta_query_overview.md)の概要。