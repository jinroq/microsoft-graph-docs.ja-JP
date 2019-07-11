---
title: 同期スケジュールリソースの種類
description: 同期ジョブの実行に使用されるスケジュールを定義します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f6802f6a5a17de53ec070621c87d077dd1b45f87
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620704"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="32243-103">同期スケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="32243-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32243-104">[同期ジョブ](synchronization-synchronizationjob.md)の実行に使用されるスケジュールを定義します。</span><span class="sxs-lookup"><span data-stu-id="32243-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="32243-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32243-105">Properties</span></span>
| <span data-ttu-id="32243-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32243-106">Property</span></span>     | <span data-ttu-id="32243-107">型</span><span class="sxs-lookup"><span data-stu-id="32243-107">Type</span></span>   |<span data-ttu-id="32243-108">説明</span><span class="sxs-lookup"><span data-stu-id="32243-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32243-109">nntp</span><span class="sxs-lookup"><span data-stu-id="32243-109">expiration</span></span>|<span data-ttu-id="32243-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32243-110">DateTimeOffset</span></span>|<span data-ttu-id="32243-111">このジョブの有効期限が切れる日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="32243-111">Date and time when this job will expire.</span></span> <span data-ttu-id="32243-112">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="32243-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="32243-113">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="32243-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="32243-114">interval</span><span class="sxs-lookup"><span data-stu-id="32243-114">interval</span></span>|<span data-ttu-id="32243-115">期間</span><span class="sxs-lookup"><span data-stu-id="32243-115">Duration</span></span>|<span data-ttu-id="32243-116">同期の反復間の間隔。</span><span class="sxs-lookup"><span data-stu-id="32243-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="32243-117">state</span><span class="sxs-lookup"><span data-stu-id="32243-117">state</span></span>|<span data-ttu-id="32243-118">String</span><span class="sxs-lookup"><span data-stu-id="32243-118">String</span></span>| <span data-ttu-id="32243-119">使用可能な値は、`Active`、`Disabled` です。</span><span class="sxs-lookup"><span data-stu-id="32243-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32243-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32243-120">JSON representation</span></span>

<span data-ttu-id="32243-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32243-121">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
