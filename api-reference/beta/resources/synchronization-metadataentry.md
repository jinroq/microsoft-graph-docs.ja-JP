---
title: metadataentry リソースの種類
description: 指定したオブジェクトのメタデータ。
localization_priority: Normal
ms.openlocfilehash: 829dc5fbbf3d73dbabb2e9e69bfff28814cc203a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345600"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="175ff-103">metadataentry リソースの種類</span><span class="sxs-lookup"><span data-stu-id="175ff-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="175ff-104">指定したオブジェクトのメタデータ。</span><span class="sxs-lookup"><span data-stu-id="175ff-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="175ff-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="175ff-105">Properties</span></span>
| <span data-ttu-id="175ff-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="175ff-106">Property</span></span>     | <span data-ttu-id="175ff-107">型</span><span class="sxs-lookup"><span data-stu-id="175ff-107">Type</span></span>   |<span data-ttu-id="175ff-108">説明</span><span class="sxs-lookup"><span data-stu-id="175ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="175ff-109">Key</span><span class="sxs-lookup"><span data-stu-id="175ff-109">key</span></span>|<span data-ttu-id="175ff-110">String</span><span class="sxs-lookup"><span data-stu-id="175ff-110">String</span></span>|<span data-ttu-id="175ff-111">メタデータプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="175ff-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="175ff-112">value</span><span class="sxs-lookup"><span data-stu-id="175ff-112">value</span></span>|<span data-ttu-id="175ff-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="175ff-113">String</span></span>|<span data-ttu-id="175ff-114">メタデータプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="175ff-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="175ff-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="175ff-115">JSON representation</span></span>

<span data-ttu-id="175ff-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="175ff-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
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
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
