---
title: educationSynchronizationCustomization リソースの種類
description: 'リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46cd20bbe016110a313d5b195a518ef81ca05afe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972454"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 

>**注:****同期**開始プロパティは、 **StudentEnrollment**エンティティにのみ適用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | 文字列のコレクション |  同期するプロパティ名のコレクション。Null に設定されている場合、すべてのプロパティが同期されます。       |
| **同期開始日** | DateTime |  同期を開始する日付を指定します。 この値は、将来の日付に設定する必要があります。 Null に設定されている場合、プロファイルの設定が完了すると、リソースが同期されます。 **注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。      |
|**isSyncDeferred** |Boolean | 親エンティティの同期を後日延期するかどうかを示します。 |
| **allowDisplayNameUpdate** | Boolean |  同期によってリソースの表示名を上書きできるかどうかを示します。         |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
