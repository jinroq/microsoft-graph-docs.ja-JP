---
title: synchronizationSchedule リソースの種類
description: SynchronizationJob を実行するために使用するスケジュールを定義します。
localization_priority: Normal
ms.openlocfilehash: b59c36a36d837c21c147033dff8de66b85c863a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877869"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="25980-103">synchronizationSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25980-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="25980-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25980-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25980-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25980-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25980-106">の[synchronizationJob](synchronization-synchronizationjob.md)を実行するために使用するスケジュールを定義します。</span><span class="sxs-lookup"><span data-stu-id="25980-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="25980-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25980-107">Properties</span></span>
| <span data-ttu-id="25980-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25980-108">Property</span></span>     | <span data-ttu-id="25980-109">種類</span><span class="sxs-lookup"><span data-stu-id="25980-109">Type</span></span>   |<span data-ttu-id="25980-110">説明</span><span class="sxs-lookup"><span data-stu-id="25980-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25980-111">有効期限</span><span class="sxs-lookup"><span data-stu-id="25980-111">expiration</span></span>|<span data-ttu-id="25980-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25980-112">DateTimeOffset</span></span>|<span data-ttu-id="25980-113">日付と時刻がこのジョブの有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="25980-113">Date and time when this job will expire.</span></span> <span data-ttu-id="25980-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25980-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25980-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25980-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25980-116">interval</span><span class="sxs-lookup"><span data-stu-id="25980-116">interval</span></span>|<span data-ttu-id="25980-117">Duration</span><span class="sxs-lookup"><span data-stu-id="25980-117">Duration</span></span>|<span data-ttu-id="25980-118">同期のイテレーション間の間隔。</span><span class="sxs-lookup"><span data-stu-id="25980-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="25980-119">state</span><span class="sxs-lookup"><span data-stu-id="25980-119">state</span></span>|<span data-ttu-id="25980-120">String</span><span class="sxs-lookup"><span data-stu-id="25980-120">String</span></span>| <span data-ttu-id="25980-121">使用可能な値は、`Active`、`Disabled` です。</span><span class="sxs-lookup"><span data-stu-id="25980-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25980-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25980-122">JSON representation</span></span>

<span data-ttu-id="25980-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25980-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
