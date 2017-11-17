---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="8d1c8-102">DateTimeColumn リソース型</span><span class="sxs-lookup"><span data-stu-id="8d1c8-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="8d1c8-103">[columnDefinition](columnDefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-103">The **dateTimeColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d1c8-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d1c8-104">JSON representation</span></span>

<span data-ttu-id="8d1c8-105">以下は、**dateTimeColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="8d1c8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d1c8-106">Properties</span></span>

| <span data-ttu-id="8d1c8-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8d1c8-107">Property name</span></span>      | <span data-ttu-id="8d1c8-108">種類</span><span class="sxs-lookup"><span data-stu-id="8d1c8-108">Type</span></span>               | <span data-ttu-id="8d1c8-109">説明</span><span class="sxs-lookup"><span data-stu-id="8d1c8-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="8d1c8-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8d1c8-110">**displayAs**</span></span>      | <span data-ttu-id="8d1c8-111">string</span><span class="sxs-lookup"><span data-stu-id="8d1c8-111">string</span></span>             | <span data-ttu-id="8d1c8-112">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="8d1c8-113">`default`、`friendly`、`standard` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="8d1c8-114">詳細については、後述します。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-114">Read below for more details.</span></span> <span data-ttu-id="8d1c8-115">指定しない場合、`default` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="8d1c8-116">**format**</span><span class="sxs-lookup"><span data-stu-id="8d1c8-116">**format**</span></span>         | <span data-ttu-id="8d1c8-117">string</span><span class="sxs-lookup"><span data-stu-id="8d1c8-117">string</span></span>             | <span data-ttu-id="8d1c8-118">値を日付のみで表示するか、日付と時刻で表示するかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="8d1c8-119">`dateOnly` または `dateTime` のいずれかでなければなりません</span><span class="sxs-lookup"><span data-stu-id="8d1c8-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="8d1c8-120">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="8d1c8-120">DisplayAs values</span></span>

| <span data-ttu-id="8d1c8-121">値</span><span class="sxs-lookup"><span data-stu-id="8d1c8-121">Value</span></span>        | <span data-ttu-id="8d1c8-122">説明</span><span class="sxs-lookup"><span data-stu-id="8d1c8-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="8d1c8-123">**default**</span><span class="sxs-lookup"><span data-stu-id="8d1c8-123">**default**</span></span>  | <span data-ttu-id="8d1c8-124">UX での既定のレンダリングを使用します。</span><span class="sxs-lookup"><span data-stu-id="8d1c8-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="8d1c8-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="8d1c8-125">**friendly**</span></span> | <span data-ttu-id="8d1c8-126">フレンドリな相対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="8d1c8-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="8d1c8-127">「今日の午後 3:00」)</span><span class="sxs-lookup"><span data-stu-id="8d1c8-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="8d1c8-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="8d1c8-128">**Standard**</span></span> | <span data-ttu-id="8d1c8-129">標準の絶対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="8d1c8-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="8d1c8-130">「2017 年 5 月 10 日、午後 3:20」)</span><span class="sxs-lookup"><span data-stu-id="8d1c8-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
