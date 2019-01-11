---
title: recordingInfo リソースの種類
description: 参加者の情報を記録します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 85c2710452905f97235928bae71ff60c2d22983f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891939"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="d1d1c-103">recordingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1d1c-103">recordingInfo resource type</span></span>

> <span data-ttu-id="d1d1c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1d1c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1d1c-106">参加者の情報を記録します。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="d1d1c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1d1c-107">Properties</span></span>

| <span data-ttu-id="d1d1c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1d1c-108">Property</span></span>       | <span data-ttu-id="d1d1c-109">種類</span><span class="sxs-lookup"><span data-stu-id="d1d1c-109">Type</span></span>    | <span data-ttu-id="d1d1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1d1c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1d1c-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d1d1c-111">initiatedBy</span></span> | [<span data-ttu-id="d1d1c-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="d1d1c-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="d1d1c-113">レコーディングを開始した参加者です。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="d1d1c-114">status</span><span class="sxs-lookup"><span data-stu-id="d1d1c-114">status</span></span> | <span data-ttu-id="d1d1c-115">String</span><span class="sxs-lookup"><span data-stu-id="d1d1c-115">String</span></span> | <span data-ttu-id="d1d1c-116">可能な値は、`recordingCapable`、`notRecording`、`startedRecording` です。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1d1c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1d1c-117">JSON representation</span></span>

<span data-ttu-id="d1d1c-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1d1c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
