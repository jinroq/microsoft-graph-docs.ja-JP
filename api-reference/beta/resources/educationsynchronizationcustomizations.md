---
title: educationSynchronizationCustomizations リソースの種類
description: 同期するエンティティのリストと、そのカスタマイズがあればそれを含みます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972440"
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
