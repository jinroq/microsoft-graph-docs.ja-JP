---
title: グループ設定を作成する
description: この API を使用して、groupSettingTemplates で利用可能なテンプレートに基づいて新しい設定を作成します。 これらの設定は、テナントレベルまたはグループレベルで行うことができます。 作成要求では、テンプレートで定義されているすべての設定の settingValues を指定する必要があります。 グループ固有の設定では、グループのメンバーがゲストユーザーを招待できるかどうかを制御する設定のみが可能です。 これは、グループにゲストユーザーを追加する機能が一般に利用可能になったときに、この動作を制御します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59fd97fad1aae4a17d213d882866a1b6bd749594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447398"
---
# <a name="create-a-group-setting"></a>グループ設定を作成する

この API を使用して、[groupSettingTemplates](../resources/groupsettingtemplate.md) で使用可能なテンプレートに基づいて新しい設定を作成します。これらの設定は、テナント レベルまたはグループ レベルで行うことができます。作成要求は、テンプレートに定義されているすべての設定の [settingValues](../resources/settingvalue.md) を提供する必要があります。グループ固有の設定では、グループのメンバーがゲスト ユーザーを招待できるかどうかの管理のみが設定できます。グループにゲスト ユーザーを追加する機能が一般的に利用可能になると、上記の動作は制御されます。

テンプレートと、それらが v2.0 でサポートするプロパティの一覧については、 [Groupsettingtemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)を使用してください (ベータ版エンドポイントの場合は、Call [directorysettingtemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta))。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type | application/json |

## <a name="request-body"></a>要求本文
要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。ただし、設定の表示名は、参照される設定テンプレート名に基づいて設定されます。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
