---
title: privilegedApproval リソースの種類
description: 要求された特権 Id 管理の役割に承認を表します。
ms.openlocfilehash: 3f900ef4a141b2f71c303becd49789b86cefb1b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070367"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="9e1d7-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e1d7-103">privilegedApproval resource type</span></span>

> <span data-ttu-id="9e1d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e1d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e1d7-106">要求された特権 Id 管理の役割に承認を表します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-106">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="9e1d7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9e1d7-107">Methods</span></span>

| <span data-ttu-id="9e1d7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9e1d7-108">Method</span></span>           | <span data-ttu-id="9e1d7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9e1d7-109">Return Type</span></span>    |<span data-ttu-id="9e1d7-110">説明</span><span class="sxs-lookup"><span data-stu-id="9e1d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e1d7-111">PrivilegedApproval を取得します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-111">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="9e1d7-112">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9e1d7-112">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="9e1d7-113">PrivilegedApproval オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-113">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="9e1d7-114">PrivilegedApproval オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="9e1d7-114">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="9e1d7-115">[privilegedApproval](privilegedapproval.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9e1d7-115">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="9e1d7-116">PrivilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-116">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="9e1d7-117">PrivilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-117">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="9e1d7-118">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9e1d7-118">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="9e1d7-119">PrivilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-119">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="9e1d7-120">PrivilegedApproval を更新します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-120">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="9e1d7-121">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9e1d7-121">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="9e1d7-122">PrivilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-122">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="9e1d7-123">Myrequests</span><span class="sxs-lookup"><span data-stu-id="9e1d7-123">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="9e1d7-124">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9e1d7-124">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="9e1d7-125">要求側の承認の要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-125">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e1d7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e1d7-126">Properties</span></span>
| <span data-ttu-id="9e1d7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e1d7-127">Property</span></span>     | <span data-ttu-id="9e1d7-128">型</span><span class="sxs-lookup"><span data-stu-id="9e1d7-128">Type</span></span>   |<span data-ttu-id="9e1d7-129">説明</span><span class="sxs-lookup"><span data-stu-id="9e1d7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e1d7-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="9e1d7-130">approvalDuration</span></span>|<span data-ttu-id="9e1d7-131">Duration</span><span class="sxs-lookup"><span data-stu-id="9e1d7-131">Duration</span></span>||
|<span data-ttu-id="9e1d7-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="9e1d7-132">approvalState</span></span>|<span data-ttu-id="9e1d7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9e1d7-133">string</span></span>| <span data-ttu-id="9e1d7-134">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="9e1d7-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="9e1d7-135">approvalType</span></span>|<span data-ttu-id="9e1d7-136">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-136">String</span></span>||
|<span data-ttu-id="9e1d7-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="9e1d7-137">approverReason</span></span>|<span data-ttu-id="9e1d7-138">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-138">String</span></span>||
|<span data-ttu-id="9e1d7-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e1d7-139">endDateTime</span></span>|<span data-ttu-id="9e1d7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e1d7-140">DateTimeOffset</span></span>|<span data-ttu-id="9e1d7-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e1d7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e1d7-143">id</span><span class="sxs-lookup"><span data-stu-id="9e1d7-143">id</span></span>|<span data-ttu-id="9e1d7-144">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-144">String</span></span>| <span data-ttu-id="9e1d7-145">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-145">Read-only.</span></span>|
|<span data-ttu-id="9e1d7-146">requestorReason</span><span class="sxs-lookup"><span data-stu-id="9e1d7-146">requestorReason</span></span>|<span data-ttu-id="9e1d7-147">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-147">String</span></span>||
|<span data-ttu-id="9e1d7-148">roleId</span><span class="sxs-lookup"><span data-stu-id="9e1d7-148">roleId</span></span>|<span data-ttu-id="9e1d7-149">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-149">String</span></span>||
|<span data-ttu-id="9e1d7-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e1d7-150">startDateTime</span></span>|<span data-ttu-id="9e1d7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e1d7-151">DateTimeOffset</span></span>|<span data-ttu-id="9e1d7-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e1d7-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e1d7-154">userId</span><span class="sxs-lookup"><span data-stu-id="9e1d7-154">userId</span></span>|<span data-ttu-id="9e1d7-155">String</span><span class="sxs-lookup"><span data-stu-id="9e1d7-155">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="9e1d7-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9e1d7-156">Relationships</span></span>
| <span data-ttu-id="9e1d7-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9e1d7-157">Relationship</span></span> | <span data-ttu-id="9e1d7-158">型</span><span class="sxs-lookup"><span data-stu-id="9e1d7-158">Type</span></span>   |<span data-ttu-id="9e1d7-159">説明</span><span class="sxs-lookup"><span data-stu-id="9e1d7-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e1d7-160">roleInfo</span><span class="sxs-lookup"><span data-stu-id="9e1d7-160">roleInfo</span></span>|[<span data-ttu-id="9e1d7-161">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9e1d7-161">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="9e1d7-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="9e1d7-164">要求</span><span class="sxs-lookup"><span data-stu-id="9e1d7-164">request</span></span>|[<span data-ttu-id="9e1d7-165">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9e1d7-165">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="9e1d7-166">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-166">Read-only.</span></span> <span data-ttu-id="9e1d7-167">この承認オブジェクトのロール割り当ての依頼</span><span class="sxs-lookup"><span data-stu-id="9e1d7-167">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e1d7-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e1d7-168">JSON representation</span></span>
<span data-ttu-id="9e1d7-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9e1d7-169">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->