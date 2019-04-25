---
title: FilterDatetime リソースの種類
description: 値をフィルター処理するときに日付をフィルター処理する方法を表します。
localization_priority: Normal
ms.openlocfilehash: 26d42b45a2e9b9cdd279f33330a877a64ea1c8d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564247"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="a9c1b-103">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9c1b-103">FilterDatetime resource type</span></span>

<span data-ttu-id="a9c1b-104">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="a9c1b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9c1b-105">Properties</span></span>
| <span data-ttu-id="a9c1b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9c1b-106">Property</span></span>     | <span data-ttu-id="a9c1b-107">型</span><span class="sxs-lookup"><span data-stu-id="a9c1b-107">Type</span></span>   |<span data-ttu-id="a9c1b-108">説明</span><span class="sxs-lookup"><span data-stu-id="a9c1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9c1b-109">date</span><span class="sxs-lookup"><span data-stu-id="a9c1b-109">date</span></span>|<span data-ttu-id="a9c1b-110">string</span><span class="sxs-lookup"><span data-stu-id="a9c1b-110">string</span></span>|<span data-ttu-id="a9c1b-111">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="a9c1b-112">specificity</span><span class="sxs-lookup"><span data-stu-id="a9c1b-112">specificity</span></span>|<span data-ttu-id="a9c1b-113">string</span><span class="sxs-lookup"><span data-stu-id="a9c1b-113">string</span></span>|<span data-ttu-id="a9c1b-114">データを保持するのに、日付をどの程度詳細に使用するか。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="a9c1b-115">たとえば、date が 2005-04-02 で "month" に設定した場合、フィルター操作では 2005 年 4 月の日付データを含むすべての行が保持されます。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="a9c1b-116">使用可能な値は`Year`、 `Monday`、 `Day` `Hour` `Minute`、、、 `Second`、です。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9c1b-117">関係</span><span class="sxs-lookup"><span data-stu-id="a9c1b-117">Relationships</span></span>
<span data-ttu-id="a9c1b-118">なし</span><span class="sxs-lookup"><span data-stu-id="a9c1b-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9c1b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9c1b-119">JSON representation</span></span>

<span data-ttu-id="a9c1b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a9c1b-120">Here is a JSON representation of the resource.</span></span>

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
