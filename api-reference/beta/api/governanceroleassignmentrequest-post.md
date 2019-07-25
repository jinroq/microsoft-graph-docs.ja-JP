---
title: GovernanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
ms.openlocfilehash: 674a69f5697f5abf6e654ea71419bdfdfd660343
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859113"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="864e8-104">GovernanceRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="864e8-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="864e8-105">役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="864e8-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="864e8-106">次の表に、操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="864e8-106">The following table lists the operations.</span></span>

| <span data-ttu-id="864e8-107">Operation</span><span class="sxs-lookup"><span data-stu-id="864e8-107">Operation</span></span>                                   | <span data-ttu-id="864e8-108">型</span><span class="sxs-lookup"><span data-stu-id="864e8-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="864e8-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="864e8-109">Assign a role assignment</span></span>                    | <span data-ttu-id="864e8-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="864e8-110">AdminAdd</span></span>    |
| <span data-ttu-id="864e8-111">適格な役割の割り当てをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="864e8-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="864e8-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="864e8-112">UserAdd</span></span>     |
| <span data-ttu-id="864e8-113">アクティブ化された役割の割り当てを無効にする</span><span class="sxs-lookup"><span data-stu-id="864e8-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="864e8-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="864e8-114">UserRemove</span></span>  |
| <span data-ttu-id="864e8-115">役割の割り当てを削除する</span><span class="sxs-lookup"><span data-stu-id="864e8-115">Remove a role assignment</span></span>                    | <span data-ttu-id="864e8-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="864e8-116">AdminRemove</span></span> |
| <span data-ttu-id="864e8-117">役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="864e8-117">Update a role assignment</span></span>                    | <span data-ttu-id="864e8-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="864e8-118">AdminUpdate</span></span> |
| <span data-ttu-id="864e8-119">自分の役割の割り当てを拡張するための要求</span><span class="sxs-lookup"><span data-stu-id="864e8-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="864e8-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="864e8-120">UserExtend</span></span>  |
| <span data-ttu-id="864e8-121">役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="864e8-121">Extend a role assignment</span></span>                    | <span data-ttu-id="864e8-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="864e8-122">AdminExtend</span></span> |
| <span data-ttu-id="864e8-123">期限切れの役割の割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="864e8-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="864e8-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="864e8-124">UserRenew</span></span>   |
| <span data-ttu-id="864e8-125">期限切れの役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="864e8-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="864e8-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="864e8-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="864e8-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="864e8-127">Permissions</span></span>

<span data-ttu-id="864e8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="864e8-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="864e8-130">Permission type</span></span>                        | <span data-ttu-id="864e8-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="864e8-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="864e8-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="864e8-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="864e8-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="864e8-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="864e8-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="864e8-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="864e8-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="864e8-135">Not supported.</span></span>                            |
| <span data-ttu-id="864e8-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="864e8-136">Application</span></span>                            | <span data-ttu-id="864e8-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="864e8-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="864e8-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="864e8-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="864e8-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="864e8-139">Request headers</span></span>

| <span data-ttu-id="864e8-140">名前</span><span class="sxs-lookup"><span data-stu-id="864e8-140">Name</span></span>          | <span data-ttu-id="864e8-141">説明</span><span class="sxs-lookup"><span data-stu-id="864e8-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="864e8-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="864e8-142">Authorization</span></span> | <span data-ttu-id="864e8-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="864e8-143">Bearer {code}</span></span>    |
| <span data-ttu-id="864e8-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="864e8-144">Content-type</span></span>  | <span data-ttu-id="864e8-145">application/json</span><span class="sxs-lookup"><span data-stu-id="864e8-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="864e8-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="864e8-146">Request body</span></span>

