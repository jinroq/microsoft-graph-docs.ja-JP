---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521636"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="a963d-103">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a963d-103">SortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a963d-104">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="a963d-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="a963d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a963d-105">Properties</span></span>
| <span data-ttu-id="a963d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a963d-106">Property</span></span>     | <span data-ttu-id="a963d-107">型</span><span class="sxs-lookup"><span data-stu-id="a963d-107">Type</span></span>   |<span data-ttu-id="a963d-108">説明</span><span class="sxs-lookup"><span data-stu-id="a963d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a963d-109">ascending</span><span class="sxs-lookup"><span data-stu-id="a963d-109">ascending</span></span>|<span data-ttu-id="a963d-110">boolean</span><span class="sxs-lookup"><span data-stu-id="a963d-110">boolean</span></span>|<span data-ttu-id="a963d-111">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="a963d-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="a963d-112">color</span><span class="sxs-lookup"><span data-stu-id="a963d-112">color</span></span>|<span data-ttu-id="a963d-113">文字列</span><span class="sxs-lookup"><span data-stu-id="a963d-113">string</span></span>|<span data-ttu-id="a963d-114">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="a963d-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="a963d-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="a963d-115">dataOption</span></span>|<span data-ttu-id="a963d-116">string</span><span class="sxs-lookup"><span data-stu-id="a963d-116">string</span></span>|<span data-ttu-id="a963d-p101">このフィールドのその他の並べ替えオプションを表します。可能な値は、`Normal`、`TextAsNumber` です。</span><span class="sxs-lookup"><span data-stu-id="a963d-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="a963d-119">Key</span><span class="sxs-lookup"><span data-stu-id="a963d-119">key</span></span>|<span data-ttu-id="a963d-120">int</span><span class="sxs-lookup"><span data-stu-id="a963d-120">int</span></span>|<span data-ttu-id="a963d-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="a963d-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="a963d-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="a963d-123">sortOn</span></span>|<span data-ttu-id="a963d-124">string</span><span class="sxs-lookup"><span data-stu-id="a963d-124">string</span></span>|<span data-ttu-id="a963d-p103">この条件の並べ替えの種類を表します。可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。</span><span class="sxs-lookup"><span data-stu-id="a963d-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a963d-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a963d-127">Relationships</span></span>
| <span data-ttu-id="a963d-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a963d-128">Relationship</span></span> | <span data-ttu-id="a963d-129">型</span><span class="sxs-lookup"><span data-stu-id="a963d-129">Type</span></span>   |<span data-ttu-id="a963d-130">説明</span><span class="sxs-lookup"><span data-stu-id="a963d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a963d-131">アイコン</span><span class="sxs-lookup"><span data-stu-id="a963d-131">icon</span></span>|[<span data-ttu-id="a963d-132">Icon</span><span class="sxs-lookup"><span data-stu-id="a963d-132">Icon</span></span>](icon.md)|<span data-ttu-id="a963d-133">並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="a963d-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a963d-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a963d-134">JSON representation</span></span>

<span data-ttu-id="a963d-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a963d-135">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
