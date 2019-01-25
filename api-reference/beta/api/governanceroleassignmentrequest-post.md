---
title: GovernanceRoleAssignmentRequest を作成します。
description: 役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523240"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="e470d-104">GovernanceRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="e470d-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e470d-105">役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="e470d-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="e470d-106">次の表に、操作をします。</span><span class="sxs-lookup"><span data-stu-id="e470d-106">The following table lists the operations.</span></span>

| <span data-ttu-id="e470d-107">Operation</span><span class="sxs-lookup"><span data-stu-id="e470d-107">Operation</span></span>       | <span data-ttu-id="e470d-108">型</span><span class="sxs-lookup"><span data-stu-id="e470d-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="e470d-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="e470d-109">Assign a role assignment</span></span>| <span data-ttu-id="e470d-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="e470d-110">AdminAdd</span></span> |
| <span data-ttu-id="e470d-111">対象のロール割り当てを有効化します。</span><span class="sxs-lookup"><span data-stu-id="e470d-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="e470d-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="e470d-112">UserAdd</span></span> | 
| <span data-ttu-id="e470d-113">アクティブ化されたロール割り当てを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="e470d-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="e470d-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="e470d-114">UserRemove</span></span> | 
| <span data-ttu-id="e470d-115">役割の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="e470d-115">Remove a role assignment</span></span>| <span data-ttu-id="e470d-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="e470d-116">AdminRemove</span></span> |
| <span data-ttu-id="e470d-117">役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="e470d-117">Update a role assignment</span></span>| <span data-ttu-id="e470d-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="e470d-118">AdminUpdate</span></span> |
| <span data-ttu-id="e470d-119">自分の役割の割り当てを拡張する要求</span><span class="sxs-lookup"><span data-stu-id="e470d-119">Request to extend my role assignment</span></span>| <span data-ttu-id="e470d-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="e470d-120">UserExtend</span></span> | 
| <span data-ttu-id="e470d-121">役割の割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="e470d-121">Extend a role assignment</span></span>| <span data-ttu-id="e470d-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="e470d-122">AdminExtend</span></span> | 
| <span data-ttu-id="e470d-123">[期限切れのロールの割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="e470d-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="e470d-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="e470d-124">UserRenew</span></span> | 
| <span data-ttu-id="e470d-125">期限切れのロール割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="e470d-125">Renew an expired role assignment</span></span>| <span data-ttu-id="e470d-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="e470d-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="e470d-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e470d-127">Permissions</span></span>
<span data-ttu-id="e470d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e470d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e470d-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e470d-130">Permission type</span></span>      | <span data-ttu-id="e470d-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e470d-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e470d-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e470d-132">Delegated (work or school account)</span></span> | <span data-ttu-id="e470d-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e470d-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e470d-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e470d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e470d-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e470d-135">Not supported.</span></span>    |
|<span data-ttu-id="e470d-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e470d-136">Application</span></span> | <span data-ttu-id="e470d-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e470d-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e470d-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e470d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="e470d-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e470d-139">Request headers</span></span>
| <span data-ttu-id="e470d-140">名前</span><span class="sxs-lookup"><span data-stu-id="e470d-140">Name</span></span>       | <span data-ttu-id="e470d-141">説明</span><span class="sxs-lookup"><span data-stu-id="e470d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e470d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e470d-142">Authorization</span></span>  | <span data-ttu-id="e470d-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e470d-143">Bearer {code}</span></span>|
| <span data-ttu-id="e470d-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="e470d-144">Content-type</span></span>  | <span data-ttu-id="e470d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="e470d-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e470d-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="e470d-146">Request body</span></span>
<span data-ttu-id="e470d-147">要求の本文には、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="e470d-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="e470d-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-148">Property</span></span>     | <span data-ttu-id="e470d-149">型</span><span class="sxs-lookup"><span data-stu-id="e470d-149">Type</span></span>    |<span data-ttu-id="e470d-150">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-150">Required</span></span>|  <span data-ttu-id="e470d-151">説明</span><span class="sxs-lookup"><span data-stu-id="e470d-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-152">resourceId</span></span>|<span data-ttu-id="e470d-153">String</span><span class="sxs-lookup"><span data-stu-id="e470d-153">String</span></span>|<span data-ttu-id="e470d-154">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-154">Yes</span></span>|<span data-ttu-id="e470d-155">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="e470d-155">The ID of the resource.</span></span>|
|<span data-ttu-id="e470d-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-156">roleDefinitionId</span></span>|<span data-ttu-id="e470d-157">String</span><span class="sxs-lookup"><span data-stu-id="e470d-157">String</span></span>|<span data-ttu-id="e470d-158">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-158">Yes</span></span>|<span data-ttu-id="e470d-159">役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="e470d-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="e470d-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-160">subjectId</span></span>|<span data-ttu-id="e470d-161">String</span><span class="sxs-lookup"><span data-stu-id="e470d-161">String</span></span>|<span data-ttu-id="e470d-162">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-162">Yes</span></span>|<span data-ttu-id="e470d-163">サブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="e470d-163">The ID of the subject.</span></span>|
|<span data-ttu-id="e470d-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-164">assignmentState</span></span>|<span data-ttu-id="e470d-165">String</span><span class="sxs-lookup"><span data-stu-id="e470d-165">String</span></span>|<span data-ttu-id="e470d-166">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-166">Yes</span></span>|<span data-ttu-id="e470d-167">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="e470d-167">The state of assignment.</span></span> <span data-ttu-id="e470d-168">値は、``Eligible``と``Active``。</span><span class="sxs-lookup"><span data-stu-id="e470d-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="e470d-169">type</span><span class="sxs-lookup"><span data-stu-id="e470d-169">type</span></span>|<span data-ttu-id="e470d-170">String</span><span class="sxs-lookup"><span data-stu-id="e470d-170">String</span></span>|<span data-ttu-id="e470d-171">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-171">Yes</span></span>|<span data-ttu-id="e470d-172">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="e470d-172">The request type.</span></span> <span data-ttu-id="e470d-173">値は、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、`AdminRenew`と`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="e470d-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="e470d-174">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-174">reason</span></span>|<span data-ttu-id="e470d-175">String</span><span class="sxs-lookup"><span data-stu-id="e470d-175">String</span></span>| |<span data-ttu-id="e470d-176">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e470d-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="e470d-177">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-177">schedule</span></span>|[<span data-ttu-id="e470d-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="e470d-179">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="e470d-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="e470d-180">要求の種類の`UserAdd`、 `AdminAdd`、`AdminUpdate`と`AdminExtend`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="e470d-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="e470d-181">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-181">Response</span></span>
<span data-ttu-id="e470d-182">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e470d-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="e470d-183">エラー コード</span><span class="sxs-lookup"><span data-stu-id="e470d-183">Error codes</span></span>
<span data-ttu-id="e470d-184">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e470d-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="e470d-185">さらに、また次の表に記載されているエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e470d-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="e470d-186">エラー コード</span><span class="sxs-lookup"><span data-stu-id="e470d-186">Error code</span></span>     | <span data-ttu-id="e470d-187">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="e470d-187">Error message</span></span>              | <span data-ttu-id="e470d-188">詳細</span><span class="sxs-lookup"><span data-stu-id="e470d-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="e470d-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-189">400 BadRequest</span></span> | <span data-ttu-id="e470d-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="e470d-190">RoleNotFound</span></span>    | <span data-ttu-id="e470d-191">`roleDefinitionId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="e470d-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="e470d-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-192">400 BadRequest</span></span> | <span data-ttu-id="e470d-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="e470d-193">ResourceIsLocked</span></span>    | <span data-ttu-id="e470d-194">状態の要求の本文に記載されているリソースは、`Locked`と、役割の割り当て要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="e470d-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="e470d-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-195">400 BadRequest</span></span> | <span data-ttu-id="e470d-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="e470d-196">SubjectNotFound</span></span>    | <span data-ttu-id="e470d-197">`subjectId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="e470d-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="e470d-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-198">400 BadRequest</span></span> | <span data-ttu-id="e470d-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="e470d-200">あるシステムで保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を既に存在します。</span><span class="sxs-lookup"><span data-stu-id="e470d-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="e470d-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-201">400 BadRequest</span></span> | <span data-ttu-id="e470d-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="e470d-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="e470d-203">既に要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在します。</span><span class="sxs-lookup"><span data-stu-id="e470d-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="e470d-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-204">400 BadRequest</span></span> | <span data-ttu-id="e470d-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="e470d-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="e470d-206">更新または拡張するように要求した[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="e470d-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="e470d-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e470d-207">400 BadRequest</span></span> | <span data-ttu-id="e470d-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="e470d-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="e470d-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は、社内ポリシーを満たしていないと、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="e470d-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="e470d-210">例</span><span class="sxs-lookup"><span data-stu-id="e470d-210">Examples</span></span>
<span data-ttu-id="e470d-211">次の例では、この API を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e470d-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="e470d-212">例 1</span><span class="sxs-lookup"><span data-stu-id="e470d-212">Example 1</span></span>
<span data-ttu-id="e470d-213">この例では、管理者は、課金情報の閲覧者の役割にユーザーの nawu@fimdev.net を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="e470d-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="e470d-214">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="e470d-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="e470d-215">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-215">Property</span></span>     | <span data-ttu-id="e470d-216">型</span><span class="sxs-lookup"><span data-stu-id="e470d-216">Type</span></span>    |<span data-ttu-id="e470d-217">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-217">Required</span></span>|  <span data-ttu-id="e470d-218">値</span><span class="sxs-lookup"><span data-stu-id="e470d-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-219">resourceId</span></span>|<span data-ttu-id="e470d-220">String</span><span class="sxs-lookup"><span data-stu-id="e470d-220">String</span></span>|<span data-ttu-id="e470d-221">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-221">Yes</span></span>|<span data-ttu-id="e470d-222">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-222">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-223">roleDefinitionId</span></span>|<span data-ttu-id="e470d-224">String</span><span class="sxs-lookup"><span data-stu-id="e470d-224">String</span></span>|<span data-ttu-id="e470d-225">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-225">Yes</span></span>|<span data-ttu-id="e470d-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-227">subjectId</span></span>|<span data-ttu-id="e470d-228">String</span><span class="sxs-lookup"><span data-stu-id="e470d-228">String</span></span>|<span data-ttu-id="e470d-229">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-229">Yes</span></span>|<span data-ttu-id="e470d-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-230">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-231">assignmentState</span></span>|<span data-ttu-id="e470d-232">String</span><span class="sxs-lookup"><span data-stu-id="e470d-232">String</span></span>|<span data-ttu-id="e470d-233">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-233">Yes</span></span>| <span data-ttu-id="e470d-234">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="e470d-234">Eligible / Active</span></span>|
|<span data-ttu-id="e470d-235">type</span><span class="sxs-lookup"><span data-stu-id="e470d-235">type</span></span>|<span data-ttu-id="e470d-236">String</span><span class="sxs-lookup"><span data-stu-id="e470d-236">String</span></span>|<span data-ttu-id="e470d-237">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-237">Yes</span></span>| <span data-ttu-id="e470d-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="e470d-238">AdminAdd</span></span>|
|<span data-ttu-id="e470d-239">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-239">reason</span></span>|<span data-ttu-id="e470d-240">String</span><span class="sxs-lookup"><span data-stu-id="e470d-240">String</span></span>| <span data-ttu-id="e470d-241">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="e470d-241">depends on role Settings</span></span>||
|<span data-ttu-id="e470d-242">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-242">schedule</span></span>|[<span data-ttu-id="e470d-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-244">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-245">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-246">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="e470d-247">例 2</span><span class="sxs-lookup"><span data-stu-id="e470d-247">Example 2</span></span>
<span data-ttu-id="e470d-248">この例では、ユーザー nawu@fimdev.net は、対象となる請求のリーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="e470d-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="e470d-249">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-249">Property</span></span>     | <span data-ttu-id="e470d-250">型</span><span class="sxs-lookup"><span data-stu-id="e470d-250">Type</span></span>    |<span data-ttu-id="e470d-251">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-251">Required</span></span>|  <span data-ttu-id="e470d-252">値</span><span class="sxs-lookup"><span data-stu-id="e470d-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-253">resourceId</span></span>|<span data-ttu-id="e470d-254">String</span><span class="sxs-lookup"><span data-stu-id="e470d-254">String</span></span>|<span data-ttu-id="e470d-255">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-255">Yes</span></span>|<span data-ttu-id="e470d-256">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-256">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-257">roleDefinitionId</span></span>|<span data-ttu-id="e470d-258">String</span><span class="sxs-lookup"><span data-stu-id="e470d-258">String</span></span>|<span data-ttu-id="e470d-259">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-259">Yes</span></span>|<span data-ttu-id="e470d-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-261">subjectId</span></span>|<span data-ttu-id="e470d-262">String</span><span class="sxs-lookup"><span data-stu-id="e470d-262">String</span></span>|<span data-ttu-id="e470d-263">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-263">Yes</span></span>|<span data-ttu-id="e470d-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-264">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-265">assignmentState</span></span>|<span data-ttu-id="e470d-266">String</span><span class="sxs-lookup"><span data-stu-id="e470d-266">String</span></span>|<span data-ttu-id="e470d-267">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-267">Yes</span></span>| <span data-ttu-id="e470d-268">Active</span><span class="sxs-lookup"><span data-stu-id="e470d-268">Active</span></span>|
|<span data-ttu-id="e470d-269">type</span><span class="sxs-lookup"><span data-stu-id="e470d-269">type</span></span>|<span data-ttu-id="e470d-270">String</span><span class="sxs-lookup"><span data-stu-id="e470d-270">String</span></span>|<span data-ttu-id="e470d-271">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-271">Yes</span></span>| <span data-ttu-id="e470d-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="e470d-272">UserAdd</span></span>|
|<span data-ttu-id="e470d-273">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-273">reason</span></span>|<span data-ttu-id="e470d-274">String</span><span class="sxs-lookup"><span data-stu-id="e470d-274">String</span></span>| <span data-ttu-id="e470d-275">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="e470d-275">depends on role Settings</span></span>||
|<span data-ttu-id="e470d-276">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-276">schedule</span></span>|[<span data-ttu-id="e470d-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-278">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-279">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-280">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="e470d-281">例 3</span><span class="sxs-lookup"><span data-stu-id="e470d-281">Example 3</span></span>
<span data-ttu-id="e470d-282">この例では、ユーザー nawu@fimdev.net には、作業中の課金情報の閲覧者の役割が無効になります。</span><span class="sxs-lookup"><span data-stu-id="e470d-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="e470d-283">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-283">Property</span></span>     | <span data-ttu-id="e470d-284">型</span><span class="sxs-lookup"><span data-stu-id="e470d-284">Type</span></span>    |<span data-ttu-id="e470d-285">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-285">Required</span></span>|  <span data-ttu-id="e470d-286">値</span><span class="sxs-lookup"><span data-stu-id="e470d-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-287">resourceId</span></span>|<span data-ttu-id="e470d-288">String</span><span class="sxs-lookup"><span data-stu-id="e470d-288">String</span></span>|<span data-ttu-id="e470d-289">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-289">Yes</span></span>|<span data-ttu-id="e470d-290">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-290">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-291">roleDefinitionId</span></span>|<span data-ttu-id="e470d-292">String</span><span class="sxs-lookup"><span data-stu-id="e470d-292">String</span></span>|<span data-ttu-id="e470d-293">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-293">Yes</span></span>|<span data-ttu-id="e470d-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-295">subjectId</span></span>|<span data-ttu-id="e470d-296">String</span><span class="sxs-lookup"><span data-stu-id="e470d-296">String</span></span>|<span data-ttu-id="e470d-297">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-297">Yes</span></span>|<span data-ttu-id="e470d-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-298">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-299">assignmentState</span></span>|<span data-ttu-id="e470d-300">String</span><span class="sxs-lookup"><span data-stu-id="e470d-300">String</span></span>|<span data-ttu-id="e470d-301">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-301">Yes</span></span>| <span data-ttu-id="e470d-302">Active</span><span class="sxs-lookup"><span data-stu-id="e470d-302">Active</span></span>|
|<span data-ttu-id="e470d-303">type</span><span class="sxs-lookup"><span data-stu-id="e470d-303">type</span></span>|<span data-ttu-id="e470d-304">String</span><span class="sxs-lookup"><span data-stu-id="e470d-304">String</span></span>|<span data-ttu-id="e470d-305">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-305">Yes</span></span>| <span data-ttu-id="e470d-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="e470d-306">UserRemove</span></span>|
|<span data-ttu-id="e470d-307">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-307">reason</span></span>|<span data-ttu-id="e470d-308">String</span><span class="sxs-lookup"><span data-stu-id="e470d-308">String</span></span>| <span data-ttu-id="e470d-309">いいえ</span><span class="sxs-lookup"><span data-stu-id="e470d-309">No</span></span>||
|<span data-ttu-id="e470d-310">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-310">schedule</span></span>|[<span data-ttu-id="e470d-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-312">いいえ</span><span class="sxs-lookup"><span data-stu-id="e470d-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-313">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-314">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="e470d-315">例 4</span><span class="sxs-lookup"><span data-stu-id="e470d-315">Example 4</span></span>
<span data-ttu-id="e470d-316">この例では、管理者は、課金情報の閲覧者の役割からユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="e470d-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="e470d-317">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="e470d-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="e470d-318">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-318">Property</span></span>     | <span data-ttu-id="e470d-319">型</span><span class="sxs-lookup"><span data-stu-id="e470d-319">Type</span></span>    |<span data-ttu-id="e470d-320">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-320">Required</span></span>|  <span data-ttu-id="e470d-321">値</span><span class="sxs-lookup"><span data-stu-id="e470d-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-322">resourceId</span></span>|<span data-ttu-id="e470d-323">String</span><span class="sxs-lookup"><span data-stu-id="e470d-323">String</span></span>|<span data-ttu-id="e470d-324">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-324">Yes</span></span>|<span data-ttu-id="e470d-325">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-325">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-326">roleDefinitionId</span></span>|<span data-ttu-id="e470d-327">String</span><span class="sxs-lookup"><span data-stu-id="e470d-327">String</span></span>|<span data-ttu-id="e470d-328">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-328">Yes</span></span>|<span data-ttu-id="e470d-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-330">subjectId</span></span>|<span data-ttu-id="e470d-331">String</span><span class="sxs-lookup"><span data-stu-id="e470d-331">String</span></span>|<span data-ttu-id="e470d-332">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-332">Yes</span></span>|<span data-ttu-id="e470d-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-333">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-334">assignmentState</span></span>|<span data-ttu-id="e470d-335">String</span><span class="sxs-lookup"><span data-stu-id="e470d-335">String</span></span>|<span data-ttu-id="e470d-336">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-336">Yes</span></span>| <span data-ttu-id="e470d-337">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="e470d-337">Eligible / Active</span></span>|
|<span data-ttu-id="e470d-338">type</span><span class="sxs-lookup"><span data-stu-id="e470d-338">type</span></span>|<span data-ttu-id="e470d-339">String</span><span class="sxs-lookup"><span data-stu-id="e470d-339">String</span></span>|<span data-ttu-id="e470d-340">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-340">Yes</span></span>| <span data-ttu-id="e470d-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="e470d-341">AdminRemove</span></span>|
|<span data-ttu-id="e470d-342">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-342">reason</span></span>|<span data-ttu-id="e470d-343">String</span><span class="sxs-lookup"><span data-stu-id="e470d-343">String</span></span>| <span data-ttu-id="e470d-344">いいえ</span><span class="sxs-lookup"><span data-stu-id="e470d-344">No</span></span>||
|<span data-ttu-id="e470d-345">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-345">schedule</span></span>|[<span data-ttu-id="e470d-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-347">いいえ</span><span class="sxs-lookup"><span data-stu-id="e470d-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-348">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-349">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="e470d-350">例 5</span><span class="sxs-lookup"><span data-stu-id="e470d-350">Example 5</span></span>
<span data-ttu-id="e470d-351">この例では、管理者は、所有者をユーザー nawu@fimdev.net の役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="e470d-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="e470d-352">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="e470d-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="e470d-353">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-353">Property</span></span>     | <span data-ttu-id="e470d-354">型</span><span class="sxs-lookup"><span data-stu-id="e470d-354">Type</span></span>    |<span data-ttu-id="e470d-355">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-355">Required</span></span>|  <span data-ttu-id="e470d-356">値</span><span class="sxs-lookup"><span data-stu-id="e470d-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-357">resourceId</span></span>|<span data-ttu-id="e470d-358">String</span><span class="sxs-lookup"><span data-stu-id="e470d-358">String</span></span>|<span data-ttu-id="e470d-359">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-359">Yes</span></span>|<span data-ttu-id="e470d-360">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-360">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-361">roleDefinitionId</span></span>|<span data-ttu-id="e470d-362">String</span><span class="sxs-lookup"><span data-stu-id="e470d-362">String</span></span>|<span data-ttu-id="e470d-363">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-363">Yes</span></span>|<span data-ttu-id="e470d-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-365">subjectId</span></span>|<span data-ttu-id="e470d-366">String</span><span class="sxs-lookup"><span data-stu-id="e470d-366">String</span></span>|<span data-ttu-id="e470d-367">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-367">Yes</span></span>|<span data-ttu-id="e470d-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-368">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-369">assignmentState</span></span>|<span data-ttu-id="e470d-370">String</span><span class="sxs-lookup"><span data-stu-id="e470d-370">String</span></span>|<span data-ttu-id="e470d-371">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-371">Yes</span></span>| <span data-ttu-id="e470d-372">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="e470d-372">Eligible / Active</span></span>|
|<span data-ttu-id="e470d-373">type</span><span class="sxs-lookup"><span data-stu-id="e470d-373">type</span></span>|<span data-ttu-id="e470d-374">String</span><span class="sxs-lookup"><span data-stu-id="e470d-374">String</span></span>|<span data-ttu-id="e470d-375">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-375">Yes</span></span>| <span data-ttu-id="e470d-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="e470d-376">AdminUpdate</span></span>|
|<span data-ttu-id="e470d-377">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-377">reason</span></span>|<span data-ttu-id="e470d-378">String</span><span class="sxs-lookup"><span data-stu-id="e470d-378">String</span></span>| <span data-ttu-id="e470d-379">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="e470d-379">depends on roleSettings</span></span>||
|<span data-ttu-id="e470d-380">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-380">schedule</span></span>|[<span data-ttu-id="e470d-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-382">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-383">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-384">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="e470d-385">例 6</span><span class="sxs-lookup"><span data-stu-id="e470d-385">Example 6</span></span>
<span data-ttu-id="e470d-386">次の使用例は、API の管理サービスの共同作成者に ANUJCUSER のユーザーの有効期限切れのロールの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="e470d-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="e470d-387">**注:** Additon アクセス許可を次の使用例が必要です、依頼者が少なくとも 1 つであること`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="e470d-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="e470d-388">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e470d-388">Property</span></span>     | <span data-ttu-id="e470d-389">型</span><span class="sxs-lookup"><span data-stu-id="e470d-389">Type</span></span>    |<span data-ttu-id="e470d-390">必須</span><span class="sxs-lookup"><span data-stu-id="e470d-390">Required</span></span>|  <span data-ttu-id="e470d-391">値</span><span class="sxs-lookup"><span data-stu-id="e470d-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="e470d-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="e470d-392">resourceId</span></span>|<span data-ttu-id="e470d-393">String</span><span class="sxs-lookup"><span data-stu-id="e470d-393">String</span></span>|<span data-ttu-id="e470d-394">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-394">Yes</span></span>|<span data-ttu-id="e470d-395">\<</span><span class="sxs-lookup"><span data-stu-id="e470d-395">\<resourceId\></span></span>|
|<span data-ttu-id="e470d-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e470d-396">roleDefinitionId</span></span>|<span data-ttu-id="e470d-397">String</span><span class="sxs-lookup"><span data-stu-id="e470d-397">String</span></span>|<span data-ttu-id="e470d-398">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-398">Yes</span></span>|<span data-ttu-id="e470d-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e470d-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="e470d-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="e470d-400">subjectId</span></span>|<span data-ttu-id="e470d-401">String</span><span class="sxs-lookup"><span data-stu-id="e470d-401">String</span></span>|<span data-ttu-id="e470d-402">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-402">Yes</span></span>|<span data-ttu-id="e470d-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e470d-403">\<subjectId\></span></span>|
|<span data-ttu-id="e470d-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e470d-404">assignmentState</span></span>|<span data-ttu-id="e470d-405">String</span><span class="sxs-lookup"><span data-stu-id="e470d-405">String</span></span>|<span data-ttu-id="e470d-406">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-406">Yes</span></span>| <span data-ttu-id="e470d-407">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="e470d-407">Eligible / Active</span></span> |
|<span data-ttu-id="e470d-408">type</span><span class="sxs-lookup"><span data-stu-id="e470d-408">type</span></span>|<span data-ttu-id="e470d-409">String</span><span class="sxs-lookup"><span data-stu-id="e470d-409">String</span></span>|<span data-ttu-id="e470d-410">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-410">Yes</span></span>| <span data-ttu-id="e470d-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="e470d-411">AdminExtend</span></span>|
|<span data-ttu-id="e470d-412">理由</span><span class="sxs-lookup"><span data-stu-id="e470d-412">reason</span></span>|<span data-ttu-id="e470d-413">String</span><span class="sxs-lookup"><span data-stu-id="e470d-413">String</span></span>| <span data-ttu-id="e470d-414">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="e470d-414">depends on roleSettings</span></span>||
|<span data-ttu-id="e470d-415">Schedule</span><span class="sxs-lookup"><span data-stu-id="e470d-415">schedule</span></span>|[<span data-ttu-id="e470d-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e470d-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="e470d-417">はい</span><span class="sxs-lookup"><span data-stu-id="e470d-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="e470d-418">要求</span><span class="sxs-lookup"><span data-stu-id="e470d-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e470d-419">応答</span><span class="sxs-lookup"><span data-stu-id="e470d-419">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