<span data-ttu-id="864e8-147">要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="864e8-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="864e8-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-148">Property</span></span>         | <span data-ttu-id="864e8-149">型</span><span class="sxs-lookup"><span data-stu-id="864e8-149">Type</span></span>                                                     | <span data-ttu-id="864e8-150">説明</span><span class="sxs-lookup"><span data-stu-id="864e8-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="864e8-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-151">resourceId</span></span>       | <span data-ttu-id="864e8-152">String</span><span class="sxs-lookup"><span data-stu-id="864e8-152">String</span></span>                                                   | <span data-ttu-id="864e8-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="864e8-153">The ID of the resource.</span></span> <span data-ttu-id="864e8-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="864e8-154">Required.</span></span> |
| <span data-ttu-id="864e8-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-155">roleDefinitionId</span></span> | <span data-ttu-id="864e8-156">String</span><span class="sxs-lookup"><span data-stu-id="864e8-156">String</span></span>                                                   | <span data-ttu-id="864e8-157">ロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="864e8-157">The ID of the role definition.</span></span> <span data-ttu-id="864e8-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="864e8-158">Required.</span></span> |
| <span data-ttu-id="864e8-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-159">subjectId</span></span>        | <span data-ttu-id="864e8-160">String</span><span class="sxs-lookup"><span data-stu-id="864e8-160">String</span></span>                                                   | <span data-ttu-id="864e8-161">件名の ID。</span><span class="sxs-lookup"><span data-stu-id="864e8-161">The ID of the subject.</span></span> <span data-ttu-id="864e8-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="864e8-162">Required.</span></span> |
| <span data-ttu-id="864e8-163">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-163">assignmentState</span></span>  | <span data-ttu-id="864e8-164">String</span><span class="sxs-lookup"><span data-stu-id="864e8-164">String</span></span>                                                   | <span data-ttu-id="864e8-165">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="864e8-165">The state of assignment.</span></span> <span data-ttu-id="864e8-166">値には、 `Eligible`および`Active`を指定できます。</span><span class="sxs-lookup"><span data-stu-id="864e8-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="864e8-167">必須。</span><span class="sxs-lookup"><span data-stu-id="864e8-167">Required.</span></span> |
| <span data-ttu-id="864e8-168">type</span><span class="sxs-lookup"><span data-stu-id="864e8-168">type</span></span>             | <span data-ttu-id="864e8-169">String</span><span class="sxs-lookup"><span data-stu-id="864e8-169">String</span></span>                                                   | <span data-ttu-id="864e8-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="864e8-170">The request type.</span></span> <span data-ttu-id="864e8-171">値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。</span><span class="sxs-lookup"><span data-stu-id="864e8-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="864e8-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="864e8-172">Required.</span></span> |
| <span data-ttu-id="864e8-173">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-173">reason</span></span>           | <span data-ttu-id="864e8-174">String</span><span class="sxs-lookup"><span data-stu-id="864e8-174">String</span></span>                                                   | <span data-ttu-id="864e8-175">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="864e8-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="864e8-176">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-176">schedule</span></span>         | [<span data-ttu-id="864e8-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-178">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="864e8-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="864e8-179">、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate`</span><span class="sxs-lookup"><span data-stu-id="864e8-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="864e8-180">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-180">Response</span></span>

<span data-ttu-id="864e8-181">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="864e8-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="864e8-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="864e8-182">Error codes</span></span>

<span data-ttu-id="864e8-183">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="864e8-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="864e8-184">また、次の表に示されているエラーコードも返します。</span><span class="sxs-lookup"><span data-stu-id="864e8-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="864e8-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="864e8-185">Error code</span></span>     | <span data-ttu-id="864e8-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="864e8-186">Error message</span></span>                               | <span data-ttu-id="864e8-187">詳細</span><span class="sxs-lookup"><span data-stu-id="864e8-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="864e8-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-188">400 BadRequest</span></span> | <span data-ttu-id="864e8-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="864e8-189">RoleNotFound</span></span>                                | <span data-ttu-id="864e8-190">要求`roleDefinitionId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="864e8-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="864e8-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-191">400 BadRequest</span></span> | <span data-ttu-id="864e8-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="864e8-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="864e8-193">要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。</span><span class="sxs-lookup"><span data-stu-id="864e8-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="864e8-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-194">400 BadRequest</span></span> | <span data-ttu-id="864e8-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="864e8-195">SubjectNotFound</span></span>                             | <span data-ttu-id="864e8-196">要求`subjectId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="864e8-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="864e8-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-197">400 BadRequest</span></span> | <span data-ttu-id="864e8-198">Pendingrole割り当て要求</span><span class="sxs-lookup"><span data-stu-id="864e8-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="864e8-199">保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="864e8-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="864e8-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-200">400 BadRequest</span></span> | <span data-ttu-id="864e8-201">Role割り当てが存在する</span><span class="sxs-lookup"><span data-stu-id="864e8-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="864e8-202">作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。</span><span class="sxs-lookup"><span data-stu-id="864e8-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="864e8-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-203">400 BadRequest</span></span> | <span data-ttu-id="864e8-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="864e8-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="864e8-205">更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="864e8-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="864e8-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="864e8-206">400 BadRequest</span></span> | <span data-ttu-id="864e8-207">Role割り当て要求 Policyvalidationfailed</span><span class="sxs-lookup"><span data-stu-id="864e8-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="864e8-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="864e8-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="864e8-209">例</span><span class="sxs-lookup"><span data-stu-id="864e8-209">Examples</span></span>

