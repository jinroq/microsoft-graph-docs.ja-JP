---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507552"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="12ae8-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12ae8-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12ae8-104">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="12ae8-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="12ae8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12ae8-105">Properties</span></span>
| <span data-ttu-id="12ae8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12ae8-106">Property</span></span>     | <span data-ttu-id="12ae8-107">型</span><span class="sxs-lookup"><span data-stu-id="12ae8-107">Type</span></span>   |<span data-ttu-id="12ae8-108">説明</span><span class="sxs-lookup"><span data-stu-id="12ae8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12ae8-109">date</span><span class="sxs-lookup"><span data-stu-id="12ae8-109">date</span></span>|<span data-ttu-id="12ae8-110">string</span><span class="sxs-lookup"><span data-stu-id="12ae8-110">string</span></span>|<span data-ttu-id="12ae8-111">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="12ae8-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="12ae8-112">specificity</span><span class="sxs-lookup"><span data-stu-id="12ae8-112">specificity</span></span>|<span data-ttu-id="12ae8-113">string</span><span class="sxs-lookup"><span data-stu-id="12ae8-113">string</span></span>|<span data-ttu-id="12ae8-p101">データを保持するのに、日付をどの程度詳細に使用するか。たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。可能な値は、`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。</span><span class="sxs-lookup"><span data-stu-id="12ae8-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12ae8-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12ae8-117">Relationships</span></span>
<span data-ttu-id="12ae8-118">なし</span><span class="sxs-lookup"><span data-stu-id="12ae8-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="12ae8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12ae8-119">JSON representation</span></span>

<span data-ttu-id="12ae8-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12ae8-120">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
