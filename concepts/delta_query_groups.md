# <a name="get-incremental-changes-for-groups"></a>グループに対する増分の変更を取得する

[デルタ クエリ](./delta_query_overview.md)では、一連の[デルタ](../api-reference/v1.0/api/group_delta.md)関数呼び出しを使用して、グループへの追加、削除、または更新に対してクエリを実行できます。デルタ クエリを使用すると、Microsoft Graph からグループのセット全体をフェッチして、変更を比較せずに、グループへの変更を検出できます。

同期するグループとローカル プロファイル ストアを使用するクライアントは、最初の完全同期とその後の増分同期の両方でデルタ クエリを使用できます。通常なら、クライアントはテナント内のすべてのグループの最初の完全同期を実行し、その後、グループへの増分の変更を定期的に取得します。

## <a name="tracking-group-changes"></a>グループ変更の追跡

グループ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。GET 要求は、次を含めることを除き、[グループの一覧表示](../api-reference/v1.0/api/group_list.md)とほぼ同じ方法で実行します。

- **デルタ**関数。
- 以前の GET **デルタ**関数呼び出しからの[状態トークン](./delta_query_overview.md) (*deltaToken* または *skipToken*)。

## <a name="example"></a>例

次の例は、グループへの変更を追跡するための一連の要求を示しています。

1. [最初の要求](#initial-request)と[応答](#initial-response)
2. [nextLink 要求](#nextlink-request)と[応答](#nextlink-response)
3. [最後の nextLink 要求](#final-nextlink-request)と[応答](#final-nextlink-response)
4. [deltaLink 要求](#deltalink-request)と [deltaLink 応答](#deltalink-response)

## <a name="initial-request"></a>最初の要求

グループ リソースの変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。

以下の点に注意してください。

- オプションの `$select` クエリ パラメーターが要求に含められているのは、クエリ パラメーターが将来の要求に自動的に含まれる方法を示すためです。
- オプションの `$expand` クエリ パラメーターが含められているのは、グループのメンバーをグループ オブジェクトと共に取り出す方法を示すためです。 それにより、グループのユーザーの追加や削除など、メンバーシップの変更を追跡できます。
- 最初の要求には、状態トークンは含まれません。状態トークンはそれ以降の要求で使用されます。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

## <a name="initial-response"></a>最初の応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../api-reference/v1.0/resources/group.md) コレクション オブジェクトを返します。 グループ セット全体が大きすぎて 1 つの応答では収まらない場合、状態トークンが含まれる `nextLink` も含められます。

この例の場合、`nextLink` が含められました。元の `$select` および `$expand` クエリ パラメーターは、状態トークンの中にエンコードされています。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**注:** 最初のグループ オブジェクト - TestGroup1 - には `members@delta` プロパティが含まれています。それにはグループの現在の 2 つのメンバーが含まれています。 TestGroup2 にはメンバーがないため、このグループにはそのプロパティが含まれていません。

## <a name="nextlink-request"></a>nextLink 要求

2 番目の要求では、前の応答の `nextLink` を使用しています。それには、`skipToken` が含まれています。 `$select` パラメーターと `$expand` パラメーターは、トークンの中にエンコードされているため、明示的には存在しないことに注意してください。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink 応答

応答には新たな `skipToken` 値を指定した別の `nextLink` が含まれています。これは、利用可能な他のグループがあることを示しています。 最後の応答で `deltaLink` URL が返されるまで、`nextLink` URL を使用して要求の発行を続けます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a>最後の nextLink 要求

3 番目の要求では、最新の `nextLink` を再び使用します。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>最後の nextLink 応答

最後に、`deltaLink` URL が返されます。これは、グループの既存の状態ではそれ以上のデータがないことを意味します。 アプリケーションは、その後の要求のため、`deltaLink` およびそれに含まれる `deltaToken` 値を使用して、グループに対する新たな変更について調べます。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
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

[最後の応答](#final-nextlink-response)の `deltaLink` を使用することにより、最後の要求以降にグループに対して加えられた、実質的な新たな変更を入手できます。 変更内容には、次のものが含まれます。
- 新たに作成されたグループ オブジェクト。
- 削除されたグループ オブジェクト。
- プロパティに変更が加えられたグループ オブジェクト (**displayName** が変更されたなど)。
- メンバー オブジェクトが追加または削除されたグループ オブジェクト。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink 応答

変更がなかった場合は、結果なしで `deltaLink` が返されます。`value` プロパティは空になります。 アプリケーションでは将来の呼び出しに備えて、以前のリンクを新しいリンクに必ず置き換えてください。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

変更があった場合は、変更されたグループのコレクションが含められます。 さらに応答には、`nextLink` (取得対象の変更のページが複数ある場合) と `deltaLink` のどちらかも含まれています。 `nextLinks` の後もそれまでと同じパターンを実装し、最後の `deltaLink` を将来の呼び出しに備えて保持しておいてください。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```
上記のサンプル応答に関する注意事項:
- オブジェクトは、当初 `$select` および `$expand` のクエリ パラメーターで指定されたのと同じプロパティ セットを伴って返されます。
- 変更されたプロパティと変更されていないプロパティの両方が含まれています。 上記の例の場合、`description` プロパティの値は新しいものになっていますが、`displayName` プロパティは変更されていません。
- `members@delta` には、メンバーシップに対して加えられた変更内容が含まれています。
  - リスト中の最初のユーザーが、メンバーシップを削除するか、またはユーザー オブジェクト自体を削除することにより、グループから削除されました。 `@removed` プロパティがそのことを記述しています。
  - 2 番目のユーザーはグループに追加されました。

## <a name="paging-through-members-in-a-large-group"></a>大規模グループ内のメンバー間のページング
`members@delta` プロパティは、`$select` クエリ パラメーターが指定されていない場合、または `$expand=members` パラメーターが明示的に指定されている場合、既定でグループ オブジェクトに含められます。 メンバー数の多いグループの場合、1 つの応答に全メンバーが収まらないことがあります。このセクションでは、そのような状況を処理するために実装しなければならないパターンについて説明します。

>**注:** このパターンは、グループ状態を最初に取得する際にも、それ以降にデルタ変更を取得するために呼び出す際にも適用されます。

グループの初期状態のすべてを取得するため、またはそれ以降にデルタ変更を取得するために、次のデータ クエリを実行しているとします。

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

1. Microsoft Graph は、`members@delta` プロパティに多くのメンバーが含まれる 1 つのグループ オブジェクトのみ含まれる応答を返すことがあります。

**最初のページ**

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. `nextLink` をたどる際、再び同じグループ オブジェクトが含まれる応答を受け取ることがあります。 同じプロパティ値が返されますが、展開された `members@delta` プロパティの内容は、異なるユーザー リストになっています。

**2 番目のページ**

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. このようにしてメンバー リスト全体が返され、他のグループが応答に出現し始めます。

このパターンを処理する際には、次のベスト プラクティスに従うことをお勧めします。
- 常に `nextLink` をたどり、各グループの状態をローカルでマージします。同じグループに関連する複数の応答を受信したなら、アプリケーションの中でその応答を使用してメンバーシップ リスト全体を作成します。
- 特定の応答シーケンスを前提にしないようにするのが最善です。 `nextLink` シーケンスのどこにでも同じグループが出現する可能性があると想定し、マージ ロジックの中でそれを処理します。


## <a name="see-also"></a>関連項目
[Microsoft Graph デルタ クエリ](../concepts/delta_query_overview.md)の概要。
