---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 524f25b6b5097197daeb8b130b10ff7513010965
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525004"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="dfce8-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfce8-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfce8-103">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="dfce8-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfce8-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfce8-104">JSON representation</span></span>

<span data-ttu-id="dfce8-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfce8-105">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="dfce8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfce8-106">Properties</span></span>

| <span data-ttu-id="dfce8-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="dfce8-107">Property name</span></span>                   | <span data-ttu-id="dfce8-108">種類</span><span class="sxs-lookup"><span data-stu-id="dfce8-108">Type</span></span>   | <span data-ttu-id="dfce8-109">説明</span><span class="sxs-lookup"><span data-stu-id="dfce8-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="dfce8-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="dfce8-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="dfce8-111">string</span><span class="sxs-lookup"><span data-stu-id="dfce8-111">string</span></span> | <span data-ttu-id="dfce8-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="dfce8-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="dfce8-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="dfce8-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="dfce8-114">string</span><span class="sxs-lookup"><span data-stu-id="dfce8-114">string</span></span> | <span data-ttu-id="dfce8-115">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="dfce8-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="dfce8-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="dfce8-116">**linesForEditing**</span></span>             | <span data-ttu-id="dfce8-117">int</span><span class="sxs-lookup"><span data-stu-id="dfce8-117">int</span></span>    | <span data-ttu-id="dfce8-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="dfce8-118">The size of the text box.</span></span>
| <span data-ttu-id="dfce8-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="dfce8-119">**maxLength**</span></span>                   | <span data-ttu-id="dfce8-120">int</span><span class="sxs-lookup"><span data-stu-id="dfce8-120">int</span></span>    | <span data-ttu-id="dfce8-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="dfce8-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="dfce8-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="dfce8-122">**textType**</span></span>                    | <span data-ttu-id="dfce8-123">string</span><span class="sxs-lookup"><span data-stu-id="dfce8-123">string</span></span> | <span data-ttu-id="dfce8-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="dfce8-124">The type of text being stored.</span></span> <span data-ttu-id="dfce8-125">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="dfce8-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
