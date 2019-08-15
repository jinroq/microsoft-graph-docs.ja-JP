---
title: GovernanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: a49bd528ffe97e33402ab8aef51f86a07b33e5fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420322"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="a9934-104">GovernanceRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="a9934-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9934-105">役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="a9934-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="a9934-106">次の表に、操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="a9934-106">The following table lists the operations.</span></span>

| <span data-ttu-id="a9934-107">Operation</span><span class="sxs-lookup"><span data-stu-id="a9934-107">Operation</span></span>                                   | <span data-ttu-id="a9934-108">型</span><span class="sxs-lookup"><span data-stu-id="a9934-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="a9934-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="a9934-109">Assign a role assignment</span></span>                    | <span data-ttu-id="a9934-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a9934-110">AdminAdd</span></span>    |
| <span data-ttu-id="a9934-111">適格な役割の割り当てをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="a9934-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="a9934-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a9934-112">UserAdd</span></span>     |
| <span data-ttu-id="a9934-113">アクティブ化された役割の割り当てを無効にする</span><span class="sxs-lookup"><span data-stu-id="a9934-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="a9934-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a9934-114">UserRemove</span></span>  |
| <span data-ttu-id="a9934-115">役割の割り当てを削除する</span><span class="sxs-lookup"><span data-stu-id="a9934-115">Remove a role assignment</span></span>                    | <span data-ttu-id="a9934-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a9934-116">AdminRemove</span></span> |
| <span data-ttu-id="a9934-117">役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="a9934-117">Update a role assignment</span></span>                    | <span data-ttu-id="a9934-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a9934-118">AdminUpdate</span></span> |
| <span data-ttu-id="a9934-119">自分の役割の割り当てを拡張するための要求</span><span class="sxs-lookup"><span data-stu-id="a9934-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="a9934-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="a9934-120">UserExtend</span></span>  |
| <span data-ttu-id="a9934-121">役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="a9934-121">Extend a role assignment</span></span>                    | <span data-ttu-id="a9934-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a9934-122">AdminExtend</span></span> |
| <span data-ttu-id="a9934-123">期限切れの役割の割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="a9934-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="a9934-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="a9934-124">UserRenew</span></span>   |
| <span data-ttu-id="a9934-125">期限切れの役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="a9934-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="a9934-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="a9934-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="a9934-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9934-127">Permissions</span></span>

<span data-ttu-id="a9934-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9934-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9934-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9934-130">Permission type</span></span>                        | <span data-ttu-id="a9934-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9934-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="a9934-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9934-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9934-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="a9934-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a9934-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9934-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9934-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9934-135">Not supported.</span></span>                            |
| <span data-ttu-id="a9934-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9934-136">Application</span></span>                            | <span data-ttu-id="a9934-137">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9934-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9934-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9934-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a9934-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9934-139">Request headers</span></span>

| <span data-ttu-id="a9934-140">名前</span><span class="sxs-lookup"><span data-stu-id="a9934-140">Name</span></span>          | <span data-ttu-id="a9934-141">説明</span><span class="sxs-lookup"><span data-stu-id="a9934-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="a9934-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9934-142">Authorization</span></span> | <span data-ttu-id="a9934-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a9934-143">Bearer {code}</span></span>    |
| <span data-ttu-id="a9934-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="a9934-144">Content-type</span></span>  | <span data-ttu-id="a9934-145">application/json</span><span class="sxs-lookup"><span data-stu-id="a9934-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9934-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9934-146">Request body</span></span>

