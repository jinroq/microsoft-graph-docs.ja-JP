---
title: organizerMeetingInfo リソースの種類
description: 会議については、会議の開催者を含みます。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: fd096a55762892ca9b2fd72c883a544e503c5f90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870733"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="aa6d0-103">organizerMeetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa6d0-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="aa6d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa6d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa6d0-106">会議については、会議の開催者を含みます。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="aa6d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa6d0-107">Properties</span></span>

| <span data-ttu-id="aa6d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa6d0-108">Property</span></span>                     | <span data-ttu-id="aa6d0-109">種類</span><span class="sxs-lookup"><span data-stu-id="aa6d0-109">Type</span></span>                          | <span data-ttu-id="aa6d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa6d0-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="aa6d0-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="aa6d0-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="aa6d0-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="aa6d0-112">Boolean</span></span>                       | <span data-ttu-id="aa6d0-113">会話のホストから離れると、会話を続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="aa6d0-114">organizer</span><span class="sxs-lookup"><span data-stu-id="aa6d0-114">organizer</span></span>                    | [<span data-ttu-id="aa6d0-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="aa6d0-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="aa6d0-116">開催者は Azure Active Directory アイデンティティであります。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="aa6d0-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa6d0-117">JSON representation</span></span>

<span data-ttu-id="aa6d0-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa6d0-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="aa6d0-119">例</span><span class="sxs-lookup"><span data-stu-id="aa6d0-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
