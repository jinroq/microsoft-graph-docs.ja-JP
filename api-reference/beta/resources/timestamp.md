---
title: タイムスタンプのリソースの種類
description: 時間のポイントの日付と時刻情報です。
ms.openlocfilehash: 24326f0c104dd4ee2be80016ce798cc843288975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070015"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="41809-103">タイムスタンプのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="41809-103">timeStamp resource type</span></span>

> <span data-ttu-id="41809-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41809-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41809-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41809-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41809-106">時間のポイントの日付と時刻情報です。</span><span class="sxs-lookup"><span data-stu-id="41809-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41809-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41809-107">JSON representation</span></span>

<span data-ttu-id="41809-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="41809-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="41809-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41809-109">Properties</span></span>
| <span data-ttu-id="41809-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41809-110">Property</span></span>     | <span data-ttu-id="41809-111">型</span><span class="sxs-lookup"><span data-stu-id="41809-111">Type</span></span>   |<span data-ttu-id="41809-112">説明</span><span class="sxs-lookup"><span data-stu-id="41809-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41809-113">date</span><span class="sxs-lookup"><span data-stu-id="41809-113">date</span></span>|<span data-ttu-id="41809-114">日付</span><span class="sxs-lookup"><span data-stu-id="41809-114">Date</span></span>|<span data-ttu-id="41809-115">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="41809-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="41809-116">time</span><span class="sxs-lookup"><span data-stu-id="41809-116">time</span></span>|<span data-ttu-id="41809-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="41809-117">TimeOfDay</span></span>|<span data-ttu-id="41809-118">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="41809-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="41809-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="41809-119">timeZone</span></span>|<span data-ttu-id="41809-120">String</span><span class="sxs-lookup"><span data-stu-id="41809-120">String</span></span>|<span data-ttu-id="41809-121">タイムスタンプは、世界中の 24 の前後の領域の 1 つのタイム ゾーンの部分です。</span><span class="sxs-lookup"><span data-stu-id="41809-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->