---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列であり、値は、attributeMappingSource は、キー/値ペアを表します。
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073529"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="813f4-103">stringKeyAttributeMappingSourceValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="813f4-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="813f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="813f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="813f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="813f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="813f4-106">キーが文字列であり、値は、 [attributeMappingSource](synchronization-attributemappingsource.md)は、キー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="813f4-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="813f4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="813f4-107">Properties</span></span>
| <span data-ttu-id="813f4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="813f4-108">Property</span></span>     | <span data-ttu-id="813f4-109">型</span><span class="sxs-lookup"><span data-stu-id="813f4-109">Type</span></span>   |<span data-ttu-id="813f4-110">説明</span><span class="sxs-lookup"><span data-stu-id="813f4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="813f4-111">Key</span><span class="sxs-lookup"><span data-stu-id="813f4-111">key</span></span>|<span data-ttu-id="813f4-112">String</span><span class="sxs-lookup"><span data-stu-id="813f4-112">String</span></span>|<span data-ttu-id="813f4-113">パラメーターの名前です。</span><span class="sxs-lookup"><span data-stu-id="813f4-113">The name of the parameter.</span></span>|
|<span data-ttu-id="813f4-114">value</span><span class="sxs-lookup"><span data-stu-id="813f4-114">value</span></span>|[<span data-ttu-id="813f4-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="813f4-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="813f4-116">パラメーターの値です。</span><span class="sxs-lookup"><span data-stu-id="813f4-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="813f4-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="813f4-117">JSON representation</span></span>

<span data-ttu-id="813f4-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="813f4-118">The following is a JSON representation of the resource.</span></span>

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
