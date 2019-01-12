---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 409cf7eff4b1151a0ded11674fcde36a519f0e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924483"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="cab95-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cab95-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="cab95-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cab95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cab95-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cab95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cab95-106">会議の参加者に関する情報です。</span><span class="sxs-lookup"><span data-stu-id="cab95-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="cab95-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cab95-107">Properties</span></span>

| <span data-ttu-id="cab95-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cab95-108">Property</span></span>       | <span data-ttu-id="cab95-109">型</span><span class="sxs-lookup"><span data-stu-id="cab95-109">Type</span></span>                          | <span data-ttu-id="cab95-110">説明</span><span class="sxs-lookup"><span data-stu-id="cab95-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="cab95-111">identity</span><span class="sxs-lookup"><span data-stu-id="cab95-111">identity</span></span>       | [<span data-ttu-id="cab95-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="cab95-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="cab95-113">参加者の識別情報です。</span><span class="sxs-lookup"><span data-stu-id="cab95-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="cab95-114">upn</span><span class="sxs-lookup"><span data-stu-id="cab95-114">upn</span></span>            | <span data-ttu-id="cab95-115">String</span><span class="sxs-lookup"><span data-stu-id="cab95-115">String</span></span>                        | <span data-ttu-id="cab95-116">参加者のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="cab95-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cab95-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cab95-117">JSON representation</span></span>

<span data-ttu-id="cab95-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cab95-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
