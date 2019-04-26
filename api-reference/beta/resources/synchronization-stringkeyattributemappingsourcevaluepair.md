---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列で、値が attributeMappingSource であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: 7b722fb681ceb64ac4dd58553010e704e7669584
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345522"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="fa0e1-103">stringKeyAttributeMappingSourceValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa0e1-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa0e1-104">キーが文字列で、値が[attributeMappingSource](synchronization-attributemappingsource.md)であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="fa0e1-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fa0e1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa0e1-105">Properties</span></span>
| <span data-ttu-id="fa0e1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa0e1-106">Property</span></span>     | <span data-ttu-id="fa0e1-107">型</span><span class="sxs-lookup"><span data-stu-id="fa0e1-107">Type</span></span>   |<span data-ttu-id="fa0e1-108">説明</span><span class="sxs-lookup"><span data-stu-id="fa0e1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa0e1-109">Key</span><span class="sxs-lookup"><span data-stu-id="fa0e1-109">key</span></span>|<span data-ttu-id="fa0e1-110">String</span><span class="sxs-lookup"><span data-stu-id="fa0e1-110">String</span></span>|<span data-ttu-id="fa0e1-111">パラメーターの名前です。</span><span class="sxs-lookup"><span data-stu-id="fa0e1-111">The name of the parameter.</span></span>|
|<span data-ttu-id="fa0e1-112">value</span><span class="sxs-lookup"><span data-stu-id="fa0e1-112">value</span></span>|[<span data-ttu-id="fa0e1-113">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="fa0e1-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="fa0e1-114">パラメーターの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa0e1-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa0e1-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa0e1-115">JSON representation</span></span>

<span data-ttu-id="fa0e1-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa0e1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
