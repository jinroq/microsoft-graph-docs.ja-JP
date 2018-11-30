---
title: organizerMeetingInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 00a7978c44c82ddd6b34802f29188a554e7e0b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070346"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="e8fda-103">organizerMeetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8fda-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="e8fda-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8fda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8fda-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8fda-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="e8fda-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8fda-106">Properties</span></span>

| <span data-ttu-id="e8fda-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8fda-107">Property</span></span>                     | <span data-ttu-id="e8fda-108">型</span><span class="sxs-lookup"><span data-stu-id="e8fda-108">Type</span></span>                          | <span data-ttu-id="e8fda-109">説明</span><span class="sxs-lookup"><span data-stu-id="e8fda-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="e8fda-110">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="e8fda-110">allowConversationWithoutHost</span></span> | <span data-ttu-id="e8fda-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="e8fda-111">Boolean</span></span>                       | <span data-ttu-id="e8fda-112">会話のホストから離れると、会話を続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8fda-112">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="e8fda-113">organizer</span><span class="sxs-lookup"><span data-stu-id="e8fda-113">organizer</span></span>                    | [<span data-ttu-id="e8fda-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="e8fda-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="e8fda-115">開催者は Azure Active Directory アイデンティティであります。</span><span class="sxs-lookup"><span data-stu-id="e8fda-115">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e8fda-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8fda-116">JSON representation</span></span>

<span data-ttu-id="e8fda-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8fda-117">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e8fda-118">使用例</span><span class="sxs-lookup"><span data-stu-id="e8fda-118">Example</span></span>

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
