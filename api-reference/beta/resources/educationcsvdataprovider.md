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
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="0e6a3-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e6a3-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e6a3-104">CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e6a3-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="0e6a3-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="0e6a3-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0e6a3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e6a3-106">Properties</span></span>

| <span data-ttu-id="0e6a3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e6a3-107">Property</span></span> | <span data-ttu-id="0e6a3-108">型</span><span class="sxs-lookup"><span data-stu-id="0e6a3-108">Type</span></span> | <span data-ttu-id="0e6a3-109">説明</span><span class="sxs-lookup"><span data-stu-id="0e6a3-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0e6a3-110">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="0e6a3-110">**customizations**</span></span> | [<span data-ttu-id="0e6a3-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="0e6a3-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="0e6a3-112">同期プロファイルに適用されるオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="0e6a3-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e6a3-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e6a3-113">JSON representation</span></span>

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
