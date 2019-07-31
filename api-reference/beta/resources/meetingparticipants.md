---
title: 会議参加者リソースの種類
description: 会議の参加者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b88a59b3d9def58217ca3badd833b275760b49c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966834"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="6b2c3-103">会議参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b2c3-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b2c3-104">会議の参加者。</span><span class="sxs-lookup"><span data-stu-id="6b2c3-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="6b2c3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b2c3-105">Properties</span></span>

| <span data-ttu-id="6b2c3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b2c3-106">Property</span></span>       | <span data-ttu-id="6b2c3-107">型</span><span class="sxs-lookup"><span data-stu-id="6b2c3-107">Type</span></span>    | <span data-ttu-id="6b2c3-108">説明</span><span class="sxs-lookup"><span data-stu-id="6b2c3-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b2c3-109">attendees</span><span class="sxs-lookup"><span data-stu-id="6b2c3-109">attendees</span></span> | <span data-ttu-id="6b2c3-110">[meetingParticipantInfo](meetingparticipantinfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6b2c3-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="6b2c3-111">構成内容変更</span><span class="sxs-lookup"><span data-stu-id="6b2c3-111">organizer</span></span> | [<span data-ttu-id="6b2c3-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6b2c3-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="6b2c3-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b2c3-113">JSON representation</span></span>

<span data-ttu-id="6b2c3-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b2c3-114">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
