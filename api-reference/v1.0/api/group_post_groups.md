# <a name="create-group"></a>グループを作成する
この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。

* Office 365 グループ (統合グループ)
* 動的グループ
* セキュリティ グループ

> **注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| 承認  | 文字列  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
次の表は、グループ作成時に指定する [group](../resources/group.md) リソースのプロパティを示します。 

| プロパティ | タイプ | 説明|
|:---------------|:--------|:----------|
| displayName | 文字列 | アドレス帳に表示するグループの名前。 必須。 |
| mailEnabled | ブール値 | メールが有効なグループの場合は、**true** に設定します。 Office 365 グループを作成する場合は、**true** に設定します。 動的グループまたはセキュリティ グループを作成する場合は、**false** に設定します。 必須。 |
| mailNickname | 文字列 | グループの電子メール エイリアス。 必須。 |
| securityEnabled | ブール値 | セキュリティが有効なグループの場合は、**  true** を設定します。 動的グループまたはセキュリティ グループを作成する場合は、**true** に設定します。 Office 365 グループを作成する場合は、**true** に設定します。 必須。 |
| owners | 文字列コレクション | このプロパティは、作成時のグループの所有者を表します。 省略可能。 |
| メンバー | 文字列コレクション | このプロパティは、作成時のグループのメンバーを表します。 省略可能。 |


Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。

### <a name="grouptypes-options"></a>groupTypes オプション

| グループの種類 | **groupTypes** プロパティ |
|:--------------|:------------------------|
| Office 365 (統合グループともいいます)| "Unified" |
| 動的 | "DynamicMembership" |
| セキュリティ | 設定しない。 |


>**注:** ユーザー コンテキストおよび所有者を指定せずにプログラムで Office 365 グループを作成すると、匿名のグループが作成されます。  これを行うと、関連する SharePoint Online サイトは手動操作が行なわれるまで自動的に作成されなくなります。  

グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティを参照してください。

## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。

## <a name="example"></a>例
#### <a name="request-1"></a>要求 1
最初の例は、Office 365 グループの作成を要求するものです。
<!-- {
  "blockType": "request",
  "name": "create_group"
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

#### <a name="response-1"></a>応答 1
応答の例を次に示します。
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
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

#### <a name="request-2"></a>要求 2
2 番目の例は、指定した所有者で Office 365 グループの作成を要求するものです。
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>応答 2
成功した応答の例を次に示します。
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
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
