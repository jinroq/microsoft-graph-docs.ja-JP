---
title: タイムスタンプのリソースの種類
description: 時間のポイントの日付と時刻情報です。
localization_priority: Normal
ms.openlocfilehash: b3e6e7384c9efdcb0e606f91d7357272f27ceaa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830227"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="9b9b0-103">タイムスタンプのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b9b0-103">timeStamp resource type</span></span>

> <span data-ttu-id="9b9b0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b9b0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b9b0-106">時間のポイントの日付と時刻情報です。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b9b0-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b9b0-107">JSON representation</span></span>

<span data-ttu-id="9b9b0-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9b9b0-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9b9b0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b9b0-109">Properties</span></span>
| <span data-ttu-id="9b9b0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b9b0-110">Property</span></span>     | <span data-ttu-id="9b9b0-111">種類</span><span class="sxs-lookup"><span data-stu-id="9b9b0-111">Type</span></span>   |<span data-ttu-id="9b9b0-112">説明</span><span class="sxs-lookup"><span data-stu-id="9b9b0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b9b0-113">date</span><span class="sxs-lookup"><span data-stu-id="9b9b0-113">date</span></span>|<span data-ttu-id="9b9b0-114">日付</span><span class="sxs-lookup"><span data-stu-id="9b9b0-114">Date</span></span>|<span data-ttu-id="9b9b0-115">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="9b9b0-116">time</span><span class="sxs-lookup"><span data-stu-id="9b9b0-116">time</span></span>|<span data-ttu-id="9b9b0-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b9b0-117">TimeOfDay</span></span>|<span data-ttu-id="9b9b0-118">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="9b9b0-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="9b9b0-119">timeZone</span></span>|<span data-ttu-id="9b9b0-120">String</span><span class="sxs-lookup"><span data-stu-id="9b9b0-120">String</span></span>|<span data-ttu-id="9b9b0-121">タイムスタンプは、世界中の 24 の前後の領域の 1 つのタイム ゾーンの部分です。</span><span class="sxs-lookup"><span data-stu-id="9b9b0-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
