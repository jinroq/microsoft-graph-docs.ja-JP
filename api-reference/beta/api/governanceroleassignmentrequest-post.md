---
title: GovernanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
ms.openlocfilehash: be27c8e0bab24f6a83e970b9aae46d0742be7c10
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422368"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="16d1f-104">GovernanceRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="16d1f-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16d1f-105">役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="16d1f-106">次の表に、操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-106">The following table lists the operations.</span></span>

| <span data-ttu-id="16d1f-107">Operation</span><span class="sxs-lookup"><span data-stu-id="16d1f-107">Operation</span></span>                                   | <span data-ttu-id="16d1f-108">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="16d1f-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="16d1f-109">Assign a role assignment</span></span>                    | <span data-ttu-id="16d1f-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="16d1f-110">AdminAdd</span></span>    |
| <span data-ttu-id="16d1f-111">適格な役割の割り当てをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="16d1f-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="16d1f-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="16d1f-112">UserAdd</span></span>     |
| <span data-ttu-id="16d1f-113">アクティブ化された役割の割り当てを無効にする</span><span class="sxs-lookup"><span data-stu-id="16d1f-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="16d1f-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="16d1f-114">UserRemove</span></span>  |
| <span data-ttu-id="16d1f-115">役割の割り当てを削除する</span><span class="sxs-lookup"><span data-stu-id="16d1f-115">Remove a role assignment</span></span>                    | <span data-ttu-id="16d1f-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="16d1f-116">AdminRemove</span></span> |
| <span data-ttu-id="16d1f-117">役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="16d1f-117">Update a role assignment</span></span>                    | <span data-ttu-id="16d1f-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="16d1f-118">AdminUpdate</span></span> |
| <span data-ttu-id="16d1f-119">自分の役割の割り当てを拡張するための要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="16d1f-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="16d1f-120">UserExtend</span></span>  |
| <span data-ttu-id="16d1f-121">役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="16d1f-121">Extend a role assignment</span></span>                    | <span data-ttu-id="16d1f-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="16d1f-122">AdminExtend</span></span> |
| <span data-ttu-id="16d1f-123">期限切れの役割の割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="16d1f-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="16d1f-124">UserRenew</span></span>   |
| <span data-ttu-id="16d1f-125">期限切れの役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="16d1f-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="16d1f-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="16d1f-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="16d1f-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16d1f-127">Permissions</span></span>

<span data-ttu-id="16d1f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16d1f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16d1f-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16d1f-130">Permission type</span></span>                        | <span data-ttu-id="16d1f-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16d1f-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="16d1f-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1f-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="16d1f-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="16d1f-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="16d1f-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1f-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16d1f-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-135">Not supported.</span></span>                            |
| <span data-ttu-id="16d1f-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16d1f-136">Application</span></span>                            | <span data-ttu-id="16d1f-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16d1f-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="16d1f-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16d1f-139">Request headers</span></span>

| <span data-ttu-id="16d1f-140">名前</span><span class="sxs-lookup"><span data-stu-id="16d1f-140">Name</span></span>          | <span data-ttu-id="16d1f-141">説明</span><span class="sxs-lookup"><span data-stu-id="16d1f-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="16d1f-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="16d1f-142">Authorization</span></span> | <span data-ttu-id="16d1f-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="16d1f-143">Bearer {code}</span></span>    |
| <span data-ttu-id="16d1f-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="16d1f-144">Content-type</span></span>  | <span data-ttu-id="16d1f-145">application/json</span><span class="sxs-lookup"><span data-stu-id="16d1f-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="16d1f-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="16d1f-146">Request body</span></span>

