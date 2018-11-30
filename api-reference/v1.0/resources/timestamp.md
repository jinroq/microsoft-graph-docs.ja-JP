---
title: タイムスタンプのリソースの種類
description: 時間のポイントの日付と時刻情報です。
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020938"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="f1c31-103">タイムスタンプのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1c31-103">timeStamp resource type</span></span>

<span data-ttu-id="f1c31-104">時間のポイントの日付と時刻情報です。</span><span class="sxs-lookup"><span data-stu-id="f1c31-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c31-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1c31-105">JSON representation</span></span>

<span data-ttu-id="f1c31-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f1c31-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f1c31-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c31-107">Properties</span></span>
| <span data-ttu-id="f1c31-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c31-108">Property</span></span>       | <span data-ttu-id="f1c31-109">型</span><span class="sxs-lookup"><span data-stu-id="f1c31-109">Type</span></span>    |<span data-ttu-id="f1c31-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1c31-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1c31-111">date</span><span class="sxs-lookup"><span data-stu-id="f1c31-111">date</span></span>|<span data-ttu-id="f1c31-112">日付</span><span class="sxs-lookup"><span data-stu-id="f1c31-112">Date</span></span>|<span data-ttu-id="f1c31-113">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="f1c31-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="f1c31-114">time</span><span class="sxs-lookup"><span data-stu-id="f1c31-114">time</span></span>|<span data-ttu-id="f1c31-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1c31-115">TimeOfDay</span></span>|<span data-ttu-id="f1c31-116">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="f1c31-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="f1c31-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="f1c31-117">timeZone</span></span>|<span data-ttu-id="f1c31-118">String</span><span class="sxs-lookup"><span data-stu-id="f1c31-118">String</span></span>|<span data-ttu-id="f1c31-119">タイムスタンプは、世界中の 24 の前後の領域の 1 つのタイム ゾーンの部分です。</span><span class="sxs-lookup"><span data-stu-id="f1c31-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->