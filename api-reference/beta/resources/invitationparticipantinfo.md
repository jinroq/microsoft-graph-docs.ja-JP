---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7a6fb418b7076b0f0a42dc05b6afe71dcda6a71e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865003"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="ce429-103">invitationParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce429-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="ce429-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce429-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce429-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce429-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce429-106">**InvitationParticipant**は、会話への招待に関連付けられている id のセットを表すために使用し、招待状の追加のパラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="ce429-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="ce429-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce429-107">Properties</span></span>

| <span data-ttu-id="ce429-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce429-108">Property</span></span>                           | <span data-ttu-id="ce429-109">種類</span><span class="sxs-lookup"><span data-stu-id="ce429-109">Type</span></span>                          | <span data-ttu-id="ce429-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce429-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="ce429-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="ce429-111">endpointType</span></span>                       | <span data-ttu-id="ce429-112">String</span><span class="sxs-lookup"><span data-stu-id="ce429-112">String</span></span>                        | <span data-ttu-id="ce429-113">使用可能な値は、`default`、`voicemail` です。</span><span class="sxs-lookup"><span data-stu-id="ce429-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="ce429-114">identity</span><span class="sxs-lookup"><span data-stu-id="ce429-114">identity</span></span>                           | [<span data-ttu-id="ce429-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="ce429-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="ce429-116">この招待状に関連付けられている[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="ce429-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="ce429-117">languageId</span><span class="sxs-lookup"><span data-stu-id="ce429-117">languageId</span></span>                         | <span data-ttu-id="ce429-118">String</span><span class="sxs-lookup"><span data-stu-id="ce429-118">String</span></span>                        | <span data-ttu-id="ce429-119">言語カルチャの文字列です。</span><span class="sxs-lookup"><span data-stu-id="ce429-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="ce429-120">地域</span><span class="sxs-lookup"><span data-stu-id="ce429-120">region</span></span>                             | <span data-ttu-id="ce429-121">String</span><span class="sxs-lookup"><span data-stu-id="ce429-121">String</span></span>                        | <span data-ttu-id="ce429-122">参加者の領域です。</span><span class="sxs-lookup"><span data-stu-id="ce429-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="ce429-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="ce429-123">replacesCallId</span></span>                     | <span data-ttu-id="ce429-124">String</span><span class="sxs-lookup"><span data-stu-id="ce429-124">String</span></span>                        | <span data-ttu-id="ce429-125">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ce429-125">Optional.</span></span> <span data-ttu-id="ce429-126">ターゲットの idenity がの一部である現在の呼び出しです。</span><span class="sxs-lookup"><span data-stu-id="ce429-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="ce429-127">参加者を追加するには、この呼び出しが削除されます。</span><span class="sxs-lookup"><span data-stu-id="ce429-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce429-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce429-128">JSON representation</span></span>

<span data-ttu-id="ce429-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce429-129">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
