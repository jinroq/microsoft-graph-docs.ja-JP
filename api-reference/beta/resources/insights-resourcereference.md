---
title: resourceReference リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005724"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="94951-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94951-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94951-104">[Insights](officegraphinsights.md)のプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="94951-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="94951-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94951-105">JSON representation</span></span>

<span data-ttu-id="94951-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="94951-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="94951-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94951-107">Properties</span></span>

| <span data-ttu-id="94951-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94951-108">Property</span></span>      | <span data-ttu-id="94951-109">型</span><span class="sxs-lookup"><span data-stu-id="94951-109">Type</span></span>      | <span data-ttu-id="94951-110">説明</span><span class="sxs-lookup"><span data-stu-id="94951-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="94951-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="94951-111">webUrl</span></span>        | <span data-ttu-id="94951-112">String</span><span class="sxs-lookup"><span data-stu-id="94951-112">String</span></span>    | <span data-ttu-id="94951-113">参照されるアイテムにつながる URL。</span><span class="sxs-lookup"><span data-stu-id="94951-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="94951-114">id</span><span class="sxs-lookup"><span data-stu-id="94951-114">id</span></span>            | <span data-ttu-id="94951-115">文字列</span><span class="sxs-lookup"><span data-stu-id="94951-115">String</span></span>    | <span data-ttu-id="94951-116">アイテムの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="94951-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="94951-117">type</span><span class="sxs-lookup"><span data-stu-id="94951-117">type</span></span>          | <span data-ttu-id="94951-118">String</span><span class="sxs-lookup"><span data-stu-id="94951-118">String</span></span>    | <span data-ttu-id="94951-119">アイテムの分類に使用できる文字列値 ("microsoft....." など)</span><span class="sxs-lookup"><span data-stu-id="94951-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
