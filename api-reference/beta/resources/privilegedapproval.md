---
title: privilegedApproval リソースの種類
description: 要求された特権 Id 管理の役割に承認を表します。
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643875"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="7ad73-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ad73-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad73-104">要求された特権 Id 管理の役割に承認を表します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="7ad73-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ad73-105">Methods</span></span>

| <span data-ttu-id="7ad73-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7ad73-106">Method</span></span>           | <span data-ttu-id="7ad73-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7ad73-107">Return Type</span></span>    |<span data-ttu-id="7ad73-108">説明</span><span class="sxs-lookup"><span data-stu-id="7ad73-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ad73-109">PrivilegedApproval を取得します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="7ad73-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7ad73-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7ad73-111">PrivilegedApproval オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ad73-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="7ad73-112">PrivilegedApproval オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="7ad73-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="7ad73-113">[privilegedApproval](privilegedapproval.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ad73-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="7ad73-114">PrivilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="7ad73-115">PrivilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="7ad73-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7ad73-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="7ad73-117">PrivilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="7ad73-118">PrivilegedApproval を更新します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="7ad73-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7ad73-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7ad73-120">PrivilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="7ad73-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="7ad73-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="7ad73-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7ad73-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="7ad73-123">要求側の承認の要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="7ad73-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ad73-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ad73-124">Properties</span></span>
| <span data-ttu-id="7ad73-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ad73-125">Property</span></span>     | <span data-ttu-id="7ad73-126">型</span><span class="sxs-lookup"><span data-stu-id="7ad73-126">Type</span></span>   |<span data-ttu-id="7ad73-127">説明</span><span class="sxs-lookup"><span data-stu-id="7ad73-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ad73-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="7ad73-128">approvalDuration</span></span>|<span data-ttu-id="7ad73-129">Duration</span><span class="sxs-lookup"><span data-stu-id="7ad73-129">Duration</span></span>||
|<span data-ttu-id="7ad73-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="7ad73-130">approvalState</span></span>|<span data-ttu-id="7ad73-131">string</span><span class="sxs-lookup"><span data-stu-id="7ad73-131">string</span></span>| <span data-ttu-id="7ad73-132">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="7ad73-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="7ad73-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="7ad73-133">approvalType</span></span>|<span data-ttu-id="7ad73-134">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-134">String</span></span>||
|<span data-ttu-id="7ad73-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="7ad73-135">approverReason</span></span>|<span data-ttu-id="7ad73-136">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-136">String</span></span>||
|<span data-ttu-id="7ad73-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad73-137">endDateTime</span></span>|<span data-ttu-id="7ad73-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad73-138">DateTimeOffset</span></span>|<span data-ttu-id="7ad73-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7ad73-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7ad73-141">id</span><span class="sxs-lookup"><span data-stu-id="7ad73-141">id</span></span>|<span data-ttu-id="7ad73-142">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-142">String</span></span>| <span data-ttu-id="7ad73-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7ad73-143">Read-only.</span></span>|
|<span data-ttu-id="7ad73-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="7ad73-144">requestorReason</span></span>|<span data-ttu-id="7ad73-145">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-145">String</span></span>||
|<span data-ttu-id="7ad73-146">roleId</span><span class="sxs-lookup"><span data-stu-id="7ad73-146">roleId</span></span>|<span data-ttu-id="7ad73-147">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-147">String</span></span>||
|<span data-ttu-id="7ad73-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad73-148">startDateTime</span></span>|<span data-ttu-id="7ad73-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad73-149">DateTimeOffset</span></span>|<span data-ttu-id="7ad73-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7ad73-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7ad73-152">userId</span><span class="sxs-lookup"><span data-stu-id="7ad73-152">userId</span></span>|<span data-ttu-id="7ad73-153">String</span><span class="sxs-lookup"><span data-stu-id="7ad73-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="7ad73-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7ad73-154">Relationships</span></span>
| <span data-ttu-id="7ad73-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7ad73-155">Relationship</span></span> | <span data-ttu-id="7ad73-156">型</span><span class="sxs-lookup"><span data-stu-id="7ad73-156">Type</span></span>   |<span data-ttu-id="7ad73-157">説明</span><span class="sxs-lookup"><span data-stu-id="7ad73-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ad73-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="7ad73-158">roleInfo</span></span>|[<span data-ttu-id="7ad73-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7ad73-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7ad73-p103">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="7ad73-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="7ad73-162">要求</span><span class="sxs-lookup"><span data-stu-id="7ad73-162">request</span></span>|[<span data-ttu-id="7ad73-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7ad73-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="7ad73-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7ad73-164">Read-only.</span></span> <span data-ttu-id="7ad73-165">この承認オブジェクトのロール割り当ての依頼</span><span class="sxs-lookup"><span data-stu-id="7ad73-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ad73-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ad73-166">JSON representation</span></span>
<span data-ttu-id="7ad73-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7ad73-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
