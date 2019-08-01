---
title: sizeRange リソースの種類
description: '条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e9c174216508679373c607dc9a2acd95df9096c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034147"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="7de22-103">sizeRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7de22-103">sizeRange resource type</span></span>


<span data-ttu-id="7de22-104">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。</span><span class="sxs-lookup"><span data-stu-id="7de22-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="7de22-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de22-105">Properties</span></span>
| <span data-ttu-id="7de22-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de22-106">Property</span></span>     | <span data-ttu-id="7de22-107">型</span><span class="sxs-lookup"><span data-stu-id="7de22-107">Type</span></span>   |<span data-ttu-id="7de22-108">説明</span><span class="sxs-lookup"><span data-stu-id="7de22-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7de22-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="7de22-109">maximumSize</span></span> | <span data-ttu-id="7de22-110">Int32</span><span class="sxs-lookup"><span data-stu-id="7de22-110">Int32</span></span> | <span data-ttu-id="7de22-111">条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="7de22-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="7de22-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="7de22-112">minimumSize</span></span> | <span data-ttu-id="7de22-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7de22-113">Int32</span></span> | <span data-ttu-id="7de22-114">条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="7de22-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7de22-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7de22-115">JSON representation</span></span>
<span data-ttu-id="7de22-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7de22-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
