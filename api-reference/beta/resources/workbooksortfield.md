---
title: workbookSortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: 239c0e3b9f95108165ed32e7e22f94049e787432
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348913"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="07cd0-103">workbookSortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07cd0-103">workbookSortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07cd0-104">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="07cd0-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="07cd0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07cd0-105">Properties</span></span>
| <span data-ttu-id="07cd0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07cd0-106">Property</span></span>     | <span data-ttu-id="07cd0-107">種類</span><span class="sxs-lookup"><span data-stu-id="07cd0-107">Type</span></span>   |<span data-ttu-id="07cd0-108">説明</span><span class="sxs-lookup"><span data-stu-id="07cd0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07cd0-109">ascending</span><span class="sxs-lookup"><span data-stu-id="07cd0-109">ascending</span></span>|<span data-ttu-id="07cd0-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="07cd0-110">boolean</span></span>|<span data-ttu-id="07cd0-111">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="07cd0-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="07cd0-112">color</span><span class="sxs-lookup"><span data-stu-id="07cd0-112">color</span></span>|<span data-ttu-id="07cd0-113">string</span><span class="sxs-lookup"><span data-stu-id="07cd0-113">string</span></span>|<span data-ttu-id="07cd0-114">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="07cd0-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="07cd0-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="07cd0-115">dataOption</span></span>|<span data-ttu-id="07cd0-116">string</span><span class="sxs-lookup"><span data-stu-id="07cd0-116">string</span></span>|<span data-ttu-id="07cd0-p101">このフィールドのその他の並べ替えオプションを表します。可能な値は、`Normal`、`TextAsNumber` です。</span><span class="sxs-lookup"><span data-stu-id="07cd0-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="07cd0-119">Key</span><span class="sxs-lookup"><span data-stu-id="07cd0-119">key</span></span>|<span data-ttu-id="07cd0-120">int</span><span class="sxs-lookup"><span data-stu-id="07cd0-120">int</span></span>|<span data-ttu-id="07cd0-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="07cd0-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="07cd0-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="07cd0-123">sortOn</span></span>|<span data-ttu-id="07cd0-124">string</span><span class="sxs-lookup"><span data-stu-id="07cd0-124">string</span></span>|<span data-ttu-id="07cd0-p103">この条件の並べ替えの種類を表します。可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。</span><span class="sxs-lookup"><span data-stu-id="07cd0-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07cd0-127">関係</span><span class="sxs-lookup"><span data-stu-id="07cd0-127">Relationships</span></span>
| <span data-ttu-id="07cd0-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07cd0-128">Relationship</span></span> | <span data-ttu-id="07cd0-129">型</span><span class="sxs-lookup"><span data-stu-id="07cd0-129">Type</span></span>   |<span data-ttu-id="07cd0-130">説明</span><span class="sxs-lookup"><span data-stu-id="07cd0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07cd0-131">アイコン</span><span class="sxs-lookup"><span data-stu-id="07cd0-131">icon</span></span>|[<span data-ttu-id="07cd0-132">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="07cd0-132">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="07cd0-133">並べ替えがセルのアイコンで行われる場合に、条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="07cd0-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07cd0-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07cd0-134">JSON representation</span></span>

<span data-ttu-id="07cd0-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07cd0-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookSortField"
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
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
