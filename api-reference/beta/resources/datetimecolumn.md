---
author: JeremyKelley
description: columnDefinition リソースの dateTimeColumn は、列の値が日付または時刻であることを示します。
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e0e69e4019530031966cde9f782c2f017ba976fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973888"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="f3f57-103">DateTimeColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3f57-103">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3f57-104">[columnDefinition](columndefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。</span><span class="sxs-lookup"><span data-stu-id="f3f57-104">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3f57-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3f57-105">JSON representation</span></span>

<span data-ttu-id="f3f57-106">以下は、**dateTimeColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3f57-106">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="f3f57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3f57-107">Properties</span></span>

| <span data-ttu-id="f3f57-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f3f57-108">Property name</span></span>      | <span data-ttu-id="f3f57-109">種類</span><span class="sxs-lookup"><span data-stu-id="f3f57-109">Type</span></span>               | <span data-ttu-id="f3f57-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3f57-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="f3f57-111">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="f3f57-111">**displayAs**</span></span>      | <span data-ttu-id="f3f57-112">string</span><span class="sxs-lookup"><span data-stu-id="f3f57-112">string</span></span>             | <span data-ttu-id="f3f57-113">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="f3f57-113">How the value should be presented in the UX.</span></span> <span data-ttu-id="f3f57-114">`default`、`friendly`、`standard` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f3f57-114">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="f3f57-115">詳細については、後述します。</span><span class="sxs-lookup"><span data-stu-id="f3f57-115">See below for more details.</span></span> <span data-ttu-id="f3f57-116">指定しない場合、`default` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="f3f57-116">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="f3f57-117">**format**</span><span class="sxs-lookup"><span data-stu-id="f3f57-117">**format**</span></span>         | <span data-ttu-id="f3f57-118">string</span><span class="sxs-lookup"><span data-stu-id="f3f57-118">string</span></span>             | <span data-ttu-id="f3f57-119">値を日付のみで表示するか、日付と時刻で表示するかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3f57-119">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="f3f57-120">`dateOnly` または `dateTime` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f3f57-120">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="f3f57-121">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="f3f57-121">DisplayAs values</span></span>

| <span data-ttu-id="f3f57-122">値</span><span class="sxs-lookup"><span data-stu-id="f3f57-122">Value</span></span>        | <span data-ttu-id="f3f57-123">説明</span><span class="sxs-lookup"><span data-stu-id="f3f57-123">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="f3f57-124">**default**</span><span class="sxs-lookup"><span data-stu-id="f3f57-124">**default**</span></span>  | <span data-ttu-id="f3f57-125">UX での既定のレンダリングを使用します。</span><span class="sxs-lookup"><span data-stu-id="f3f57-125">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="f3f57-126">**friendly**</span><span class="sxs-lookup"><span data-stu-id="f3f57-126">**friendly**</span></span> | <span data-ttu-id="f3f57-127">フレンドリーな相対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="f3f57-127">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="f3f57-128">「今日の午後 3:00」)</span><span class="sxs-lookup"><span data-stu-id="f3f57-128">"today at 3:00 PM")</span></span>
| <span data-ttu-id="f3f57-129">**standard**</span><span class="sxs-lookup"><span data-stu-id="f3f57-129">**standard**</span></span> | <span data-ttu-id="f3f57-130">標準の絶対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="f3f57-130">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="f3f57-131">「2017 年 5 月 10 日、午後 3:20」)</span><span class="sxs-lookup"><span data-stu-id="f3f57-131">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": []
}
-->
