---
title: addIn リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 46daa8c4f1218b3de485643a47f7acbe881c661c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974544"
---
# <a name="addin-resource-type"></a><span data-ttu-id="34c2e-103">addIn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34c2e-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="34c2e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c2e-104">Properties</span></span>
| <span data-ttu-id="34c2e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c2e-105">Property</span></span>     | <span data-ttu-id="34c2e-106">型</span><span class="sxs-lookup"><span data-stu-id="34c2e-106">Type</span></span>   |<span data-ttu-id="34c2e-107">説明</span><span class="sxs-lookup"><span data-stu-id="34c2e-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34c2e-108">id</span><span class="sxs-lookup"><span data-stu-id="34c2e-108">id</span></span>|<span data-ttu-id="34c2e-109">guid</span><span class="sxs-lookup"><span data-stu-id="34c2e-109">guid</span></span>||
|<span data-ttu-id="34c2e-110">properties</span><span class="sxs-lookup"><span data-stu-id="34c2e-110">properties</span></span>|<span data-ttu-id="34c2e-111">[keyvalue](keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34c2e-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="34c2e-112">type</span><span class="sxs-lookup"><span data-stu-id="34c2e-112">type</span></span>|<span data-ttu-id="34c2e-113">string</span><span class="sxs-lookup"><span data-stu-id="34c2e-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="34c2e-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34c2e-114">JSON representation</span></span>

<span data-ttu-id="34c2e-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34c2e-115">Here is a JSON representation of the resource.</span></span>

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
