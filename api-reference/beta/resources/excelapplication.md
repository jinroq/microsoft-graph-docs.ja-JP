---
title: アプリケーションリソースの種類
description: ブックを管理する Excel アプリケーションを表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506532"
---
# <a name="application-resource-type"></a><span data-ttu-id="7f519-103">アプリケーションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f519-103">Application resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f519-104">ブックを管理する Excel アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="7f519-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="7f519-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f519-105">Methods</span></span>

| <span data-ttu-id="7f519-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f519-106">Method</span></span>           | <span data-ttu-id="7f519-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f519-107">Return Type</span></span>    |<span data-ttu-id="7f519-108">説明</span><span class="sxs-lookup"><span data-stu-id="7f519-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f519-109">アプリケーションを取得する</span><span class="sxs-lookup"><span data-stu-id="7f519-109">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="7f519-110">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f519-110">Application</span></span>](application.md) |<span data-ttu-id="7f519-111">アプリケーション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f519-111">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="7f519-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="7f519-112">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="7f519-113">なし</span><span class="sxs-lookup"><span data-stu-id="7f519-113">None</span></span>|<span data-ttu-id="7f519-114">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="7f519-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f519-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f519-115">Properties</span></span>
| <span data-ttu-id="7f519-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f519-116">Property</span></span>     | <span data-ttu-id="7f519-117">型</span><span class="sxs-lookup"><span data-stu-id="7f519-117">Type</span></span>   |<span data-ttu-id="7f519-118">説明</span><span class="sxs-lookup"><span data-stu-id="7f519-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f519-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="7f519-119">calculationMode</span></span>|<span data-ttu-id="7f519-120">string</span><span class="sxs-lookup"><span data-stu-id="7f519-120">string</span></span>|<span data-ttu-id="7f519-121">ブックで使用されている計算モードを返します。</span><span class="sxs-lookup"><span data-stu-id="7f519-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="7f519-122">使用可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。</span><span class="sxs-lookup"><span data-stu-id="7f519-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="7f519-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f519-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f519-124">関係</span><span class="sxs-lookup"><span data-stu-id="7f519-124">Relationships</span></span>
<span data-ttu-id="7f519-125">なし</span><span class="sxs-lookup"><span data-stu-id="7f519-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7f519-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f519-126">JSON representation</span></span>

<span data-ttu-id="7f519-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f519-127">Here is a JSON representation of the resource.</span></span>

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
