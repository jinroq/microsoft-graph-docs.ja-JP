---
title: internetMessageHeader リソースの種類
description: '提供する、RFC5322 で定義されている、インターネット メッセージのヘッダーを表すキーと値のペア '
localization_priority: Normal
ms.openlocfilehash: e748e6badd3e6bad6adb02a9df46a40a7241d636
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511668"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[RFC5322](https://www.ietf.org/rfc/rfc5322.txt) によって定義された、インターネット メッセージ ヘッダーを表すキーと値のペア。メッセージが送信者から受信者に到達するまでに辿ったネットワーク パスの詳細を説明します。 

インターネット メッセージ ヘッダーの例については、「[View e-mail message headers (電子メールのメッセージ ヘッダーを表示する)](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)」を参照してください。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|string|キーと値のペアの、キーの部分を表します。|
|value|string|キーと値のペアの、値の部分を表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/internetmessageheader.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