<span data-ttu-id="864e8-210">次の例は、この API の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="864e8-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="864e8-211">例 1: 管理者がユーザーを役割に割り当てる</span><span class="sxs-lookup"><span data-stu-id="864e8-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="864e8-212">この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="864e8-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="864e8-213">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="864e8-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="864e8-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-214">Property</span></span>         | <span data-ttu-id="864e8-215">型</span><span class="sxs-lookup"><span data-stu-id="864e8-215">Type</span></span>                                                     | <span data-ttu-id="864e8-216">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-216">Required</span></span>                 | <span data-ttu-id="864e8-217">値</span><span class="sxs-lookup"><span data-stu-id="864e8-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="864e8-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-218">resourceId</span></span>       | <span data-ttu-id="864e8-219">String</span><span class="sxs-lookup"><span data-stu-id="864e8-219">String</span></span>                                                   | <span data-ttu-id="864e8-220">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-220">Yes</span></span>                      | <span data-ttu-id="864e8-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-221">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-222">roleDefinitionId</span></span> | <span data-ttu-id="864e8-223">String</span><span class="sxs-lookup"><span data-stu-id="864e8-223">String</span></span>                                                   | <span data-ttu-id="864e8-224">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-224">Yes</span></span>                      | <span data-ttu-id="864e8-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-226">subjectId</span></span>        | <span data-ttu-id="864e8-227">String</span><span class="sxs-lookup"><span data-stu-id="864e8-227">String</span></span>                                                   | <span data-ttu-id="864e8-228">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-228">Yes</span></span>                      | <span data-ttu-id="864e8-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-229">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-230">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-230">assignmentState</span></span>  | <span data-ttu-id="864e8-231">String</span><span class="sxs-lookup"><span data-stu-id="864e8-231">String</span></span>                                                   | <span data-ttu-id="864e8-232">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-232">Yes</span></span>                      | <span data-ttu-id="864e8-233">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="864e8-233">Eligible / Active</span></span> |
| <span data-ttu-id="864e8-234">type</span><span class="sxs-lookup"><span data-stu-id="864e8-234">type</span></span>             | <span data-ttu-id="864e8-235">String</span><span class="sxs-lookup"><span data-stu-id="864e8-235">String</span></span>                                                   | <span data-ttu-id="864e8-236">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-236">Yes</span></span>                      | <span data-ttu-id="864e8-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="864e8-237">AdminAdd</span></span> |
| <span data-ttu-id="864e8-238">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-238">reason</span></span>           | <span data-ttu-id="864e8-239">String</span><span class="sxs-lookup"><span data-stu-id="864e8-239">String</span></span>                                                   | <span data-ttu-id="864e8-240">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="864e8-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="864e8-241">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-241">schedule</span></span>         | [<span data-ttu-id="864e8-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-243">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="864e8-244">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="864e8-245">プロトコル</span><span class="sxs-lookup"><span data-stu-id="864e8-245">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="864e8-246">C#</span><span class="sxs-lookup"><span data-stu-id="864e8-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="864e8-247">Javascript</span><span class="sxs-lookup"><span data-stu-id="864e8-247">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="864e8-248">目的-C</span><span class="sxs-lookup"><span data-stu-id="864e8-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="864e8-249">Java</span><span class="sxs-lookup"><span data-stu-id="864e8-249">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="864e8-250">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-250">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="864e8-251">例 2: ユーザーが対象となる役割をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="864e8-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="864e8-252">この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="864e8-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="864e8-253">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-253">Property</span></span>         | <span data-ttu-id="864e8-254">型</span><span class="sxs-lookup"><span data-stu-id="864e8-254">Type</span></span>                                                     | <span data-ttu-id="864e8-255">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-255">Required</span></span>                 | <span data-ttu-id="864e8-256">値</span><span class="sxs-lookup"><span data-stu-id="864e8-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="864e8-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-257">resourceId</span></span>       | <span data-ttu-id="864e8-258">String</span><span class="sxs-lookup"><span data-stu-id="864e8-258">String</span></span>                                                   | <span data-ttu-id="864e8-259">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-259">Yes</span></span>                      | <span data-ttu-id="864e8-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-260">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-261">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-261">roleDefinitionId</span></span> | <span data-ttu-id="864e8-262">String</span><span class="sxs-lookup"><span data-stu-id="864e8-262">String</span></span>                                                   | <span data-ttu-id="864e8-263">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-263">Yes</span></span>                      | <span data-ttu-id="864e8-264">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-265">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-265">subjectId</span></span>        | <span data-ttu-id="864e8-266">String</span><span class="sxs-lookup"><span data-stu-id="864e8-266">String</span></span>                                                   | <span data-ttu-id="864e8-267">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-267">Yes</span></span>                      | <span data-ttu-id="864e8-268">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-268">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-269">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-269">assignmentState</span></span>  | <span data-ttu-id="864e8-270">String</span><span class="sxs-lookup"><span data-stu-id="864e8-270">String</span></span>                                                   | <span data-ttu-id="864e8-271">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-271">Yes</span></span>                      | <span data-ttu-id="864e8-272">Active</span><span class="sxs-lookup"><span data-stu-id="864e8-272">Active</span></span> |
| <span data-ttu-id="864e8-273">type</span><span class="sxs-lookup"><span data-stu-id="864e8-273">type</span></span>             | <span data-ttu-id="864e8-274">String</span><span class="sxs-lookup"><span data-stu-id="864e8-274">String</span></span>                                                   | <span data-ttu-id="864e8-275">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-275">Yes</span></span>                      | <span data-ttu-id="864e8-276">UserAdd</span><span class="sxs-lookup"><span data-stu-id="864e8-276">UserAdd</span></span> |
| <span data-ttu-id="864e8-277">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-277">reason</span></span>           | <span data-ttu-id="864e8-278">String</span><span class="sxs-lookup"><span data-stu-id="864e8-278">String</span></span>                                                   | <span data-ttu-id="864e8-279">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="864e8-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="864e8-280">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-280">schedule</span></span>         | [<span data-ttu-id="864e8-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-282">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="864e8-283">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-283">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a><span data-ttu-id="864e8-284">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-284">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="864e8-285">例 3: ユーザーが割り当てられた役割を非アクティブにする</span><span class="sxs-lookup"><span data-stu-id="864e8-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="864e8-286">この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="864e8-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="864e8-287">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-287">Property</span></span>         | <span data-ttu-id="864e8-288">型</span><span class="sxs-lookup"><span data-stu-id="864e8-288">Type</span></span>                                                     | <span data-ttu-id="864e8-289">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-289">Required</span></span> | <span data-ttu-id="864e8-290">値</span><span class="sxs-lookup"><span data-stu-id="864e8-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="864e8-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-291">resourceId</span></span>       | <span data-ttu-id="864e8-292">String</span><span class="sxs-lookup"><span data-stu-id="864e8-292">String</span></span>                                                   | <span data-ttu-id="864e8-293">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-293">Yes</span></span>      | <span data-ttu-id="864e8-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-294">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-295">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-295">roleDefinitionId</span></span> | <span data-ttu-id="864e8-296">String</span><span class="sxs-lookup"><span data-stu-id="864e8-296">String</span></span>                                                   | <span data-ttu-id="864e8-297">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-297">Yes</span></span>      | <span data-ttu-id="864e8-298">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-299">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-299">subjectId</span></span>        | <span data-ttu-id="864e8-300">String</span><span class="sxs-lookup"><span data-stu-id="864e8-300">String</span></span>                                                   | <span data-ttu-id="864e8-301">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-301">Yes</span></span>      | <span data-ttu-id="864e8-302">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-302">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-303">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-303">assignmentState</span></span>  | <span data-ttu-id="864e8-304">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-304">String</span></span>                                                   | <span data-ttu-id="864e8-305">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-305">Yes</span></span>      | <span data-ttu-id="864e8-306">Active</span><span class="sxs-lookup"><span data-stu-id="864e8-306">Active</span></span> |
| <span data-ttu-id="864e8-307">type</span><span class="sxs-lookup"><span data-stu-id="864e8-307">type</span></span>             | <span data-ttu-id="864e8-308">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-308">String</span></span>                                                   | <span data-ttu-id="864e8-309">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-309">Yes</span></span>      | <span data-ttu-id="864e8-310">UserRemove</span><span class="sxs-lookup"><span data-stu-id="864e8-310">UserRemove</span></span> |
| <span data-ttu-id="864e8-311">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-311">reason</span></span>           | <span data-ttu-id="864e8-312">String</span><span class="sxs-lookup"><span data-stu-id="864e8-312">String</span></span>                                                   | <span data-ttu-id="864e8-313">いいえ</span><span class="sxs-lookup"><span data-stu-id="864e8-313">No</span></span>       |   |
| <span data-ttu-id="864e8-314">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-314">schedule</span></span>         | [<span data-ttu-id="864e8-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-316">いいえ</span><span class="sxs-lookup"><span data-stu-id="864e8-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="864e8-317">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-317">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a><span data-ttu-id="864e8-318">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-318">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="864e8-319">例 4: 管理者が役割からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="864e8-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="864e8-320">この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="864e8-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="864e8-321">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="864e8-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="864e8-322">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-322">Property</span></span>         | <span data-ttu-id="864e8-323">型</span><span class="sxs-lookup"><span data-stu-id="864e8-323">Type</span></span>                                                     | <span data-ttu-id="864e8-324">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-324">Required</span></span> | <span data-ttu-id="864e8-325">値</span><span class="sxs-lookup"><span data-stu-id="864e8-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="864e8-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-326">resourceId</span></span>       | <span data-ttu-id="864e8-327">String</span><span class="sxs-lookup"><span data-stu-id="864e8-327">String</span></span>                                                   | <span data-ttu-id="864e8-328">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-328">Yes</span></span>      | <span data-ttu-id="864e8-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-329">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-330">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-330">roleDefinitionId</span></span> | <span data-ttu-id="864e8-331">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-331">String</span></span>                                                   | <span data-ttu-id="864e8-332">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-332">Yes</span></span>      | <span data-ttu-id="864e8-333">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-334">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-334">subjectId</span></span>        | <span data-ttu-id="864e8-335">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-335">String</span></span>                                                   | <span data-ttu-id="864e8-336">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-336">Yes</span></span>      | <span data-ttu-id="864e8-337">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-337">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-338">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-338">assignmentState</span></span>  | <span data-ttu-id="864e8-339">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-339">String</span></span>                                                   | <span data-ttu-id="864e8-340">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-340">Yes</span></span>      | <span data-ttu-id="864e8-341">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="864e8-341">Eligible / Active</span></span> |
| <span data-ttu-id="864e8-342">type</span><span class="sxs-lookup"><span data-stu-id="864e8-342">type</span></span>             | <span data-ttu-id="864e8-343">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-343">String</span></span>                                                   | <span data-ttu-id="864e8-344">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-344">Yes</span></span>      | <span data-ttu-id="864e8-345">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="864e8-345">AdminRemove</span></span> |
| <span data-ttu-id="864e8-346">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-346">reason</span></span>           | <span data-ttu-id="864e8-347">String</span><span class="sxs-lookup"><span data-stu-id="864e8-347">String</span></span>                                                   | <span data-ttu-id="864e8-348">いいえ</span><span class="sxs-lookup"><span data-stu-id="864e8-348">No</span></span>       |   |
| <span data-ttu-id="864e8-349">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-349">schedule</span></span>         | [<span data-ttu-id="864e8-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-351">いいえ</span><span class="sxs-lookup"><span data-stu-id="864e8-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="864e8-352">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-352">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a><span data-ttu-id="864e8-353">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-353">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="864e8-354">例 5: 管理者の更新の役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="864e8-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="864e8-355">この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。</span><span class="sxs-lookup"><span data-stu-id="864e8-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="864e8-356">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="864e8-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="864e8-357">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-357">Property</span></span>         | <span data-ttu-id="864e8-358">型</span><span class="sxs-lookup"><span data-stu-id="864e8-358">Type</span></span>                                                     | <span data-ttu-id="864e8-359">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-359">Required</span></span>                | <span data-ttu-id="864e8-360">値</span><span class="sxs-lookup"><span data-stu-id="864e8-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="864e8-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-361">resourceId</span></span>       | <span data-ttu-id="864e8-362">String</span><span class="sxs-lookup"><span data-stu-id="864e8-362">String</span></span>                                                   | <span data-ttu-id="864e8-363">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-363">Yes</span></span>                     | <span data-ttu-id="864e8-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-364">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-365">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-365">roleDefinitionId</span></span> | <span data-ttu-id="864e8-366">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-366">String</span></span>                                                   | <span data-ttu-id="864e8-367">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-367">Yes</span></span>                     | <span data-ttu-id="864e8-368">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-369">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-369">subjectId</span></span>        | <span data-ttu-id="864e8-370">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-370">String</span></span>                                                   | <span data-ttu-id="864e8-371">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-371">Yes</span></span>                     | <span data-ttu-id="864e8-372">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-372">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-373">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-373">assignmentState</span></span>  | <span data-ttu-id="864e8-374">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-374">String</span></span>                                                   | <span data-ttu-id="864e8-375">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-375">Yes</span></span>                     | <span data-ttu-id="864e8-376">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="864e8-376">Eligible / Active</span></span> |
| <span data-ttu-id="864e8-377">type</span><span class="sxs-lookup"><span data-stu-id="864e8-377">type</span></span>             | <span data-ttu-id="864e8-378">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-378">String</span></span>                                                   | <span data-ttu-id="864e8-379">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-379">Yes</span></span>                     | <span data-ttu-id="864e8-380">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="864e8-380">AdminUpdate</span></span> |
| <span data-ttu-id="864e8-381">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-381">reason</span></span>           | <span data-ttu-id="864e8-382">String</span><span class="sxs-lookup"><span data-stu-id="864e8-382">String</span></span>                                                   | <span data-ttu-id="864e8-383">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="864e8-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="864e8-384">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-384">schedule</span></span>         | [<span data-ttu-id="864e8-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-386">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="864e8-387">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-387">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="864e8-388">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-388">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="864e8-389">例 6: 管理者が期限切れの役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="864e8-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="864e8-390">この例では、user ANUCUSER の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。</span><span class="sxs-lookup"><span data-stu-id="864e8-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="864e8-391">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="864e8-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="864e8-392">プロパティ</span><span class="sxs-lookup"><span data-stu-id="864e8-392">Property</span></span>         | <span data-ttu-id="864e8-393">型</span><span class="sxs-lookup"><span data-stu-id="864e8-393">Type</span></span>                                                     | <span data-ttu-id="864e8-394">必須</span><span class="sxs-lookup"><span data-stu-id="864e8-394">Required</span></span>                | <span data-ttu-id="864e8-395">値</span><span class="sxs-lookup"><span data-stu-id="864e8-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="864e8-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="864e8-396">resourceId</span></span>       | <span data-ttu-id="864e8-397">String</span><span class="sxs-lookup"><span data-stu-id="864e8-397">String</span></span>                                                   | <span data-ttu-id="864e8-398">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-398">Yes</span></span>                     | <span data-ttu-id="864e8-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="864e8-399">\<resourceId\></span></span> |
| <span data-ttu-id="864e8-400">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="864e8-400">roleDefinitionId</span></span> | <span data-ttu-id="864e8-401">文字列</span><span class="sxs-lookup"><span data-stu-id="864e8-401">String</span></span>                                                   | <span data-ttu-id="864e8-402">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-402">Yes</span></span>                     | <span data-ttu-id="864e8-403">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="864e8-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="864e8-404">subjectId</span><span class="sxs-lookup"><span data-stu-id="864e8-404">subjectId</span></span>        | <span data-ttu-id="864e8-405">String</span><span class="sxs-lookup"><span data-stu-id="864e8-405">String</span></span>                                                   | <span data-ttu-id="864e8-406">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-406">Yes</span></span>                     | <span data-ttu-id="864e8-407">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="864e8-407">\<subjectId\></span></span> |
| <span data-ttu-id="864e8-408">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="864e8-408">assignmentState</span></span>  | <span data-ttu-id="864e8-409">String</span><span class="sxs-lookup"><span data-stu-id="864e8-409">String</span></span>                                                   | <span data-ttu-id="864e8-410">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-410">Yes</span></span>                     | <span data-ttu-id="864e8-411">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="864e8-411">Eligible / Active</span></span> |
| <span data-ttu-id="864e8-412">type</span><span class="sxs-lookup"><span data-stu-id="864e8-412">type</span></span>             | <span data-ttu-id="864e8-413">String</span><span class="sxs-lookup"><span data-stu-id="864e8-413">String</span></span>                                                   | <span data-ttu-id="864e8-414">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-414">Yes</span></span>                     | <span data-ttu-id="864e8-415">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="864e8-415">AdminExtend</span></span> |
| <span data-ttu-id="864e8-416">したがっ</span><span class="sxs-lookup"><span data-stu-id="864e8-416">reason</span></span>           | <span data-ttu-id="864e8-417">String</span><span class="sxs-lookup"><span data-stu-id="864e8-417">String</span></span>                                                   | <span data-ttu-id="864e8-418">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="864e8-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="864e8-419">schedule</span><span class="sxs-lookup"><span data-stu-id="864e8-419">schedule</span></span>         | [<span data-ttu-id="864e8-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="864e8-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="864e8-421">はい</span><span class="sxs-lookup"><span data-stu-id="864e8-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="864e8-422">要求</span><span class="sxs-lookup"><span data-stu-id="864e8-422">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="864e8-423">応答</span><span class="sxs-lookup"><span data-stu-id="864e8-423">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
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
  ]
}
-->
