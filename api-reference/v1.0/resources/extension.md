---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
localization_priority: Normal
ms.openlocfilehash: 2633c8a28c1be1a670a80834ce869b5156fc1de9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834672"
---
# <a name="extension-resource-type"></a><span data-ttu-id="019ec-103">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="019ec-103">extension resource type</span></span>

<span data-ttu-id="019ec-104">OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="019ec-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="019ec-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="019ec-105">JSON representation</span></span>

<span data-ttu-id="019ec-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="019ec-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="019ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="019ec-107">Properties</span></span>
| <span data-ttu-id="019ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="019ec-108">Property</span></span>     | <span data-ttu-id="019ec-109">種類</span><span class="sxs-lookup"><span data-stu-id="019ec-109">Type</span></span>   |<span data-ttu-id="019ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="019ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="019ec-111">ID</span><span class="sxs-lookup"><span data-stu-id="019ec-111">id</span></span>|<span data-ttu-id="019ec-112">String</span><span class="sxs-lookup"><span data-stu-id="019ec-112">String</span></span>| <span data-ttu-id="019ec-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="019ec-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="019ec-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="019ec-114">Relationships</span></span>
<span data-ttu-id="019ec-115">なし</span><span class="sxs-lookup"><span data-stu-id="019ec-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="019ec-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="019ec-116">Methods</span></span>

<span data-ttu-id="019ec-117">実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="019ec-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
