---
title: locationConstraint リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
ms.openlocfilehash: e15acbac529179b0d79fd8b9b52f691fa9ef1322
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573033"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="324bc-103">locationConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="324bc-103">locationConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="324bc-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="324bc-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="324bc-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="324bc-105">JSON representation</span></span>

<span data-ttu-id="324bc-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="324bc-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="324bc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="324bc-107">Properties</span></span>
| <span data-ttu-id="324bc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="324bc-108">Property</span></span>     | <span data-ttu-id="324bc-109">型</span><span class="sxs-lookup"><span data-stu-id="324bc-109">Type</span></span>   |<span data-ttu-id="324bc-110">説明</span><span class="sxs-lookup"><span data-stu-id="324bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="324bc-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="324bc-111">isRequired</span></span>|<span data-ttu-id="324bc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="324bc-112">Boolean</span></span>|<span data-ttu-id="324bc-p101">クライアントは、応答に会議の場所を含めるようにサービスに要求します。この値が true で、すべてのリソースがビジー状態の場合、[findMeetingTimes](../api/user-findmeetingtimes.md) は会議時間の提案を返しません。この値が false で、すべてのリソースがビジー状態の場合は、**findMeetingTimes** は位置指定のないまま会議時間を検索します。</span><span class="sxs-lookup"><span data-stu-id="324bc-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="324bc-116">locations</span><span class="sxs-lookup"><span data-stu-id="324bc-116">locations</span></span>|<span data-ttu-id="324bc-117">[locationConstraintItem](locationconstraintitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="324bc-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="324bc-118">クライアントが会議のために要求する 1 つ以上の場所に関する制約情報。</span><span class="sxs-lookup"><span data-stu-id="324bc-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="324bc-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="324bc-119">suggestLocation</span></span>|<span data-ttu-id="324bc-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="324bc-120">Boolean</span></span>|<span data-ttu-id="324bc-121">クライアントは、1 つ以上の会議場所を提案するようサービスに要求します。</span><span class="sxs-lookup"><span data-stu-id="324bc-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
