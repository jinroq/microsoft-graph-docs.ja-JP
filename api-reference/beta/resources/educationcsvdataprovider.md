---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4dbbf5d5791df1035fcd9fe1a953d8a9a347070a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340582"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="a333a-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a333a-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a333a-104">CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="a333a-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="a333a-105">[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="a333a-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a333a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a333a-106">Properties</span></span>

| <span data-ttu-id="a333a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a333a-107">Property</span></span> | <span data-ttu-id="a333a-108">型</span><span class="sxs-lookup"><span data-stu-id="a333a-108">Type</span></span> | <span data-ttu-id="a333a-109">説明</span><span class="sxs-lookup"><span data-stu-id="a333a-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a333a-110">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="a333a-110">**customizations**</span></span> | [<span data-ttu-id="a333a-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="a333a-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="a333a-112">同期プロファイルに適用されるオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="a333a-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a333a-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a333a-113">JSON representation</span></span>

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
