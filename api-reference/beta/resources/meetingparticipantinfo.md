---
title: meetingParticipantInfo リソースの種類
description: 会議の参加者に関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457117"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="94525-103">meetingParticipantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94525-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94525-104">会議の参加者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="94525-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="94525-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94525-105">Properties</span></span>

| <span data-ttu-id="94525-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94525-106">Property</span></span>       | <span data-ttu-id="94525-107">型</span><span class="sxs-lookup"><span data-stu-id="94525-107">Type</span></span>                          | <span data-ttu-id="94525-108">説明</span><span class="sxs-lookup"><span data-stu-id="94525-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="94525-109">独自性</span><span class="sxs-lookup"><span data-stu-id="94525-109">identity</span></span>       | [<span data-ttu-id="94525-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="94525-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="94525-111">参加者の id 情報。</span><span class="sxs-lookup"><span data-stu-id="94525-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="94525-112">プリンシパル</span><span class="sxs-lookup"><span data-stu-id="94525-112">upn</span></span>            | <span data-ttu-id="94525-113">String</span><span class="sxs-lookup"><span data-stu-id="94525-113">String</span></span>                        | <span data-ttu-id="94525-114">参加者のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="94525-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="94525-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94525-115">JSON representation</span></span>

<span data-ttu-id="94525-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94525-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
