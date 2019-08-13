---
title: グループを作成する
description: 新しい Office 365 グループまたはセキュリティ グループを作成してください。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f0bbd5d242936e01c61a13f7e81ff46bf6270e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323263"
---
# <a name="create-group"></a>グループを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

要求本文で指定した新しい[グループ](../resources/group.md)を作成します。 以下のいずれかのグループを作成できます:

* Office 365 グループ (統合グループ)
* セキュリティ グループ

この操作は既定で各グループのプロパティのサブセットのみを返します。 これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。 既定で_返されない_プロパティを取得するには、[GET 操作](group-get.md)を実行し、`$select` OData クエリ オプションでプロパティを指定します。

>**注:** [チーム](../resources/team.md)を作成するには、まずグループを作成し、それからそのグループにチームを追加します。[チームの作成](../api/team-put-teams.md)に関するページを参照してください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。 

| プロパティ | 型 | 説明|
|:---------------|:--------|:----------|
| displayName | string | アドレス帳に表示するグループの名前。 必須です。 |
| mailEnabled | boolean | メールが有効なグループの場合は、**true** に設定します。 必須。 |
| mailNickname | string | グループのメール エイリアス。 必須です。 |
| securityEnabled | ブール値 | Office 365 グループを含む、セキュリティが有効なグループに **true** を設定します。 必須。 |
| owners | [directoryObject](../resources/directoryobject.md) コレクション | このプロパティは、作成時のグループの所有者を表します。 省略可能。 |
| members | [directoryObject](../resources/directoryobject.md) コレクション | このプロパティは、作成時のグループのメンバーを表します。 省略可能。 |

> **注**: Microsoft Azure portal を使用して作成されるグループでは、**securityEnabled** は最初は常に `true` に設定されます。

**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにグループに追加することができます。

>**注:** アプリ専用コンテキストを使用し、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。 この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。  

グループの必要に応じて他の書き込み可能なプロパティを指定します。 詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。

### <a name="grouptypes-options"></a>groupTypes オプション

示すように、**groupTypes** プロパティを使用し、グループの種類とグループのメンバーシップを管理します:

| グループの種類 | 割り当て済みのメンバーシップ | 動的メンバーシップ |
|:--------------|:------------------------|:---------------|
| Office 365 (統合グループともいいます)| `["Unified"]` | `["Unified","DynamicMembership"]`
| Dynamic | `[]` (_null_) | `["DynamicMembership"]`|

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。 応答には、そのグループの既定のプロパティのみが含まれます。

## <a name="examples"></a>例

### <a name="example-1-create-an-office-365-group"></a>例 1: Office 365 グループを作成する

次の例では、Office 365 グループを作成します。

#### <a name="request"></a>要求


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答

応答の例を次に示します。

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しからは、すべての既定のプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a>例 2: 所有者とメンバーを指定して Office 365 グループを作成する

次の例では、所有者とメンバーを指定して Office 365 グループを作成しています。

#### <a name="request"></a>要求


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答 

成功応答の例を次に示します。 既定のプロパティのみが含まれています。 その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しからは、すべての既定のプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
