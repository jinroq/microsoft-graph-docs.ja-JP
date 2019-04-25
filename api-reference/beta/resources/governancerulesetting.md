---
title: governanceRuleSetting リソースの種類
description: ロール設定が構成されているルールを表します。
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547460"
---
# <a name="governancerulesetting-resource-type"></a>governanceRuleSetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ロール設定が構成されているルールを表します。


## <a name="properties"></a>プロパティ
|プロパティ      | 型         |説明|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |ルールの id。 たとえば、 ``ExpirationRule``と``MfaRule``のようになります。|
|setting       |String        |ルールの設定。 この値は、Parameter_Name: Parameter_Value という形式のペアのリストを含む JSON 文字列です。 たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` のように指定します。|

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
