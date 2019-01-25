---
title: タイムスタンプのリソースの種類
description: 時間のポイントの日付と時刻情報です。
localization_priority: Normal
ms.openlocfilehash: 79faa8f74fbaf64eb6756183ecc309c6522873e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529363"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="319fa-103">タイムスタンプのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="319fa-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="319fa-104">時間のポイントの日付と時刻情報です。</span><span class="sxs-lookup"><span data-stu-id="319fa-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="319fa-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="319fa-105">JSON representation</span></span>

<span data-ttu-id="319fa-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="319fa-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="319fa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319fa-107">Properties</span></span>
| <span data-ttu-id="319fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319fa-108">Property</span></span>     | <span data-ttu-id="319fa-109">型</span><span class="sxs-lookup"><span data-stu-id="319fa-109">Type</span></span>   |<span data-ttu-id="319fa-110">説明</span><span class="sxs-lookup"><span data-stu-id="319fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="319fa-111">date</span><span class="sxs-lookup"><span data-stu-id="319fa-111">date</span></span>|<span data-ttu-id="319fa-112">日付</span><span class="sxs-lookup"><span data-stu-id="319fa-112">Date</span></span>|<span data-ttu-id="319fa-113">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="319fa-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="319fa-114">time</span><span class="sxs-lookup"><span data-stu-id="319fa-114">time</span></span>|<span data-ttu-id="319fa-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="319fa-115">TimeOfDay</span></span>|<span data-ttu-id="319fa-116">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="319fa-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="319fa-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="319fa-117">timeZone</span></span>|<span data-ttu-id="319fa-118">String</span><span class="sxs-lookup"><span data-stu-id="319fa-118">String</span></span>|<span data-ttu-id="319fa-119">タイムスタンプは、世界中の 24 の前後の領域の 1 つのタイム ゾーンの部分です。</span><span class="sxs-lookup"><span data-stu-id="319fa-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timestamp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
