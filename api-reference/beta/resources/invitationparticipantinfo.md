---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641919"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="f42be-103">invitationParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f42be-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f42be-104">**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="f42be-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="f42be-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f42be-105">Properties</span></span>

| <span data-ttu-id="f42be-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f42be-106">Property</span></span>                           | <span data-ttu-id="f42be-107">型</span><span class="sxs-lookup"><span data-stu-id="f42be-107">Type</span></span>                          | <span data-ttu-id="f42be-108">説明</span><span class="sxs-lookup"><span data-stu-id="f42be-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="f42be-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="f42be-109">endpointType</span></span>                       | <span data-ttu-id="f42be-110">String</span><span class="sxs-lookup"><span data-stu-id="f42be-110">String</span></span>                        | <span data-ttu-id="f42be-111">使用可能な値は、`default`、`voicemail` です。</span><span class="sxs-lookup"><span data-stu-id="f42be-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="f42be-112">identity</span><span class="sxs-lookup"><span data-stu-id="f42be-112">identity</span></span>                           | [<span data-ttu-id="f42be-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="f42be-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="f42be-114">この招待状に関連付けられている[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="f42be-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="f42be-115">languageId</span><span class="sxs-lookup"><span data-stu-id="f42be-115">languageId</span></span>                         | <span data-ttu-id="f42be-116">String</span><span class="sxs-lookup"><span data-stu-id="f42be-116">String</span></span>                        | <span data-ttu-id="f42be-117">言語カルチャの文字列です。</span><span class="sxs-lookup"><span data-stu-id="f42be-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="f42be-118">地域</span><span class="sxs-lookup"><span data-stu-id="f42be-118">region</span></span>                             | <span data-ttu-id="f42be-119">String</span><span class="sxs-lookup"><span data-stu-id="f42be-119">String</span></span>                        | <span data-ttu-id="f42be-120">参加者の領域です。</span><span class="sxs-lookup"><span data-stu-id="f42be-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="f42be-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="f42be-121">replacesCallId</span></span>                     | <span data-ttu-id="f42be-122">String</span><span class="sxs-lookup"><span data-stu-id="f42be-122">String</span></span>                        | <span data-ttu-id="f42be-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f42be-123">Optional.</span></span> <span data-ttu-id="f42be-124">ターゲットの idenity がの一部である現在の呼び出しです。</span><span class="sxs-lookup"><span data-stu-id="f42be-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="f42be-125">参加者を追加するには、この呼び出しが削除されます。</span><span class="sxs-lookup"><span data-stu-id="f42be-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f42be-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f42be-126">JSON representation</span></span>

<span data-ttu-id="f42be-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f42be-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
