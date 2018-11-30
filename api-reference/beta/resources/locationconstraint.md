---
title: locationConstraint リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
ms.openlocfilehash: d151ea97aa65aabdb759be4cb90b577606c648a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068182"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="30e57-103">locationConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30e57-103">locationConstraint resource type</span></span>

> <span data-ttu-id="30e57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30e57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30e57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30e57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30e57-106">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="30e57-106">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30e57-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30e57-107">JSON representation</span></span>

<span data-ttu-id="30e57-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="30e57-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationconstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="30e57-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30e57-109">Properties</span></span>
| <span data-ttu-id="30e57-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30e57-110">Property</span></span>     | <span data-ttu-id="30e57-111">型</span><span class="sxs-lookup"><span data-stu-id="30e57-111">Type</span></span>   |<span data-ttu-id="30e57-112">説明</span><span class="sxs-lookup"><span data-stu-id="30e57-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30e57-113">isRequired</span><span class="sxs-lookup"><span data-stu-id="30e57-113">isRequired</span></span>|<span data-ttu-id="30e57-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="30e57-114">Boolean</span></span>|<span data-ttu-id="30e57-p102">クライアントは、応答に会議の場所を含めるようにサービスに要求します。この値が true で、すべてのリソースがビジー状態の場合、[findMeetingTimes](../api/user-findmeetingtimes.md) は会議時間の提案を返しません。この値が false で、すべてのリソースがビジー状態の場合は、**findMeetingTimes** は位置指定のないまま会議時間を検索します。</span><span class="sxs-lookup"><span data-stu-id="30e57-p102">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="30e57-118">locations</span><span class="sxs-lookup"><span data-stu-id="30e57-118">locations</span></span>|<span data-ttu-id="30e57-119">[locationConstraintItem](locationconstraintitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="30e57-119">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="30e57-120">クライアントが会議のために要求する 1 つ以上の場所に関する制約情報。</span><span class="sxs-lookup"><span data-stu-id="30e57-120">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="30e57-121">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="30e57-121">suggestLocation</span></span>|<span data-ttu-id="30e57-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="30e57-122">Boolean</span></span>|<span data-ttu-id="30e57-123">クライアントは、1 つ以上の会議場所を提案するようサービスに要求します。</span><span class="sxs-lookup"><span data-stu-id="30e57-123">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->