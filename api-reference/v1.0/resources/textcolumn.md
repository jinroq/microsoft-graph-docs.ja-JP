---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: d064253cfad141d5879afb52451ca28fa2aeca67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860880"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="e5133-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5133-102">TextColumn resource type</span></span>

<span data-ttu-id="e5133-103">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e5133-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5133-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5133-104">JSON representation</span></span>

<span data-ttu-id="e5133-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5133-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e5133-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5133-106">Properties</span></span>

| <span data-ttu-id="e5133-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e5133-107">Property name</span></span>                   | <span data-ttu-id="e5133-108">種類</span><span class="sxs-lookup"><span data-stu-id="e5133-108">Type</span></span>    | <span data-ttu-id="e5133-109">説明</span><span class="sxs-lookup"><span data-stu-id="e5133-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="e5133-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="e5133-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="e5133-111">ブール</span><span class="sxs-lookup"><span data-stu-id="e5133-111">boolean</span></span> | <span data-ttu-id="e5133-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="e5133-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="e5133-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="e5133-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="e5133-114">ブール</span><span class="sxs-lookup"><span data-stu-id="e5133-114">boolean</span></span> | <span data-ttu-id="e5133-115">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="e5133-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="e5133-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="e5133-116">**linesForEditing**</span></span>             | <span data-ttu-id="e5133-117">int32</span><span class="sxs-lookup"><span data-stu-id="e5133-117">int32</span></span>   | <span data-ttu-id="e5133-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="e5133-118">The size of the text box.</span></span>
| <span data-ttu-id="e5133-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="e5133-119">**maxLength**</span></span>                   | <span data-ttu-id="e5133-120">int32</span><span class="sxs-lookup"><span data-stu-id="e5133-120">int32</span></span>   | <span data-ttu-id="e5133-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="e5133-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="e5133-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="e5133-122">**textType**</span></span>                    | <span data-ttu-id="e5133-123">string</span><span class="sxs-lookup"><span data-stu-id="e5133-123">string</span></span>  | <span data-ttu-id="e5133-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="e5133-124">The type of text being stored.</span></span> <span data-ttu-id="e5133-125">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="e5133-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
