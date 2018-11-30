---
title: meetingParticipantInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070142"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="8b2e6-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b2e6-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="8b2e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b2e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b2e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b2e6-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="8b2e6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2e6-106">Properties</span></span>

| <span data-ttu-id="8b2e6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2e6-107">Property</span></span>       | <span data-ttu-id="8b2e6-108">型</span><span class="sxs-lookup"><span data-stu-id="8b2e6-108">Type</span></span>                          | <span data-ttu-id="8b2e6-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b2e6-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="8b2e6-110">identity</span><span class="sxs-lookup"><span data-stu-id="8b2e6-110">identity</span></span>       | [<span data-ttu-id="8b2e6-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="8b2e6-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="8b2e6-112">参加者の識別情報です。</span><span class="sxs-lookup"><span data-stu-id="8b2e6-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="8b2e6-113">upn</span><span class="sxs-lookup"><span data-stu-id="8b2e6-113">upn</span></span>            | <span data-ttu-id="8b2e6-114">String</span><span class="sxs-lookup"><span data-stu-id="8b2e6-114">String</span></span>                        | <span data-ttu-id="8b2e6-115">参加者のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="8b2e6-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8b2e6-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b2e6-116">JSON representation</span></span>

<span data-ttu-id="8b2e6-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b2e6-117">The following is a JSON representation of the resource.</span></span>

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
