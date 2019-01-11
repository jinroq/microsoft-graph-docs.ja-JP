---
title: meetingParticipants リソースの種類
description: 会議の参加者です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: fad06a015429a7264d808b4997c94e90e4799825
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815121"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="08a4e-103">meetingParticipants リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08a4e-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="08a4e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08a4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08a4e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08a4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08a4e-106">会議の参加者です。</span><span class="sxs-lookup"><span data-stu-id="08a4e-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="08a4e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08a4e-107">Properties</span></span>

| <span data-ttu-id="08a4e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08a4e-108">Property</span></span>       | <span data-ttu-id="08a4e-109">種類</span><span class="sxs-lookup"><span data-stu-id="08a4e-109">Type</span></span>    | <span data-ttu-id="08a4e-110">説明</span><span class="sxs-lookup"><span data-stu-id="08a4e-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08a4e-111">attendees</span><span class="sxs-lookup"><span data-stu-id="08a4e-111">attendees</span></span> | <span data-ttu-id="08a4e-112">[meetingParticipantInfo](meetingparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="08a4e-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="08a4e-113">organizer</span><span class="sxs-lookup"><span data-stu-id="08a4e-113">organizer</span></span> | [<span data-ttu-id="08a4e-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="08a4e-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="08a4e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08a4e-115">JSON representation</span></span>

<span data-ttu-id="08a4e-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08a4e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
