---
title: educationSynchronizationCustomizations リソースの種類
description: 存在する場合は、同期と、カスタマイズするエンティティの一覧に含まれています。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 3254915887afc1e6b0da0b3b6c44b59689219ab1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918190"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

存在する場合は、同期を[カスタマイズ](educationsynchronizationcustomization.md)して、エンティティの一覧に含まれています。

> **注:** 同期プロパティのカスタマイズは、 **studentEnrollment**と**teacherRoster**のエンティティには適用されません。

このリソースは、次のデータ プロバイダーのメンバーです。

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **学校** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学校のエンティティのカスタマイズです。        |
| **セクション** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  セクション エンティティをカスタマイズします。         |
| **受講者用** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  受講者用のエンティティのカスタマイズです。         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  先生のエンティティのカスタマイズです。         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  受講者の登録用にカスタマイズします。           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       教師名簿をカスタマイズします。    |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
