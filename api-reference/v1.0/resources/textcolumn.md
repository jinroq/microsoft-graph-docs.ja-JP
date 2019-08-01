---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: columnDefinition リソースの textColumn は、列の値がテキストであることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 37a5bbd985d163cf627f4bc0a16a756eaf00af66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033657"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="f476c-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f476c-103">TextColumn resource type</span></span>

<span data-ttu-id="f476c-104">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="f476c-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f476c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f476c-105">JSON representation</span></span>

<span data-ttu-id="f476c-106">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f476c-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="f476c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f476c-107">Properties</span></span>

| <span data-ttu-id="f476c-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f476c-108">Property name</span></span>                   | <span data-ttu-id="f476c-109">種類</span><span class="sxs-lookup"><span data-stu-id="f476c-109">Type</span></span>    | <span data-ttu-id="f476c-110">説明</span><span class="sxs-lookup"><span data-stu-id="f476c-110">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="f476c-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="f476c-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="f476c-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="f476c-112">boolean</span></span> | <span data-ttu-id="f476c-113">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f476c-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="f476c-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="f476c-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="f476c-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="f476c-115">boolean</span></span> | <span data-ttu-id="f476c-116">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="f476c-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="f476c-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="f476c-117">**linesForEditing**</span></span>             | <span data-ttu-id="f476c-118">int32</span><span class="sxs-lookup"><span data-stu-id="f476c-118">int32</span></span>   | <span data-ttu-id="f476c-119">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="f476c-119">The size of the text box.</span></span>
| <span data-ttu-id="f476c-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="f476c-120">**maxLength**</span></span>                   | <span data-ttu-id="f476c-121">int32</span><span class="sxs-lookup"><span data-stu-id="f476c-121">int32</span></span>   | <span data-ttu-id="f476c-122">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="f476c-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="f476c-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="f476c-123">**textType**</span></span>                    | <span data-ttu-id="f476c-124">string</span><span class="sxs-lookup"><span data-stu-id="f476c-124">string</span></span>  | <span data-ttu-id="f476c-125">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="f476c-125">The type of text being stored.</span></span> <span data-ttu-id="f476c-126">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f476c-126">Must be one of `plain` or `richText`</span></span>

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
