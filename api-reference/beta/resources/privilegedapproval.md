---
title: privilegedApproval リソースの種類
description: ロールを取得するために特権 id 管理で要求される承認を表します。
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563650"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="59e7e-103">privilegedApproval リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59e7e-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e7e-104">ロールを取得するために特権 id 管理で要求される承認を表します。</span><span class="sxs-lookup"><span data-stu-id="59e7e-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="59e7e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="59e7e-105">Methods</span></span>

| <span data-ttu-id="59e7e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="59e7e-106">Method</span></span>           | <span data-ttu-id="59e7e-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59e7e-107">Return Type</span></span>    |<span data-ttu-id="59e7e-108">説明</span><span class="sxs-lookup"><span data-stu-id="59e7e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59e7e-109">privilegedApproval を取得する</span><span class="sxs-lookup"><span data-stu-id="59e7e-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="59e7e-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="59e7e-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="59e7e-111">privilegedApproval オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="59e7e-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="59e7e-112">privilegedApproval オブジェクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59e7e-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="59e7e-113">[privilegedApproval](privilegedapproval.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="59e7e-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="59e7e-114">privilegedApproval のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="59e7e-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="59e7e-115">privilegedApproval を作成する</span><span class="sxs-lookup"><span data-stu-id="59e7e-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="59e7e-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="59e7e-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="59e7e-117">privilegedApproval オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="59e7e-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="59e7e-118">privilegedApproval の更新</span><span class="sxs-lookup"><span data-stu-id="59e7e-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="59e7e-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="59e7e-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="59e7e-120">privilegedApproval オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="59e7e-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="59e7e-121">myrequests</span><span class="sxs-lookup"><span data-stu-id="59e7e-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="59e7e-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="59e7e-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="59e7e-123">要求者の承認要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="59e7e-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="59e7e-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59e7e-124">Properties</span></span>
| <span data-ttu-id="59e7e-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59e7e-125">Property</span></span>     | <span data-ttu-id="59e7e-126">型</span><span class="sxs-lookup"><span data-stu-id="59e7e-126">Type</span></span>   |<span data-ttu-id="59e7e-127">説明</span><span class="sxs-lookup"><span data-stu-id="59e7e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e7e-128">approvalduration</span><span class="sxs-lookup"><span data-stu-id="59e7e-128">approvalDuration</span></span>|<span data-ttu-id="59e7e-129">期間</span><span class="sxs-lookup"><span data-stu-id="59e7e-129">Duration</span></span>||
|<span data-ttu-id="59e7e-130">approvalstate</span><span class="sxs-lookup"><span data-stu-id="59e7e-130">approvalState</span></span>|<span data-ttu-id="59e7e-131">string</span><span class="sxs-lookup"><span data-stu-id="59e7e-131">string</span></span>| <span data-ttu-id="59e7e-132">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="59e7e-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="59e7e-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="59e7e-133">approvalType</span></span>|<span data-ttu-id="59e7e-134">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-134">String</span></span>||
|<span data-ttu-id="59e7e-135">approverreason</span><span class="sxs-lookup"><span data-stu-id="59e7e-135">approverReason</span></span>|<span data-ttu-id="59e7e-136">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-136">String</span></span>||
|<span data-ttu-id="59e7e-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59e7e-137">endDateTime</span></span>|<span data-ttu-id="59e7e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59e7e-138">DateTimeOffset</span></span>|<span data-ttu-id="59e7e-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="59e7e-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="59e7e-141">id</span><span class="sxs-lookup"><span data-stu-id="59e7e-141">id</span></span>|<span data-ttu-id="59e7e-142">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-142">String</span></span>| <span data-ttu-id="59e7e-143">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="59e7e-143">Read-only.</span></span>|
|<span data-ttu-id="59e7e-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="59e7e-144">requestorReason</span></span>|<span data-ttu-id="59e7e-145">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-145">String</span></span>||
|<span data-ttu-id="59e7e-146">roleId</span><span class="sxs-lookup"><span data-stu-id="59e7e-146">roleId</span></span>|<span data-ttu-id="59e7e-147">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-147">String</span></span>||
|<span data-ttu-id="59e7e-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59e7e-148">startDateTime</span></span>|<span data-ttu-id="59e7e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59e7e-149">DateTimeOffset</span></span>|<span data-ttu-id="59e7e-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="59e7e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="59e7e-152">userId</span><span class="sxs-lookup"><span data-stu-id="59e7e-152">userId</span></span>|<span data-ttu-id="59e7e-153">String</span><span class="sxs-lookup"><span data-stu-id="59e7e-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="59e7e-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59e7e-154">Relationships</span></span>
| <span data-ttu-id="59e7e-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59e7e-155">Relationship</span></span> | <span data-ttu-id="59e7e-156">型</span><span class="sxs-lookup"><span data-stu-id="59e7e-156">Type</span></span>   |<span data-ttu-id="59e7e-157">説明</span><span class="sxs-lookup"><span data-stu-id="59e7e-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e7e-158">roleinfo</span><span class="sxs-lookup"><span data-stu-id="59e7e-158">roleInfo</span></span>|[<span data-ttu-id="59e7e-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="59e7e-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="59e7e-160">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="59e7e-160">Read-only.</span></span> <span data-ttu-id="59e7e-161">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="59e7e-161">Nullable.</span></span>|
|<span data-ttu-id="59e7e-162">タキ</span><span class="sxs-lookup"><span data-stu-id="59e7e-162">request</span></span>|[<span data-ttu-id="59e7e-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="59e7e-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="59e7e-164">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="59e7e-164">Read-only.</span></span> <span data-ttu-id="59e7e-165">この承認オブジェクトの役割の割り当て要求</span><span class="sxs-lookup"><span data-stu-id="59e7e-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59e7e-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59e7e-166">JSON representation</span></span>
<span data-ttu-id="59e7e-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59e7e-167">Here is a JSON representation of the resource.</span></span>

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
