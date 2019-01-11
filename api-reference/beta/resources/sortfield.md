---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: fc93f33f7e1c6f366986cd5d1ca82ea186ad44b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894279"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="2d22e-103">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d22e-103">SortField resource type</span></span>

> <span data-ttu-id="2d22e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d22e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d22e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d22e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d22e-106">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="2d22e-106">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="2d22e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d22e-107">Properties</span></span>
| <span data-ttu-id="2d22e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d22e-108">Property</span></span>     | <span data-ttu-id="2d22e-109">種類</span><span class="sxs-lookup"><span data-stu-id="2d22e-109">Type</span></span>   |<span data-ttu-id="2d22e-110">説明</span><span class="sxs-lookup"><span data-stu-id="2d22e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d22e-111">ascending</span><span class="sxs-lookup"><span data-stu-id="2d22e-111">ascending</span></span>|<span data-ttu-id="2d22e-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="2d22e-112">boolean</span></span>|<span data-ttu-id="2d22e-113">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="2d22e-113">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="2d22e-114">color</span><span class="sxs-lookup"><span data-stu-id="2d22e-114">color</span></span>|<span data-ttu-id="2d22e-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2d22e-115">string</span></span>|<span data-ttu-id="2d22e-116">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="2d22e-116">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="2d22e-117">dataOption</span><span class="sxs-lookup"><span data-stu-id="2d22e-117">dataOption</span></span>|<span data-ttu-id="2d22e-118">文字列</span><span class="sxs-lookup"><span data-stu-id="2d22e-118">string</span></span>|<span data-ttu-id="2d22e-p102">このフィールドのその他の並べ替えオプションを表します。可能な値は、`Normal`、`TextAsNumber` です。</span><span class="sxs-lookup"><span data-stu-id="2d22e-p102">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="2d22e-121">Key</span><span class="sxs-lookup"><span data-stu-id="2d22e-121">key</span></span>|<span data-ttu-id="2d22e-122">int</span><span class="sxs-lookup"><span data-stu-id="2d22e-122">int</span></span>|<span data-ttu-id="2d22e-p103">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="2d22e-p103">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="2d22e-125">sortOn</span><span class="sxs-lookup"><span data-stu-id="2d22e-125">sortOn</span></span>|<span data-ttu-id="2d22e-126">文字列</span><span class="sxs-lookup"><span data-stu-id="2d22e-126">string</span></span>|<span data-ttu-id="2d22e-p104">この条件の並べ替えの種類を表します。可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。</span><span class="sxs-lookup"><span data-stu-id="2d22e-p104">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d22e-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d22e-129">Relationships</span></span>
| <span data-ttu-id="2d22e-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d22e-130">Relationship</span></span> | <span data-ttu-id="2d22e-131">型</span><span class="sxs-lookup"><span data-stu-id="2d22e-131">Type</span></span>   |<span data-ttu-id="2d22e-132">説明</span><span class="sxs-lookup"><span data-stu-id="2d22e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d22e-133">アイコン</span><span class="sxs-lookup"><span data-stu-id="2d22e-133">icon</span></span>|[<span data-ttu-id="2d22e-134">Icon</span><span class="sxs-lookup"><span data-stu-id="2d22e-134">Icon</span></span>](icon.md)|<span data-ttu-id="2d22e-135">並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="2d22e-135">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d22e-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d22e-136">JSON representation</span></span>

<span data-ttu-id="2d22e-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d22e-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
