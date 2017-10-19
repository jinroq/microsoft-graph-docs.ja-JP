---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="e2158-102">TextColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2158-102">TextColumn resource type</span></span>

<span data-ttu-id="e2158-103">[columnDefinition](columnDefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e2158-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2158-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2158-104">JSON representation</span></span>

<span data-ttu-id="e2158-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2158-105">Here is a JSON representation of a **baseItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e2158-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2158-106">Properties</span></span>

| <span data-ttu-id="e2158-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e2158-107">Property name</span></span>                   | <span data-ttu-id="e2158-108">種類</span><span class="sxs-lookup"><span data-stu-id="e2158-108">Type</span></span>   | <span data-ttu-id="e2158-109">説明</span><span class="sxs-lookup"><span data-stu-id="e2158-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="e2158-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="e2158-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="e2158-111">string</span><span class="sxs-lookup"><span data-stu-id="e2158-111">string</span></span> | <span data-ttu-id="e2158-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="e2158-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="e2158-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="e2158-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="e2158-114">string</span><span class="sxs-lookup"><span data-stu-id="e2158-114">string</span></span> | <span data-ttu-id="e2158-115">この列への更新により、既存のテキストを置き換えるか、既存のテキストに追加するか。</span><span class="sxs-lookup"><span data-stu-id="e2158-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="e2158-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="e2158-116">**linesForEditing**</span></span>             | <span data-ttu-id="e2158-117">int</span><span class="sxs-lookup"><span data-stu-id="e2158-117">int</span></span>    | <span data-ttu-id="e2158-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="e2158-118">The size of the text box.</span></span>
| <span data-ttu-id="e2158-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="e2158-119">**maxLength**</span></span>                   | <span data-ttu-id="e2158-120">int</span><span class="sxs-lookup"><span data-stu-id="e2158-120">int</span></span>    | <span data-ttu-id="e2158-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="e2158-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="e2158-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="e2158-122">**textType**</span></span>                    | <span data-ttu-id="e2158-123">string</span><span class="sxs-lookup"><span data-stu-id="e2158-123">string</span></span> | <span data-ttu-id="e2158-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="e2158-124">The type of text being stored.</span></span> <span data-ttu-id="e2158-125">`plain` または `richText` のいずれかでなければなりません</span><span class="sxs-lookup"><span data-stu-id="e2158-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
