---
title: 契約書を作成します。
description: 契約の新しいオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514426"
---
# <a name="create-agreement"></a>契約書を作成します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[契約](../resources/agreement.md)の新しいオブジェクトを作成します。
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
| Authorization | string | ベアラー トークン 必須です。 |

## <a name="request-body"></a>要求本文
要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。

次の表に、ユーザーの作成時に必要になるプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|契約書の名前を表示します。|
|isViewingBeforeAcceptanceRequired|ブール値|ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。|
|ファイルまたはファイル名|String|契約ファイル (TOU.pdf など) の名前です。|
|ファイル/isDefault|ブール値|クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。 ファイルの [なし] は、既定として設定された、1 つ目は既定値として扱われます。|
|ファイルと言語|String|形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。 languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。 国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。|
|ファイル、構造体、データ fileData|Binary|PDF ドキュメントの使用条件を表すデータです。|

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、 `201, Created` 、応答の本体で応答コードおよび[契約](../resources/agreement.md)のオブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。

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
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
