---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dd1e6d7f0a4ae9c17794035c8103cda8d189d5ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569061"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="094cf-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="094cf-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="094cf-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="094cf-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="094cf-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="094cf-105">Methods</span></span>
<span data-ttu-id="094cf-106">なし</span><span class="sxs-lookup"><span data-stu-id="094cf-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="094cf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="094cf-107">Properties</span></span>
<span data-ttu-id="094cf-108">なし</span><span class="sxs-lookup"><span data-stu-id="094cf-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="094cf-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="094cf-109">Relationships</span></span>
| <span data-ttu-id="094cf-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="094cf-110">Relationship</span></span> | <span data-ttu-id="094cf-111">型</span><span class="sxs-lookup"><span data-stu-id="094cf-111">Type</span></span>   |<span data-ttu-id="094cf-112">説明</span><span class="sxs-lookup"><span data-stu-id="094cf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="094cf-113">line</span><span class="sxs-lookup"><span data-stu-id="094cf-113">line</span></span>|[<span data-ttu-id="094cf-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="094cf-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="094cf-115">グラフの線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="094cf-115">Represents chart line formatting.</span></span> <span data-ttu-id="094cf-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="094cf-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="094cf-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="094cf-117">JSON representation</span></span>

<span data-ttu-id="094cf-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="094cf-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
