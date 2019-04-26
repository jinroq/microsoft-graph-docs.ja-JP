---
title: addIn リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 777b9e2eac1ec4052fae30b13d09aaf91a808375
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339129"
---
# <a name="addin-resource-type"></a><span data-ttu-id="c4131-103">addIn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4131-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="c4131-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4131-104">Properties</span></span>
| <span data-ttu-id="c4131-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4131-105">Property</span></span>     | <span data-ttu-id="c4131-106">型</span><span class="sxs-lookup"><span data-stu-id="c4131-106">Type</span></span>   |<span data-ttu-id="c4131-107">説明</span><span class="sxs-lookup"><span data-stu-id="c4131-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4131-108">id</span><span class="sxs-lookup"><span data-stu-id="c4131-108">id</span></span>|<span data-ttu-id="c4131-109">guid</span><span class="sxs-lookup"><span data-stu-id="c4131-109">guid</span></span>||
|<span data-ttu-id="c4131-110">properties</span><span class="sxs-lookup"><span data-stu-id="c4131-110">properties</span></span>|<span data-ttu-id="c4131-111">[keyvalue](keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4131-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="c4131-112">type</span><span class="sxs-lookup"><span data-stu-id="c4131-112">type</span></span>|<span data-ttu-id="c4131-113">string</span><span class="sxs-lookup"><span data-stu-id="c4131-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="c4131-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4131-114">JSON representation</span></span>

<span data-ttu-id="c4131-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4131-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
