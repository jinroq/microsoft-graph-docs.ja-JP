---
title: 同期テンプレートの作成
description: 指定したアプリケーションの新しい同期テンプレートを作成します。
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536965"
---
# <a name="create-synchronizationtemplate"></a>同期テンプレートの作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したアプリケーションの新しい同期テンプレートを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。|
|アプリケーション                            |サポートされていません。| 

### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 型    | 説明|
|:---------------|:--------|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、作成する[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。 `id`、 `applicationId`および`factoryTag`プロパティは必須です。 テンプレートに`schema`何も指定されていない場合は、 `factoryTag`プロパティに関連付けられている既定のスキーマが使用されます。

### <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを返します。

### <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a>応答
応答の例を次に示します。
>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しでは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
