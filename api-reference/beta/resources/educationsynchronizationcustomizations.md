---
title: educationSynchronizationCustomizations リソースの種類
description: 同期するエンティティのリストと、そのカスタマイズがあればそれを含みます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543204"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期するエンティティのリストと、その[カスタマイズ](educationsynchronizationcustomization.md)があればそれを含みます。

> **注:** 同期するプロパティのカスタマイズは、 **studentEnrollment**エンティティおよび**teacherRoster**エンティティには適用されません。

このリソースは、次のデータプロバイダーのメンバーです。

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **筆記** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学校エンティティのカスタマイズ。        |
| **セクション** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  セクションエンティティのカスタマイズ。         |
| **学生** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学生エンティティのカスタマイズ。         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  教師エンティティのカスタマイズ。         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学生登録のカスタマイズ。           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       教師名簿のカスタマイズ。    |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
