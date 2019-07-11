---
title: stringKeyLongValuePair リソースの種類
description: キーが文字列で、値が Int64 であるキーと値のペアを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c422c565ebdbea58baa3f6709fdd5deef6cb1929
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620410"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="ee1fb-103">stringKeyLongValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee1fb-103">stringKeyLongValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee1fb-104">キーが文字列で、値が Int64 であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="ee1fb-104">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="ee1fb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee1fb-105">Properties</span></span>
| <span data-ttu-id="ee1fb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee1fb-106">Property</span></span>     | <span data-ttu-id="ee1fb-107">型</span><span class="sxs-lookup"><span data-stu-id="ee1fb-107">Type</span></span>   |<span data-ttu-id="ee1fb-108">説明</span><span class="sxs-lookup"><span data-stu-id="ee1fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee1fb-109">Key</span><span class="sxs-lookup"><span data-stu-id="ee1fb-109">key</span></span>|<span data-ttu-id="ee1fb-110">String</span><span class="sxs-lookup"><span data-stu-id="ee1fb-110">String</span></span>|<span data-ttu-id="ee1fb-111">キー。</span><span class="sxs-lookup"><span data-stu-id="ee1fb-111">Key.</span></span>|
|<span data-ttu-id="ee1fb-112">value</span><span class="sxs-lookup"><span data-stu-id="ee1fb-112">value</span></span>|<span data-ttu-id="ee1fb-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ee1fb-113">Int64</span></span>|<span data-ttu-id="ee1fb-114">値</span><span class="sxs-lookup"><span data-stu-id="ee1fb-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee1fb-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee1fb-115">JSON representation</span></span>

<span data-ttu-id="ee1fb-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee1fb-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
