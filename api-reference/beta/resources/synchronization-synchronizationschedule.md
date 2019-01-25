---
title: synchronizationSchedule リソースの種類
description: SynchronizationJob を実行するために使用するスケジュールを定義します。
localization_priority: Normal
ms.openlocfilehash: 0e9714e4833c5586e54c8d812a0d72e41a513e5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515588"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="cca05-103">synchronizationSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cca05-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cca05-104">の[synchronizationJob](synchronization-synchronizationjob.md)を実行するために使用するスケジュールを定義します。</span><span class="sxs-lookup"><span data-stu-id="cca05-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cca05-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cca05-105">Properties</span></span>
| <span data-ttu-id="cca05-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cca05-106">Property</span></span>     | <span data-ttu-id="cca05-107">型</span><span class="sxs-lookup"><span data-stu-id="cca05-107">Type</span></span>   |<span data-ttu-id="cca05-108">説明</span><span class="sxs-lookup"><span data-stu-id="cca05-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cca05-109">有効期限</span><span class="sxs-lookup"><span data-stu-id="cca05-109">expiration</span></span>|<span data-ttu-id="cca05-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cca05-110">DateTimeOffset</span></span>|<span data-ttu-id="cca05-111">日付と時刻がこのジョブの有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="cca05-111">Date and time when this job will expire.</span></span> <span data-ttu-id="cca05-112">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cca05-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cca05-113">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="cca05-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cca05-114">interval</span><span class="sxs-lookup"><span data-stu-id="cca05-114">interval</span></span>|<span data-ttu-id="cca05-115">Duration</span><span class="sxs-lookup"><span data-stu-id="cca05-115">Duration</span></span>|<span data-ttu-id="cca05-116">同期のイテレーション間の間隔。</span><span class="sxs-lookup"><span data-stu-id="cca05-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="cca05-117">state</span><span class="sxs-lookup"><span data-stu-id="cca05-117">state</span></span>|<span data-ttu-id="cca05-118">String</span><span class="sxs-lookup"><span data-stu-id="cca05-118">String</span></span>| <span data-ttu-id="cca05-119">使用可能な値は、`Active`、`Disabled` です。</span><span class="sxs-lookup"><span data-stu-id="cca05-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cca05-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cca05-120">JSON representation</span></span>

<span data-ttu-id="cca05-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cca05-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
