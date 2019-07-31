---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な Securescorecontrolprofiles のプロパティを更新して、担当者または tenantNote などのさまざまなプロパティを変更します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3450422320cf1d80bdd4cfd2f7e67960c0bafdbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978052"
---
# <a name="update-securescorecontrolprofiles"></a>secureScoreControlProfiles の更新

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

任意の統合ソリューション内の編集可能な**securescorecontrolprofiles の**プロパティを更新して、**担当者**または**tenantnote**などのさまざまなプロパティを変更します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |   SecurityEvents。  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | ベアラー {code}。 必須です。|
|Prefer | 戻り値 = 表現。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。 次の表に、secureScoreControlProfile で更新できるフィールドを示します。 要求本文に含まれていない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|assignedTo|String|トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。|
|tenantNote|String|コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。|
|controlStateUpdates| String|コントロールに対するアナリスト主導の設定。 可能な値は、`ignore`、`thirdParty`、`reviewed` です。|


## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofiles.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

成功応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
