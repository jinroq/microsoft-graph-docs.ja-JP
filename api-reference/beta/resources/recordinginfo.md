---
title: recordingInfo リソースの種類
description: 参加者に関する情報を記録します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6025259bafdcff78c3c7dbfa19aa39f5f6648f84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563141"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="3371a-103">recordingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3371a-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3371a-104">参加者に関する情報を記録します。</span><span class="sxs-lookup"><span data-stu-id="3371a-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="3371a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3371a-105">Properties</span></span>

| <span data-ttu-id="3371a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3371a-106">Property</span></span>       | <span data-ttu-id="3371a-107">型</span><span class="sxs-lookup"><span data-stu-id="3371a-107">Type</span></span>    | <span data-ttu-id="3371a-108">説明</span><span class="sxs-lookup"><span data-stu-id="3371a-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3371a-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="3371a-109">initiatedBy</span></span> | [<span data-ttu-id="3371a-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="3371a-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="3371a-111">レコーディングを開始した参加者。</span><span class="sxs-lookup"><span data-stu-id="3371a-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="3371a-112">status</span><span class="sxs-lookup"><span data-stu-id="3371a-112">status</span></span> | <span data-ttu-id="3371a-113">String</span><span class="sxs-lookup"><span data-stu-id="3371a-113">String</span></span> | <span data-ttu-id="3371a-114">可能な値は `recordingCapable`、`notRecording`、`startedRecording` です。</span><span class="sxs-lookup"><span data-stu-id="3371a-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3371a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3371a-115">JSON representation</span></span>

<span data-ttu-id="3371a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3371a-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