<span data-ttu-id="16d1f-147">要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="16d1f-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-148">Property</span></span>         | <span data-ttu-id="16d1f-149">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-149">Type</span></span>                                                     | <span data-ttu-id="16d1f-150">説明</span><span class="sxs-lookup"><span data-stu-id="16d1f-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="16d1f-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-151">resourceId</span></span>       | <span data-ttu-id="16d1f-152">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-152">String</span></span>                                                   | <span data-ttu-id="16d1f-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="16d1f-153">The ID of the resource.</span></span> <span data-ttu-id="16d1f-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="16d1f-154">Required.</span></span> |
| <span data-ttu-id="16d1f-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-155">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-156">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-156">String</span></span>                                                   | <span data-ttu-id="16d1f-157">ロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="16d1f-157">The ID of the role definition.</span></span> <span data-ttu-id="16d1f-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="16d1f-158">Required.</span></span> |
| <span data-ttu-id="16d1f-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-159">subjectId</span></span>        | <span data-ttu-id="16d1f-160">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-160">String</span></span>                                                   | <span data-ttu-id="16d1f-161">件名の ID。</span><span class="sxs-lookup"><span data-stu-id="16d1f-161">The ID of the subject.</span></span> <span data-ttu-id="16d1f-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="16d1f-162">Required.</span></span> |
| <span data-ttu-id="16d1f-163">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-163">assignmentState</span></span>  | <span data-ttu-id="16d1f-164">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-164">String</span></span>                                                   | <span data-ttu-id="16d1f-165">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-165">The state of assignment.</span></span> <span data-ttu-id="16d1f-166">値には、 `Eligible`および`Active`を指定できます。</span><span class="sxs-lookup"><span data-stu-id="16d1f-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="16d1f-167">必須。</span><span class="sxs-lookup"><span data-stu-id="16d1f-167">Required.</span></span> |
| <span data-ttu-id="16d1f-168">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-168">type</span></span>             | <span data-ttu-id="16d1f-169">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-169">String</span></span>                                                   | <span data-ttu-id="16d1f-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="16d1f-170">The request type.</span></span> <span data-ttu-id="16d1f-171">値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。</span><span class="sxs-lookup"><span data-stu-id="16d1f-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="16d1f-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="16d1f-172">Required.</span></span> |
| <span data-ttu-id="16d1f-173">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-173">reason</span></span>           | <span data-ttu-id="16d1f-174">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-174">String</span></span>                                                   | <span data-ttu-id="16d1f-175">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1f-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="16d1f-176">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-176">schedule</span></span>         | [<span data-ttu-id="16d1f-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-178">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="16d1f-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="16d1f-179">、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate`</span><span class="sxs-lookup"><span data-stu-id="16d1f-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="16d1f-180">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-180">Response</span></span>

<span data-ttu-id="16d1f-181">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="16d1f-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="16d1f-182">Error codes</span></span>

<span data-ttu-id="16d1f-183">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="16d1f-184">また、次の表に示されているエラーコードも返します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="16d1f-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="16d1f-185">Error code</span></span>     | <span data-ttu-id="16d1f-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="16d1f-186">Error message</span></span>                               | <span data-ttu-id="16d1f-187">詳細</span><span class="sxs-lookup"><span data-stu-id="16d1f-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="16d1f-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-188">400 BadRequest</span></span> | <span data-ttu-id="16d1f-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="16d1f-189">RoleNotFound</span></span>                                | <span data-ttu-id="16d1f-190">要求`roleDefinitionId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="16d1f-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-191">400 BadRequest</span></span> | <span data-ttu-id="16d1f-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="16d1f-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="16d1f-193">要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="16d1f-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-194">400 BadRequest</span></span> | <span data-ttu-id="16d1f-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="16d1f-195">SubjectNotFound</span></span>                             | <span data-ttu-id="16d1f-196">要求`subjectId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="16d1f-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-197">400 BadRequest</span></span> | <span data-ttu-id="16d1f-198">Pendingrole割り当て要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="16d1f-199">保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="16d1f-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-200">400 BadRequest</span></span> | <span data-ttu-id="16d1f-201">Role割り当てが存在する</span><span class="sxs-lookup"><span data-stu-id="16d1f-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="16d1f-202">作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。</span><span class="sxs-lookup"><span data-stu-id="16d1f-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="16d1f-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-203">400 BadRequest</span></span> | <span data-ttu-id="16d1f-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="16d1f-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="16d1f-205">更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="16d1f-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="16d1f-206">400 BadRequest</span></span> | <span data-ttu-id="16d1f-207">Role割り当て要求 Policyvalidationfailed</span><span class="sxs-lookup"><span data-stu-id="16d1f-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="16d1f-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="16d1f-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="16d1f-209">例</span><span class="sxs-lookup"><span data-stu-id="16d1f-209">Examples</span></span>

