---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: c69dc7c30bff0f43327ec256af6071e34de6b898
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481497"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="eb319-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb319-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb319-103">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="eb319-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb319-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb319-104">JSON representation</span></span>

<span data-ttu-id="eb319-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb319-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="eb319-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb319-106">Properties</span></span>

| <span data-ttu-id="eb319-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="eb319-107">Property name</span></span>                   | <span data-ttu-id="eb319-108">種類</span><span class="sxs-lookup"><span data-stu-id="eb319-108">Type</span></span>   | <span data-ttu-id="eb319-109">説明</span><span class="sxs-lookup"><span data-stu-id="eb319-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="eb319-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="eb319-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="eb319-111">string</span><span class="sxs-lookup"><span data-stu-id="eb319-111">string</span></span> | <span data-ttu-id="eb319-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="eb319-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="eb319-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="eb319-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="eb319-114">string</span><span class="sxs-lookup"><span data-stu-id="eb319-114">string</span></span> | <span data-ttu-id="eb319-115">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="eb319-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="eb319-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="eb319-116">**linesForEditing**</span></span>             | <span data-ttu-id="eb319-117">int</span><span class="sxs-lookup"><span data-stu-id="eb319-117">int</span></span>    | <span data-ttu-id="eb319-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="eb319-118">The size of the text box.</span></span>
| <span data-ttu-id="eb319-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="eb319-119">**maxLength**</span></span>                   | <span data-ttu-id="eb319-120">int</span><span class="sxs-lookup"><span data-stu-id="eb319-120">int</span></span>    | <span data-ttu-id="eb319-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="eb319-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="eb319-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="eb319-122">**textType**</span></span>                    | <span data-ttu-id="eb319-123">string</span><span class="sxs-lookup"><span data-stu-id="eb319-123">string</span></span> | <span data-ttu-id="eb319-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="eb319-124">The type of text being stored.</span></span> <span data-ttu-id="eb319-125">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="eb319-125">Must be one of `plain` or `richText`</span></span>

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
