---
title: locationconstraints リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9ac80069a7ffe61171a9e24feb2e65895c469bd
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057398"
---
# <a name="locationconstraints-resource-type"></a><span data-ttu-id="59a0e-103">locationconstraints リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59a0e-103">locationConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59a0e-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="59a0e-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59a0e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59a0e-105">JSON representation</span></span>

<span data-ttu-id="59a0e-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="59a0e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraints"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="59a0e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59a0e-107">Properties</span></span>
| <span data-ttu-id="59a0e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59a0e-108">Property</span></span>     | <span data-ttu-id="59a0e-109">型</span><span class="sxs-lookup"><span data-stu-id="59a0e-109">Type</span></span>   |<span data-ttu-id="59a0e-110">説明</span><span class="sxs-lookup"><span data-stu-id="59a0e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59a0e-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="59a0e-111">isRequired</span></span>|<span data-ttu-id="59a0e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="59a0e-112">Boolean</span></span>|<span data-ttu-id="59a0e-p101">クライアントは、応答に会議の場所を含めるようにサービスに要求します。この値が true で、すべてのリソースがビジー状態の場合、[findMeetingTimes](../api/user-findmeetingtimes.md) は会議時間の提案を返しません。この値が false で、すべてのリソースがビジー状態の場合は、**findMeetingTimes** は位置指定のないまま会議時間を検索します。</span><span class="sxs-lookup"><span data-stu-id="59a0e-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="59a0e-116">locations</span><span class="sxs-lookup"><span data-stu-id="59a0e-116">locations</span></span>|<span data-ttu-id="59a0e-117">[locationConstraintItem](locationconstraintitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59a0e-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="59a0e-118">クライアントが会議のために要求する 1 つ以上の場所に関する制約情報。</span><span class="sxs-lookup"><span data-stu-id="59a0e-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="59a0e-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="59a0e-119">suggestLocation</span></span>|<span data-ttu-id="59a0e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="59a0e-120">Boolean</span></span>|<span data-ttu-id="59a0e-121">クライアントは、1 つ以上の会議場所を提案するようサービスに要求します。</span><span class="sxs-lookup"><span data-stu-id="59a0e-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->