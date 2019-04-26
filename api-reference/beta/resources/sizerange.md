---
title: sizeRange リソースの種類
description: '条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。'
localization_priority: Normal
ms.openlocfilehash: c2a37c91c968eddffc4aca0c8cf783e5aac1f3eb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343008"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="91e7d-103">sizeRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91e7d-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91e7d-104">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。</span><span class="sxs-lookup"><span data-stu-id="91e7d-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="91e7d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e7d-105">Properties</span></span>
| <span data-ttu-id="91e7d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e7d-106">Property</span></span>     | <span data-ttu-id="91e7d-107">型</span><span class="sxs-lookup"><span data-stu-id="91e7d-107">Type</span></span>   |<span data-ttu-id="91e7d-108">説明</span><span class="sxs-lookup"><span data-stu-id="91e7d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91e7d-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="91e7d-109">maximumSize</span></span> | <span data-ttu-id="91e7d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="91e7d-110">Int32</span></span> | <span data-ttu-id="91e7d-111">条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="91e7d-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="91e7d-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="91e7d-112">minimumSize</span></span> | <span data-ttu-id="91e7d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="91e7d-113">Int32</span></span> | <span data-ttu-id="91e7d-114">条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="91e7d-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="91e7d-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91e7d-115">JSON representation</span></span>
<span data-ttu-id="91e7d-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91e7d-116">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
