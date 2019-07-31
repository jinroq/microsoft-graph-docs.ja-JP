---
author: JeremyKelley
description: columnDefinition リソースの textColumn は、列の値がテキストであることを示します。
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964342"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="bb01f-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb01f-103">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb01f-104">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="bb01f-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb01f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb01f-105">JSON representation</span></span>

<span data-ttu-id="bb01f-106">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb01f-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="bb01f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb01f-107">Properties</span></span>

| <span data-ttu-id="bb01f-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="bb01f-108">Property name</span></span>                   | <span data-ttu-id="bb01f-109">種類</span><span class="sxs-lookup"><span data-stu-id="bb01f-109">Type</span></span>   | <span data-ttu-id="bb01f-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb01f-110">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="bb01f-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="bb01f-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="bb01f-112">string</span><span class="sxs-lookup"><span data-stu-id="bb01f-112">string</span></span> | <span data-ttu-id="bb01f-113">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="bb01f-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="bb01f-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="bb01f-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="bb01f-115">string</span><span class="sxs-lookup"><span data-stu-id="bb01f-115">string</span></span> | <span data-ttu-id="bb01f-116">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="bb01f-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="bb01f-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="bb01f-117">**linesForEditing**</span></span>             | <span data-ttu-id="bb01f-118">int</span><span class="sxs-lookup"><span data-stu-id="bb01f-118">int</span></span>    | <span data-ttu-id="bb01f-119">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="bb01f-119">The size of the text box.</span></span>
| <span data-ttu-id="bb01f-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="bb01f-120">**maxLength**</span></span>                   | <span data-ttu-id="bb01f-121">int</span><span class="sxs-lookup"><span data-stu-id="bb01f-121">int</span></span>    | <span data-ttu-id="bb01f-122">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="bb01f-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="bb01f-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="bb01f-123">**textType**</span></span>                    | <span data-ttu-id="bb01f-124">string</span><span class="sxs-lookup"><span data-stu-id="bb01f-124">string</span></span> | <span data-ttu-id="bb01f-125">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="bb01f-125">The type of text being stored.</span></span> <span data-ttu-id="bb01f-126">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bb01f-126">Must be one of `plain` or `richText`</span></span>

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
