---
title: workbookApplication リソースの種類
description: ブックを管理する Excel workbookApplication を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 71c7c92e623fc2a9c05b9e1e8448f329615c51e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964110"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="92e1d-103">workbookApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92e1d-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92e1d-104">ブックを管理する Excel アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="92e1d-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="92e1d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="92e1d-105">Methods</span></span>

| <span data-ttu-id="92e1d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="92e1d-106">Method</span></span>           | <span data-ttu-id="92e1d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92e1d-107">Return Type</span></span>    |<span data-ttu-id="92e1d-108">説明</span><span class="sxs-lookup"><span data-stu-id="92e1d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92e1d-109">WorkbookApplication を取得する</span><span class="sxs-lookup"><span data-stu-id="92e1d-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="92e1d-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="92e1d-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="92e1d-111">WorkbookApplication オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="92e1d-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="92e1d-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="92e1d-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="92e1d-113">None</span><span class="sxs-lookup"><span data-stu-id="92e1d-113">None</span></span>|<span data-ttu-id="92e1d-114">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="92e1d-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="92e1d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e1d-115">Properties</span></span>
| <span data-ttu-id="92e1d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e1d-116">Property</span></span>     | <span data-ttu-id="92e1d-117">型</span><span class="sxs-lookup"><span data-stu-id="92e1d-117">Type</span></span>   |<span data-ttu-id="92e1d-118">説明</span><span class="sxs-lookup"><span data-stu-id="92e1d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92e1d-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="92e1d-119">calculationMode</span></span>|<span data-ttu-id="92e1d-120">string</span><span class="sxs-lookup"><span data-stu-id="92e1d-120">string</span></span>|<span data-ttu-id="92e1d-121">ブックで使用されている計算モードを返します。</span><span class="sxs-lookup"><span data-stu-id="92e1d-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="92e1d-122">可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。</span><span class="sxs-lookup"><span data-stu-id="92e1d-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="92e1d-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="92e1d-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92e1d-124">関係</span><span class="sxs-lookup"><span data-stu-id="92e1d-124">Relationships</span></span>
<span data-ttu-id="92e1d-125">なし</span><span class="sxs-lookup"><span data-stu-id="92e1d-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="92e1d-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92e1d-126">JSON representation</span></span>

<span data-ttu-id="92e1d-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92e1d-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
