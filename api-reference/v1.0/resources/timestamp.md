---
title: timeStamp リソースの種類
description: 特定の時点の日付と時刻の情報。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33dbc9821d2a58763d81249aebe21a9a2c3aee08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033587"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="f1c14-103">timeStamp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1c14-103">timeStamp resource type</span></span>

<span data-ttu-id="f1c14-104">特定の時点の日付と時刻の情報。</span><span class="sxs-lookup"><span data-stu-id="f1c14-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c14-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1c14-105">JSON representation</span></span>

<span data-ttu-id="f1c14-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f1c14-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f1c14-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c14-107">Properties</span></span>
| <span data-ttu-id="f1c14-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c14-108">Property</span></span>       | <span data-ttu-id="f1c14-109">型</span><span class="sxs-lookup"><span data-stu-id="f1c14-109">Type</span></span>    |<span data-ttu-id="f1c14-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1c14-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1c14-111">date</span><span class="sxs-lookup"><span data-stu-id="f1c14-111">date</span></span>|<span data-ttu-id="f1c14-112">日付</span><span class="sxs-lookup"><span data-stu-id="f1c14-112">Date</span></span>|<span data-ttu-id="f1c14-113">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="f1c14-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="f1c14-114">time</span><span class="sxs-lookup"><span data-stu-id="f1c14-114">time</span></span>|<span data-ttu-id="f1c14-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1c14-115">TimeOfDay</span></span>|<span data-ttu-id="f1c14-116">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="f1c14-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="f1c14-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="f1c14-117">timeZone</span></span>|<span data-ttu-id="f1c14-118">String</span><span class="sxs-lookup"><span data-stu-id="f1c14-118">String</span></span>|<span data-ttu-id="f1c14-119">タイムスタンプのタイムゾーン部分。世界中の24の前後の地域の1つです。</span><span class="sxs-lookup"><span data-stu-id="f1c14-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
