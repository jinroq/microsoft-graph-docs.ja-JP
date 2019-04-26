---
title: educationSynchronizationCustomization リソースの種類
description: 'リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397f4d732bc25d086b2aeae6efc697d2048e6a03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334094"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 

>**注:****同期**開始プロパティは、 **StudentEnrollment**エンティティにのみ適用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | 文字列のコレクション |  同期するプロパティ名のコレクション。null に設定されている場合、すべてのプロパティが同期されます。       |
| **同期開始日** | DateTime |  同期を開始する日付を指定します。 この値は、将来の日付に設定する必要があります。 null に設定されている場合、プロファイルの設定が完了すると、リソースが同期されます。 **注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。      |
|**issyncdeferred** |Boolean | 親エンティティの同期を後日延期するかどうかを示します。 |
| **allowdisplaynameupdate** | Boolean |  同期によってリソースの表示名を上書きできるかどうかを示します。         |


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
