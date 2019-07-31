---
title: privilegedApproval リソースの種類
description: ロールを取得するために特権 Id 管理で要求される承認を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e920d34cc9a42c29138a97a83786087c86b7ee10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008916"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="dc1be-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc1be-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc1be-104">ロールを取得するために特権 Id 管理で要求される承認を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1be-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="dc1be-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc1be-105">Methods</span></span>

| <span data-ttu-id="dc1be-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc1be-106">Method</span></span>           | <span data-ttu-id="dc1be-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dc1be-107">Return Type</span></span>    |<span data-ttu-id="dc1be-108">説明</span><span class="sxs-lookup"><span data-stu-id="dc1be-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc1be-109">privilegedApproval を取得する</span><span class="sxs-lookup"><span data-stu-id="dc1be-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="dc1be-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="dc1be-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="dc1be-111">PrivilegedApproval オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dc1be-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="dc1be-112">PrivilegedApproval オブジェクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dc1be-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="dc1be-113">[privilegedApproval](privilegedapproval.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1be-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="dc1be-114">PrivilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc1be-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="dc1be-115">privilegedApproval を作成する</span><span class="sxs-lookup"><span data-stu-id="dc1be-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="dc1be-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="dc1be-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="dc1be-117">privilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc1be-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="dc1be-118">privilegedApproval を更新する</span><span class="sxs-lookup"><span data-stu-id="dc1be-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="dc1be-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="dc1be-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="dc1be-120">privilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="dc1be-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="dc1be-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="dc1be-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="dc1be-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="dc1be-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="dc1be-123">リクエスターの承認要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="dc1be-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc1be-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc1be-124">Properties</span></span>
| <span data-ttu-id="dc1be-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc1be-125">Property</span></span>     | <span data-ttu-id="dc1be-126">型</span><span class="sxs-lookup"><span data-stu-id="dc1be-126">Type</span></span>   |<span data-ttu-id="dc1be-127">説明</span><span class="sxs-lookup"><span data-stu-id="dc1be-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc1be-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="dc1be-128">approvalDuration</span></span>|<span data-ttu-id="dc1be-129">期間</span><span class="sxs-lookup"><span data-stu-id="dc1be-129">Duration</span></span>||
|<span data-ttu-id="dc1be-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="dc1be-130">approvalState</span></span>|<span data-ttu-id="dc1be-131">string</span><span class="sxs-lookup"><span data-stu-id="dc1be-131">string</span></span>| <span data-ttu-id="dc1be-132">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="dc1be-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="dc1be-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="dc1be-133">approvalType</span></span>|<span data-ttu-id="dc1be-134">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-134">String</span></span>||
|<span data-ttu-id="dc1be-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="dc1be-135">approverReason</span></span>|<span data-ttu-id="dc1be-136">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-136">String</span></span>||
|<span data-ttu-id="dc1be-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1be-137">endDateTime</span></span>|<span data-ttu-id="dc1be-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1be-138">DateTimeOffset</span></span>|<span data-ttu-id="dc1be-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dc1be-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dc1be-141">id</span><span class="sxs-lookup"><span data-stu-id="dc1be-141">id</span></span>|<span data-ttu-id="dc1be-142">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-142">String</span></span>| <span data-ttu-id="dc1be-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1be-143">Read-only.</span></span>|
|<span data-ttu-id="dc1be-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="dc1be-144">requestorReason</span></span>|<span data-ttu-id="dc1be-145">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-145">String</span></span>||
|<span data-ttu-id="dc1be-146">roleId</span><span class="sxs-lookup"><span data-stu-id="dc1be-146">roleId</span></span>|<span data-ttu-id="dc1be-147">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-147">String</span></span>||
|<span data-ttu-id="dc1be-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1be-148">startDateTime</span></span>|<span data-ttu-id="dc1be-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1be-149">DateTimeOffset</span></span>|<span data-ttu-id="dc1be-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dc1be-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dc1be-152">userId</span><span class="sxs-lookup"><span data-stu-id="dc1be-152">userId</span></span>|<span data-ttu-id="dc1be-153">String</span><span class="sxs-lookup"><span data-stu-id="dc1be-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="dc1be-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc1be-154">Relationships</span></span>
| <span data-ttu-id="dc1be-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc1be-155">Relationship</span></span> | <span data-ttu-id="dc1be-156">型</span><span class="sxs-lookup"><span data-stu-id="dc1be-156">Type</span></span>   |<span data-ttu-id="dc1be-157">説明</span><span class="sxs-lookup"><span data-stu-id="dc1be-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc1be-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="dc1be-158">roleInfo</span></span>|[<span data-ttu-id="dc1be-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="dc1be-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="dc1be-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1be-160">Read-only.</span></span> <span data-ttu-id="dc1be-161">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dc1be-161">Nullable.</span></span>|
|<span data-ttu-id="dc1be-162">タキ</span><span class="sxs-lookup"><span data-stu-id="dc1be-162">request</span></span>|[<span data-ttu-id="dc1be-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="dc1be-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="dc1be-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1be-164">Read-only.</span></span> <span data-ttu-id="dc1be-165">この承認オブジェクトの役割の割り当て要求</span><span class="sxs-lookup"><span data-stu-id="dc1be-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc1be-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc1be-166">JSON representation</span></span>
<span data-ttu-id="dc1be-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc1be-167">Here is a JSON representation of the resource.</span></span>

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
