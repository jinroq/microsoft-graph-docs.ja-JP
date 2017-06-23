# <a name="create-group"></a>グループを作成する

この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。

* Office 365 グループ (統合グループ)
* 動的グループ
* セキュリティ グループ

> **注**:Microsoft Teams は Office 365 グループでビルドされますが、この API を使用してチームを作成することは現在できません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下の**スコープ**が必要です。_Group.ReadWrite.All_ 
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
次の表は、グループを作成するときに最低限指定する必要のある [group](../resources/group.md) リソースのプロパティを示しています。 

| プロパティ | 型 | 説明|
|:---------------|:--------|:----------|
| displayName | string | アドレス帳に表示するグループの名前。 |
| mailEnabled | boolean | メールが有効なグループの場合は、**true** に設定します。Office 365 グループを作成する場合は、これを **true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。|
| mailNickname | string | グループの電子メール エイリアス。 |
| securityEnabled | boolean | セキュリティが有効なグループの場合は、**true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。Office 365 グループを作成する場合は、これを **false** に設定します。 |

Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。

| グループの種類 | **groupTypes** プロパティ |
|:--------------|:------------------------|
| Office 365 (統合グループともいいます)| "Unified" | 
| Dynamic | "DynamicMembership" | 
| Security | 設定しない。 | 

グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。

## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
これは、Office 365 グループを作成する要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは、さらに多くのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
