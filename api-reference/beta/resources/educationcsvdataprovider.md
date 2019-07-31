---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f515744f5206ea132531373e3df317e02dd6cbb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006403"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **ユーザー** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルに適用されるオプションのカスタマイズ。|

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
