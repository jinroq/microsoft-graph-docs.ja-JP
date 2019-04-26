---
title: stringkeystringvaluepair リソースの種類
description: キーが文字列で、値が文字列であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: 99e92f542ece2895591a76fcb80c322e3f6d6613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324749"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="895f1-103">stringkeystringvaluepair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="895f1-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="895f1-104">キーが文字列で、値が文字列であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="895f1-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="895f1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="895f1-105">Properties</span></span>
| <span data-ttu-id="895f1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="895f1-106">Property</span></span>     | <span data-ttu-id="895f1-107">型</span><span class="sxs-lookup"><span data-stu-id="895f1-107">Type</span></span>   |<span data-ttu-id="895f1-108">説明</span><span class="sxs-lookup"><span data-stu-id="895f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="895f1-109">Key</span><span class="sxs-lookup"><span data-stu-id="895f1-109">key</span></span>|<span data-ttu-id="895f1-110">String</span><span class="sxs-lookup"><span data-stu-id="895f1-110">String</span></span>|<span data-ttu-id="895f1-111">キー。</span><span class="sxs-lookup"><span data-stu-id="895f1-111">Key.</span></span>|
|<span data-ttu-id="895f1-112">value</span><span class="sxs-lookup"><span data-stu-id="895f1-112">value</span></span>|<span data-ttu-id="895f1-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="895f1-113">String</span></span>|<span data-ttu-id="895f1-114">値。</span><span class="sxs-lookup"><span data-stu-id="895f1-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="895f1-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="895f1-115">JSON representation</span></span>

<span data-ttu-id="895f1-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="895f1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
