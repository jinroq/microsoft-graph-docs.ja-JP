---
title: GovernanceRoleAssignmentRequest を作成します。
description: 役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。
localization_priority: Normal
ms.openlocfilehash: 09adb824147dba745649efc7589ca763f815278d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823773"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="269e5-104">GovernanceRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="269e5-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="269e5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="269e5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="269e5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="269e5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="269e5-107">役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="269e5-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="269e5-108">次の表に、操作をします。</span><span class="sxs-lookup"><span data-stu-id="269e5-108">The following table lists the operations.</span></span>

| <span data-ttu-id="269e5-109">操作</span><span class="sxs-lookup"><span data-stu-id="269e5-109">Operation</span></span>       | <span data-ttu-id="269e5-110">Type</span><span class="sxs-lookup"><span data-stu-id="269e5-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="269e5-111">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="269e5-111">Assign a role assignment</span></span>| <span data-ttu-id="269e5-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="269e5-112">AdminAdd</span></span> |
| <span data-ttu-id="269e5-113">対象のロール割り当てを有効化します。</span><span class="sxs-lookup"><span data-stu-id="269e5-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="269e5-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="269e5-114">UserAdd</span></span> | 
| <span data-ttu-id="269e5-115">アクティブ化されたロール割り当てを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="269e5-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="269e5-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="269e5-116">UserRemove</span></span> | 
| <span data-ttu-id="269e5-117">役割の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="269e5-117">Remove a role assignment</span></span>| <span data-ttu-id="269e5-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="269e5-118">AdminRemove</span></span> |
| <span data-ttu-id="269e5-119">役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="269e5-119">Update a role assignment</span></span>| <span data-ttu-id="269e5-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="269e5-120">AdminUpdate</span></span> |
| <span data-ttu-id="269e5-121">自分の役割の割り当てを拡張する要求</span><span class="sxs-lookup"><span data-stu-id="269e5-121">Request to extend my role assignment</span></span>| <span data-ttu-id="269e5-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="269e5-122">UserExtend</span></span> | 
| <span data-ttu-id="269e5-123">役割の割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="269e5-123">Extend a role assignment</span></span>| <span data-ttu-id="269e5-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="269e5-124">AdminExtend</span></span> | 
| <span data-ttu-id="269e5-125">[期限切れのロールの割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="269e5-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="269e5-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="269e5-126">UserRenew</span></span> | 
| <span data-ttu-id="269e5-127">期限切れのロール割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="269e5-127">Renew an expired role assignment</span></span>| <span data-ttu-id="269e5-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="269e5-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="269e5-129">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="269e5-129">Permissions</span></span>
<span data-ttu-id="269e5-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="269e5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="269e5-132">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="269e5-132">Permission type</span></span>      | <span data-ttu-id="269e5-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="269e5-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="269e5-134">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="269e5-134">Delegated (work or school account)</span></span> | <span data-ttu-id="269e5-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="269e5-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="269e5-136">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="269e5-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="269e5-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="269e5-137">Not supported.</span></span>    |
|<span data-ttu-id="269e5-138">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="269e5-138">Application</span></span> | <span data-ttu-id="269e5-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="269e5-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="269e5-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="269e5-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="269e5-141">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="269e5-141">Request headers</span></span>
| <span data-ttu-id="269e5-142">名前</span><span class="sxs-lookup"><span data-stu-id="269e5-142">Name</span></span>       | <span data-ttu-id="269e5-143">説明</span><span class="sxs-lookup"><span data-stu-id="269e5-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="269e5-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="269e5-144">Authorization</span></span>  | <span data-ttu-id="269e5-145">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="269e5-145">Bearer {code}</span></span>|
| <span data-ttu-id="269e5-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="269e5-146">Content-type</span></span>  | <span data-ttu-id="269e5-147">application/json</span><span class="sxs-lookup"><span data-stu-id="269e5-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="269e5-148">要求本文</span><span class="sxs-lookup"><span data-stu-id="269e5-148">Request body</span></span>
<span data-ttu-id="269e5-149">要求の本文には、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="269e5-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="269e5-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-150">Property</span></span>     | <span data-ttu-id="269e5-151">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-151">Type</span></span>    |<span data-ttu-id="269e5-152">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-152">Required</span></span>|  <span data-ttu-id="269e5-153">説明</span><span class="sxs-lookup"><span data-stu-id="269e5-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-154">resourceId</span></span>|<span data-ttu-id="269e5-155">String</span><span class="sxs-lookup"><span data-stu-id="269e5-155">String</span></span>|<span data-ttu-id="269e5-156">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-156">Yes</span></span>|<span data-ttu-id="269e5-157">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="269e5-157">The ID of the resource.</span></span>|
|<span data-ttu-id="269e5-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-158">roleDefinitionId</span></span>|<span data-ttu-id="269e5-159">String</span><span class="sxs-lookup"><span data-stu-id="269e5-159">String</span></span>|<span data-ttu-id="269e5-160">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-160">Yes</span></span>|<span data-ttu-id="269e5-161">役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="269e5-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="269e5-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-162">subjectId</span></span>|<span data-ttu-id="269e5-163">String</span><span class="sxs-lookup"><span data-stu-id="269e5-163">String</span></span>|<span data-ttu-id="269e5-164">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-164">Yes</span></span>|<span data-ttu-id="269e5-165">サブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="269e5-165">The ID of the subject.</span></span>|
|<span data-ttu-id="269e5-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-166">assignmentState</span></span>|<span data-ttu-id="269e5-167">String</span><span class="sxs-lookup"><span data-stu-id="269e5-167">String</span></span>|<span data-ttu-id="269e5-168">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-168">Yes</span></span>|<span data-ttu-id="269e5-169">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="269e5-169">The state of assignment.</span></span> <span data-ttu-id="269e5-170">値は、``Eligible``と``Active``。</span><span class="sxs-lookup"><span data-stu-id="269e5-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="269e5-171">type</span><span class="sxs-lookup"><span data-stu-id="269e5-171">type</span></span>|<span data-ttu-id="269e5-172">String</span><span class="sxs-lookup"><span data-stu-id="269e5-172">String</span></span>|<span data-ttu-id="269e5-173">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-173">Yes</span></span>|<span data-ttu-id="269e5-174">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="269e5-174">The request type.</span></span> <span data-ttu-id="269e5-175">値は、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、`AdminRenew`と`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="269e5-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="269e5-176">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-176">reason</span></span>|<span data-ttu-id="269e5-177">String</span><span class="sxs-lookup"><span data-stu-id="269e5-177">String</span></span>| |<span data-ttu-id="269e5-178">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="269e5-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="269e5-179">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-179">schedule</span></span>|[<span data-ttu-id="269e5-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="269e5-181">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="269e5-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="269e5-182">要求の種類の`UserAdd`、 `AdminAdd`、`AdminUpdate`と`AdminExtend`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="269e5-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="269e5-183">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-183">Response</span></span>
<span data-ttu-id="269e5-184">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="269e5-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="269e5-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="269e5-185">Error codes</span></span>
<span data-ttu-id="269e5-186">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="269e5-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="269e5-187">さらに、また次の表に記載されているエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="269e5-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="269e5-188">エラー コード</span><span class="sxs-lookup"><span data-stu-id="269e5-188">Error code</span></span>     | <span data-ttu-id="269e5-189">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="269e5-189">Error message</span></span>              | <span data-ttu-id="269e5-190">詳細</span><span class="sxs-lookup"><span data-stu-id="269e5-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="269e5-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-191">400 BadRequest</span></span> | <span data-ttu-id="269e5-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="269e5-192">RoleNotFound</span></span>    | <span data-ttu-id="269e5-193">`roleDefinitionId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="269e5-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="269e5-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-194">400 BadRequest</span></span> | <span data-ttu-id="269e5-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="269e5-195">ResourceIsLocked</span></span>    | <span data-ttu-id="269e5-196">状態の要求の本文に記載されているリソースは、`Locked`と、役割の割り当て要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="269e5-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="269e5-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-197">400 BadRequest</span></span> | <span data-ttu-id="269e5-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="269e5-198">SubjectNotFound</span></span>    | <span data-ttu-id="269e5-199">`subjectId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="269e5-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="269e5-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-200">400 BadRequest</span></span> | <span data-ttu-id="269e5-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="269e5-202">あるシステムで保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を既に存在します。</span><span class="sxs-lookup"><span data-stu-id="269e5-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="269e5-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-203">400 BadRequest</span></span> | <span data-ttu-id="269e5-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="269e5-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="269e5-205">既に要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在します。</span><span class="sxs-lookup"><span data-stu-id="269e5-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="269e5-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-206">400 BadRequest</span></span> | <span data-ttu-id="269e5-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="269e5-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="269e5-208">更新または拡張するように要求した[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="269e5-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="269e5-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="269e5-209">400 BadRequest</span></span> | <span data-ttu-id="269e5-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="269e5-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="269e5-211">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は、社内ポリシーを満たしていないと、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="269e5-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="269e5-212">例</span><span class="sxs-lookup"><span data-stu-id="269e5-212">Examples</span></span>
<span data-ttu-id="269e5-213">次の例では、この API を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="269e5-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="269e5-214">例 1</span><span class="sxs-lookup"><span data-stu-id="269e5-214">Example 1</span></span>
<span data-ttu-id="269e5-215">この例では、管理者は、課金情報の閲覧者の役割にユーザーの nawu@fimdev.net を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="269e5-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="269e5-216">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="269e5-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="269e5-217">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-217">Property</span></span>     | <span data-ttu-id="269e5-218">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-218">Type</span></span>    |<span data-ttu-id="269e5-219">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-219">Required</span></span>|  <span data-ttu-id="269e5-220">値</span><span class="sxs-lookup"><span data-stu-id="269e5-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-221">resourceId</span></span>|<span data-ttu-id="269e5-222">String</span><span class="sxs-lookup"><span data-stu-id="269e5-222">String</span></span>|<span data-ttu-id="269e5-223">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-223">Yes</span></span>|<span data-ttu-id="269e5-224">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-224">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-225">roleDefinitionId</span></span>|<span data-ttu-id="269e5-226">String</span><span class="sxs-lookup"><span data-stu-id="269e5-226">String</span></span>|<span data-ttu-id="269e5-227">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-227">Yes</span></span>|<span data-ttu-id="269e5-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-229">subjectId</span></span>|<span data-ttu-id="269e5-230">String</span><span class="sxs-lookup"><span data-stu-id="269e5-230">String</span></span>|<span data-ttu-id="269e5-231">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-231">Yes</span></span>|<span data-ttu-id="269e5-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-232">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-233">assignmentState</span></span>|<span data-ttu-id="269e5-234">String</span><span class="sxs-lookup"><span data-stu-id="269e5-234">String</span></span>|<span data-ttu-id="269e5-235">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-235">Yes</span></span>| <span data-ttu-id="269e5-236">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="269e5-236">Eligible / Active</span></span>|
|<span data-ttu-id="269e5-237">type</span><span class="sxs-lookup"><span data-stu-id="269e5-237">type</span></span>|<span data-ttu-id="269e5-238">String</span><span class="sxs-lookup"><span data-stu-id="269e5-238">String</span></span>|<span data-ttu-id="269e5-239">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-239">Yes</span></span>| <span data-ttu-id="269e5-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="269e5-240">AdminAdd</span></span>|
|<span data-ttu-id="269e5-241">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-241">reason</span></span>|<span data-ttu-id="269e5-242">String</span><span class="sxs-lookup"><span data-stu-id="269e5-242">String</span></span>| <span data-ttu-id="269e5-243">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="269e5-243">depends on role Settings</span></span>||
|<span data-ttu-id="269e5-244">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-244">schedule</span></span>|[<span data-ttu-id="269e5-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-246">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-247">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-247">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="269e5-248">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-248">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

### <a name="example-2"></a><span data-ttu-id="269e5-249">例 2</span><span class="sxs-lookup"><span data-stu-id="269e5-249">Example 2</span></span>
<span data-ttu-id="269e5-250">この例では、ユーザー nawu@fimdev.net は、対象となる請求のリーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="269e5-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="269e5-251">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-251">Property</span></span>     | <span data-ttu-id="269e5-252">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-252">Type</span></span>    |<span data-ttu-id="269e5-253">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-253">Required</span></span>|  <span data-ttu-id="269e5-254">値</span><span class="sxs-lookup"><span data-stu-id="269e5-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-255">resourceId</span></span>|<span data-ttu-id="269e5-256">String</span><span class="sxs-lookup"><span data-stu-id="269e5-256">String</span></span>|<span data-ttu-id="269e5-257">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-257">Yes</span></span>|<span data-ttu-id="269e5-258">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-258">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-259">roleDefinitionId</span></span>|<span data-ttu-id="269e5-260">String</span><span class="sxs-lookup"><span data-stu-id="269e5-260">String</span></span>|<span data-ttu-id="269e5-261">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-261">Yes</span></span>|<span data-ttu-id="269e5-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-263">subjectId</span></span>|<span data-ttu-id="269e5-264">String</span><span class="sxs-lookup"><span data-stu-id="269e5-264">String</span></span>|<span data-ttu-id="269e5-265">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-265">Yes</span></span>|<span data-ttu-id="269e5-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-266">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-267">assignmentState</span></span>|<span data-ttu-id="269e5-268">String</span><span class="sxs-lookup"><span data-stu-id="269e5-268">String</span></span>|<span data-ttu-id="269e5-269">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-269">Yes</span></span>| <span data-ttu-id="269e5-270">Active</span><span class="sxs-lookup"><span data-stu-id="269e5-270">Active</span></span>|
|<span data-ttu-id="269e5-271">type</span><span class="sxs-lookup"><span data-stu-id="269e5-271">type</span></span>|<span data-ttu-id="269e5-272">String</span><span class="sxs-lookup"><span data-stu-id="269e5-272">String</span></span>|<span data-ttu-id="269e5-273">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-273">Yes</span></span>| <span data-ttu-id="269e5-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="269e5-274">UserAdd</span></span>|
|<span data-ttu-id="269e5-275">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-275">reason</span></span>|<span data-ttu-id="269e5-276">String</span><span class="sxs-lookup"><span data-stu-id="269e5-276">String</span></span>| <span data-ttu-id="269e5-277">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="269e5-277">depends on role Settings</span></span>||
|<span data-ttu-id="269e5-278">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-278">schedule</span></span>|[<span data-ttu-id="269e5-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-280">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-281">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-281">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="269e5-282">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-282">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

### <a name="example-3"></a><span data-ttu-id="269e5-283">例 3</span><span class="sxs-lookup"><span data-stu-id="269e5-283">Example 3</span></span>
<span data-ttu-id="269e5-284">この例では、ユーザー nawu@fimdev.net には、作業中の課金情報の閲覧者の役割が無効になります。</span><span class="sxs-lookup"><span data-stu-id="269e5-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="269e5-285">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-285">Property</span></span>     | <span data-ttu-id="269e5-286">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-286">Type</span></span>    |<span data-ttu-id="269e5-287">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-287">Required</span></span>|  <span data-ttu-id="269e5-288">値</span><span class="sxs-lookup"><span data-stu-id="269e5-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-289">resourceId</span></span>|<span data-ttu-id="269e5-290">String</span><span class="sxs-lookup"><span data-stu-id="269e5-290">String</span></span>|<span data-ttu-id="269e5-291">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-291">Yes</span></span>|<span data-ttu-id="269e5-292">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-292">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-293">roleDefinitionId</span></span>|<span data-ttu-id="269e5-294">String</span><span class="sxs-lookup"><span data-stu-id="269e5-294">String</span></span>|<span data-ttu-id="269e5-295">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-295">Yes</span></span>|<span data-ttu-id="269e5-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-297">subjectId</span></span>|<span data-ttu-id="269e5-298">String</span><span class="sxs-lookup"><span data-stu-id="269e5-298">String</span></span>|<span data-ttu-id="269e5-299">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-299">Yes</span></span>|<span data-ttu-id="269e5-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-300">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-301">assignmentState</span></span>|<span data-ttu-id="269e5-302">String</span><span class="sxs-lookup"><span data-stu-id="269e5-302">String</span></span>|<span data-ttu-id="269e5-303">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-303">Yes</span></span>| <span data-ttu-id="269e5-304">Active</span><span class="sxs-lookup"><span data-stu-id="269e5-304">Active</span></span>|
|<span data-ttu-id="269e5-305">type</span><span class="sxs-lookup"><span data-stu-id="269e5-305">type</span></span>|<span data-ttu-id="269e5-306">String</span><span class="sxs-lookup"><span data-stu-id="269e5-306">String</span></span>|<span data-ttu-id="269e5-307">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-307">Yes</span></span>| <span data-ttu-id="269e5-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="269e5-308">UserRemove</span></span>|
|<span data-ttu-id="269e5-309">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-309">reason</span></span>|<span data-ttu-id="269e5-310">String</span><span class="sxs-lookup"><span data-stu-id="269e5-310">String</span></span>| <span data-ttu-id="269e5-311">いいえ</span><span class="sxs-lookup"><span data-stu-id="269e5-311">No</span></span>||
|<span data-ttu-id="269e5-312">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-312">schedule</span></span>|[<span data-ttu-id="269e5-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-314">いいえ</span><span class="sxs-lookup"><span data-stu-id="269e5-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-315">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-315">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="269e5-316">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-316">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="269e5-317">例 4</span><span class="sxs-lookup"><span data-stu-id="269e5-317">Example 4</span></span>
<span data-ttu-id="269e5-318">この例では、管理者は、課金情報の閲覧者の役割からユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="269e5-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="269e5-319">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="269e5-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="269e5-320">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-320">Property</span></span>     | <span data-ttu-id="269e5-321">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-321">Type</span></span>    |<span data-ttu-id="269e5-322">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-322">Required</span></span>|  <span data-ttu-id="269e5-323">値</span><span class="sxs-lookup"><span data-stu-id="269e5-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-324">resourceId</span></span>|<span data-ttu-id="269e5-325">String</span><span class="sxs-lookup"><span data-stu-id="269e5-325">String</span></span>|<span data-ttu-id="269e5-326">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-326">Yes</span></span>|<span data-ttu-id="269e5-327">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-327">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-328">roleDefinitionId</span></span>|<span data-ttu-id="269e5-329">String</span><span class="sxs-lookup"><span data-stu-id="269e5-329">String</span></span>|<span data-ttu-id="269e5-330">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-330">Yes</span></span>|<span data-ttu-id="269e5-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-332">subjectId</span></span>|<span data-ttu-id="269e5-333">String</span><span class="sxs-lookup"><span data-stu-id="269e5-333">String</span></span>|<span data-ttu-id="269e5-334">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-334">Yes</span></span>|<span data-ttu-id="269e5-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-335">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-336">assignmentState</span></span>|<span data-ttu-id="269e5-337">String</span><span class="sxs-lookup"><span data-stu-id="269e5-337">String</span></span>|<span data-ttu-id="269e5-338">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-338">Yes</span></span>| <span data-ttu-id="269e5-339">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="269e5-339">Eligible / Active</span></span>|
|<span data-ttu-id="269e5-340">type</span><span class="sxs-lookup"><span data-stu-id="269e5-340">type</span></span>|<span data-ttu-id="269e5-341">String</span><span class="sxs-lookup"><span data-stu-id="269e5-341">String</span></span>|<span data-ttu-id="269e5-342">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-342">Yes</span></span>| <span data-ttu-id="269e5-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="269e5-343">AdminRemove</span></span>|
|<span data-ttu-id="269e5-344">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-344">reason</span></span>|<span data-ttu-id="269e5-345">String</span><span class="sxs-lookup"><span data-stu-id="269e5-345">String</span></span>| <span data-ttu-id="269e5-346">いいえ</span><span class="sxs-lookup"><span data-stu-id="269e5-346">No</span></span>||
|<span data-ttu-id="269e5-347">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-347">schedule</span></span>|[<span data-ttu-id="269e5-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-349">いいえ</span><span class="sxs-lookup"><span data-stu-id="269e5-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-350">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-350">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="269e5-351">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-351">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="269e5-352">例 5</span><span class="sxs-lookup"><span data-stu-id="269e5-352">Example 5</span></span>
<span data-ttu-id="269e5-353">この例では、管理者は、所有者をユーザー nawu@fimdev.net の役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="269e5-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="269e5-354">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="269e5-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="269e5-355">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-355">Property</span></span>     | <span data-ttu-id="269e5-356">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-356">Type</span></span>    |<span data-ttu-id="269e5-357">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-357">Required</span></span>|  <span data-ttu-id="269e5-358">値</span><span class="sxs-lookup"><span data-stu-id="269e5-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-359">resourceId</span></span>|<span data-ttu-id="269e5-360">String</span><span class="sxs-lookup"><span data-stu-id="269e5-360">String</span></span>|<span data-ttu-id="269e5-361">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-361">Yes</span></span>|<span data-ttu-id="269e5-362">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-362">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-363">roleDefinitionId</span></span>|<span data-ttu-id="269e5-364">String</span><span class="sxs-lookup"><span data-stu-id="269e5-364">String</span></span>|<span data-ttu-id="269e5-365">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-365">Yes</span></span>|<span data-ttu-id="269e5-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-367">subjectId</span></span>|<span data-ttu-id="269e5-368">String</span><span class="sxs-lookup"><span data-stu-id="269e5-368">String</span></span>|<span data-ttu-id="269e5-369">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-369">Yes</span></span>|<span data-ttu-id="269e5-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-370">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-371">assignmentState</span></span>|<span data-ttu-id="269e5-372">String</span><span class="sxs-lookup"><span data-stu-id="269e5-372">String</span></span>|<span data-ttu-id="269e5-373">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-373">Yes</span></span>| <span data-ttu-id="269e5-374">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="269e5-374">Eligible / Active</span></span>|
|<span data-ttu-id="269e5-375">type</span><span class="sxs-lookup"><span data-stu-id="269e5-375">type</span></span>|<span data-ttu-id="269e5-376">String</span><span class="sxs-lookup"><span data-stu-id="269e5-376">String</span></span>|<span data-ttu-id="269e5-377">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-377">Yes</span></span>| <span data-ttu-id="269e5-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="269e5-378">AdminUpdate</span></span>|
|<span data-ttu-id="269e5-379">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-379">reason</span></span>|<span data-ttu-id="269e5-380">String</span><span class="sxs-lookup"><span data-stu-id="269e5-380">String</span></span>| <span data-ttu-id="269e5-381">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="269e5-381">depends on roleSettings</span></span>||
|<span data-ttu-id="269e5-382">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-382">schedule</span></span>|[<span data-ttu-id="269e5-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-384">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-385">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-385">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="269e5-386">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-386">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="269e5-387">例 6</span><span class="sxs-lookup"><span data-stu-id="269e5-387">Example 6</span></span>
<span data-ttu-id="269e5-388">次の使用例は、API の管理サービスの共同作成者に ANUJCUSER のユーザーの有効期限切れのロールの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="269e5-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="269e5-389">**注:** Additon アクセス許可を次の使用例が必要です、依頼者が少なくとも 1 つであること`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="269e5-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="269e5-390">プロパティ</span><span class="sxs-lookup"><span data-stu-id="269e5-390">Property</span></span>     | <span data-ttu-id="269e5-391">種類</span><span class="sxs-lookup"><span data-stu-id="269e5-391">Type</span></span>    |<span data-ttu-id="269e5-392">必須</span><span class="sxs-lookup"><span data-stu-id="269e5-392">Required</span></span>|  <span data-ttu-id="269e5-393">値</span><span class="sxs-lookup"><span data-stu-id="269e5-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="269e5-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="269e5-394">resourceId</span></span>|<span data-ttu-id="269e5-395">String</span><span class="sxs-lookup"><span data-stu-id="269e5-395">String</span></span>|<span data-ttu-id="269e5-396">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-396">Yes</span></span>|<span data-ttu-id="269e5-397">\<とります\></span><span class="sxs-lookup"><span data-stu-id="269e5-397">\<resourceId\></span></span>|
|<span data-ttu-id="269e5-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="269e5-398">roleDefinitionId</span></span>|<span data-ttu-id="269e5-399">String</span><span class="sxs-lookup"><span data-stu-id="269e5-399">String</span></span>|<span data-ttu-id="269e5-400">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-400">Yes</span></span>|<span data-ttu-id="269e5-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="269e5-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="269e5-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="269e5-402">subjectId</span></span>|<span data-ttu-id="269e5-403">String</span><span class="sxs-lookup"><span data-stu-id="269e5-403">String</span></span>|<span data-ttu-id="269e5-404">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-404">Yes</span></span>|<span data-ttu-id="269e5-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="269e5-405">\<subjectId\></span></span>|
|<span data-ttu-id="269e5-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="269e5-406">assignmentState</span></span>|<span data-ttu-id="269e5-407">String</span><span class="sxs-lookup"><span data-stu-id="269e5-407">String</span></span>|<span data-ttu-id="269e5-408">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-408">Yes</span></span>| <span data-ttu-id="269e5-409">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="269e5-409">Eligible / Active</span></span> |
|<span data-ttu-id="269e5-410">type</span><span class="sxs-lookup"><span data-stu-id="269e5-410">type</span></span>|<span data-ttu-id="269e5-411">String</span><span class="sxs-lookup"><span data-stu-id="269e5-411">String</span></span>|<span data-ttu-id="269e5-412">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-412">Yes</span></span>| <span data-ttu-id="269e5-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="269e5-413">AdminExtend</span></span>|
|<span data-ttu-id="269e5-414">理由</span><span class="sxs-lookup"><span data-stu-id="269e5-414">reason</span></span>|<span data-ttu-id="269e5-415">String</span><span class="sxs-lookup"><span data-stu-id="269e5-415">String</span></span>| <span data-ttu-id="269e5-416">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="269e5-416">depends on roleSettings</span></span>||
|<span data-ttu-id="269e5-417">スケジュール</span><span class="sxs-lookup"><span data-stu-id="269e5-417">schedule</span></span>|[<span data-ttu-id="269e5-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="269e5-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="269e5-419">はい</span><span class="sxs-lookup"><span data-stu-id="269e5-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="269e5-420">要求</span><span class="sxs-lookup"><span data-stu-id="269e5-420">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="269e5-421">応答</span><span class="sxs-lookup"><span data-stu-id="269e5-421">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
