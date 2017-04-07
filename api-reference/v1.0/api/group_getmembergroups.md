# <a name="group-getmembergroups"></a>グループ: getMemberGroups
指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group_list_memberof.md) ナビゲーション プロパティの読み取りとは異なります。

この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター       | 型    |説明|
|:---------------|:--------|:----------|
|securityEnabledOnly|Boolean|**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。|

## <a name="response"></a>応答
成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200, OK` 応答コードと文字列コレクションを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
