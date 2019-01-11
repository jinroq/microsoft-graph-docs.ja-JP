---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列であり、値は、attributeMappingSource は、キー/値ペアを表します。
localization_priority: Normal
ms.openlocfilehash: 24695cc64fd3c240d5416a7b37e9a5d373e5a88a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805090"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="4a957-103">stringKeyAttributeMappingSourceValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a957-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="4a957-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a957-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a957-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a957-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a957-106">キーが文字列であり、値は、 [attributeMappingSource](synchronization-attributemappingsource.md)は、キー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="4a957-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4a957-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a957-107">Properties</span></span>
| <span data-ttu-id="4a957-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a957-108">Property</span></span>     | <span data-ttu-id="4a957-109">種類</span><span class="sxs-lookup"><span data-stu-id="4a957-109">Type</span></span>   |<span data-ttu-id="4a957-110">説明</span><span class="sxs-lookup"><span data-stu-id="4a957-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a957-111">Key</span><span class="sxs-lookup"><span data-stu-id="4a957-111">key</span></span>|<span data-ttu-id="4a957-112">String</span><span class="sxs-lookup"><span data-stu-id="4a957-112">String</span></span>|<span data-ttu-id="4a957-113">パラメーターの名前です。</span><span class="sxs-lookup"><span data-stu-id="4a957-113">The name of the parameter.</span></span>|
|<span data-ttu-id="4a957-114">value</span><span class="sxs-lookup"><span data-stu-id="4a957-114">value</span></span>|[<span data-ttu-id="4a957-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="4a957-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="4a957-116">パラメーターの値です。</span><span class="sxs-lookup"><span data-stu-id="4a957-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a957-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a957-117">JSON representation</span></span>

<span data-ttu-id="4a957-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a957-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
