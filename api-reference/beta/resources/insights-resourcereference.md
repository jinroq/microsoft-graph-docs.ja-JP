---
title: resourceReference リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340003"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d9ff9-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9ff9-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ff9-104">[insights](officegraphinsights.md)のプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="d9ff9-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9ff9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9ff9-105">JSON representation</span></span>

<span data-ttu-id="d9ff9-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d9ff9-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="d9ff9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9ff9-107">Properties</span></span>

| <span data-ttu-id="d9ff9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9ff9-108">Property</span></span>      | <span data-ttu-id="d9ff9-109">型</span><span class="sxs-lookup"><span data-stu-id="d9ff9-109">Type</span></span>      | <span data-ttu-id="d9ff9-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9ff9-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d9ff9-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="d9ff9-111">webUrl</span></span>        | <span data-ttu-id="d9ff9-112">String</span><span class="sxs-lookup"><span data-stu-id="d9ff9-112">String</span></span>    | <span data-ttu-id="d9ff9-113">参照されるアイテムにつながる URL。</span><span class="sxs-lookup"><span data-stu-id="d9ff9-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d9ff9-114">id</span><span class="sxs-lookup"><span data-stu-id="d9ff9-114">id</span></span>            | <span data-ttu-id="d9ff9-115">String</span><span class="sxs-lookup"><span data-stu-id="d9ff9-115">String</span></span>    | <span data-ttu-id="d9ff9-116">アイテムの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="d9ff9-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d9ff9-117">type</span><span class="sxs-lookup"><span data-stu-id="d9ff9-117">type</span></span>          | <span data-ttu-id="d9ff9-118">String</span><span class="sxs-lookup"><span data-stu-id="d9ff9-118">String</span></span>    | <span data-ttu-id="d9ff9-119">アイテムの分類に使用できる文字列値 ("microsoft....." など)</span><span class="sxs-lookup"><span data-stu-id="d9ff9-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
