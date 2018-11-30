---
title: GovernanceRoleAssignmentRequest を作成します。
description: 役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069350"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="590cb-104">GovernanceRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="590cb-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="590cb-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="590cb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="590cb-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="590cb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="590cb-107">役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="590cb-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="590cb-108">次の表に、操作をします。</span><span class="sxs-lookup"><span data-stu-id="590cb-108">The following table lists the operations.</span></span>

| <span data-ttu-id="590cb-109">操作</span><span class="sxs-lookup"><span data-stu-id="590cb-109">Operation</span></span>       | <span data-ttu-id="590cb-110">型</span><span class="sxs-lookup"><span data-stu-id="590cb-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="590cb-111">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="590cb-111">Assign a role assignment</span></span>| <span data-ttu-id="590cb-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="590cb-112">AdminAdd</span></span> |
| <span data-ttu-id="590cb-113">対象のロール割り当てを有効化します。</span><span class="sxs-lookup"><span data-stu-id="590cb-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="590cb-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="590cb-114">UserAdd</span></span> | 
| <span data-ttu-id="590cb-115">アクティブ化されたロール割り当てを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="590cb-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="590cb-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="590cb-116">UserRemove</span></span> | 
| <span data-ttu-id="590cb-117">役割の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="590cb-117">Remove a role assignment</span></span>| <span data-ttu-id="590cb-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="590cb-118">AdminRemove</span></span> |
| <span data-ttu-id="590cb-119">役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="590cb-119">Update a role assignment</span></span>| <span data-ttu-id="590cb-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="590cb-120">AdminUpdate</span></span> |
| <span data-ttu-id="590cb-121">自分の役割の割り当てを拡張する要求</span><span class="sxs-lookup"><span data-stu-id="590cb-121">Request to extend my role assignment</span></span>| <span data-ttu-id="590cb-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="590cb-122">UserExtend</span></span> | 
| <span data-ttu-id="590cb-123">役割の割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="590cb-123">Extend a role assignment</span></span>| <span data-ttu-id="590cb-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="590cb-124">AdminExtend</span></span> | 
| <span data-ttu-id="590cb-125">[期限切れのロールの割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="590cb-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="590cb-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="590cb-126">UserRenew</span></span> | 
| <span data-ttu-id="590cb-127">期限切れのロール割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="590cb-127">Renew an expired role assignment</span></span>| <span data-ttu-id="590cb-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="590cb-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="590cb-129">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="590cb-129">Permissions</span></span>
<span data-ttu-id="590cb-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="590cb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="590cb-132">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="590cb-132">Permission type</span></span>      | <span data-ttu-id="590cb-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="590cb-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="590cb-134">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="590cb-134">Delegated (work or school account)</span></span> | <span data-ttu-id="590cb-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="590cb-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="590cb-136">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="590cb-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="590cb-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="590cb-137">Not supported.</span></span>    |
|<span data-ttu-id="590cb-138">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="590cb-138">Application</span></span> | <span data-ttu-id="590cb-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="590cb-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="590cb-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="590cb-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="590cb-141">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="590cb-141">Optional query parameters</span></span>
<span data-ttu-id="590cb-142">このメソッドは[OData クエリ パラメーター](/graph/query-parameters)はサポート**されません**。</span><span class="sxs-lookup"><span data-stu-id="590cb-142">This method does **not** support [OData query parameters](/graph/query-parameters).</span></span>

### <a name="request-headers"></a><span data-ttu-id="590cb-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="590cb-143">Request headers</span></span>
| <span data-ttu-id="590cb-144">名前</span><span class="sxs-lookup"><span data-stu-id="590cb-144">Name</span></span>       | <span data-ttu-id="590cb-145">説明</span><span class="sxs-lookup"><span data-stu-id="590cb-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="590cb-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="590cb-146">Authorization</span></span>  | <span data-ttu-id="590cb-147">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="590cb-147">Bearer {code}</span></span>|
| <span data-ttu-id="590cb-148">Content-type</span><span class="sxs-lookup"><span data-stu-id="590cb-148">Content-type</span></span>  | <span data-ttu-id="590cb-149">application/json</span><span class="sxs-lookup"><span data-stu-id="590cb-149">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="590cb-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="590cb-150">Request body</span></span>
<span data-ttu-id="590cb-151">要求の本文には、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="590cb-151">In the request body, supply a JSON representation of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="590cb-152">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-152">Property</span></span>     | <span data-ttu-id="590cb-153">型</span><span class="sxs-lookup"><span data-stu-id="590cb-153">Type</span></span>    |<span data-ttu-id="590cb-154">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-154">Required</span></span>|  <span data-ttu-id="590cb-155">説明</span><span class="sxs-lookup"><span data-stu-id="590cb-155">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-156">resourceId</span></span>|<span data-ttu-id="590cb-157">String</span><span class="sxs-lookup"><span data-stu-id="590cb-157">String</span></span>|<span data-ttu-id="590cb-158">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-158">Yes</span></span>|<span data-ttu-id="590cb-159">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="590cb-159">The ID of the resource.</span></span>|
|<span data-ttu-id="590cb-160">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-160">roleDefinitionId</span></span>|<span data-ttu-id="590cb-161">String</span><span class="sxs-lookup"><span data-stu-id="590cb-161">String</span></span>|<span data-ttu-id="590cb-162">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-162">Yes</span></span>|<span data-ttu-id="590cb-163">役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="590cb-163">The ID of the role definition.</span></span>|
|<span data-ttu-id="590cb-164">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-164">subjectId</span></span>|<span data-ttu-id="590cb-165">String</span><span class="sxs-lookup"><span data-stu-id="590cb-165">String</span></span>|<span data-ttu-id="590cb-166">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-166">Yes</span></span>|<span data-ttu-id="590cb-167">サブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="590cb-167">The ID of the subject.</span></span>|
|<span data-ttu-id="590cb-168">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-168">assignmentState</span></span>|<span data-ttu-id="590cb-169">String</span><span class="sxs-lookup"><span data-stu-id="590cb-169">String</span></span>|<span data-ttu-id="590cb-170">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-170">Yes</span></span>|<span data-ttu-id="590cb-171">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="590cb-171">The state of assignment.</span></span> <span data-ttu-id="590cb-172">値は、``Eligible``と``Active``。</span><span class="sxs-lookup"><span data-stu-id="590cb-172">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="590cb-173">type</span><span class="sxs-lookup"><span data-stu-id="590cb-173">type</span></span>|<span data-ttu-id="590cb-174">String</span><span class="sxs-lookup"><span data-stu-id="590cb-174">String</span></span>|<span data-ttu-id="590cb-175">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-175">Yes</span></span>|<span data-ttu-id="590cb-176">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="590cb-176">The request type.</span></span> <span data-ttu-id="590cb-177">値は、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、`AdminRenew`と`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="590cb-177">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="590cb-178">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-178">reason</span></span>|<span data-ttu-id="590cb-179">String</span><span class="sxs-lookup"><span data-stu-id="590cb-179">String</span></span>| |<span data-ttu-id="590cb-180">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="590cb-180">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="590cb-181">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-181">schedule</span></span>|[<span data-ttu-id="590cb-182">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-182">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="590cb-183">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="590cb-183">The schedule of the role assignment request.</span></span> <span data-ttu-id="590cb-184">要求の種類の`UserAdd`、 `AdminAdd`、`AdminUpdate`と`AdminExtend`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="590cb-184">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

### <a name="response"></a><span data-ttu-id="590cb-185">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-185">Response</span></span>
<span data-ttu-id="590cb-186">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="590cb-186">If successful, this method returns a `201, Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="error-codes"></a><span data-ttu-id="590cb-187">エラー コード</span><span class="sxs-lookup"><span data-stu-id="590cb-187">Error codes</span></span>
<span data-ttu-id="590cb-188">この API は、HTTP コード、次の表に記載されているエラー コードの他の標準に準拠します。</span><span class="sxs-lookup"><span data-stu-id="590cb-188">This API follows the standard of HTTP codes, in addition to the error codes listed in the following table.</span></span>

|<span data-ttu-id="590cb-189">エラー コード</span><span class="sxs-lookup"><span data-stu-id="590cb-189">Error code</span></span>     | <span data-ttu-id="590cb-190">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="590cb-190">Error message</span></span>              | <span data-ttu-id="590cb-191">詳細</span><span class="sxs-lookup"><span data-stu-id="590cb-191">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="590cb-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-192">400 BadRequest</span></span> | <span data-ttu-id="590cb-193">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="590cb-193">RoleNotFound</span></span>    | <span data-ttu-id="590cb-194">`roleDefinitionId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="590cb-194">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="590cb-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-195">400 BadRequest</span></span> | <span data-ttu-id="590cb-196">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="590cb-196">ResourceIsLocked</span></span>    | <span data-ttu-id="590cb-197">状態の要求の本文に記載されているリソースは、`Locked`と、役割の割り当て要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="590cb-197">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="590cb-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-198">400 BadRequest</span></span> | <span data-ttu-id="590cb-199">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="590cb-199">SubjectNotFound</span></span>    | <span data-ttu-id="590cb-200">`subjectId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="590cb-200">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="590cb-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-201">400 BadRequest</span></span> | <span data-ttu-id="590cb-202">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-202">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="590cb-203">あるシステムで保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を既に存在します。</span><span class="sxs-lookup"><span data-stu-id="590cb-203">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="590cb-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-204">400 BadRequest</span></span> | <span data-ttu-id="590cb-205">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="590cb-205">RoleAssignmentExists</span></span>    | <span data-ttu-id="590cb-206">既に要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在します。</span><span class="sxs-lookup"><span data-stu-id="590cb-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="590cb-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-207">400 BadRequest</span></span> | <span data-ttu-id="590cb-208">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="590cb-208">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="590cb-209">更新または拡張するように要求した[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="590cb-209">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="590cb-210">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="590cb-210">400 BadRequest</span></span> | <span data-ttu-id="590cb-211">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="590cb-211">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="590cb-212">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は、社内ポリシーを満たしていないと、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="590cb-212">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="example-1"></a><span data-ttu-id="590cb-213">例 1</span><span class="sxs-lookup"><span data-stu-id="590cb-213">Example 1</span></span>
<span data-ttu-id="590cb-214">この例では、管理者は、課金情報の閲覧者の役割にユーザーの nawu@fimdev.net を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="590cb-214">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="590cb-215">**注:** 次の使用例以外にも、アクセス許可が少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="590cb-215">**Note:** Besides the permission, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="590cb-216">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-216">Property</span></span>     | <span data-ttu-id="590cb-217">型</span><span class="sxs-lookup"><span data-stu-id="590cb-217">Type</span></span>    |<span data-ttu-id="590cb-218">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-218">Required</span></span>|  <span data-ttu-id="590cb-219">値</span><span class="sxs-lookup"><span data-stu-id="590cb-219">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-220">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-220">resourceId</span></span>|<span data-ttu-id="590cb-221">String</span><span class="sxs-lookup"><span data-stu-id="590cb-221">String</span></span>|<span data-ttu-id="590cb-222">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-222">Yes</span></span>|<span data-ttu-id="590cb-223">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-223">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-224">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-224">roleDefinitionId</span></span>|<span data-ttu-id="590cb-225">String</span><span class="sxs-lookup"><span data-stu-id="590cb-225">String</span></span>|<span data-ttu-id="590cb-226">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-226">Yes</span></span>|<span data-ttu-id="590cb-227">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-227">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-228">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-228">subjectId</span></span>|<span data-ttu-id="590cb-229">String</span><span class="sxs-lookup"><span data-stu-id="590cb-229">String</span></span>|<span data-ttu-id="590cb-230">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-230">Yes</span></span>|<span data-ttu-id="590cb-231">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-231">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-232">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-232">assignmentState</span></span>|<span data-ttu-id="590cb-233">String</span><span class="sxs-lookup"><span data-stu-id="590cb-233">String</span></span>|<span data-ttu-id="590cb-234">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-234">Yes</span></span>| <span data-ttu-id="590cb-235">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-235">Eligible / Active</span></span>|
|<span data-ttu-id="590cb-236">type</span><span class="sxs-lookup"><span data-stu-id="590cb-236">type</span></span>|<span data-ttu-id="590cb-237">String</span><span class="sxs-lookup"><span data-stu-id="590cb-237">String</span></span>|<span data-ttu-id="590cb-238">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-238">Yes</span></span>| <span data-ttu-id="590cb-239">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="590cb-239">AdminAdd</span></span>|
|<span data-ttu-id="590cb-240">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-240">reason</span></span>|<span data-ttu-id="590cb-241">String</span><span class="sxs-lookup"><span data-stu-id="590cb-241">String</span></span>| <span data-ttu-id="590cb-242">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="590cb-242">depends on role Settings</span></span>||
|<span data-ttu-id="590cb-243">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-243">schedule</span></span>|[<span data-ttu-id="590cb-244">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-244">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-245">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-245">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-246">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-246">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-247">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-247">Response</span></span>
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
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
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

## <a name="example-2"></a><span data-ttu-id="590cb-248">例 2</span><span class="sxs-lookup"><span data-stu-id="590cb-248">Example 2</span></span>
<span data-ttu-id="590cb-249">この例では、ユーザー nawu@fimdev.net は、対象となる請求のリーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="590cb-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="590cb-250">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-250">Property</span></span>     | <span data-ttu-id="590cb-251">型</span><span class="sxs-lookup"><span data-stu-id="590cb-251">Type</span></span>    |<span data-ttu-id="590cb-252">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-252">Required</span></span>|  <span data-ttu-id="590cb-253">値</span><span class="sxs-lookup"><span data-stu-id="590cb-253">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-254">resourceId</span></span>|<span data-ttu-id="590cb-255">String</span><span class="sxs-lookup"><span data-stu-id="590cb-255">String</span></span>|<span data-ttu-id="590cb-256">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-256">Yes</span></span>|<span data-ttu-id="590cb-257">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-257">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-258">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-258">roleDefinitionId</span></span>|<span data-ttu-id="590cb-259">String</span><span class="sxs-lookup"><span data-stu-id="590cb-259">String</span></span>|<span data-ttu-id="590cb-260">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-260">Yes</span></span>|<span data-ttu-id="590cb-261">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-261">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-262">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-262">subjectId</span></span>|<span data-ttu-id="590cb-263">String</span><span class="sxs-lookup"><span data-stu-id="590cb-263">String</span></span>|<span data-ttu-id="590cb-264">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-264">Yes</span></span>|<span data-ttu-id="590cb-265">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-265">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-266">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-266">assignmentState</span></span>|<span data-ttu-id="590cb-267">String</span><span class="sxs-lookup"><span data-stu-id="590cb-267">String</span></span>|<span data-ttu-id="590cb-268">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-268">Yes</span></span>| <span data-ttu-id="590cb-269">アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-269">Active</span></span>|
|<span data-ttu-id="590cb-270">type</span><span class="sxs-lookup"><span data-stu-id="590cb-270">type</span></span>|<span data-ttu-id="590cb-271">String</span><span class="sxs-lookup"><span data-stu-id="590cb-271">String</span></span>|<span data-ttu-id="590cb-272">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-272">Yes</span></span>| <span data-ttu-id="590cb-273">UserAdd</span><span class="sxs-lookup"><span data-stu-id="590cb-273">UserAdd</span></span>|
|<span data-ttu-id="590cb-274">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-274">reason</span></span>|<span data-ttu-id="590cb-275">String</span><span class="sxs-lookup"><span data-stu-id="590cb-275">String</span></span>| <span data-ttu-id="590cb-276">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="590cb-276">depends on role Settings</span></span>||
|<span data-ttu-id="590cb-277">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-277">schedule</span></span>|[<span data-ttu-id="590cb-278">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-278">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-279">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-279">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-280">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-280">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-281">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-281">Response</span></span>
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
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
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

## <a name="example-3"></a><span data-ttu-id="590cb-282">例 3</span><span class="sxs-lookup"><span data-stu-id="590cb-282">Example 3</span></span>
<span data-ttu-id="590cb-283">この例では、ユーザー nawu@fimdev.net には、作業中の課金情報の閲覧者の役割が無効になります。</span><span class="sxs-lookup"><span data-stu-id="590cb-283">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="590cb-284">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-284">Property</span></span>     | <span data-ttu-id="590cb-285">型</span><span class="sxs-lookup"><span data-stu-id="590cb-285">Type</span></span>    |<span data-ttu-id="590cb-286">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-286">Required</span></span>|  <span data-ttu-id="590cb-287">値</span><span class="sxs-lookup"><span data-stu-id="590cb-287">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-288">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-288">resourceId</span></span>|<span data-ttu-id="590cb-289">String</span><span class="sxs-lookup"><span data-stu-id="590cb-289">String</span></span>|<span data-ttu-id="590cb-290">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-290">Yes</span></span>|<span data-ttu-id="590cb-291">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-291">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-292">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-292">roleDefinitionId</span></span>|<span data-ttu-id="590cb-293">String</span><span class="sxs-lookup"><span data-stu-id="590cb-293">String</span></span>|<span data-ttu-id="590cb-294">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-294">Yes</span></span>|<span data-ttu-id="590cb-295">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-295">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-296">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-296">subjectId</span></span>|<span data-ttu-id="590cb-297">String</span><span class="sxs-lookup"><span data-stu-id="590cb-297">String</span></span>|<span data-ttu-id="590cb-298">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-298">Yes</span></span>|<span data-ttu-id="590cb-299">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-299">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-300">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-300">assignmentState</span></span>|<span data-ttu-id="590cb-301">String</span><span class="sxs-lookup"><span data-stu-id="590cb-301">String</span></span>|<span data-ttu-id="590cb-302">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-302">Yes</span></span>| <span data-ttu-id="590cb-303">アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-303">Active</span></span>|
|<span data-ttu-id="590cb-304">type</span><span class="sxs-lookup"><span data-stu-id="590cb-304">type</span></span>|<span data-ttu-id="590cb-305">String</span><span class="sxs-lookup"><span data-stu-id="590cb-305">String</span></span>|<span data-ttu-id="590cb-306">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-306">Yes</span></span>| <span data-ttu-id="590cb-307">UserRemove</span><span class="sxs-lookup"><span data-stu-id="590cb-307">UserRemove</span></span>|
|<span data-ttu-id="590cb-308">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-308">reason</span></span>|<span data-ttu-id="590cb-309">String</span><span class="sxs-lookup"><span data-stu-id="590cb-309">String</span></span>| <span data-ttu-id="590cb-310">いいえ</span><span class="sxs-lookup"><span data-stu-id="590cb-310">No</span></span>||
|<span data-ttu-id="590cb-311">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-311">schedule</span></span>|[<span data-ttu-id="590cb-312">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-312">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-313">いいえ</span><span class="sxs-lookup"><span data-stu-id="590cb-313">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-314">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-314">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-315">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-315">Response</span></span>
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
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="590cb-316">例 4</span><span class="sxs-lookup"><span data-stu-id="590cb-316">Example 4</span></span>
<span data-ttu-id="590cb-317">この例では、管理者は、課金情報の閲覧者の役割からユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="590cb-317">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="590cb-318">**注:** 次の使用例以外にも、アクセス許可のスコープに少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="590cb-318">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="590cb-319">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-319">Property</span></span>     | <span data-ttu-id="590cb-320">型</span><span class="sxs-lookup"><span data-stu-id="590cb-320">Type</span></span>    |<span data-ttu-id="590cb-321">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-321">Required</span></span>|  <span data-ttu-id="590cb-322">値</span><span class="sxs-lookup"><span data-stu-id="590cb-322">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-323">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-323">resourceId</span></span>|<span data-ttu-id="590cb-324">String</span><span class="sxs-lookup"><span data-stu-id="590cb-324">String</span></span>|<span data-ttu-id="590cb-325">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-325">Yes</span></span>|<span data-ttu-id="590cb-326">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-326">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-327">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-327">roleDefinitionId</span></span>|<span data-ttu-id="590cb-328">String</span><span class="sxs-lookup"><span data-stu-id="590cb-328">String</span></span>|<span data-ttu-id="590cb-329">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-329">Yes</span></span>|<span data-ttu-id="590cb-330">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-330">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-331">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-331">subjectId</span></span>|<span data-ttu-id="590cb-332">String</span><span class="sxs-lookup"><span data-stu-id="590cb-332">String</span></span>|<span data-ttu-id="590cb-333">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-333">Yes</span></span>|<span data-ttu-id="590cb-334">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-334">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-335">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-335">assignmentState</span></span>|<span data-ttu-id="590cb-336">String</span><span class="sxs-lookup"><span data-stu-id="590cb-336">String</span></span>|<span data-ttu-id="590cb-337">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-337">Yes</span></span>| <span data-ttu-id="590cb-338">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-338">Eligible / Active</span></span>|
|<span data-ttu-id="590cb-339">type</span><span class="sxs-lookup"><span data-stu-id="590cb-339">type</span></span>|<span data-ttu-id="590cb-340">String</span><span class="sxs-lookup"><span data-stu-id="590cb-340">String</span></span>|<span data-ttu-id="590cb-341">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-341">Yes</span></span>| <span data-ttu-id="590cb-342">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="590cb-342">AdminRemove</span></span>|
|<span data-ttu-id="590cb-343">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-343">reason</span></span>|<span data-ttu-id="590cb-344">String</span><span class="sxs-lookup"><span data-stu-id="590cb-344">String</span></span>| <span data-ttu-id="590cb-345">いいえ</span><span class="sxs-lookup"><span data-stu-id="590cb-345">No</span></span>||
|<span data-ttu-id="590cb-346">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-346">schedule</span></span>|[<span data-ttu-id="590cb-347">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-347">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-348">いいえ</span><span class="sxs-lookup"><span data-stu-id="590cb-348">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-349">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-349">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-350">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-350">Response</span></span>
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
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="590cb-351">例 5</span><span class="sxs-lookup"><span data-stu-id="590cb-351">Example 5</span></span>
<span data-ttu-id="590cb-352">この例では、管理者は、所有者をユーザー nawu@fimdev.net の役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="590cb-352">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="590cb-353">**注:** 次の使用例以外にも、アクセス許可のスコープに少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="590cb-353">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 
| <span data-ttu-id="590cb-354">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-354">Property</span></span>     | <span data-ttu-id="590cb-355">型</span><span class="sxs-lookup"><span data-stu-id="590cb-355">Type</span></span>    |<span data-ttu-id="590cb-356">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-356">Required</span></span>|  <span data-ttu-id="590cb-357">値</span><span class="sxs-lookup"><span data-stu-id="590cb-357">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-358">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-358">resourceId</span></span>|<span data-ttu-id="590cb-359">String</span><span class="sxs-lookup"><span data-stu-id="590cb-359">String</span></span>|<span data-ttu-id="590cb-360">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-360">Yes</span></span>|<span data-ttu-id="590cb-361">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-361">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-362">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-362">roleDefinitionId</span></span>|<span data-ttu-id="590cb-363">String</span><span class="sxs-lookup"><span data-stu-id="590cb-363">String</span></span>|<span data-ttu-id="590cb-364">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-364">Yes</span></span>|<span data-ttu-id="590cb-365">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-365">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-366">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-366">subjectId</span></span>|<span data-ttu-id="590cb-367">String</span><span class="sxs-lookup"><span data-stu-id="590cb-367">String</span></span>|<span data-ttu-id="590cb-368">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-368">Yes</span></span>|<span data-ttu-id="590cb-369">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-369">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-370">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-370">assignmentState</span></span>|<span data-ttu-id="590cb-371">String</span><span class="sxs-lookup"><span data-stu-id="590cb-371">String</span></span>|<span data-ttu-id="590cb-372">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-372">Yes</span></span>| <span data-ttu-id="590cb-373">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-373">Eligible / Active</span></span>|
|<span data-ttu-id="590cb-374">type</span><span class="sxs-lookup"><span data-stu-id="590cb-374">type</span></span>|<span data-ttu-id="590cb-375">String</span><span class="sxs-lookup"><span data-stu-id="590cb-375">String</span></span>|<span data-ttu-id="590cb-376">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-376">Yes</span></span>| <span data-ttu-id="590cb-377">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="590cb-377">AdminUpdate</span></span>|
|<span data-ttu-id="590cb-378">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-378">reason</span></span>|<span data-ttu-id="590cb-379">String</span><span class="sxs-lookup"><span data-stu-id="590cb-379">String</span></span>| <span data-ttu-id="590cb-380">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="590cb-380">depends on roleSettings</span></span>||
|<span data-ttu-id="590cb-381">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-381">schedule</span></span>|[<span data-ttu-id="590cb-382">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-382">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-383">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-383">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-384">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-384">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-385">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-385">Response</span></span>
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
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
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

### <a name="example-6"></a><span data-ttu-id="590cb-386">例 6</span><span class="sxs-lookup"><span data-stu-id="590cb-386">Example 6</span></span>
<span data-ttu-id="590cb-387">次の使用例は、API の管理サービスの共同作成者に ANUJCUSER のユーザーの有効期限切れのロールの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="590cb-387">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="590cb-388">**注:** 次の使用例以外にも、アクセス許可のスコープに少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="590cb-388">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="590cb-389">プロパティ</span><span class="sxs-lookup"><span data-stu-id="590cb-389">Property</span></span>     | <span data-ttu-id="590cb-390">型</span><span class="sxs-lookup"><span data-stu-id="590cb-390">Type</span></span>    |<span data-ttu-id="590cb-391">必須</span><span class="sxs-lookup"><span data-stu-id="590cb-391">Required</span></span>|  <span data-ttu-id="590cb-392">値</span><span class="sxs-lookup"><span data-stu-id="590cb-392">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="590cb-393">resourceId</span><span class="sxs-lookup"><span data-stu-id="590cb-393">resourceId</span></span>|<span data-ttu-id="590cb-394">String</span><span class="sxs-lookup"><span data-stu-id="590cb-394">String</span></span>|<span data-ttu-id="590cb-395">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-395">Yes</span></span>|<span data-ttu-id="590cb-396">\<とります\></span><span class="sxs-lookup"><span data-stu-id="590cb-396">\<resourceId\></span></span>|
|<span data-ttu-id="590cb-397">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="590cb-397">roleDefinitionId</span></span>|<span data-ttu-id="590cb-398">String</span><span class="sxs-lookup"><span data-stu-id="590cb-398">String</span></span>|<span data-ttu-id="590cb-399">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-399">Yes</span></span>|<span data-ttu-id="590cb-400">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="590cb-400">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="590cb-401">subjectId</span><span class="sxs-lookup"><span data-stu-id="590cb-401">subjectId</span></span>|<span data-ttu-id="590cb-402">String</span><span class="sxs-lookup"><span data-stu-id="590cb-402">String</span></span>|<span data-ttu-id="590cb-403">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-403">Yes</span></span>|<span data-ttu-id="590cb-404">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="590cb-404">\<subjectId\></span></span>|
|<span data-ttu-id="590cb-405">assignmentState</span><span class="sxs-lookup"><span data-stu-id="590cb-405">assignmentState</span></span>|<span data-ttu-id="590cb-406">String</span><span class="sxs-lookup"><span data-stu-id="590cb-406">String</span></span>|<span data-ttu-id="590cb-407">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-407">Yes</span></span>| <span data-ttu-id="590cb-408">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="590cb-408">Eligible / Active</span></span> |
|<span data-ttu-id="590cb-409">type</span><span class="sxs-lookup"><span data-stu-id="590cb-409">type</span></span>|<span data-ttu-id="590cb-410">String</span><span class="sxs-lookup"><span data-stu-id="590cb-410">String</span></span>|<span data-ttu-id="590cb-411">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-411">Yes</span></span>| <span data-ttu-id="590cb-412">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="590cb-412">AdminExtend</span></span>|
|<span data-ttu-id="590cb-413">理由</span><span class="sxs-lookup"><span data-stu-id="590cb-413">reason</span></span>|<span data-ttu-id="590cb-414">String</span><span class="sxs-lookup"><span data-stu-id="590cb-414">String</span></span>| <span data-ttu-id="590cb-415">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="590cb-415">depends on roleSettings</span></span>||
|<span data-ttu-id="590cb-416">スケジュール</span><span class="sxs-lookup"><span data-stu-id="590cb-416">schedule</span></span>|[<span data-ttu-id="590cb-417">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="590cb-417">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="590cb-418">はい</span><span class="sxs-lookup"><span data-stu-id="590cb-418">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="590cb-419">要求</span><span class="sxs-lookup"><span data-stu-id="590cb-419">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="590cb-420">応答</span><span class="sxs-lookup"><span data-stu-id="590cb-420">Response</span></span>
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
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
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
