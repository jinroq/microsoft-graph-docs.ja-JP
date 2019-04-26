---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: b57caa76f8376bbd7f119546009f3aca97b78385
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339833"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="96eed-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96eed-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96eed-103">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="96eed-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96eed-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96eed-104">JSON representation</span></span>

<span data-ttu-id="96eed-105">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96eed-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="96eed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96eed-106">Properties</span></span>

| <span data-ttu-id="96eed-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="96eed-107">Property name</span></span>                   | <span data-ttu-id="96eed-108">種類</span><span class="sxs-lookup"><span data-stu-id="96eed-108">Type</span></span>   | <span data-ttu-id="96eed-109">説明</span><span class="sxs-lookup"><span data-stu-id="96eed-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="96eed-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="96eed-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="96eed-111">string</span><span class="sxs-lookup"><span data-stu-id="96eed-111">string</span></span> | <span data-ttu-id="96eed-112">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="96eed-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="96eed-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="96eed-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="96eed-114">string</span><span class="sxs-lookup"><span data-stu-id="96eed-114">string</span></span> | <span data-ttu-id="96eed-115">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="96eed-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="96eed-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="96eed-116">**linesForEditing**</span></span>             | <span data-ttu-id="96eed-117">int</span><span class="sxs-lookup"><span data-stu-id="96eed-117">int</span></span>    | <span data-ttu-id="96eed-118">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="96eed-118">The size of the text box.</span></span>
| <span data-ttu-id="96eed-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="96eed-119">**maxLength**</span></span>                   | <span data-ttu-id="96eed-120">int</span><span class="sxs-lookup"><span data-stu-id="96eed-120">int</span></span>    | <span data-ttu-id="96eed-121">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="96eed-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="96eed-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="96eed-122">**textType**</span></span>                    | <span data-ttu-id="96eed-123">string</span><span class="sxs-lookup"><span data-stu-id="96eed-123">string</span></span> | <span data-ttu-id="96eed-124">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="96eed-124">The type of text being stored.</span></span> <span data-ttu-id="96eed-125">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="96eed-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
