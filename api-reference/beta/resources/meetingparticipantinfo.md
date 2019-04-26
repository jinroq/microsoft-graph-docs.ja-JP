---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3df338760bd1d2ff74cc79c706944c9b5fa7104d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342395"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="dc48e-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc48e-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc48e-104">会議の参加者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="dc48e-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="dc48e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc48e-105">Properties</span></span>

| <span data-ttu-id="dc48e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc48e-106">Property</span></span>       | <span data-ttu-id="dc48e-107">型</span><span class="sxs-lookup"><span data-stu-id="dc48e-107">Type</span></span>                          | <span data-ttu-id="dc48e-108">説明</span><span class="sxs-lookup"><span data-stu-id="dc48e-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="dc48e-109">独自性</span><span class="sxs-lookup"><span data-stu-id="dc48e-109">identity</span></span>       | [<span data-ttu-id="dc48e-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="dc48e-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="dc48e-111">参加者の id 情報。</span><span class="sxs-lookup"><span data-stu-id="dc48e-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="dc48e-112">プリンシパル</span><span class="sxs-lookup"><span data-stu-id="dc48e-112">upn</span></span>            | <span data-ttu-id="dc48e-113">String</span><span class="sxs-lookup"><span data-stu-id="dc48e-113">String</span></span>                        | <span data-ttu-id="dc48e-114">参加者のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="dc48e-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="dc48e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc48e-115">JSON representation</span></span>

<span data-ttu-id="dc48e-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc48e-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
