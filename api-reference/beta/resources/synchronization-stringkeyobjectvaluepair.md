---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831452"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="73e80-104">stringKeyObjectValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73e80-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="73e80-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73e80-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73e80-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73e80-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73e80-107">キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="73e80-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="73e80-108">これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="73e80-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="73e80-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73e80-109">Properties</span></span>
| <span data-ttu-id="73e80-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73e80-110">Property</span></span>     | <span data-ttu-id="73e80-111">種類</span><span class="sxs-lookup"><span data-stu-id="73e80-111">Type</span></span>   |<span data-ttu-id="73e80-112">説明</span><span class="sxs-lookup"><span data-stu-id="73e80-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73e80-113">Key</span><span class="sxs-lookup"><span data-stu-id="73e80-113">key</span></span>|<span data-ttu-id="73e80-114">String</span><span class="sxs-lookup"><span data-stu-id="73e80-114">String</span></span>|<span data-ttu-id="73e80-115">キー。</span><span class="sxs-lookup"><span data-stu-id="73e80-115">Key.</span></span>|
|<span data-ttu-id="73e80-116">value</span><span class="sxs-lookup"><span data-stu-id="73e80-116">value</span></span>|<span data-ttu-id="73e80-117">Any</span><span class="sxs-lookup"><span data-stu-id="73e80-117">Any</span></span>|<span data-ttu-id="73e80-118">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="73e80-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73e80-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73e80-119">JSON representation</span></span>

<span data-ttu-id="73e80-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73e80-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
