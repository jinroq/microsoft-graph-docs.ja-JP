---
title: sizeRange リソースの種類
description: '条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。'
localization_priority: Normal
ms.openlocfilehash: 14dd86502feb0a5082d3af142202f77ec9eac75c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876406"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="31ce0-103">sizeRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31ce0-103">sizeRange resource type</span></span>

> <span data-ttu-id="31ce0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31ce0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31ce0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31ce0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31ce0-106">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。</span><span class="sxs-lookup"><span data-stu-id="31ce0-106">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="31ce0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31ce0-107">Properties</span></span>
| <span data-ttu-id="31ce0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31ce0-108">Property</span></span>     | <span data-ttu-id="31ce0-109">種類</span><span class="sxs-lookup"><span data-stu-id="31ce0-109">Type</span></span>   |<span data-ttu-id="31ce0-110">説明</span><span class="sxs-lookup"><span data-stu-id="31ce0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="31ce0-111">maximumSize</span><span class="sxs-lookup"><span data-stu-id="31ce0-111">maximumSize</span></span> | <span data-ttu-id="31ce0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="31ce0-112">Int32</span></span> | <span data-ttu-id="31ce0-113">条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="31ce0-113">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="31ce0-114">minimumSize</span><span class="sxs-lookup"><span data-stu-id="31ce0-114">minimumSize</span></span> | <span data-ttu-id="31ce0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="31ce0-115">Int32</span></span> | <span data-ttu-id="31ce0-116">条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="31ce0-116">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="31ce0-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31ce0-117">JSON representation</span></span>
<span data-ttu-id="31ce0-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31ce0-118">Here is a JSON representation of the resource.</span></span>

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
