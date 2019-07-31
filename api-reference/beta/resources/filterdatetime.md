---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 27dafb0583380af299a4f5d8632c60a7e8af1a54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973556"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="66679-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66679-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66679-104">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="66679-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="66679-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66679-105">Properties</span></span>
| <span data-ttu-id="66679-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66679-106">Property</span></span>     | <span data-ttu-id="66679-107">型</span><span class="sxs-lookup"><span data-stu-id="66679-107">Type</span></span>   |<span data-ttu-id="66679-108">説明</span><span class="sxs-lookup"><span data-stu-id="66679-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66679-109">date</span><span class="sxs-lookup"><span data-stu-id="66679-109">date</span></span>|<span data-ttu-id="66679-110">string</span><span class="sxs-lookup"><span data-stu-id="66679-110">string</span></span>|<span data-ttu-id="66679-111">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="66679-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="66679-112">specificity</span><span class="sxs-lookup"><span data-stu-id="66679-112">specificity</span></span>|<span data-ttu-id="66679-113">string</span><span class="sxs-lookup"><span data-stu-id="66679-113">string</span></span>|<span data-ttu-id="66679-p101">データを保持するのに、日付をどの程度詳細に使用するか。たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。可能な値は、`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。</span><span class="sxs-lookup"><span data-stu-id="66679-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66679-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66679-117">Relationships</span></span>
<span data-ttu-id="66679-118">なし</span><span class="sxs-lookup"><span data-stu-id="66679-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="66679-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66679-119">JSON representation</span></span>

<span data-ttu-id="66679-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66679-120">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
