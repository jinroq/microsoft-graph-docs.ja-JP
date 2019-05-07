---
title: 契約を作成する
description: 新しいアグリーメントオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 47f5c6572192f08dbbd3f954f9dd30678269c8e0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636591"
---
# <a name="create-agreement"></a>契約を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

新しい[アグリーメント](../resources/agreement.md)オブジェクトを作成します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | Agreement.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、[アグリーメント](../resources/agreement.md)オブジェクトの JSON 表記を指定します。

次の表に、ユーザーの作成時に必要になるプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|アグリーメントの表示名。|
|isViewingBeforeAcceptanceRequired|Boolean|ユーザーが同意する前に、契約を展開して表示する必要があるかどうかを示します。|
|ファイル/ファイル名|String|アグリーメントファイルの名前 (たとえば、「お持ちの形式」)。|
|ファイル/isDefault|Boolean|クライアントの優先度に一致するカルチャがない場合に、これが既定のアグリーメントファイルであるかどうかを示します。 ファイルが既定として設定されていない場合は、最初のファイルが既定として扱われます。|
|ファイル/言語|String|Languagecode2-country/regioncode2 という形式の、アグリーメントファイルのカルチャ。 languagecode2 は、ISO 639-1 から派生した、小文字の2文字のコードです。 country/regioncode2 は ISO 3166 から派生し、通常は2つの大文字または BCP-47 language タグ (例: en-us) で構成されます。|
|ファイル/fileData/データ|Binary|PDF ドキュメントの使用条件を表すデータ。|

## <a name="response"></a>応答
成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求本文で、[アグリーメント](../resources/agreement.md)オブジェクトの JSON 表記を指定します。

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/create_agreement_from_agreements-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_agreement_from_agreements-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
