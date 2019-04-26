---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561300"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="816a9-103">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="816a9-103">SortField resource type</span></span>

<span data-ttu-id="816a9-104">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="816a9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="816a9-105">Properties</span></span>
| <span data-ttu-id="816a9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="816a9-106">Property</span></span>     | <span data-ttu-id="816a9-107">型</span><span class="sxs-lookup"><span data-stu-id="816a9-107">Type</span></span>   |<span data-ttu-id="816a9-108">説明</span><span class="sxs-lookup"><span data-stu-id="816a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="816a9-109">ascending</span><span class="sxs-lookup"><span data-stu-id="816a9-109">ascending</span></span>|<span data-ttu-id="816a9-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="816a9-110">boolean</span></span>|<span data-ttu-id="816a9-111">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="816a9-112">color</span><span class="sxs-lookup"><span data-stu-id="816a9-112">color</span></span>|<span data-ttu-id="816a9-113">string</span><span class="sxs-lookup"><span data-stu-id="816a9-113">string</span></span>|<span data-ttu-id="816a9-114">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="816a9-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="816a9-115">dataOption</span></span>|<span data-ttu-id="816a9-116">string</span><span class="sxs-lookup"><span data-stu-id="816a9-116">string</span></span>|<span data-ttu-id="816a9-117">このフィールドのその他の並べ替えオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="816a9-118">使用可能な値は`Normal`、 `TextAsNumber`、です。</span><span class="sxs-lookup"><span data-stu-id="816a9-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="816a9-119">Key</span><span class="sxs-lookup"><span data-stu-id="816a9-119">key</span></span>|<span data-ttu-id="816a9-120">int</span><span class="sxs-lookup"><span data-stu-id="816a9-120">int</span></span>|<span data-ttu-id="816a9-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="816a9-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="816a9-123">sortOn</span></span>|<span data-ttu-id="816a9-124">string</span><span class="sxs-lookup"><span data-stu-id="816a9-124">string</span></span>|<span data-ttu-id="816a9-125">この条件の並べ替えの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="816a9-126">使用可能な値は`Value`、 `CellColor`、 `FontColor`、 `Icon`、です。</span><span class="sxs-lookup"><span data-stu-id="816a9-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="816a9-127">アイコン</span><span class="sxs-lookup"><span data-stu-id="816a9-127">icon</span></span>|[<span data-ttu-id="816a9-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="816a9-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="816a9-129">並べ替えがセルのアイコンで行われる場合に、条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="816a9-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="816a9-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="816a9-130">JSON representation</span></span>

<span data-ttu-id="816a9-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="816a9-131">Here is a JSON representation of the resource.</span></span>

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
