---
title: recordingInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 92af3fcb52ab08f3f25a2c16cc720a4053a9bdfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069798"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="6f07b-103">recordingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f07b-103">recordingInfo resource type</span></span>

> <span data-ttu-id="6f07b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f07b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f07b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f07b-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="6f07b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f07b-106">Properties</span></span>

| <span data-ttu-id="6f07b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f07b-107">Property</span></span>       | <span data-ttu-id="6f07b-108">型</span><span class="sxs-lookup"><span data-stu-id="6f07b-108">Type</span></span>    | <span data-ttu-id="6f07b-109">説明</span><span class="sxs-lookup"><span data-stu-id="6f07b-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f07b-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6f07b-110">initiatedBy</span></span> | [<span data-ttu-id="6f07b-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="6f07b-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="6f07b-112">レコーディングを開始した参加者です。</span><span class="sxs-lookup"><span data-stu-id="6f07b-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="6f07b-113">status</span><span class="sxs-lookup"><span data-stu-id="6f07b-113">status</span></span> | <span data-ttu-id="6f07b-114">String</span><span class="sxs-lookup"><span data-stu-id="6f07b-114">String</span></span> | <span data-ttu-id="6f07b-115">可能な値は、`recordingCapable`、`notRecording`、`startedRecording` です。</span><span class="sxs-lookup"><span data-stu-id="6f07b-115">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f07b-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f07b-116">JSON representation</span></span>

<span data-ttu-id="6f07b-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f07b-117">The following is a JSON representation of the resource.</span></span>

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
