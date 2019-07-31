---
title: stringKeyStringValuePair リソースの種類
description: キーが文字列で、値が文字列であるキーと値のペアを表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 697985c2258c8535aaa076e578501b15944d5687
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007838"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="08aac-103">stringKeyStringValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08aac-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08aac-104">キーが文字列で、値が文字列であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="08aac-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="08aac-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08aac-105">Properties</span></span>
| <span data-ttu-id="08aac-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08aac-106">Property</span></span>     | <span data-ttu-id="08aac-107">型</span><span class="sxs-lookup"><span data-stu-id="08aac-107">Type</span></span>   |<span data-ttu-id="08aac-108">説明</span><span class="sxs-lookup"><span data-stu-id="08aac-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08aac-109">Key</span><span class="sxs-lookup"><span data-stu-id="08aac-109">key</span></span>|<span data-ttu-id="08aac-110">String</span><span class="sxs-lookup"><span data-stu-id="08aac-110">String</span></span>|<span data-ttu-id="08aac-111">キー。</span><span class="sxs-lookup"><span data-stu-id="08aac-111">Key.</span></span>|
|<span data-ttu-id="08aac-112">value</span><span class="sxs-lookup"><span data-stu-id="08aac-112">value</span></span>|<span data-ttu-id="08aac-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="08aac-113">String</span></span>|<span data-ttu-id="08aac-114">値。</span><span class="sxs-lookup"><span data-stu-id="08aac-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08aac-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08aac-115">JSON representation</span></span>

<span data-ttu-id="08aac-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08aac-116">The following is a JSON representation of the resource.</span></span>

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
