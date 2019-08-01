---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33c2d37f46d4fdfdaef4bc5b6d92557668bf9d70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034056"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="86152-103">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86152-103">SortField resource type</span></span>

<span data-ttu-id="86152-104">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="86152-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="86152-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86152-105">Properties</span></span>
| <span data-ttu-id="86152-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86152-106">Property</span></span>     | <span data-ttu-id="86152-107">型</span><span class="sxs-lookup"><span data-stu-id="86152-107">Type</span></span>   |<span data-ttu-id="86152-108">説明</span><span class="sxs-lookup"><span data-stu-id="86152-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86152-109">ascending</span><span class="sxs-lookup"><span data-stu-id="86152-109">ascending</span></span>|<span data-ttu-id="86152-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="86152-110">boolean</span></span>|<span data-ttu-id="86152-111">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="86152-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="86152-112">color</span><span class="sxs-lookup"><span data-stu-id="86152-112">color</span></span>|<span data-ttu-id="86152-113">string</span><span class="sxs-lookup"><span data-stu-id="86152-113">string</span></span>|<span data-ttu-id="86152-114">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="86152-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="86152-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="86152-115">dataOption</span></span>|<span data-ttu-id="86152-116">string</span><span class="sxs-lookup"><span data-stu-id="86152-116">string</span></span>|<span data-ttu-id="86152-117">このフィールドのその他の並べ替えオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="86152-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="86152-118">使用可能な値は`Normal`、 `TextAsNumber`、です。</span><span class="sxs-lookup"><span data-stu-id="86152-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="86152-119">Key</span><span class="sxs-lookup"><span data-stu-id="86152-119">key</span></span>|<span data-ttu-id="86152-120">int</span><span class="sxs-lookup"><span data-stu-id="86152-120">int</span></span>|<span data-ttu-id="86152-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="86152-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="86152-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="86152-123">sortOn</span></span>|<span data-ttu-id="86152-124">string</span><span class="sxs-lookup"><span data-stu-id="86152-124">string</span></span>|<span data-ttu-id="86152-125">この条件の並べ替えの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="86152-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="86152-126">使用可能な値: `Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="86152-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="86152-127">アイコン</span><span class="sxs-lookup"><span data-stu-id="86152-127">icon</span></span>|[<span data-ttu-id="86152-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="86152-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="86152-129">並べ替えがセルのアイコンで行われる場合に、条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="86152-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86152-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86152-130">JSON representation</span></span>

<span data-ttu-id="86152-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86152-131">Here is a JSON representation of the resource.</span></span>

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
