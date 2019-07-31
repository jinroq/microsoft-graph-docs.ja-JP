---
title: locationConstraint リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6828d7afdb9caec79978f4196106ff687faa2a1d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009938"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="a9198-103">locationConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9198-103">locationConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9198-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="a9198-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9198-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9198-105">JSON representation</span></span>

<span data-ttu-id="a9198-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a9198-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a9198-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9198-107">Properties</span></span>
| <span data-ttu-id="a9198-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9198-108">Property</span></span>     | <span data-ttu-id="a9198-109">型</span><span class="sxs-lookup"><span data-stu-id="a9198-109">Type</span></span>   |<span data-ttu-id="a9198-110">説明</span><span class="sxs-lookup"><span data-stu-id="a9198-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9198-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="a9198-111">isRequired</span></span>|<span data-ttu-id="a9198-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9198-112">Boolean</span></span>|<span data-ttu-id="a9198-p101">クライアントは、応答に会議の場所を含めるようにサービスに要求します。この値が true で、すべてのリソースがビジー状態の場合、[findMeetingTimes](../api/user-findmeetingtimes.md) は会議時間の提案を返しません。この値が false で、すべてのリソースがビジー状態の場合は、**findMeetingTimes** は位置指定のないまま会議時間を検索します。</span><span class="sxs-lookup"><span data-stu-id="a9198-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="a9198-116">locations</span><span class="sxs-lookup"><span data-stu-id="a9198-116">locations</span></span>|<span data-ttu-id="a9198-117">[locationConstraintItem](locationconstraintitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a9198-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="a9198-118">クライアントが会議のために要求する 1 つ以上の場所に関する制約情報。</span><span class="sxs-lookup"><span data-stu-id="a9198-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="a9198-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="a9198-119">suggestLocation</span></span>|<span data-ttu-id="a9198-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9198-120">Boolean</span></span>|<span data-ttu-id="a9198-121">クライアントは、1 つ以上の会議場所を提案するようサービスに要求します。</span><span class="sxs-lookup"><span data-stu-id="a9198-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