<span data-ttu-id="16d1f-210">次の例は、この API の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="16d1f-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="16d1f-211">例 1: 管理者がユーザーを役割に割り当てる</span><span class="sxs-lookup"><span data-stu-id="16d1f-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="16d1f-212">この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="16d1f-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="16d1f-213">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1f-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="16d1f-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-214">Property</span></span>         | <span data-ttu-id="16d1f-215">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-215">Type</span></span>                                                     | <span data-ttu-id="16d1f-216">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-216">Required</span></span>                 | <span data-ttu-id="16d1f-217">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="16d1f-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-218">resourceId</span></span>       | <span data-ttu-id="16d1f-219">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-219">String</span></span>                                                   | <span data-ttu-id="16d1f-220">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-220">Yes</span></span>                      | <span data-ttu-id="16d1f-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-221">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-222">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-223">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-223">String</span></span>                                                   | <span data-ttu-id="16d1f-224">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-224">Yes</span></span>                      | <span data-ttu-id="16d1f-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-226">subjectId</span></span>        | <span data-ttu-id="16d1f-227">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-227">String</span></span>                                                   | <span data-ttu-id="16d1f-228">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-228">Yes</span></span>                      | <span data-ttu-id="16d1f-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-229">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-230">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-230">assignmentState</span></span>  | <span data-ttu-id="16d1f-231">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-231">String</span></span>                                                   | <span data-ttu-id="16d1f-232">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-232">Yes</span></span>                      | <span data-ttu-id="16d1f-233">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="16d1f-233">Eligible / Active</span></span> |
| <span data-ttu-id="16d1f-234">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-234">type</span></span>             | <span data-ttu-id="16d1f-235">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-235">String</span></span>                                                   | <span data-ttu-id="16d1f-236">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-236">Yes</span></span>                      | <span data-ttu-id="16d1f-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="16d1f-237">AdminAdd</span></span> |
| <span data-ttu-id="16d1f-238">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-238">reason</span></span>           | <span data-ttu-id="16d1f-239">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-239">String</span></span>                                                   | <span data-ttu-id="16d1f-240">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="16d1f-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="16d1f-241">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-241">schedule</span></span>         | [<span data-ttu-id="16d1f-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-243">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="16d1f-244">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-244">Request</span></span>

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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="16d1f-245">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-245">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="16d1f-246">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="16d1f-246">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="16d1f-247">C#</span><span class="sxs-lookup"><span data-stu-id="16d1f-247">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d1f-248">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d1f-248">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="16d1f-249">例 2: ユーザーが対象となる役割をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="16d1f-249">Example 2: User activates eligible role</span></span>

<span data-ttu-id="16d1f-250">この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="16d1f-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="16d1f-251">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-251">Property</span></span>         | <span data-ttu-id="16d1f-252">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-252">Type</span></span>                                                     | <span data-ttu-id="16d1f-253">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-253">Required</span></span>                 | <span data-ttu-id="16d1f-254">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-254">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="16d1f-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-255">resourceId</span></span>       | <span data-ttu-id="16d1f-256">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-256">String</span></span>                                                   | <span data-ttu-id="16d1f-257">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-257">Yes</span></span>                      | <span data-ttu-id="16d1f-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-258">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-259">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-260">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-260">String</span></span>                                                   | <span data-ttu-id="16d1f-261">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-261">Yes</span></span>                      | <span data-ttu-id="16d1f-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-262">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-263">subjectId</span></span>        | <span data-ttu-id="16d1f-264">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-264">String</span></span>                                                   | <span data-ttu-id="16d1f-265">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-265">Yes</span></span>                      | <span data-ttu-id="16d1f-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-266">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-267">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-267">assignmentState</span></span>  | <span data-ttu-id="16d1f-268">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-268">String</span></span>                                                   | <span data-ttu-id="16d1f-269">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-269">Yes</span></span>                      | <span data-ttu-id="16d1f-270">Active</span><span class="sxs-lookup"><span data-stu-id="16d1f-270">Active</span></span> |
| <span data-ttu-id="16d1f-271">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-271">type</span></span>             | <span data-ttu-id="16d1f-272">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-272">String</span></span>                                                   | <span data-ttu-id="16d1f-273">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-273">Yes</span></span>                      | <span data-ttu-id="16d1f-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="16d1f-274">UserAdd</span></span> |
| <span data-ttu-id="16d1f-275">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-275">reason</span></span>           | <span data-ttu-id="16d1f-276">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-276">String</span></span>                                                   | <span data-ttu-id="16d1f-277">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="16d1f-277">depends on role Settings</span></span> |   |
| <span data-ttu-id="16d1f-278">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-278">schedule</span></span>         | [<span data-ttu-id="16d1f-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-279">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-280">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-280">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="16d1f-281">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-281">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="16d1f-282">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-282">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="16d1f-283">例 3: ユーザーが割り当てられた役割を非アクティブにする</span><span class="sxs-lookup"><span data-stu-id="16d1f-283">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="16d1f-284">この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="16d1f-285">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-285">Property</span></span>         | <span data-ttu-id="16d1f-286">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-286">Type</span></span>                                                     | <span data-ttu-id="16d1f-287">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-287">Required</span></span> | <span data-ttu-id="16d1f-288">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-288">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="16d1f-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-289">resourceId</span></span>       | <span data-ttu-id="16d1f-290">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-290">String</span></span>                                                   | <span data-ttu-id="16d1f-291">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-291">Yes</span></span>      | <span data-ttu-id="16d1f-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-292">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-293">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-294">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-294">String</span></span>                                                   | <span data-ttu-id="16d1f-295">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-295">Yes</span></span>      | <span data-ttu-id="16d1f-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-296">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-297">subjectId</span></span>        | <span data-ttu-id="16d1f-298">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-298">String</span></span>                                                   | <span data-ttu-id="16d1f-299">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-299">Yes</span></span>      | <span data-ttu-id="16d1f-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-300">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-301">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-301">assignmentState</span></span>  | <span data-ttu-id="16d1f-302">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-302">String</span></span>                                                   | <span data-ttu-id="16d1f-303">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-303">Yes</span></span>      | <span data-ttu-id="16d1f-304">Active</span><span class="sxs-lookup"><span data-stu-id="16d1f-304">Active</span></span> |
| <span data-ttu-id="16d1f-305">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-305">type</span></span>             | <span data-ttu-id="16d1f-306">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-306">String</span></span>                                                   | <span data-ttu-id="16d1f-307">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-307">Yes</span></span>      | <span data-ttu-id="16d1f-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="16d1f-308">UserRemove</span></span> |
| <span data-ttu-id="16d1f-309">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-309">reason</span></span>           | <span data-ttu-id="16d1f-310">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-310">String</span></span>                                                   | <span data-ttu-id="16d1f-311">いいえ</span><span class="sxs-lookup"><span data-stu-id="16d1f-311">No</span></span>       |   |
| <span data-ttu-id="16d1f-312">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-312">schedule</span></span>         | [<span data-ttu-id="16d1f-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-313">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-314">いいえ</span><span class="sxs-lookup"><span data-stu-id="16d1f-314">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="16d1f-315">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-315">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="16d1f-316">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-316">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="16d1f-317">例 4: 管理者が役割からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="16d1f-317">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="16d1f-318">この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-318">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="16d1f-319">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1f-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="16d1f-320">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-320">Property</span></span>         | <span data-ttu-id="16d1f-321">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-321">Type</span></span>                                                     | <span data-ttu-id="16d1f-322">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-322">Required</span></span> | <span data-ttu-id="16d1f-323">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-323">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="16d1f-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-324">resourceId</span></span>       | <span data-ttu-id="16d1f-325">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-325">String</span></span>                                                   | <span data-ttu-id="16d1f-326">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-326">Yes</span></span>      | <span data-ttu-id="16d1f-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-327">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-328">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-329">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-329">String</span></span>                                                   | <span data-ttu-id="16d1f-330">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-330">Yes</span></span>      | <span data-ttu-id="16d1f-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-331">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-332">subjectId</span></span>        | <span data-ttu-id="16d1f-333">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-333">String</span></span>                                                   | <span data-ttu-id="16d1f-334">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-334">Yes</span></span>      | <span data-ttu-id="16d1f-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-335">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-336">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-336">assignmentState</span></span>  | <span data-ttu-id="16d1f-337">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-337">String</span></span>                                                   | <span data-ttu-id="16d1f-338">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-338">Yes</span></span>      | <span data-ttu-id="16d1f-339">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="16d1f-339">Eligible / Active</span></span> |
| <span data-ttu-id="16d1f-340">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-340">type</span></span>             | <span data-ttu-id="16d1f-341">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-341">String</span></span>                                                   | <span data-ttu-id="16d1f-342">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-342">Yes</span></span>      | <span data-ttu-id="16d1f-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="16d1f-343">AdminRemove</span></span> |
| <span data-ttu-id="16d1f-344">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-344">reason</span></span>           | <span data-ttu-id="16d1f-345">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-345">String</span></span>                                                   | <span data-ttu-id="16d1f-346">いいえ</span><span class="sxs-lookup"><span data-stu-id="16d1f-346">No</span></span>       |   |
| <span data-ttu-id="16d1f-347">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-347">schedule</span></span>         | [<span data-ttu-id="16d1f-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-348">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-349">いいえ</span><span class="sxs-lookup"><span data-stu-id="16d1f-349">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="16d1f-350">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-350">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="16d1f-351">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-351">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="16d1f-352">例 5: 管理者の更新の役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="16d1f-352">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="16d1f-353">この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="16d1f-354">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1f-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="16d1f-355">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-355">Property</span></span>         | <span data-ttu-id="16d1f-356">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-356">Type</span></span>                                                     | <span data-ttu-id="16d1f-357">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-357">Required</span></span>                | <span data-ttu-id="16d1f-358">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-358">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="16d1f-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-359">resourceId</span></span>       | <span data-ttu-id="16d1f-360">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-360">String</span></span>                                                   | <span data-ttu-id="16d1f-361">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-361">Yes</span></span>                     | <span data-ttu-id="16d1f-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-362">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-363">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-364">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-364">String</span></span>                                                   | <span data-ttu-id="16d1f-365">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-365">Yes</span></span>                     | <span data-ttu-id="16d1f-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-366">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-367">subjectId</span></span>        | <span data-ttu-id="16d1f-368">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-368">String</span></span>                                                   | <span data-ttu-id="16d1f-369">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-369">Yes</span></span>                     | <span data-ttu-id="16d1f-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-370">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-371">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-371">assignmentState</span></span>  | <span data-ttu-id="16d1f-372">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-372">String</span></span>                                                   | <span data-ttu-id="16d1f-373">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-373">Yes</span></span>                     | <span data-ttu-id="16d1f-374">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="16d1f-374">Eligible / Active</span></span> |
| <span data-ttu-id="16d1f-375">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-375">type</span></span>             | <span data-ttu-id="16d1f-376">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-376">String</span></span>                                                   | <span data-ttu-id="16d1f-377">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-377">Yes</span></span>                     | <span data-ttu-id="16d1f-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="16d1f-378">AdminUpdate</span></span> |
| <span data-ttu-id="16d1f-379">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-379">reason</span></span>           | <span data-ttu-id="16d1f-380">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-380">String</span></span>                                                   | <span data-ttu-id="16d1f-381">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="16d1f-381">depends on roleSettings</span></span> |   |
| <span data-ttu-id="16d1f-382">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-382">schedule</span></span>         | [<span data-ttu-id="16d1f-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-383">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-384">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-384">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="16d1f-385">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-385">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="16d1f-386">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-386">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="16d1f-387">例 6: 管理者が期限切れの役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="16d1f-387">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="16d1f-388">この例では、user ANUCUSER の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。</span><span class="sxs-lookup"><span data-stu-id="16d1f-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="16d1f-389">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16d1f-389">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="16d1f-390">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d1f-390">Property</span></span>         | <span data-ttu-id="16d1f-391">型</span><span class="sxs-lookup"><span data-stu-id="16d1f-391">Type</span></span>                                                     | <span data-ttu-id="16d1f-392">必須</span><span class="sxs-lookup"><span data-stu-id="16d1f-392">Required</span></span>                | <span data-ttu-id="16d1f-393">値</span><span class="sxs-lookup"><span data-stu-id="16d1f-393">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="16d1f-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="16d1f-394">resourceId</span></span>       | <span data-ttu-id="16d1f-395">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-395">String</span></span>                                                   | <span data-ttu-id="16d1f-396">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-396">Yes</span></span>                     | <span data-ttu-id="16d1f-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-397">\<resourceId\></span></span> |
| <span data-ttu-id="16d1f-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="16d1f-398">roleDefinitionId</span></span> | <span data-ttu-id="16d1f-399">文字列</span><span class="sxs-lookup"><span data-stu-id="16d1f-399">String</span></span>                                                   | <span data-ttu-id="16d1f-400">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-400">Yes</span></span>                     | <span data-ttu-id="16d1f-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-401">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="16d1f-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="16d1f-402">subjectId</span></span>        | <span data-ttu-id="16d1f-403">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-403">String</span></span>                                                   | <span data-ttu-id="16d1f-404">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-404">Yes</span></span>                     | <span data-ttu-id="16d1f-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="16d1f-405">\<subjectId\></span></span> |
| <span data-ttu-id="16d1f-406">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="16d1f-406">assignmentState</span></span>  | <span data-ttu-id="16d1f-407">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-407">String</span></span>                                                   | <span data-ttu-id="16d1f-408">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-408">Yes</span></span>                     | <span data-ttu-id="16d1f-409">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="16d1f-409">Eligible / Active</span></span> |
| <span data-ttu-id="16d1f-410">type</span><span class="sxs-lookup"><span data-stu-id="16d1f-410">type</span></span>             | <span data-ttu-id="16d1f-411">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-411">String</span></span>                                                   | <span data-ttu-id="16d1f-412">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-412">Yes</span></span>                     | <span data-ttu-id="16d1f-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="16d1f-413">AdminExtend</span></span> |
| <span data-ttu-id="16d1f-414">したがっ</span><span class="sxs-lookup"><span data-stu-id="16d1f-414">reason</span></span>           | <span data-ttu-id="16d1f-415">String</span><span class="sxs-lookup"><span data-stu-id="16d1f-415">String</span></span>                                                   | <span data-ttu-id="16d1f-416">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="16d1f-416">depends on roleSettings</span></span> |   |
| <span data-ttu-id="16d1f-417">schedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-417">schedule</span></span>         | [<span data-ttu-id="16d1f-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="16d1f-418">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="16d1f-419">はい</span><span class="sxs-lookup"><span data-stu-id="16d1f-419">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="16d1f-420">要求</span><span class="sxs-lookup"><span data-stu-id="16d1f-420">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="16d1f-421">応答</span><span class="sxs-lookup"><span data-stu-id="16d1f-421">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
