---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 810554620e747d3160a6d8c74913518b8590c19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023480"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="fd271-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd271-102">TextColumn resource type</span></span>

<span data-ttu-id="fd271-103">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="fd271-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd271-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd271-104">JSON representation</span></span>

<span data-ttu-id="fd271-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd271-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="fd271-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd271-106">Properties</span></span>

| <span data-ttu-id="fd271-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="fd271-107">Property name</span></span>                   | <span data-ttu-id="fd271-108">種類</span><span class="sxs-lookup"><span data-stu-id="fd271-108">Type</span></span>    | <span data-ttu-id="fd271-109">説明</span><span class="sxs-lookup"><span data-stu-id="fd271-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="fd271-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="fd271-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="fd271-111">ブール</span><span class="sxs-lookup"><span data-stu-id="fd271-111">boolean</span></span> | <span data-ttu-id="fd271-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="fd271-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="fd271-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="fd271-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="fd271-114">ブール</span><span class="sxs-lookup"><span data-stu-id="fd271-114">boolean</span></span> | <span data-ttu-id="fd271-115">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="fd271-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="fd271-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="fd271-116">**linesForEditing**</span></span>             | <span data-ttu-id="fd271-117">int32</span><span class="sxs-lookup"><span data-stu-id="fd271-117">int32</span></span>   | <span data-ttu-id="fd271-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="fd271-118">The size of the text box.</span></span>
| <span data-ttu-id="fd271-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="fd271-119">**maxLength**</span></span>                   | <span data-ttu-id="fd271-120">int32</span><span class="sxs-lookup"><span data-stu-id="fd271-120">int32</span></span>   | <span data-ttu-id="fd271-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="fd271-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="fd271-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="fd271-122">**textType**</span></span>                    | <span data-ttu-id="fd271-123">string</span><span class="sxs-lookup"><span data-stu-id="fd271-123">string</span></span>  | <span data-ttu-id="fd271-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="fd271-124">The type of text being stored.</span></span> <span data-ttu-id="fd271-125">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="fd271-125">Must be one of `plain` or `richText`</span></span>

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
