---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825971"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="ba264-103">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba264-103">SortField resource type</span></span>

<span data-ttu-id="ba264-104">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="ba264-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba264-105">Properties</span></span>
| <span data-ttu-id="ba264-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba264-106">Property</span></span>     | <span data-ttu-id="ba264-107">種類</span><span class="sxs-lookup"><span data-stu-id="ba264-107">Type</span></span>   |<span data-ttu-id="ba264-108">説明</span><span class="sxs-lookup"><span data-stu-id="ba264-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba264-109">ascending</span><span class="sxs-lookup"><span data-stu-id="ba264-109">ascending</span></span>|<span data-ttu-id="ba264-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="ba264-110">boolean</span></span>|<span data-ttu-id="ba264-111">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="ba264-112">color</span><span class="sxs-lookup"><span data-stu-id="ba264-112">color</span></span>|<span data-ttu-id="ba264-113">文字列</span><span class="sxs-lookup"><span data-stu-id="ba264-113">string</span></span>|<span data-ttu-id="ba264-114">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="ba264-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="ba264-115">dataOption</span></span>|<span data-ttu-id="ba264-116">文字列</span><span class="sxs-lookup"><span data-stu-id="ba264-116">string</span></span>|<span data-ttu-id="ba264-117">このフィールドの他の並べ替えオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="ba264-118">可能な値: `Normal`、 `TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="ba264-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="ba264-119">Key</span><span class="sxs-lookup"><span data-stu-id="ba264-119">key</span></span>|<span data-ttu-id="ba264-120">int</span><span class="sxs-lookup"><span data-stu-id="ba264-120">int</span></span>|<span data-ttu-id="ba264-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="ba264-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="ba264-123">sortOn</span></span>|<span data-ttu-id="ba264-124">文字列</span><span class="sxs-lookup"><span data-stu-id="ba264-124">string</span></span>|<span data-ttu-id="ba264-125">この条件の並べ替えの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="ba264-126">可能な値: `Value`、 `CellColor`、 `FontColor`、 `Icon`。</span><span class="sxs-lookup"><span data-stu-id="ba264-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="ba264-127">アイコン</span><span class="sxs-lookup"><span data-stu-id="ba264-127">icon</span></span>|[<span data-ttu-id="ba264-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="ba264-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="ba264-129">並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="ba264-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba264-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba264-130">JSON representation</span></span>

<span data-ttu-id="ba264-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba264-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
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
