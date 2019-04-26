---
title: invitationParticipantInfo リソースの種類
description: '**InvitationParticipant**は、会話出席依頼に関連付けられている id のセットを表すために使用され、追加の招待パラメーターを提供します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569964"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="2c13b-103">invitationParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c13b-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c13b-104">**InvitationParticipant**は、会話出席依頼に関連付けられている id のセットを表すために使用され、追加の招待パラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="2c13b-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="2c13b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c13b-105">Properties</span></span>

| <span data-ttu-id="2c13b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c13b-106">Property</span></span>                           | <span data-ttu-id="2c13b-107">型</span><span class="sxs-lookup"><span data-stu-id="2c13b-107">Type</span></span>                          | <span data-ttu-id="2c13b-108">説明</span><span class="sxs-lookup"><span data-stu-id="2c13b-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="2c13b-109">endpointtype</span><span class="sxs-lookup"><span data-stu-id="2c13b-109">endpointType</span></span>                       | <span data-ttu-id="2c13b-110">String</span><span class="sxs-lookup"><span data-stu-id="2c13b-110">String</span></span>                        | <span data-ttu-id="2c13b-111">使用可能な値は、`default`、`voicemail` です。</span><span class="sxs-lookup"><span data-stu-id="2c13b-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="2c13b-112">独自性</span><span class="sxs-lookup"><span data-stu-id="2c13b-112">identity</span></span>                           | [<span data-ttu-id="2c13b-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c13b-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="2c13b-114">この招待に関連付けられている id[セット](identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="2c13b-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="2c13b-115">languageId</span><span class="sxs-lookup"><span data-stu-id="2c13b-115">languageId</span></span>                         | <span data-ttu-id="2c13b-116">String</span><span class="sxs-lookup"><span data-stu-id="2c13b-116">String</span></span>                        | <span data-ttu-id="2c13b-117">言語のカルチャ文字列。</span><span class="sxs-lookup"><span data-stu-id="2c13b-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="2c13b-118">エリア</span><span class="sxs-lookup"><span data-stu-id="2c13b-118">region</span></span>                             | <span data-ttu-id="2c13b-119">String</span><span class="sxs-lookup"><span data-stu-id="2c13b-119">String</span></span>                        | <span data-ttu-id="2c13b-120">参加者の地域。</span><span class="sxs-lookup"><span data-stu-id="2c13b-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="2c13b-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="2c13b-121">replacesCallId</span></span>                     | <span data-ttu-id="2c13b-122">文字列</span><span class="sxs-lookup"><span data-stu-id="2c13b-122">String</span></span>                        | <span data-ttu-id="2c13b-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2c13b-123">Optional.</span></span> <span data-ttu-id="2c13b-124">ターゲット id が現在一部である通話。</span><span class="sxs-lookup"><span data-stu-id="2c13b-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="2c13b-125">この呼び出しは、参加者が追加されると削除されます。</span><span class="sxs-lookup"><span data-stu-id="2c13b-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c13b-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c13b-126">JSON representation</span></span>

<span data-ttu-id="2c13b-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c13b-127">The following is a JSON representation of the resource.</span></span>

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
