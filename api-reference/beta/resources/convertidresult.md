---
title: convertIdResult リソースの種類
description: translateExchangeIds 関数によって実行される ID 形式変換の結果。
localization_priority: Normal
ms.openlocfilehash: 5981f75ee071777f9119d0db2c0078153a160180
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341041"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="ab79e-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab79e-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab79e-104">[translateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果。</span><span class="sxs-lookup"><span data-stu-id="ab79e-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="ab79e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab79e-105">Properties</span></span>

| <span data-ttu-id="ab79e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab79e-106">Property</span></span> | <span data-ttu-id="ab79e-107">型</span><span class="sxs-lookup"><span data-stu-id="ab79e-107">Type</span></span> | <span data-ttu-id="ab79e-108">説明</span><span class="sxs-lookup"><span data-stu-id="ab79e-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ab79e-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="ab79e-109">sourceId</span></span> | <span data-ttu-id="ab79e-110">String</span><span class="sxs-lookup"><span data-stu-id="ab79e-110">String</span></span> | <span data-ttu-id="ab79e-111">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="ab79e-111">The identifier that was converted.</span></span> <span data-ttu-id="ab79e-112">この値は、元の、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="ab79e-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="ab79e-113">targetId</span><span class="sxs-lookup"><span data-stu-id="ab79e-113">targetId</span></span> | <span data-ttu-id="ab79e-114">String</span><span class="sxs-lookup"><span data-stu-id="ab79e-114">String</span></span> | <span data-ttu-id="ab79e-115">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="ab79e-115">The converted identifier.</span></span> <span data-ttu-id="ab79e-116">変換が失敗した場合、この値は表示されません。</span><span class="sxs-lookup"><span data-stu-id="ab79e-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="ab79e-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="ab79e-117">errorDetails</span></span> | [<span data-ttu-id="ab79e-118">genericerror</span><span class="sxs-lookup"><span data-stu-id="ab79e-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="ab79e-119">変換エラーの理由を示す error オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="ab79e-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="ab79e-120">この値は、変換に成功した場合は表示されません。</span><span class="sxs-lookup"><span data-stu-id="ab79e-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab79e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab79e-121">JSON representation</span></span>

<span data-ttu-id="ab79e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab79e-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
