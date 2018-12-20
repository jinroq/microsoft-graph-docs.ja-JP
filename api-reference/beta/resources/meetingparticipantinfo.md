---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報です。
author: VinodRavichandran
ms.openlocfilehash: 2bbb410ea26640ec05d66b5beb0c4b4ea24a42bd
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380199"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="a1716-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1716-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="a1716-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1716-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1716-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1716-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1716-106">会議の参加者に関する情報です。</span><span class="sxs-lookup"><span data-stu-id="a1716-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="a1716-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1716-107">Properties</span></span>

| <span data-ttu-id="a1716-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1716-108">Property</span></span>       | <span data-ttu-id="a1716-109">型</span><span class="sxs-lookup"><span data-stu-id="a1716-109">Type</span></span>                          | <span data-ttu-id="a1716-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1716-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="a1716-111">identity</span><span class="sxs-lookup"><span data-stu-id="a1716-111">identity</span></span>       | [<span data-ttu-id="a1716-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1716-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="a1716-113">参加者の識別情報です。</span><span class="sxs-lookup"><span data-stu-id="a1716-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="a1716-114">upn</span><span class="sxs-lookup"><span data-stu-id="a1716-114">upn</span></span>            | <span data-ttu-id="a1716-115">String</span><span class="sxs-lookup"><span data-stu-id="a1716-115">String</span></span>                        | <span data-ttu-id="a1716-116">参加者のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="a1716-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a1716-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1716-117">JSON representation</span></span>

<span data-ttu-id="a1716-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1716-118">The following is a JSON representation of the resource.</span></span>

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
