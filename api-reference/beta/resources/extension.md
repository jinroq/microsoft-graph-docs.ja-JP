---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
localization_priority: Normal
ms.openlocfilehash: 6a07a341e812ebb119c13b7003841450163cbdd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869301"
---
# <a name="extension-resource-type"></a><span data-ttu-id="a1c4e-103">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1c4e-103">extension resource type</span></span>

> <span data-ttu-id="a1c4e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1c4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1c4e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1c4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1c4e-106">OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="a1c4e-106">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1c4e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1c4e-107">JSON representation</span></span>

<span data-ttu-id="a1c4e-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a1c4e-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="a1c4e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1c4e-109">Properties</span></span>
| <span data-ttu-id="a1c4e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1c4e-110">Property</span></span>     | <span data-ttu-id="a1c4e-111">種類</span><span class="sxs-lookup"><span data-stu-id="a1c4e-111">Type</span></span>   |<span data-ttu-id="a1c4e-112">説明</span><span class="sxs-lookup"><span data-stu-id="a1c4e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1c4e-113">ID</span><span class="sxs-lookup"><span data-stu-id="a1c4e-113">id</span></span>|<span data-ttu-id="a1c4e-114">String</span><span class="sxs-lookup"><span data-stu-id="a1c4e-114">String</span></span>| <span data-ttu-id="a1c4e-115">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a1c4e-115">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1c4e-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1c4e-116">Relationships</span></span>
<span data-ttu-id="a1c4e-117">なし</span><span class="sxs-lookup"><span data-stu-id="a1c4e-117">None</span></span>


## <a name="methods"></a><span data-ttu-id="a1c4e-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1c4e-118">Methods</span></span>

<span data-ttu-id="a1c4e-119">実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1c4e-119">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
