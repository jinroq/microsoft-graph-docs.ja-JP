---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 87a5e27544a49613d1d1e44cd6f3e0e3b7fcf8c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822569"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="c1bb5-102">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1bb5-102">TextColumn resource type</span></span>

> <span data-ttu-id="c1bb5-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1bb5-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1bb5-105">[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1bb5-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1bb5-106">JSON representation</span></span>

<span data-ttu-id="c1bb5-107">以下は、**textColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="c1bb5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1bb5-108">Properties</span></span>

| <span data-ttu-id="c1bb5-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c1bb5-109">Property name</span></span>                   | <span data-ttu-id="c1bb5-110">Type</span><span class="sxs-lookup"><span data-stu-id="c1bb5-110">Type</span></span>   | <span data-ttu-id="c1bb5-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1bb5-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="c1bb5-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="c1bb5-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="c1bb5-113">文字列</span><span class="sxs-lookup"><span data-stu-id="c1bb5-113">string</span></span> | <span data-ttu-id="c1bb5-114">複数行のテキストを許可するかどうか。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="c1bb5-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="c1bb5-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="c1bb5-116">文字列</span><span class="sxs-lookup"><span data-stu-id="c1bb5-116">string</span></span> | <span data-ttu-id="c1bb5-117">この列への更新が既存のテキストを置き換えるか、または追加するか。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="c1bb5-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="c1bb5-118">**linesForEditing**</span></span>             | <span data-ttu-id="c1bb5-119">int</span><span class="sxs-lookup"><span data-stu-id="c1bb5-119">int</span></span>    | <span data-ttu-id="c1bb5-120">テキスト ボックスのサイズ。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-120">The size of the text box.</span></span>
| <span data-ttu-id="c1bb5-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="c1bb5-121">**maxLength**</span></span>                   | <span data-ttu-id="c1bb5-122">int</span><span class="sxs-lookup"><span data-stu-id="c1bb5-122">int</span></span>    | <span data-ttu-id="c1bb5-123">値に使用できる最大文字数。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="c1bb5-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="c1bb5-124">**textType**</span></span>                    | <span data-ttu-id="c1bb5-125">文字列</span><span class="sxs-lookup"><span data-stu-id="c1bb5-125">string</span></span> | <span data-ttu-id="c1bb5-126">格納されているテキストの種類。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-126">The type of text being stored.</span></span> <span data-ttu-id="c1bb5-127">`plain` または `richText` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c1bb5-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
