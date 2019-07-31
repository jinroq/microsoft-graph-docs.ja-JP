---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 62843378d53774d19ad3428e6b52c985761edda2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009770"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="02a2b-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02a2b-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a2b-104">会議の参加者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="02a2b-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="02a2b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02a2b-105">Properties</span></span>

| <span data-ttu-id="02a2b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02a2b-106">Property</span></span>       | <span data-ttu-id="02a2b-107">型</span><span class="sxs-lookup"><span data-stu-id="02a2b-107">Type</span></span>                          | <span data-ttu-id="02a2b-108">説明</span><span class="sxs-lookup"><span data-stu-id="02a2b-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="02a2b-109">独自性</span><span class="sxs-lookup"><span data-stu-id="02a2b-109">identity</span></span>       | [<span data-ttu-id="02a2b-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="02a2b-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="02a2b-111">参加者の id 情報。</span><span class="sxs-lookup"><span data-stu-id="02a2b-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="02a2b-112">プリンシパル</span><span class="sxs-lookup"><span data-stu-id="02a2b-112">upn</span></span>            | <span data-ttu-id="02a2b-113">String</span><span class="sxs-lookup"><span data-stu-id="02a2b-113">String</span></span>                        | <span data-ttu-id="02a2b-114">参加者のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="02a2b-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="02a2b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02a2b-115">JSON representation</span></span>

<span data-ttu-id="02a2b-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02a2b-116">The following is a JSON representation of the resource.</span></span>

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
