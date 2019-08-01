---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e2938c151e052372df1b959e6e24d4a2c0d94ea4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032460"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="c3cb9-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3cb9-103">FilterDatetime resource type</span></span>

<span data-ttu-id="c3cb9-104">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="c3cb9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3cb9-105">Properties</span></span>
| <span data-ttu-id="c3cb9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3cb9-106">Property</span></span>     | <span data-ttu-id="c3cb9-107">型</span><span class="sxs-lookup"><span data-stu-id="c3cb9-107">Type</span></span>   |<span data-ttu-id="c3cb9-108">説明</span><span class="sxs-lookup"><span data-stu-id="c3cb9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3cb9-109">date</span><span class="sxs-lookup"><span data-stu-id="c3cb9-109">date</span></span>|<span data-ttu-id="c3cb9-110">string</span><span class="sxs-lookup"><span data-stu-id="c3cb9-110">string</span></span>|<span data-ttu-id="c3cb9-111">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="c3cb9-112">specificity</span><span class="sxs-lookup"><span data-stu-id="c3cb9-112">specificity</span></span>|<span data-ttu-id="c3cb9-113">string</span><span class="sxs-lookup"><span data-stu-id="c3cb9-113">string</span></span>|<span data-ttu-id="c3cb9-114">データを保持するのに、日付をどの程度詳細に使用するか。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="c3cb9-115">たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="c3cb9-116">使用可能な値: `Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3cb9-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3cb9-117">Relationships</span></span>
<span data-ttu-id="c3cb9-118">なし</span><span class="sxs-lookup"><span data-stu-id="c3cb9-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3cb9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3cb9-119">JSON representation</span></span>

<span data-ttu-id="c3cb9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3cb9-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
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
