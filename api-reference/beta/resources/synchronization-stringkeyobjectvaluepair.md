---
title: stringkeyobjectvaluepair リソースの種類
description: キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。 これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。
localization_priority: Normal
ms.openlocfilehash: 66b4438b73f0000c172db1df385088528d221be4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324803"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="26699-104">stringkeyobjectvaluepair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26699-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26699-105">キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="26699-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="26699-106">これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。</span><span class="sxs-lookup"><span data-stu-id="26699-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="26699-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26699-107">Properties</span></span>
| <span data-ttu-id="26699-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26699-108">Property</span></span>     | <span data-ttu-id="26699-109">型</span><span class="sxs-lookup"><span data-stu-id="26699-109">Type</span></span>   |<span data-ttu-id="26699-110">説明</span><span class="sxs-lookup"><span data-stu-id="26699-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26699-111">Key</span><span class="sxs-lookup"><span data-stu-id="26699-111">key</span></span>|<span data-ttu-id="26699-112">String</span><span class="sxs-lookup"><span data-stu-id="26699-112">String</span></span>|<span data-ttu-id="26699-113">キー。</span><span class="sxs-lookup"><span data-stu-id="26699-113">Key.</span></span>|
|<span data-ttu-id="26699-114">value</span><span class="sxs-lookup"><span data-stu-id="26699-114">value</span></span>|<span data-ttu-id="26699-115">Json</span><span class="sxs-lookup"><span data-stu-id="26699-115">Json</span></span>|<span data-ttu-id="26699-116">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="26699-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26699-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26699-117">JSON representation</span></span>

<span data-ttu-id="26699-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26699-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
