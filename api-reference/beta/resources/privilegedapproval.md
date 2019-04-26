---
title: privilegedApproval リソースの種類
description: ロールを取得するために特権 id 管理で要求される承認を表します。
localization_priority: Normal
ms.openlocfilehash: 754fcd9b61321db1675408172c945557e38dc0e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344235"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="b655b-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b655b-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b655b-104">ロールを取得するために特権 id 管理で要求される承認を表します。</span><span class="sxs-lookup"><span data-stu-id="b655b-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="b655b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b655b-105">Methods</span></span>

| <span data-ttu-id="b655b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b655b-106">Method</span></span>           | <span data-ttu-id="b655b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b655b-107">Return Type</span></span>    |<span data-ttu-id="b655b-108">説明</span><span class="sxs-lookup"><span data-stu-id="b655b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b655b-109">privilegedApproval を取得する</span><span class="sxs-lookup"><span data-stu-id="b655b-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="b655b-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="b655b-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="b655b-111">privilegedApproval オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b655b-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="b655b-112">privilegedApproval オブジェクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b655b-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="b655b-113">[privilegedApproval](privilegedapproval.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b655b-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="b655b-114">privilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b655b-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="b655b-115">privilegedApproval を作成する</span><span class="sxs-lookup"><span data-stu-id="b655b-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="b655b-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="b655b-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="b655b-117">privilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b655b-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="b655b-118">privilegedApproval の更新</span><span class="sxs-lookup"><span data-stu-id="b655b-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="b655b-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="b655b-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="b655b-120">privilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b655b-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="b655b-121">myrequests</span><span class="sxs-lookup"><span data-stu-id="b655b-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="b655b-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="b655b-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="b655b-123">要求者の承認要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="b655b-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="b655b-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b655b-124">Properties</span></span>
| <span data-ttu-id="b655b-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b655b-125">Property</span></span>     | <span data-ttu-id="b655b-126">型</span><span class="sxs-lookup"><span data-stu-id="b655b-126">Type</span></span>   |<span data-ttu-id="b655b-127">説明</span><span class="sxs-lookup"><span data-stu-id="b655b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b655b-128">approvalduration</span><span class="sxs-lookup"><span data-stu-id="b655b-128">approvalDuration</span></span>|<span data-ttu-id="b655b-129">期間</span><span class="sxs-lookup"><span data-stu-id="b655b-129">Duration</span></span>||
|<span data-ttu-id="b655b-130">approvalstate</span><span class="sxs-lookup"><span data-stu-id="b655b-130">approvalState</span></span>|<span data-ttu-id="b655b-131">string</span><span class="sxs-lookup"><span data-stu-id="b655b-131">string</span></span>| <span data-ttu-id="b655b-132">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="b655b-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="b655b-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="b655b-133">approvalType</span></span>|<span data-ttu-id="b655b-134">String</span><span class="sxs-lookup"><span data-stu-id="b655b-134">String</span></span>||
|<span data-ttu-id="b655b-135">approverreason</span><span class="sxs-lookup"><span data-stu-id="b655b-135">approverReason</span></span>|<span data-ttu-id="b655b-136">String</span><span class="sxs-lookup"><span data-stu-id="b655b-136">String</span></span>||
|<span data-ttu-id="b655b-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b655b-137">endDateTime</span></span>|<span data-ttu-id="b655b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b655b-138">DateTimeOffset</span></span>|<span data-ttu-id="b655b-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b655b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b655b-141">id</span><span class="sxs-lookup"><span data-stu-id="b655b-141">id</span></span>|<span data-ttu-id="b655b-142">String</span><span class="sxs-lookup"><span data-stu-id="b655b-142">String</span></span>| <span data-ttu-id="b655b-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b655b-143">Read-only.</span></span>|
|<span data-ttu-id="b655b-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="b655b-144">requestorReason</span></span>|<span data-ttu-id="b655b-145">String</span><span class="sxs-lookup"><span data-stu-id="b655b-145">String</span></span>||
|<span data-ttu-id="b655b-146">roleId</span><span class="sxs-lookup"><span data-stu-id="b655b-146">roleId</span></span>|<span data-ttu-id="b655b-147">String</span><span class="sxs-lookup"><span data-stu-id="b655b-147">String</span></span>||
|<span data-ttu-id="b655b-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b655b-148">startDateTime</span></span>|<span data-ttu-id="b655b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b655b-149">DateTimeOffset</span></span>|<span data-ttu-id="b655b-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b655b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b655b-152">userId</span><span class="sxs-lookup"><span data-stu-id="b655b-152">userId</span></span>|<span data-ttu-id="b655b-153">String</span><span class="sxs-lookup"><span data-stu-id="b655b-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="b655b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b655b-154">Relationships</span></span>
| <span data-ttu-id="b655b-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b655b-155">Relationship</span></span> | <span data-ttu-id="b655b-156">型</span><span class="sxs-lookup"><span data-stu-id="b655b-156">Type</span></span>   |<span data-ttu-id="b655b-157">説明</span><span class="sxs-lookup"><span data-stu-id="b655b-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b655b-158">roleinfo</span><span class="sxs-lookup"><span data-stu-id="b655b-158">roleInfo</span></span>|[<span data-ttu-id="b655b-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b655b-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="b655b-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b655b-160">Read-only.</span></span> <span data-ttu-id="b655b-161">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b655b-161">Nullable.</span></span>|
|<span data-ttu-id="b655b-162">タキ</span><span class="sxs-lookup"><span data-stu-id="b655b-162">request</span></span>|[<span data-ttu-id="b655b-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b655b-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="b655b-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b655b-164">Read-only.</span></span> <span data-ttu-id="b655b-165">この承認オブジェクトの役割の割り当て要求</span><span class="sxs-lookup"><span data-stu-id="b655b-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b655b-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b655b-166">JSON representation</span></span>
<span data-ttu-id="b655b-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b655b-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
