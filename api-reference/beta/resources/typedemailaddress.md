---
title: typedEmailAddress リソースの種類
description: 名前、電子メール アドレス、および連絡先の対応する電子メール アドレス タイプを表します。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510709"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

名前、電子メール アドレス、および、対応する電子メール アドレスの種類[にお問い合わせください](contact.md)を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|String|連絡先の電子メール アドレスです。|
|name|String|連絡先の表示名。|
|type |String |電子メール アドレスの種類。 可能な値は、`unknown`、`work`、`personal`、`main`、`other` です。 既定値は、 `unknown`、つまり、**アドレス**が設定されていない特定の種類として。 |
|otherLabel |String  |電子メール アドレスのカスタムの型を指定する**の種類**を設定`other`、 **otherLabel**を独自の文字列を割り当てるとします。 など、ボランティア活動の特定の電子メール アドレスを使用する場合があります。 **タイプ**を設定`other`、 **otherLabel**を次のように独自の文字列を設定して`Volunteer work`。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
