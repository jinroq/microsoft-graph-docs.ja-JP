---
title: governanceRuleSetting リソースの種類
description: ロールの設定で構成されたルールを表します。
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522239"
---
# <a name="governancerulesetting-resource-type"></a>governanceRuleSetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ロールの設定で構成されたルールを表します。


## <a name="properties"></a>プロパティ
|プロパティ      | 型         |説明|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |ルールの id です。 たとえば、``ExpirationRule``と``MfaRule``。|
|setting       |String        |ルールの設定をします。 値は、Parameter_Name:Parameter_Value の形式でのペアの一覧を JSON 文字列です。 たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` のように指定します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
