# <a name="list-deleted-items-owned-by-a-user"></a>**ユーザーによって所有されている削除済みのアイテムをリスト表示します。**

指定されたユーザーによって所有されている、最近削除したアイテムのリストを取得します。  

現在、削除済みアイテムのリスト表示機能は、ユーザーによって所有されている [グループ化](../resources/group.md) 参照資料に対してのみサポートされています。

これは、サービスの操作です。つまり、改ページ位置の自動修正はサポートしません。  API は、ID で分別された、ユーザーが所有する最大 1,000 の削除済みオブジェクトを返還します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
| --- | --- |
| 委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) |  サポートされていません。 |
| アプリケーション | Group.Read.All、Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP 要求

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明               |
| ------------- | ------------------------- |
| 承認 | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

要求本文には、次のパラメーターが必要です。

| パラメーター    | 型 |説明|
|:---------------|:--------|:----------|
|ユーザーID|文字列|所有者の ID です。|
|活字|文字列|返還用所有オブジェクトの種類； `Group` は、現在サポートされている唯一の値です。|


## <a name="response"></a>応答

成功した要求の返答 `200 OK` 応答コードです。応答オブジェクトには、 [ディレクトリ (削除済みアイテム)](../resources/directory.md) のプロパティが含まれています。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>応答

以下は、応答の例です。 注: この応答オブジェクトは簡潔にするために短縮されている場合があります。 サポートされているすべてのプロパティは、実際の呼び出しから返還されます。

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


