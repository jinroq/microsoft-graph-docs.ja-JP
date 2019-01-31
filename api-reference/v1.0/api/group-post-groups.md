---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574867"
---
# <a name="create-group"></a>グループを作成する
この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。

* Office 365 グループ (統合グループ)
* 動的グループ
* セキュリティ グループ

この操作は既定で各グループのプロパティのサブセットのみを返します。 これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。

既定で_返されない_プロパティを取得するには、GET 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。 [例](group-get.md#request-2)を参照してください。

> **注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。 

| プロパティ | 型 | 説明|
|:---------------|:--------|:----------|
| displayName | string | アドレス帳に表示するグループの名前。 必須です。 |
| mailEnabled | boolean | メールが有効なグループの場合は、**true** に設定します。 Office 365 グループを作成する場合は、これを **true** に設定します。 動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。 必須です。 |
| mailNickname | string | グループのメール エイリアス。 必須です。 |
| securityEnabled | ブール値 | セキュリティが有効なグループの場合は、**true** に設定します。 動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。 Office 365 グループを作成する場合は、これを **false** に設定します。 必須です。 |
| owners | string collection | このプロパティは、作成時のグループの所有者を表します。 省略可能。 |
| members | string collection | このプロパティは、作成時のグループのメンバーを表します。 省略可能。 |


Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。

### <a name="grouptypes-options"></a>groupTypes オプション

| グループの種類 | **groupTypes** プロパティ |
|:--------------|:------------------------|
| Office 365 (統合グループともいいます)| "Unified" |
| Dynamic | "DynamicMembership" |
| Security | 設定しない。 |


>**注:** ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。  この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。  

グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティを参照してください。

## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。 応答には、そのグループの既定のプロパティのみが含まれます。

## <a name="example"></a>例
#### <a name="request-1"></a>要求 1
最初の要求例では、Office 365 グループを作成しています。
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
>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しからは、すべての既定のプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a>要求 2
2 つ目の要求例では、所有者とメンバーを指定して Office 365 グループを作成しています。
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
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
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a>応答 2
成功応答の例を次に示します。 既定のプロパティのみが含まれています。 その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。 
>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しからは、すべての既定のプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