<span data-ttu-id="a9934-147">要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9934-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="a9934-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-148">Property</span></span>         | <span data-ttu-id="a9934-149">型</span><span class="sxs-lookup"><span data-stu-id="a9934-149">Type</span></span>                                                     | <span data-ttu-id="a9934-150">説明</span><span class="sxs-lookup"><span data-stu-id="a9934-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="a9934-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-151">resourceId</span></span>       | <span data-ttu-id="a9934-152">String</span><span class="sxs-lookup"><span data-stu-id="a9934-152">String</span></span>                                                   | <span data-ttu-id="a9934-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="a9934-153">The ID of the resource.</span></span> <span data-ttu-id="a9934-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="a9934-154">Required.</span></span> |
| <span data-ttu-id="a9934-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-155">roleDefinitionId</span></span> | <span data-ttu-id="a9934-156">String</span><span class="sxs-lookup"><span data-stu-id="a9934-156">String</span></span>                                                   | <span data-ttu-id="a9934-157">ロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="a9934-157">The ID of the role definition.</span></span> <span data-ttu-id="a9934-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="a9934-158">Required.</span></span> |
| <span data-ttu-id="a9934-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-159">subjectId</span></span>        | <span data-ttu-id="a9934-160">String</span><span class="sxs-lookup"><span data-stu-id="a9934-160">String</span></span>                                                   | <span data-ttu-id="a9934-161">件名の ID。</span><span class="sxs-lookup"><span data-stu-id="a9934-161">The ID of the subject.</span></span> <span data-ttu-id="a9934-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="a9934-162">Required.</span></span> |
| <span data-ttu-id="a9934-163">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-163">assignmentState</span></span>  | <span data-ttu-id="a9934-164">String</span><span class="sxs-lookup"><span data-stu-id="a9934-164">String</span></span>                                                   | <span data-ttu-id="a9934-165">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9934-165">The state of assignment.</span></span> <span data-ttu-id="a9934-166">値には、 `Eligible`および`Active`を指定できます。</span><span class="sxs-lookup"><span data-stu-id="a9934-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="a9934-167">必須。</span><span class="sxs-lookup"><span data-stu-id="a9934-167">Required.</span></span> |
| <span data-ttu-id="a9934-168">type</span><span class="sxs-lookup"><span data-stu-id="a9934-168">type</span></span>             | <span data-ttu-id="a9934-169">String</span><span class="sxs-lookup"><span data-stu-id="a9934-169">String</span></span>                                                   | <span data-ttu-id="a9934-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="a9934-170">The request type.</span></span> <span data-ttu-id="a9934-171">値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9934-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="a9934-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="a9934-172">Required.</span></span> |
| <span data-ttu-id="a9934-173">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-173">reason</span></span>           | <span data-ttu-id="a9934-174">String</span><span class="sxs-lookup"><span data-stu-id="a9934-174">String</span></span>                                                   | <span data-ttu-id="a9934-175">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9934-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="a9934-176">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-176">schedule</span></span>         | [<span data-ttu-id="a9934-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-178">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="a9934-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="a9934-179">、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate`</span><span class="sxs-lookup"><span data-stu-id="a9934-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9934-180">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-180">Response</span></span>

<span data-ttu-id="a9934-181">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9934-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a9934-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a9934-182">Error codes</span></span>

<span data-ttu-id="a9934-183">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="a9934-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="a9934-184">また、次の表に示されているエラーコードも返します。</span><span class="sxs-lookup"><span data-stu-id="a9934-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="a9934-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a9934-185">Error code</span></span>     | <span data-ttu-id="a9934-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="a9934-186">Error message</span></span>                               | <span data-ttu-id="a9934-187">詳細</span><span class="sxs-lookup"><span data-stu-id="a9934-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="a9934-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-188">400 BadRequest</span></span> | <span data-ttu-id="a9934-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="a9934-189">RoleNotFound</span></span>                                | <span data-ttu-id="a9934-190">要求`roleDefinitionId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="a9934-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a9934-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-191">400 BadRequest</span></span> | <span data-ttu-id="a9934-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="a9934-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="a9934-193">要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。</span><span class="sxs-lookup"><span data-stu-id="a9934-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="a9934-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-194">400 BadRequest</span></span> | <span data-ttu-id="a9934-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="a9934-195">SubjectNotFound</span></span>                             | <span data-ttu-id="a9934-196">要求`subjectId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="a9934-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a9934-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-197">400 BadRequest</span></span> | <span data-ttu-id="a9934-198">Pendingrole割り当て要求</span><span class="sxs-lookup"><span data-stu-id="a9934-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="a9934-199">保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="a9934-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="a9934-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-200">400 BadRequest</span></span> | <span data-ttu-id="a9934-201">Role割り当てが存在する</span><span class="sxs-lookup"><span data-stu-id="a9934-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="a9934-202">作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。</span><span class="sxs-lookup"><span data-stu-id="a9934-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="a9934-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-203">400 BadRequest</span></span> | <span data-ttu-id="a9934-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="a9934-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="a9934-205">更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="a9934-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="a9934-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9934-206">400 BadRequest</span></span> | <span data-ttu-id="a9934-207">Role割り当て要求 Policyvalidationfailed</span><span class="sxs-lookup"><span data-stu-id="a9934-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="a9934-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9934-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="a9934-209">例</span><span class="sxs-lookup"><span data-stu-id="a9934-209">Examples</span></span>

<span data-ttu-id="a9934-210">次の例は、この API の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a9934-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="a9934-211">例 1: 管理者がユーザーを役割に割り当てる</span><span class="sxs-lookup"><span data-stu-id="a9934-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="a9934-212">この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a9934-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="a9934-213">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9934-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a9934-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-214">Property</span></span>         | <span data-ttu-id="a9934-215">型</span><span class="sxs-lookup"><span data-stu-id="a9934-215">Type</span></span>                                                     | <span data-ttu-id="a9934-216">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-216">Required</span></span>                 | <span data-ttu-id="a9934-217">値</span><span class="sxs-lookup"><span data-stu-id="a9934-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a9934-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-218">resourceId</span></span>       | <span data-ttu-id="a9934-219">String</span><span class="sxs-lookup"><span data-stu-id="a9934-219">String</span></span>                                                   | <span data-ttu-id="a9934-220">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-220">Yes</span></span>                      | <span data-ttu-id="a9934-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-221">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-222">roleDefinitionId</span></span> | <span data-ttu-id="a9934-223">String</span><span class="sxs-lookup"><span data-stu-id="a9934-223">String</span></span>                                                   | <span data-ttu-id="a9934-224">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-224">Yes</span></span>                      | <span data-ttu-id="a9934-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-226">subjectId</span></span>        | <span data-ttu-id="a9934-227">String</span><span class="sxs-lookup"><span data-stu-id="a9934-227">String</span></span>                                                   | <span data-ttu-id="a9934-228">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-228">Yes</span></span>                      | <span data-ttu-id="a9934-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-229">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-230">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-230">assignmentState</span></span>  | <span data-ttu-id="a9934-231">String</span><span class="sxs-lookup"><span data-stu-id="a9934-231">String</span></span>                                                   | <span data-ttu-id="a9934-232">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-232">Yes</span></span>                      | <span data-ttu-id="a9934-233">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="a9934-233">Eligible / Active</span></span> |
| <span data-ttu-id="a9934-234">type</span><span class="sxs-lookup"><span data-stu-id="a9934-234">type</span></span>             | <span data-ttu-id="a9934-235">String</span><span class="sxs-lookup"><span data-stu-id="a9934-235">String</span></span>                                                   | <span data-ttu-id="a9934-236">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-236">Yes</span></span>                      | <span data-ttu-id="a9934-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a9934-237">AdminAdd</span></span> |
| <span data-ttu-id="a9934-238">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-238">reason</span></span>           | <span data-ttu-id="a9934-239">String</span><span class="sxs-lookup"><span data-stu-id="a9934-239">String</span></span>                                                   | <span data-ttu-id="a9934-240">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="a9934-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="a9934-241">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-241">schedule</span></span>         | [<span data-ttu-id="a9934-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-243">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a9934-244">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a9934-245">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a9934-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9934-246">C#</span><span class="sxs-lookup"><span data-stu-id="a9934-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9934-247">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9934-247">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9934-248">目的-C</span><span class="sxs-lookup"><span data-stu-id="a9934-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a9934-249">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-249">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="a9934-250">例 2: ユーザーが対象となる役割をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="a9934-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="a9934-251">この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="a9934-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="a9934-252">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-252">Property</span></span>         | <span data-ttu-id="a9934-253">型</span><span class="sxs-lookup"><span data-stu-id="a9934-253">Type</span></span>                                                     | <span data-ttu-id="a9934-254">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-254">Required</span></span>                 | <span data-ttu-id="a9934-255">値</span><span class="sxs-lookup"><span data-stu-id="a9934-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a9934-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-256">resourceId</span></span>       | <span data-ttu-id="a9934-257">String</span><span class="sxs-lookup"><span data-stu-id="a9934-257">String</span></span>                                                   | <span data-ttu-id="a9934-258">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-258">Yes</span></span>                      | <span data-ttu-id="a9934-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-259">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-260">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-260">roleDefinitionId</span></span> | <span data-ttu-id="a9934-261">String</span><span class="sxs-lookup"><span data-stu-id="a9934-261">String</span></span>                                                   | <span data-ttu-id="a9934-262">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-262">Yes</span></span>                      | <span data-ttu-id="a9934-263">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-264">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-264">subjectId</span></span>        | <span data-ttu-id="a9934-265">String</span><span class="sxs-lookup"><span data-stu-id="a9934-265">String</span></span>                                                   | <span data-ttu-id="a9934-266">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-266">Yes</span></span>                      | <span data-ttu-id="a9934-267">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-267">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-268">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-268">assignmentState</span></span>  | <span data-ttu-id="a9934-269">String</span><span class="sxs-lookup"><span data-stu-id="a9934-269">String</span></span>                                                   | <span data-ttu-id="a9934-270">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-270">Yes</span></span>                      | <span data-ttu-id="a9934-271">Active</span><span class="sxs-lookup"><span data-stu-id="a9934-271">Active</span></span> |
| <span data-ttu-id="a9934-272">type</span><span class="sxs-lookup"><span data-stu-id="a9934-272">type</span></span>             | <span data-ttu-id="a9934-273">String</span><span class="sxs-lookup"><span data-stu-id="a9934-273">String</span></span>                                                   | <span data-ttu-id="a9934-274">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-274">Yes</span></span>                      | <span data-ttu-id="a9934-275">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a9934-275">UserAdd</span></span> |
| <span data-ttu-id="a9934-276">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-276">reason</span></span>           | <span data-ttu-id="a9934-277">String</span><span class="sxs-lookup"><span data-stu-id="a9934-277">String</span></span>                                                   | <span data-ttu-id="a9934-278">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="a9934-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="a9934-279">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-279">schedule</span></span>         | [<span data-ttu-id="a9934-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-281">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a9934-282">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a9934-283">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="a9934-284">例 3: ユーザーが割り当てられた役割を非アクティブにする</span><span class="sxs-lookup"><span data-stu-id="a9934-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="a9934-285">この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="a9934-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="a9934-286">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-286">Property</span></span>         | <span data-ttu-id="a9934-287">型</span><span class="sxs-lookup"><span data-stu-id="a9934-287">Type</span></span>                                                     | <span data-ttu-id="a9934-288">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-288">Required</span></span> | <span data-ttu-id="a9934-289">値</span><span class="sxs-lookup"><span data-stu-id="a9934-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a9934-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-290">resourceId</span></span>       | <span data-ttu-id="a9934-291">String</span><span class="sxs-lookup"><span data-stu-id="a9934-291">String</span></span>                                                   | <span data-ttu-id="a9934-292">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-292">Yes</span></span>      | <span data-ttu-id="a9934-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-293">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-294">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-294">roleDefinitionId</span></span> | <span data-ttu-id="a9934-295">String</span><span class="sxs-lookup"><span data-stu-id="a9934-295">String</span></span>                                                   | <span data-ttu-id="a9934-296">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-296">Yes</span></span>      | <span data-ttu-id="a9934-297">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-298">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-298">subjectId</span></span>        | <span data-ttu-id="a9934-299">String</span><span class="sxs-lookup"><span data-stu-id="a9934-299">String</span></span>                                                   | <span data-ttu-id="a9934-300">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-300">Yes</span></span>      | <span data-ttu-id="a9934-301">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-301">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-302">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-302">assignmentState</span></span>  | <span data-ttu-id="a9934-303">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-303">String</span></span>                                                   | <span data-ttu-id="a9934-304">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-304">Yes</span></span>      | <span data-ttu-id="a9934-305">Active</span><span class="sxs-lookup"><span data-stu-id="a9934-305">Active</span></span> |
| <span data-ttu-id="a9934-306">type</span><span class="sxs-lookup"><span data-stu-id="a9934-306">type</span></span>             | <span data-ttu-id="a9934-307">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-307">String</span></span>                                                   | <span data-ttu-id="a9934-308">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-308">Yes</span></span>      | <span data-ttu-id="a9934-309">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a9934-309">UserRemove</span></span> |
| <span data-ttu-id="a9934-310">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-310">reason</span></span>           | <span data-ttu-id="a9934-311">String</span><span class="sxs-lookup"><span data-stu-id="a9934-311">String</span></span>                                                   | <span data-ttu-id="a9934-312">いいえ</span><span class="sxs-lookup"><span data-stu-id="a9934-312">No</span></span>       |   |
| <span data-ttu-id="a9934-313">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-313">schedule</span></span>         | [<span data-ttu-id="a9934-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-315">いいえ</span><span class="sxs-lookup"><span data-stu-id="a9934-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a9934-316">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a9934-317">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="a9934-318">例 4: 管理者が役割からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="a9934-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="a9934-319">この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="a9934-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="a9934-320">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9934-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a9934-321">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-321">Property</span></span>         | <span data-ttu-id="a9934-322">型</span><span class="sxs-lookup"><span data-stu-id="a9934-322">Type</span></span>                                                     | <span data-ttu-id="a9934-323">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-323">Required</span></span> | <span data-ttu-id="a9934-324">値</span><span class="sxs-lookup"><span data-stu-id="a9934-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a9934-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-325">resourceId</span></span>       | <span data-ttu-id="a9934-326">String</span><span class="sxs-lookup"><span data-stu-id="a9934-326">String</span></span>                                                   | <span data-ttu-id="a9934-327">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-327">Yes</span></span>      | <span data-ttu-id="a9934-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-328">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-329">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-329">roleDefinitionId</span></span> | <span data-ttu-id="a9934-330">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-330">String</span></span>                                                   | <span data-ttu-id="a9934-331">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-331">Yes</span></span>      | <span data-ttu-id="a9934-332">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-333">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-333">subjectId</span></span>        | <span data-ttu-id="a9934-334">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-334">String</span></span>                                                   | <span data-ttu-id="a9934-335">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-335">Yes</span></span>      | <span data-ttu-id="a9934-336">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-336">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-337">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-337">assignmentState</span></span>  | <span data-ttu-id="a9934-338">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-338">String</span></span>                                                   | <span data-ttu-id="a9934-339">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-339">Yes</span></span>      | <span data-ttu-id="a9934-340">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="a9934-340">Eligible / Active</span></span> |
| <span data-ttu-id="a9934-341">type</span><span class="sxs-lookup"><span data-stu-id="a9934-341">type</span></span>             | <span data-ttu-id="a9934-342">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-342">String</span></span>                                                   | <span data-ttu-id="a9934-343">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-343">Yes</span></span>      | <span data-ttu-id="a9934-344">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a9934-344">AdminRemove</span></span> |
| <span data-ttu-id="a9934-345">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-345">reason</span></span>           | <span data-ttu-id="a9934-346">String</span><span class="sxs-lookup"><span data-stu-id="a9934-346">String</span></span>                                                   | <span data-ttu-id="a9934-347">いいえ</span><span class="sxs-lookup"><span data-stu-id="a9934-347">No</span></span>       |   |
| <span data-ttu-id="a9934-348">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-348">schedule</span></span>         | [<span data-ttu-id="a9934-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-350">いいえ</span><span class="sxs-lookup"><span data-stu-id="a9934-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a9934-351">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a9934-352">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="a9934-353">例 5: 管理者の更新の役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="a9934-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="a9934-354">この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。</span><span class="sxs-lookup"><span data-stu-id="a9934-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="a9934-355">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9934-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a9934-356">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-356">Property</span></span>         | <span data-ttu-id="a9934-357">型</span><span class="sxs-lookup"><span data-stu-id="a9934-357">Type</span></span>                                                     | <span data-ttu-id="a9934-358">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-358">Required</span></span>                | <span data-ttu-id="a9934-359">値</span><span class="sxs-lookup"><span data-stu-id="a9934-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a9934-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-360">resourceId</span></span>       | <span data-ttu-id="a9934-361">String</span><span class="sxs-lookup"><span data-stu-id="a9934-361">String</span></span>                                                   | <span data-ttu-id="a9934-362">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-362">Yes</span></span>                     | <span data-ttu-id="a9934-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-363">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-364">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-364">roleDefinitionId</span></span> | <span data-ttu-id="a9934-365">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-365">String</span></span>                                                   | <span data-ttu-id="a9934-366">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-366">Yes</span></span>                     | <span data-ttu-id="a9934-367">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-368">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-368">subjectId</span></span>        | <span data-ttu-id="a9934-369">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-369">String</span></span>                                                   | <span data-ttu-id="a9934-370">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-370">Yes</span></span>                     | <span data-ttu-id="a9934-371">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-371">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-372">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-372">assignmentState</span></span>  | <span data-ttu-id="a9934-373">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-373">String</span></span>                                                   | <span data-ttu-id="a9934-374">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-374">Yes</span></span>                     | <span data-ttu-id="a9934-375">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="a9934-375">Eligible / Active</span></span> |
| <span data-ttu-id="a9934-376">type</span><span class="sxs-lookup"><span data-stu-id="a9934-376">type</span></span>             | <span data-ttu-id="a9934-377">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-377">String</span></span>                                                   | <span data-ttu-id="a9934-378">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-378">Yes</span></span>                     | <span data-ttu-id="a9934-379">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a9934-379">AdminUpdate</span></span> |
| <span data-ttu-id="a9934-380">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-380">reason</span></span>           | <span data-ttu-id="a9934-381">String</span><span class="sxs-lookup"><span data-stu-id="a9934-381">String</span></span>                                                   | <span data-ttu-id="a9934-382">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="a9934-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a9934-383">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-383">schedule</span></span>         | [<span data-ttu-id="a9934-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-385">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a9934-386">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a9934-387">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="a9934-388">例 6: 管理者が期限切れの役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="a9934-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="a9934-389">この例では、user ANUCUSER の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。</span><span class="sxs-lookup"><span data-stu-id="a9934-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="a9934-390">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9934-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a9934-391">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9934-391">Property</span></span>         | <span data-ttu-id="a9934-392">型</span><span class="sxs-lookup"><span data-stu-id="a9934-392">Type</span></span>                                                     | <span data-ttu-id="a9934-393">必須</span><span class="sxs-lookup"><span data-stu-id="a9934-393">Required</span></span>                | <span data-ttu-id="a9934-394">値</span><span class="sxs-lookup"><span data-stu-id="a9934-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a9934-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9934-395">resourceId</span></span>       | <span data-ttu-id="a9934-396">String</span><span class="sxs-lookup"><span data-stu-id="a9934-396">String</span></span>                                                   | <span data-ttu-id="a9934-397">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-397">Yes</span></span>                     | <span data-ttu-id="a9934-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a9934-398">\<resourceId\></span></span> |
| <span data-ttu-id="a9934-399">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a9934-399">roleDefinitionId</span></span> | <span data-ttu-id="a9934-400">文字列</span><span class="sxs-lookup"><span data-stu-id="a9934-400">String</span></span>                                                   | <span data-ttu-id="a9934-401">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-401">Yes</span></span>                     | <span data-ttu-id="a9934-402">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a9934-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a9934-403">subjectId</span><span class="sxs-lookup"><span data-stu-id="a9934-403">subjectId</span></span>        | <span data-ttu-id="a9934-404">String</span><span class="sxs-lookup"><span data-stu-id="a9934-404">String</span></span>                                                   | <span data-ttu-id="a9934-405">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-405">Yes</span></span>                     | <span data-ttu-id="a9934-406">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a9934-406">\<subjectId\></span></span> |
| <span data-ttu-id="a9934-407">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="a9934-407">assignmentState</span></span>  | <span data-ttu-id="a9934-408">String</span><span class="sxs-lookup"><span data-stu-id="a9934-408">String</span></span>                                                   | <span data-ttu-id="a9934-409">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-409">Yes</span></span>                     | <span data-ttu-id="a9934-410">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="a9934-410">Eligible / Active</span></span> |
| <span data-ttu-id="a9934-411">type</span><span class="sxs-lookup"><span data-stu-id="a9934-411">type</span></span>             | <span data-ttu-id="a9934-412">String</span><span class="sxs-lookup"><span data-stu-id="a9934-412">String</span></span>                                                   | <span data-ttu-id="a9934-413">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-413">Yes</span></span>                     | <span data-ttu-id="a9934-414">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a9934-414">AdminExtend</span></span> |
| <span data-ttu-id="a9934-415">したがっ</span><span class="sxs-lookup"><span data-stu-id="a9934-415">reason</span></span>           | <span data-ttu-id="a9934-416">String</span><span class="sxs-lookup"><span data-stu-id="a9934-416">String</span></span>                                                   | <span data-ttu-id="a9934-417">roleSettings に依存</span><span class="sxs-lookup"><span data-stu-id="a9934-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a9934-418">schedule</span><span class="sxs-lookup"><span data-stu-id="a9934-418">schedule</span></span>         | [<span data-ttu-id="a9934-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9934-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a9934-420">はい</span><span class="sxs-lookup"><span data-stu-id="a9934-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a9934-421">要求</span><span class="sxs-lookup"><span data-stu-id="a9934-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a9934-422">応答</span><span class="sxs-lookup"><span data-stu-id="a9934-422">Response</span></span>

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
