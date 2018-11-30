---
title: assignedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの両方の **assignedPlans** プロパティは、**assignedPlan** のコレクションです。
ms.openlocfilehash: 0df1540819b569b62607bf0e56c1c8f53d2749da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066764"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="9f97f-103">assignedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f97f-103">assignedPlan resource type</span></span>

> <span data-ttu-id="9f97f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f97f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f97f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f97f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f97f-106">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの両方の **assignedPlans** プロパティは、**assignedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9f97f-106">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="9f97f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f97f-107">Properties</span></span>
| <span data-ttu-id="9f97f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f97f-108">Property</span></span>     | <span data-ttu-id="9f97f-109">型</span><span class="sxs-lookup"><span data-stu-id="9f97f-109">Type</span></span>   |<span data-ttu-id="9f97f-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f97f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f97f-111">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f97f-111">assignedDateTime</span></span>|<span data-ttu-id="9f97f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f97f-112">DateTimeOffset</span></span>|<span data-ttu-id="9f97f-p102">プランが割り当てられた日時です。例:2013-01-02T19:32:30Z。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9f97f-p102">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9f97f-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9f97f-116">capabilityStatus</span></span>|<span data-ttu-id="9f97f-117">String</span><span class="sxs-lookup"><span data-stu-id="9f97f-117">String</span></span>|<span data-ttu-id="9f97f-118">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="9f97f-118">For example, “Enabled”.</span></span>|
|<span data-ttu-id="9f97f-119">service</span><span class="sxs-lookup"><span data-stu-id="9f97f-119">service</span></span>|<span data-ttu-id="9f97f-120">String</span><span class="sxs-lookup"><span data-stu-id="9f97f-120">String</span></span>|<span data-ttu-id="9f97f-121">サービスの名前。「Exchange」など。</span><span class="sxs-lookup"><span data-stu-id="9f97f-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="9f97f-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="9f97f-122">servicePlanId</span></span>|<span data-ttu-id="9f97f-123">Guid</span><span class="sxs-lookup"><span data-stu-id="9f97f-123">Guid</span></span>|<span data-ttu-id="9f97f-124">サービス プランを識別する GUID。</span><span class="sxs-lookup"><span data-stu-id="9f97f-124">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f97f-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f97f-125">JSON representation</span></span>

<span data-ttu-id="9f97f-126">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9f97f-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
