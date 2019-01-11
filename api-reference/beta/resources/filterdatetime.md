---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
ms.openlocfilehash: 24929695ff65173933b91fd82ac3e82de1f04da0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871310"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="3d86c-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d86c-103">FilterDatetime resource type</span></span>

> <span data-ttu-id="3d86c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d86c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d86c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d86c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d86c-106">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="3d86c-106">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="3d86c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d86c-107">Properties</span></span>
| <span data-ttu-id="3d86c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d86c-108">Property</span></span>     | <span data-ttu-id="3d86c-109">種類</span><span class="sxs-lookup"><span data-stu-id="3d86c-109">Type</span></span>   |<span data-ttu-id="3d86c-110">説明</span><span class="sxs-lookup"><span data-stu-id="3d86c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d86c-111">date</span><span class="sxs-lookup"><span data-stu-id="3d86c-111">date</span></span>|<span data-ttu-id="3d86c-112">文字列</span><span class="sxs-lookup"><span data-stu-id="3d86c-112">string</span></span>|<span data-ttu-id="3d86c-113">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="3d86c-113">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="3d86c-114">specificity</span><span class="sxs-lookup"><span data-stu-id="3d86c-114">specificity</span></span>|<span data-ttu-id="3d86c-115">文字列</span><span class="sxs-lookup"><span data-stu-id="3d86c-115">string</span></span>|<span data-ttu-id="3d86c-p102">データを保持するのに、日付をどの程度詳細に使用するか。たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。可能な値は、`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。</span><span class="sxs-lookup"><span data-stu-id="3d86c-p102">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d86c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d86c-119">Relationships</span></span>
<span data-ttu-id="3d86c-120">なし</span><span class="sxs-lookup"><span data-stu-id="3d86c-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d86c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d86c-121">JSON representation</span></span>

<span data-ttu-id="3d86c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d86c-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
