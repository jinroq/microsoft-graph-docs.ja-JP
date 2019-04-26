---
title: 組織の情報リソースの種類
description: 会議の開催者を含むミーティング情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 129e8a60edd89d45eb6e48715a59231475d52b99
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341761"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="3be34-103">組織の情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3be34-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be34-104">会議の開催者を含むミーティング情報。</span><span class="sxs-lookup"><span data-stu-id="3be34-104">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="3be34-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3be34-105">Properties</span></span>

| <span data-ttu-id="3be34-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3be34-106">Property</span></span>                     | <span data-ttu-id="3be34-107">型</span><span class="sxs-lookup"><span data-stu-id="3be34-107">Type</span></span>                          | <span data-ttu-id="3be34-108">説明</span><span class="sxs-lookup"><span data-stu-id="3be34-108">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="3be34-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="3be34-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="3be34-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="3be34-110">Boolean</span></span>                       | <span data-ttu-id="3be34-111">会話のホストが離れると、会話が続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3be34-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="3be34-112">organizer</span><span class="sxs-lookup"><span data-stu-id="3be34-112">organizer</span></span>                    | [<span data-ttu-id="3be34-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3be34-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="3be34-114">開催者 Azure Active Directory の id。</span><span class="sxs-lookup"><span data-stu-id="3be34-114">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3be34-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3be34-115">JSON representation</span></span>

<span data-ttu-id="3be34-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3be34-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.meetingInfo",
   "openType": true,
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="3be34-117">例</span><span class="sxs-lookup"><span data-stu-id="3be34-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
