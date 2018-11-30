---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
ms.openlocfilehash: 8156b9f5779dd8d70ff3a839d8a6ef4f5753bacd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020349"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="db87d-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db87d-103">FilterDatetime resource type</span></span>

<span data-ttu-id="db87d-104">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="db87d-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="db87d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db87d-105">Properties</span></span>
| <span data-ttu-id="db87d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db87d-106">Property</span></span>     | <span data-ttu-id="db87d-107">型</span><span class="sxs-lookup"><span data-stu-id="db87d-107">Type</span></span>   |<span data-ttu-id="db87d-108">説明</span><span class="sxs-lookup"><span data-stu-id="db87d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db87d-109">date</span><span class="sxs-lookup"><span data-stu-id="db87d-109">date</span></span>|<span data-ttu-id="db87d-110">文字列</span><span class="sxs-lookup"><span data-stu-id="db87d-110">string</span></span>|<span data-ttu-id="db87d-111">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="db87d-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="db87d-112">specificity</span><span class="sxs-lookup"><span data-stu-id="db87d-112">specificity</span></span>|<span data-ttu-id="db87d-113">文字列</span><span class="sxs-lookup"><span data-stu-id="db87d-113">string</span></span>|<span data-ttu-id="db87d-114">特定日付に使用するデータを保持します。</span><span class="sxs-lookup"><span data-stu-id="db87d-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="db87d-115">など、この日 2005-04-02 では、specifity は、「月」に設定されて場合は、フィルター操作は 2009 年 4 月の月の日付を含むすべての行が保持されます。</span><span class="sxs-lookup"><span data-stu-id="db87d-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="db87d-116">可能な値: `Year`、 `Monday`、 `Day`、 `Hour`、 `Minute`、 `Second`。</span><span class="sxs-lookup"><span data-stu-id="db87d-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db87d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db87d-117">Relationships</span></span>
<span data-ttu-id="db87d-118">なし</span><span class="sxs-lookup"><span data-stu-id="db87d-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="db87d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db87d-119">JSON representation</span></span>

<span data-ttu-id="db87d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db87d-120">Here is a JSON representation of the resource.</span></span>

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