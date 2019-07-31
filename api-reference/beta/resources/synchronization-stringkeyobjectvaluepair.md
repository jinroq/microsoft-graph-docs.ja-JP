---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。 これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3ec55eee1f6b5f60e8936f906390d5343fbafbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007831"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="03092-104">stringKeyObjectValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03092-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03092-105">キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="03092-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="03092-106">これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。</span><span class="sxs-lookup"><span data-stu-id="03092-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="03092-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03092-107">Properties</span></span>
| <span data-ttu-id="03092-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03092-108">Property</span></span>     | <span data-ttu-id="03092-109">型</span><span class="sxs-lookup"><span data-stu-id="03092-109">Type</span></span>   |<span data-ttu-id="03092-110">説明</span><span class="sxs-lookup"><span data-stu-id="03092-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03092-111">Key</span><span class="sxs-lookup"><span data-stu-id="03092-111">key</span></span>|<span data-ttu-id="03092-112">String</span><span class="sxs-lookup"><span data-stu-id="03092-112">String</span></span>|<span data-ttu-id="03092-113">キー。</span><span class="sxs-lookup"><span data-stu-id="03092-113">Key.</span></span>|
|<span data-ttu-id="03092-114">value</span><span class="sxs-lookup"><span data-stu-id="03092-114">value</span></span>|<span data-ttu-id="03092-115">Json</span><span class="sxs-lookup"><span data-stu-id="03092-115">Json</span></span>|<span data-ttu-id="03092-116">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="03092-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03092-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03092-117">JSON representation</span></span>

<span data-ttu-id="03092-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03092-118">The following is a JSON representation of the resource.</span></span>

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
