---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
ms.openlocfilehash: 1b3d735e0997ca128b539bff9a05c9c7c56799df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020449"
---
# <a name="extension-resource-type"></a><span data-ttu-id="bc1f6-103">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc1f6-103">extension resource type</span></span>

<span data-ttu-id="bc1f6-104">OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="bc1f6-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc1f6-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc1f6-105">JSON representation</span></span>

<span data-ttu-id="bc1f6-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bc1f6-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="bc1f6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc1f6-107">Properties</span></span>
| <span data-ttu-id="bc1f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc1f6-108">Property</span></span>     | <span data-ttu-id="bc1f6-109">型</span><span class="sxs-lookup"><span data-stu-id="bc1f6-109">Type</span></span>   |<span data-ttu-id="bc1f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc1f6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc1f6-111">id</span><span class="sxs-lookup"><span data-stu-id="bc1f6-111">id</span></span>|<span data-ttu-id="bc1f6-112">String</span><span class="sxs-lookup"><span data-stu-id="bc1f6-112">String</span></span>| <span data-ttu-id="bc1f6-113">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bc1f6-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc1f6-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc1f6-114">Relationships</span></span>
<span data-ttu-id="bc1f6-115">なし</span><span class="sxs-lookup"><span data-stu-id="bc1f6-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="bc1f6-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc1f6-116">Methods</span></span>

<span data-ttu-id="bc1f6-117">実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc1f6-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->