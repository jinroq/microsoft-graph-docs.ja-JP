---
title: convertIdResult リソースの種類
description: TranslateExchangeIds 関数によって実行される ID 形式変換の結果です。
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821456"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="a6fc8-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6fc8-103">convertIdResult resource type</span></span>

> <span data-ttu-id="a6fc8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6fc8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6fc8-106">[TranslateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果です。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="a6fc8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6fc8-107">Properties</span></span>

| <span data-ttu-id="a6fc8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6fc8-108">Property</span></span> | <span data-ttu-id="a6fc8-109">種類</span><span class="sxs-lookup"><span data-stu-id="a6fc8-109">Type</span></span> | <span data-ttu-id="a6fc8-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6fc8-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a6fc8-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="a6fc8-111">sourceId</span></span> | <span data-ttu-id="a6fc8-112">String</span><span class="sxs-lookup"><span data-stu-id="a6fc8-112">String</span></span> | <span data-ttu-id="a6fc8-113">変換された識別子です。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-113">The identifier that was converted.</span></span> <span data-ttu-id="a6fc8-114">この値は、元、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="a6fc8-115">targetId</span><span class="sxs-lookup"><span data-stu-id="a6fc8-115">targetId</span></span> | <span data-ttu-id="a6fc8-116">String</span><span class="sxs-lookup"><span data-stu-id="a6fc8-116">String</span></span> | <span data-ttu-id="a6fc8-117">変換後の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-117">The converted identifier.</span></span> <span data-ttu-id="a6fc8-118">この値は、変換が失敗した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="a6fc8-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="a6fc8-119">errorDetails</span></span> | [<span data-ttu-id="a6fc8-120">genericError</span><span class="sxs-lookup"><span data-stu-id="a6fc8-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="a6fc8-121">変換エラーの原因を示すエラー オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="a6fc8-122">この値は、変換が成功した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6fc8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6fc8-123">JSON representation</span></span>

<span data-ttu-id="a6fc8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6fc8-124">Here is a JSON representation of the resource.</span></span>

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
