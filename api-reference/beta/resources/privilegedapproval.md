---
title: privilegedApproval リソースの種類
description: 要求された特権 Id 管理の役割に承認を表します。
localization_priority: Normal
ms.openlocfilehash: dee8cffba02270308c6786b2549b66aa5ad9dfa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868349"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="cbd6b-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbd6b-103">privilegedApproval resource type</span></span>

> <span data-ttu-id="cbd6b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd6b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbd6b-106">要求された特権 Id 管理の役割に承認を表します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-106">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="cbd6b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbd6b-107">Methods</span></span>

| <span data-ttu-id="cbd6b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbd6b-108">Method</span></span>           | <span data-ttu-id="cbd6b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbd6b-109">Return Type</span></span>    |<span data-ttu-id="cbd6b-110">説明</span><span class="sxs-lookup"><span data-stu-id="cbd6b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbd6b-111">PrivilegedApproval を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-111">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="cbd6b-112">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cbd6b-112">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="cbd6b-113">PrivilegedApproval オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-113">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="cbd6b-114">PrivilegedApproval オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="cbd6b-114">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="cbd6b-115">[privilegedApproval](privilegedapproval.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cbd6b-115">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="cbd6b-116">PrivilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-116">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="cbd6b-117">PrivilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-117">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="cbd6b-118">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cbd6b-118">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="cbd6b-119">PrivilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-119">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="cbd6b-120">PrivilegedApproval を更新します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-120">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="cbd6b-121">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cbd6b-121">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="cbd6b-122">PrivilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-122">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="cbd6b-123">Myrequests</span><span class="sxs-lookup"><span data-stu-id="cbd6b-123">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="cbd6b-124">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cbd6b-124">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="cbd6b-125">要求側の承認の要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-125">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbd6b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd6b-126">Properties</span></span>
| <span data-ttu-id="cbd6b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd6b-127">Property</span></span>     | <span data-ttu-id="cbd6b-128">種類</span><span class="sxs-lookup"><span data-stu-id="cbd6b-128">Type</span></span>   |<span data-ttu-id="cbd6b-129">説明</span><span class="sxs-lookup"><span data-stu-id="cbd6b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbd6b-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="cbd6b-130">approvalDuration</span></span>|<span data-ttu-id="cbd6b-131">Duration</span><span class="sxs-lookup"><span data-stu-id="cbd6b-131">Duration</span></span>||
|<span data-ttu-id="cbd6b-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="cbd6b-132">approvalState</span></span>|<span data-ttu-id="cbd6b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="cbd6b-133">string</span></span>| <span data-ttu-id="cbd6b-134">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="cbd6b-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="cbd6b-135">approvalType</span></span>|<span data-ttu-id="cbd6b-136">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-136">String</span></span>||
|<span data-ttu-id="cbd6b-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="cbd6b-137">approverReason</span></span>|<span data-ttu-id="cbd6b-138">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-138">String</span></span>||
|<span data-ttu-id="cbd6b-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cbd6b-139">endDateTime</span></span>|<span data-ttu-id="cbd6b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbd6b-140">DateTimeOffset</span></span>|<span data-ttu-id="cbd6b-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cbd6b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cbd6b-143">id</span><span class="sxs-lookup"><span data-stu-id="cbd6b-143">id</span></span>|<span data-ttu-id="cbd6b-144">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-144">String</span></span>| <span data-ttu-id="cbd6b-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-145">Read-only.</span></span>|
|<span data-ttu-id="cbd6b-146">requestorReason</span><span class="sxs-lookup"><span data-stu-id="cbd6b-146">requestorReason</span></span>|<span data-ttu-id="cbd6b-147">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-147">String</span></span>||
|<span data-ttu-id="cbd6b-148">roleId</span><span class="sxs-lookup"><span data-stu-id="cbd6b-148">roleId</span></span>|<span data-ttu-id="cbd6b-149">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-149">String</span></span>||
|<span data-ttu-id="cbd6b-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cbd6b-150">startDateTime</span></span>|<span data-ttu-id="cbd6b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbd6b-151">DateTimeOffset</span></span>|<span data-ttu-id="cbd6b-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cbd6b-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cbd6b-154">userId</span><span class="sxs-lookup"><span data-stu-id="cbd6b-154">userId</span></span>|<span data-ttu-id="cbd6b-155">String</span><span class="sxs-lookup"><span data-stu-id="cbd6b-155">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="cbd6b-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbd6b-156">Relationships</span></span>
| <span data-ttu-id="cbd6b-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbd6b-157">Relationship</span></span> | <span data-ttu-id="cbd6b-158">型</span><span class="sxs-lookup"><span data-stu-id="cbd6b-158">Type</span></span>   |<span data-ttu-id="cbd6b-159">説明</span><span class="sxs-lookup"><span data-stu-id="cbd6b-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbd6b-160">roleInfo</span><span class="sxs-lookup"><span data-stu-id="cbd6b-160">roleInfo</span></span>|[<span data-ttu-id="cbd6b-161">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="cbd6b-161">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="cbd6b-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="cbd6b-164">要求</span><span class="sxs-lookup"><span data-stu-id="cbd6b-164">request</span></span>|[<span data-ttu-id="cbd6b-165">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cbd6b-165">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="cbd6b-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-166">Read-only.</span></span> <span data-ttu-id="cbd6b-167">この承認オブジェクトのロール割り当ての依頼</span><span class="sxs-lookup"><span data-stu-id="cbd6b-167">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbd6b-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbd6b-168">JSON representation</span></span>
<span data-ttu-id="cbd6b-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbd6b-169">Here is a JSON representation of the resource.</span></span>

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
