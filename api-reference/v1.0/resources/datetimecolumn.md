---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 6f2c14d5fa67fa80c869c20081250bfa55e0f5e4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267830"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="74d8d-102">DateTimeColumn リソース型</span><span class="sxs-lookup"><span data-stu-id="74d8d-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="74d8d-103">[columnDefinition](columnDefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。</span><span class="sxs-lookup"><span data-stu-id="74d8d-103">The **dateTimeColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74d8d-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74d8d-104">JSON representation</span></span>

<span data-ttu-id="74d8d-105">以下は、**dateTimeColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="74d8d-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="74d8d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74d8d-106">Properties</span></span>

| <span data-ttu-id="74d8d-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="74d8d-107">Property name</span></span>      | <span data-ttu-id="74d8d-108">型</span><span class="sxs-lookup"><span data-stu-id="74d8d-108">Type</span></span>               | <span data-ttu-id="74d8d-109">説明</span><span class="sxs-lookup"><span data-stu-id="74d8d-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="74d8d-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="74d8d-110">**displayAs**</span></span>      | <span data-ttu-id="74d8d-111">文字列</span><span class="sxs-lookup"><span data-stu-id="74d8d-111">string</span></span>             | <span data-ttu-id="74d8d-112">UX での値の表示方法です。</span><span class="sxs-lookup"><span data-stu-id="74d8d-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="74d8d-113">`default`、`friendly`、`standard` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="74d8d-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="74d8d-114">詳細については、後述します。</span><span class="sxs-lookup"><span data-stu-id="74d8d-114">See below for more details.</span></span> <span data-ttu-id="74d8d-115">指定しない場合、`default` として扱われます。</span><span class="sxs-lookup"><span data-stu-id="74d8d-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="74d8d-116">**format**</span><span class="sxs-lookup"><span data-stu-id="74d8d-116">**format**</span></span>         | <span data-ttu-id="74d8d-117">文字列</span><span class="sxs-lookup"><span data-stu-id="74d8d-117">string</span></span>             | <span data-ttu-id="74d8d-118">値を日付のみで表示するか、日付と時刻で表示するかを示します。</span><span class="sxs-lookup"><span data-stu-id="74d8d-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="74d8d-119">`dateOnly` のいずれかでなければなりません。 `dateTime`</span><span class="sxs-lookup"><span data-stu-id="74d8d-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="74d8d-120">DisplayAs オプション</span><span class="sxs-lookup"><span data-stu-id="74d8d-120">DisplayAs options</span></span>

| <span data-ttu-id="74d8d-121">値</span><span class="sxs-lookup"><span data-stu-id="74d8d-121">Value</span></span>        | <span data-ttu-id="74d8d-122">説明</span><span class="sxs-lookup"><span data-stu-id="74d8d-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="74d8d-123">**default**</span><span class="sxs-lookup"><span data-stu-id="74d8d-123">**default**</span></span>  | <span data-ttu-id="74d8d-124">UX での既定のレンダリングを使用します。</span><span class="sxs-lookup"><span data-stu-id="74d8d-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="74d8d-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="74d8d-125">**friendly**</span></span> | <span data-ttu-id="74d8d-126">フレンドリーな相対表現を使用します。(例:</span><span class="sxs-lookup"><span data-stu-id="74d8d-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="74d8d-127">「今日の午後 3:00」)</span><span class="sxs-lookup"><span data-stu-id="74d8d-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="74d8d-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="74d8d-128">**standard**</span></span> | <span data-ttu-id="74d8d-129">標準の絶対表現を使用します。(例:</span><span class="sxs-lookup"><span data-stu-id="74d8d-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="74d8d-130">「2017 年 5 月 10 日、午後 3:20」)</span><span class="sxs-lookup"><span data-stu-id="74d8d-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
