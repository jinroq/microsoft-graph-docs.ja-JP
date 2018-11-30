---
title: keyValue リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: 86f5f3c434a52c63536f36e6e7a0dbd1fabf3125
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072181"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="28d30-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28d30-103">keyValue resource type</span></span>

> <span data-ttu-id="28d30-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28d30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28d30-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28d30-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28d30-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28d30-106">JSON representation</span></span>

<span data-ttu-id="28d30-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28d30-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="28d30-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28d30-108">Properties</span></span>
| <span data-ttu-id="28d30-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28d30-109">Property</span></span>     | <span data-ttu-id="28d30-110">型</span><span class="sxs-lookup"><span data-stu-id="28d30-110">Type</span></span>   |<span data-ttu-id="28d30-111">説明</span><span class="sxs-lookup"><span data-stu-id="28d30-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28d30-112">Key</span><span class="sxs-lookup"><span data-stu-id="28d30-112">key</span></span>|<span data-ttu-id="28d30-113">文字列</span><span class="sxs-lookup"><span data-stu-id="28d30-113">string</span></span>||
|<span data-ttu-id="28d30-114">value</span><span class="sxs-lookup"><span data-stu-id="28d30-114">value</span></span>|<span data-ttu-id="28d30-115">文字列</span><span class="sxs-lookup"><span data-stu-id="28d30-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->