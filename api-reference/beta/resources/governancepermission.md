---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643784"
---
# <a name="governancepermission-resource-type"></a>governancePermission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。  


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accessLevel|String|アクセス レベルです。 有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。|
|isActive|Boolean|指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。|
|isEligible|Boolean|リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
