---
title: convertIdResult リソースの種類
description: TranslateExchangeIds 関数によって実行される ID 形式変換の結果。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 040b13ab83eacffb33e8903f7d11823adb6e1bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973205"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="8b8c4-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b8c4-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8c4-104">[TranslateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="8b8c4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b8c4-105">Properties</span></span>

| <span data-ttu-id="8b8c4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b8c4-106">Property</span></span> | <span data-ttu-id="8b8c4-107">型</span><span class="sxs-lookup"><span data-stu-id="8b8c4-107">Type</span></span> | <span data-ttu-id="8b8c4-108">説明</span><span class="sxs-lookup"><span data-stu-id="8b8c4-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8b8c4-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="8b8c4-109">sourceId</span></span> | <span data-ttu-id="8b8c4-110">String</span><span class="sxs-lookup"><span data-stu-id="8b8c4-110">String</span></span> | <span data-ttu-id="8b8c4-111">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-111">The identifier that was converted.</span></span> <span data-ttu-id="8b8c4-112">この値は、元の、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="8b8c4-113">targetId</span><span class="sxs-lookup"><span data-stu-id="8b8c4-113">targetId</span></span> | <span data-ttu-id="8b8c4-114">String</span><span class="sxs-lookup"><span data-stu-id="8b8c4-114">String</span></span> | <span data-ttu-id="8b8c4-115">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-115">The converted identifier.</span></span> <span data-ttu-id="8b8c4-116">変換が失敗した場合、この値は表示されません。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="8b8c4-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="8b8c4-117">errorDetails</span></span> | [<span data-ttu-id="8b8c4-118">genericError</span><span class="sxs-lookup"><span data-stu-id="8b8c4-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="8b8c4-119">変換エラーの理由を示す error オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="8b8c4-120">この値は、変換に成功した場合は表示されません。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b8c4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b8c4-121">JSON representation</span></span>

<span data-ttu-id="8b8c4-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b8c4-122">Here is a JSON representation of the resource.</span></span>

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
