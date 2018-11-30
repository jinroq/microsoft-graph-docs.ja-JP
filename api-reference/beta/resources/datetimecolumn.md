---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067197"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="932c0-102">DateTimeColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="932c0-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="932c0-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="932c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="932c0-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="932c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="932c0-105">[columnDefinition](columndefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。</span><span class="sxs-lookup"><span data-stu-id="932c0-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="932c0-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="932c0-106">JSON representation</span></span>

<span data-ttu-id="932c0-107">以下は、**dateTimeColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="932c0-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="932c0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="932c0-108">Properties</span></span>

| <span data-ttu-id="932c0-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="932c0-109">Property name</span></span>      | <span data-ttu-id="932c0-110">型</span><span class="sxs-lookup"><span data-stu-id="932c0-110">Type</span></span>               | <span data-ttu-id="932c0-111">説明</span><span class="sxs-lookup"><span data-stu-id="932c0-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="932c0-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="932c0-112">**displayAs**</span></span>      | <span data-ttu-id="932c0-113">文字列</span><span class="sxs-lookup"><span data-stu-id="932c0-113">string</span></span>             | <span data-ttu-id="932c0-114">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="932c0-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="932c0-115">`default`、`friendly`、`standard` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="932c0-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="932c0-116">詳細については、後述します。</span><span class="sxs-lookup"><span data-stu-id="932c0-116">See below for more details.</span></span> <span data-ttu-id="932c0-117">指定しない場合、`default` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="932c0-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="932c0-118">**format**</span><span class="sxs-lookup"><span data-stu-id="932c0-118">**format**</span></span>         | <span data-ttu-id="932c0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="932c0-119">string</span></span>             | <span data-ttu-id="932c0-120">値を日付のみで表示するか、日付と時刻で表示するかを示します。</span><span class="sxs-lookup"><span data-stu-id="932c0-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="932c0-121">`dateOnly` または `dateTime` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="932c0-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="932c0-122">DisplayAs 値</span><span class="sxs-lookup"><span data-stu-id="932c0-122">DisplayAs values</span></span>

| <span data-ttu-id="932c0-123">値</span><span class="sxs-lookup"><span data-stu-id="932c0-123">Value</span></span>        | <span data-ttu-id="932c0-124">説明</span><span class="sxs-lookup"><span data-stu-id="932c0-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="932c0-125">**default**</span><span class="sxs-lookup"><span data-stu-id="932c0-125">**default**</span></span>  | <span data-ttu-id="932c0-126">UX での既定のレンダリングを使用します。</span><span class="sxs-lookup"><span data-stu-id="932c0-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="932c0-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="932c0-127">**friendly**</span></span> | <span data-ttu-id="932c0-128">フレンドリーな相対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="932c0-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="932c0-129">「今日の午後 3:00」)</span><span class="sxs-lookup"><span data-stu-id="932c0-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="932c0-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="932c0-130">**standard**</span></span> | <span data-ttu-id="932c0-131">標準の絶対表現を使用します。(例: </span><span class="sxs-lookup"><span data-stu-id="932c0-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="932c0-132">「2017 年 5 月 10 日、午後 3:20」)</span><span class="sxs-lookup"><span data-stu-id="932c0-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
