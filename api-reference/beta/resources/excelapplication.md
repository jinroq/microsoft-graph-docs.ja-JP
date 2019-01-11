---
title: アプリケーション リソースの種類
description: ブックを管理する Excel アプリケーションを表します。
localization_priority: Normal
ms.openlocfilehash: a8e2124910301818e753b1f90a3168da3a072862
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804439"
---
# <a name="application-resource-type"></a><span data-ttu-id="a7276-103">アプリケーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7276-103">Application resource type</span></span>

> <span data-ttu-id="a7276-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7276-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7276-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7276-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7276-106">ブックを管理する Excel アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="a7276-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a7276-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7276-107">Methods</span></span>

| <span data-ttu-id="a7276-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7276-108">Method</span></span>           | <span data-ttu-id="a7276-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7276-109">Return Type</span></span>    |<span data-ttu-id="a7276-110">説明</span><span class="sxs-lookup"><span data-stu-id="a7276-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7276-111">アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a7276-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="a7276-112">Application</span><span class="sxs-lookup"><span data-stu-id="a7276-112">Application</span></span>](application.md) |<span data-ttu-id="a7276-113">アプリケーション オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7276-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="a7276-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="a7276-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="a7276-115">なし</span><span class="sxs-lookup"><span data-stu-id="a7276-115">None</span></span>|<span data-ttu-id="a7276-116">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="a7276-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7276-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7276-117">Properties</span></span>
| <span data-ttu-id="a7276-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7276-118">Property</span></span>     | <span data-ttu-id="a7276-119">種類</span><span class="sxs-lookup"><span data-stu-id="a7276-119">Type</span></span>   |<span data-ttu-id="a7276-120">説明</span><span class="sxs-lookup"><span data-stu-id="a7276-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7276-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="a7276-121">calculationMode</span></span>|<span data-ttu-id="a7276-122">文字列</span><span class="sxs-lookup"><span data-stu-id="a7276-122">string</span></span>|<span data-ttu-id="a7276-123">ブックで使用される計算モードを返します。</span><span class="sxs-lookup"><span data-stu-id="a7276-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="a7276-124">可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。</span><span class="sxs-lookup"><span data-stu-id="a7276-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="a7276-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a7276-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7276-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7276-126">Relationships</span></span>
<span data-ttu-id="a7276-127">なし</span><span class="sxs-lookup"><span data-stu-id="a7276-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a7276-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7276-128">JSON representation</span></span>

<span data-ttu-id="a7276-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7276-129">Here is a JSON representation of the resource.</span></span>

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
