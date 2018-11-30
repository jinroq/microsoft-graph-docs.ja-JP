---
title: stringKeyLongValuePair リソースの種類
description: キーが文字列であり、値は、int64 型のキー/値ペアを表します。
ms.openlocfilehash: 0ceafbc4ab683469e616e068c0abc00804578908
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073088"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="faabb-103">stringKeyLongValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="faabb-103">stringKeyLongValuePair resource type</span></span>

> <span data-ttu-id="faabb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="faabb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faabb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faabb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faabb-106">キーが文字列であり、値は、int64 型のキー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="faabb-106">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="faabb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="faabb-107">Properties</span></span>
| <span data-ttu-id="faabb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="faabb-108">Property</span></span>     | <span data-ttu-id="faabb-109">型</span><span class="sxs-lookup"><span data-stu-id="faabb-109">Type</span></span>   |<span data-ttu-id="faabb-110">説明</span><span class="sxs-lookup"><span data-stu-id="faabb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faabb-111">Key</span><span class="sxs-lookup"><span data-stu-id="faabb-111">key</span></span>|<span data-ttu-id="faabb-112">String</span><span class="sxs-lookup"><span data-stu-id="faabb-112">String</span></span>|<span data-ttu-id="faabb-113">キー。</span><span class="sxs-lookup"><span data-stu-id="faabb-113">Key.</span></span>|
|<span data-ttu-id="faabb-114">value</span><span class="sxs-lookup"><span data-stu-id="faabb-114">value</span></span>|<span data-ttu-id="faabb-115">Int64</span><span class="sxs-lookup"><span data-stu-id="faabb-115">Int64</span></span>|<span data-ttu-id="faabb-116">値</span><span class="sxs-lookup"><span data-stu-id="faabb-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="faabb-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="faabb-117">JSON representation</span></span>

<span data-ttu-id="faabb-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="faabb-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->