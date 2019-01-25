---
title: アプリケーション リソースの種類
description: ブックを管理する Excel アプリケーションを表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517618"
---
# <a name="application-resource-type"></a><span data-ttu-id="46d79-103">アプリケーション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46d79-103">Application resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d79-104">ブックを管理する Excel アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="46d79-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="46d79-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="46d79-105">Methods</span></span>

| <span data-ttu-id="46d79-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="46d79-106">Method</span></span>           | <span data-ttu-id="46d79-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="46d79-107">Return Type</span></span>    |<span data-ttu-id="46d79-108">説明</span><span class="sxs-lookup"><span data-stu-id="46d79-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46d79-109">アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="46d79-109">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="46d79-110">Application</span><span class="sxs-lookup"><span data-stu-id="46d79-110">Application</span></span>](application.md) |<span data-ttu-id="46d79-111">アプリケーション オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46d79-111">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="46d79-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="46d79-112">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="46d79-113">なし</span><span class="sxs-lookup"><span data-stu-id="46d79-113">None</span></span>|<span data-ttu-id="46d79-114">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="46d79-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="46d79-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46d79-115">Properties</span></span>
| <span data-ttu-id="46d79-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46d79-116">Property</span></span>     | <span data-ttu-id="46d79-117">型</span><span class="sxs-lookup"><span data-stu-id="46d79-117">Type</span></span>   |<span data-ttu-id="46d79-118">説明</span><span class="sxs-lookup"><span data-stu-id="46d79-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46d79-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="46d79-119">calculationMode</span></span>|<span data-ttu-id="46d79-120">文字列</span><span class="sxs-lookup"><span data-stu-id="46d79-120">string</span></span>|<span data-ttu-id="46d79-121">ブックで使用される計算モードを返します。</span><span class="sxs-lookup"><span data-stu-id="46d79-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="46d79-122">可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。</span><span class="sxs-lookup"><span data-stu-id="46d79-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="46d79-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46d79-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46d79-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46d79-124">Relationships</span></span>
<span data-ttu-id="46d79-125">なし</span><span class="sxs-lookup"><span data-stu-id="46d79-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="46d79-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46d79-126">JSON representation</span></span>

<span data-ttu-id="46d79-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46d79-127">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
