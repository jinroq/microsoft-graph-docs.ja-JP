---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: b5c41091b9193aabc36ee04e9dcc310bfc110af1
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264288"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="6cf2f-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cf2f-102">TextColumn resource type</span></span>

<span data-ttu-id="6cf2f-103">[columnDefinition](columnDefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cf2f-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cf2f-104">JSON representation</span></span>

<span data-ttu-id="6cf2f-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="6cf2f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cf2f-106">Properties</span></span>

| <span data-ttu-id="6cf2f-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6cf2f-107">Property name</span></span>                   | <span data-ttu-id="6cf2f-108">型</span><span class="sxs-lookup"><span data-stu-id="6cf2f-108">Type</span></span>    | <span data-ttu-id="6cf2f-109">説明</span><span class="sxs-lookup"><span data-stu-id="6cf2f-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="6cf2f-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="6cf2f-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="6cf2f-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="6cf2f-111">boolean</span></span> | <span data-ttu-id="6cf2f-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="6cf2f-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="6cf2f-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="6cf2f-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="6cf2f-114">boolean</span></span> | <span data-ttu-id="6cf2f-115">この列への更新が既存のテキストを置き換えるか、または追加するかどうか。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="6cf2f-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="6cf2f-116">**linesForEditing**</span></span>             | <span data-ttu-id="6cf2f-117">int32</span><span class="sxs-lookup"><span data-stu-id="6cf2f-117">int32</span></span>   | <span data-ttu-id="6cf2f-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-118">The size of the text box.</span></span>
| <span data-ttu-id="6cf2f-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="6cf2f-119">**maxLength**</span></span>                   | <span data-ttu-id="6cf2f-120">int32</span><span class="sxs-lookup"><span data-stu-id="6cf2f-120">int32</span></span>   | <span data-ttu-id="6cf2f-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="6cf2f-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="6cf2f-122">**textType**</span></span>                    | <span data-ttu-id="6cf2f-123">文字列</span><span class="sxs-lookup"><span data-stu-id="6cf2f-123">string</span></span>  | <span data-ttu-id="6cf2f-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="6cf2f-124">The type of text being stored.</span></span> <span data-ttu-id="6cf2f-125">または `richText` のいずれかでなければなりません。 `richText`</span><span class="sxs-lookup"><span data-stu-id="6cf2f-125">Must be one of `plain` or `richText`</span></span>

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
