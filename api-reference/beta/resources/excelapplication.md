---
title: アプリケーション リソースの種類
description: ブックを管理する Excel アプリケーションを表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921977"
---
# <a name="application-resource-type"></a><span data-ttu-id="43589-103">アプリケーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43589-103">Application resource type</span></span>

> <span data-ttu-id="43589-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43589-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43589-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43589-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43589-106">ブックを管理する Excel アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="43589-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="43589-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="43589-107">Methods</span></span>

| <span data-ttu-id="43589-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="43589-108">Method</span></span>           | <span data-ttu-id="43589-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43589-109">Return Type</span></span>    |<span data-ttu-id="43589-110">説明</span><span class="sxs-lookup"><span data-stu-id="43589-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43589-111">アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="43589-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="43589-112">Application</span><span class="sxs-lookup"><span data-stu-id="43589-112">Application</span></span>](application.md) |<span data-ttu-id="43589-113">アプリケーション オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43589-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="43589-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="43589-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="43589-115">なし</span><span class="sxs-lookup"><span data-stu-id="43589-115">None</span></span>|<span data-ttu-id="43589-116">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="43589-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="43589-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43589-117">Properties</span></span>
| <span data-ttu-id="43589-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43589-118">Property</span></span>     | <span data-ttu-id="43589-119">種類</span><span class="sxs-lookup"><span data-stu-id="43589-119">Type</span></span>   |<span data-ttu-id="43589-120">説明</span><span class="sxs-lookup"><span data-stu-id="43589-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43589-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="43589-121">calculationMode</span></span>|<span data-ttu-id="43589-122">文字列</span><span class="sxs-lookup"><span data-stu-id="43589-122">string</span></span>|<span data-ttu-id="43589-123">ブックで使用される計算モードを返します。</span><span class="sxs-lookup"><span data-stu-id="43589-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="43589-124">可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。</span><span class="sxs-lookup"><span data-stu-id="43589-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="43589-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43589-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43589-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43589-126">Relationships</span></span>
<span data-ttu-id="43589-127">なし</span><span class="sxs-lookup"><span data-stu-id="43589-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="43589-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43589-128">JSON representation</span></span>

<span data-ttu-id="43589-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43589-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
