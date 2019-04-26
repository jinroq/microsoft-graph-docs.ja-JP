---
title: governanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
ms.openlocfilehash: b9b5f701f3f8ad283f589d07b250ce8ea63aa479
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329628"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="b2639-104">governanceRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="b2639-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2639-105">役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="b2639-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="b2639-106">次の表に、操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="b2639-106">The following table lists the operations.</span></span>

| <span data-ttu-id="b2639-107">操作</span><span class="sxs-lookup"><span data-stu-id="b2639-107">Operation</span></span>                                   | <span data-ttu-id="b2639-108">型</span><span class="sxs-lookup"><span data-stu-id="b2639-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="b2639-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b2639-109">Assign a role assignment</span></span>                    | <span data-ttu-id="b2639-110">adminadd</span><span class="sxs-lookup"><span data-stu-id="b2639-110">AdminAdd</span></span>    |
| <span data-ttu-id="b2639-111">適格な役割の割り当てをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="b2639-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="b2639-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="b2639-112">UserAdd</span></span>     |
| <span data-ttu-id="b2639-113">アクティブ化された役割の割り当てを無効にする</span><span class="sxs-lookup"><span data-stu-id="b2639-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="b2639-114">userremove</span><span class="sxs-lookup"><span data-stu-id="b2639-114">UserRemove</span></span>  |
| <span data-ttu-id="b2639-115">役割の割り当てを削除する</span><span class="sxs-lookup"><span data-stu-id="b2639-115">Remove a role assignment</span></span>                    | <span data-ttu-id="b2639-116">adminremove</span><span class="sxs-lookup"><span data-stu-id="b2639-116">AdminRemove</span></span> |
| <span data-ttu-id="b2639-117">役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="b2639-117">Update a role assignment</span></span>                    | <span data-ttu-id="b2639-118">adminupdate</span><span class="sxs-lookup"><span data-stu-id="b2639-118">AdminUpdate</span></span> |
| <span data-ttu-id="b2639-119">自分の役割の割り当てを拡張するための要求</span><span class="sxs-lookup"><span data-stu-id="b2639-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="b2639-120">userextend</span><span class="sxs-lookup"><span data-stu-id="b2639-120">UserExtend</span></span>  |
| <span data-ttu-id="b2639-121">役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="b2639-121">Extend a role assignment</span></span>                    | <span data-ttu-id="b2639-122">adminextend</span><span class="sxs-lookup"><span data-stu-id="b2639-122">AdminExtend</span></span> |
| <span data-ttu-id="b2639-123">期限切れの役割の割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="b2639-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="b2639-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="b2639-124">UserRenew</span></span>   |
| <span data-ttu-id="b2639-125">期限切れの役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="b2639-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="b2639-126">adminrenew</span><span class="sxs-lookup"><span data-stu-id="b2639-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="b2639-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2639-127">Permissions</span></span>

<span data-ttu-id="b2639-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2639-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2639-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2639-130">Permission type</span></span>                        | <span data-ttu-id="b2639-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2639-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="b2639-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2639-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2639-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="b2639-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b2639-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2639-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2639-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2639-135">Not supported.</span></span>                            |
| <span data-ttu-id="b2639-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2639-136">Application</span></span>                            | <span data-ttu-id="b2639-137">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="b2639-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2639-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2639-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="b2639-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2639-139">Request headers</span></span>

| <span data-ttu-id="b2639-140">名前</span><span class="sxs-lookup"><span data-stu-id="b2639-140">Name</span></span>          | <span data-ttu-id="b2639-141">説明</span><span class="sxs-lookup"><span data-stu-id="b2639-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="b2639-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2639-142">Authorization</span></span> | <span data-ttu-id="b2639-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b2639-143">Bearer {code}</span></span>    |
| <span data-ttu-id="b2639-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="b2639-144">Content-type</span></span>  | <span data-ttu-id="b2639-145">application/json</span><span class="sxs-lookup"><span data-stu-id="b2639-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2639-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2639-146">Request body</span></span>

<span data-ttu-id="b2639-147">要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2639-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="b2639-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-148">Property</span></span>         | <span data-ttu-id="b2639-149">型</span><span class="sxs-lookup"><span data-stu-id="b2639-149">Type</span></span>                                                     | <span data-ttu-id="b2639-150">説明</span><span class="sxs-lookup"><span data-stu-id="b2639-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="b2639-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-151">resourceId</span></span>       | <span data-ttu-id="b2639-152">String</span><span class="sxs-lookup"><span data-stu-id="b2639-152">String</span></span>                                                   | <span data-ttu-id="b2639-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="b2639-153">The ID of the resource.</span></span> <span data-ttu-id="b2639-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="b2639-154">Required.</span></span> |
| <span data-ttu-id="b2639-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-155">roleDefinitionId</span></span> | <span data-ttu-id="b2639-156">String</span><span class="sxs-lookup"><span data-stu-id="b2639-156">String</span></span>                                                   | <span data-ttu-id="b2639-157">ロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="b2639-157">The ID of the role definition.</span></span> <span data-ttu-id="b2639-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="b2639-158">Required.</span></span> |
| <span data-ttu-id="b2639-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-159">subjectId</span></span>        | <span data-ttu-id="b2639-160">String</span><span class="sxs-lookup"><span data-stu-id="b2639-160">String</span></span>                                                   | <span data-ttu-id="b2639-161">件名の ID。</span><span class="sxs-lookup"><span data-stu-id="b2639-161">The ID of the subject.</span></span> <span data-ttu-id="b2639-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="b2639-162">Required.</span></span> |
| <span data-ttu-id="b2639-163">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-163">assignmentState</span></span>  | <span data-ttu-id="b2639-164">String</span><span class="sxs-lookup"><span data-stu-id="b2639-164">String</span></span>                                                   | <span data-ttu-id="b2639-165">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2639-165">The state of assignment.</span></span> <span data-ttu-id="b2639-166">値には、 `Eligible`および`Active`を指定できます。</span><span class="sxs-lookup"><span data-stu-id="b2639-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="b2639-167">必須。</span><span class="sxs-lookup"><span data-stu-id="b2639-167">Required.</span></span> |
| <span data-ttu-id="b2639-168">type</span><span class="sxs-lookup"><span data-stu-id="b2639-168">type</span></span>             | <span data-ttu-id="b2639-169">String</span><span class="sxs-lookup"><span data-stu-id="b2639-169">String</span></span>                                                   | <span data-ttu-id="b2639-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="b2639-170">The request type.</span></span> <span data-ttu-id="b2639-171">値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2639-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="b2639-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="b2639-172">Required.</span></span> |
| <span data-ttu-id="b2639-173">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-173">reason</span></span>           | <span data-ttu-id="b2639-174">String</span><span class="sxs-lookup"><span data-stu-id="b2639-174">String</span></span>                                                   | <span data-ttu-id="b2639-175">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2639-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="b2639-176">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-176">schedule</span></span>         | [<span data-ttu-id="b2639-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-178">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="b2639-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="b2639-179">、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate`</span><span class="sxs-lookup"><span data-stu-id="b2639-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="b2639-180">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-180">Response</span></span>

<span data-ttu-id="b2639-181">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b2639-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="b2639-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="b2639-182">Error codes</span></span>

<span data-ttu-id="b2639-183">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="b2639-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="b2639-184">また、次の表に示されているエラーコードも返します。</span><span class="sxs-lookup"><span data-stu-id="b2639-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="b2639-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="b2639-185">Error code</span></span>     | <span data-ttu-id="b2639-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="b2639-186">Error message</span></span>                               | <span data-ttu-id="b2639-187">詳細</span><span class="sxs-lookup"><span data-stu-id="b2639-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="b2639-188">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-188">400 BadRequest</span></span> | <span data-ttu-id="b2639-189">rolenotfound</span><span class="sxs-lookup"><span data-stu-id="b2639-189">RoleNotFound</span></span>                                | <span data-ttu-id="b2639-190">要求`roleDefinitionId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="b2639-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="b2639-191">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-191">400 BadRequest</span></span> | <span data-ttu-id="b2639-192">resourceislocked</span><span class="sxs-lookup"><span data-stu-id="b2639-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="b2639-193">要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。</span><span class="sxs-lookup"><span data-stu-id="b2639-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="b2639-194">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-194">400 BadRequest</span></span> | <span data-ttu-id="b2639-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="b2639-195">SubjectNotFound</span></span>                             | <span data-ttu-id="b2639-196">要求`subjectId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="b2639-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="b2639-197">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-197">400 BadRequest</span></span> | <span data-ttu-id="b2639-198">pendingrole割り当て要求</span><span class="sxs-lookup"><span data-stu-id="b2639-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="b2639-199">保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="b2639-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="b2639-200">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-200">400 BadRequest</span></span> | <span data-ttu-id="b2639-201">role割り当てが存在する</span><span class="sxs-lookup"><span data-stu-id="b2639-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="b2639-202">作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。</span><span class="sxs-lookup"><span data-stu-id="b2639-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="b2639-203">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-203">400 BadRequest</span></span> | <span data-ttu-id="b2639-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="b2639-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="b2639-205">更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="b2639-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="b2639-206">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="b2639-206">400 BadRequest</span></span> | <span data-ttu-id="b2639-207">role割り当て要求 policyvalidationfailed</span><span class="sxs-lookup"><span data-stu-id="b2639-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="b2639-208">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="b2639-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="b2639-209">例</span><span class="sxs-lookup"><span data-stu-id="b2639-209">Examples</span></span>

<span data-ttu-id="b2639-210">次の例は、この API の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b2639-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="b2639-211">例 1: 管理者がユーザーを役割に割り当てる</span><span class="sxs-lookup"><span data-stu-id="b2639-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="b2639-212">この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b2639-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="b2639-213">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2639-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b2639-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-214">Property</span></span>         | <span data-ttu-id="b2639-215">型</span><span class="sxs-lookup"><span data-stu-id="b2639-215">Type</span></span>                                                     | <span data-ttu-id="b2639-216">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-216">Required</span></span>                 | <span data-ttu-id="b2639-217">値</span><span class="sxs-lookup"><span data-stu-id="b2639-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="b2639-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-218">resourceId</span></span>       | <span data-ttu-id="b2639-219">String</span><span class="sxs-lookup"><span data-stu-id="b2639-219">String</span></span>                                                   | <span data-ttu-id="b2639-220">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-220">Yes</span></span>                      | <span data-ttu-id="b2639-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-221">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-222">roleDefinitionId</span></span> | <span data-ttu-id="b2639-223">String</span><span class="sxs-lookup"><span data-stu-id="b2639-223">String</span></span>                                                   | <span data-ttu-id="b2639-224">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-224">Yes</span></span>                      | <span data-ttu-id="b2639-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-226">subjectId</span></span>        | <span data-ttu-id="b2639-227">String</span><span class="sxs-lookup"><span data-stu-id="b2639-227">String</span></span>                                                   | <span data-ttu-id="b2639-228">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-228">Yes</span></span>                      | <span data-ttu-id="b2639-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-229">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-230">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-230">assignmentState</span></span>  | <span data-ttu-id="b2639-231">String</span><span class="sxs-lookup"><span data-stu-id="b2639-231">String</span></span>                                                   | <span data-ttu-id="b2639-232">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-232">Yes</span></span>                      | <span data-ttu-id="b2639-233">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-233">Eligible / Active</span></span> |
| <span data-ttu-id="b2639-234">type</span><span class="sxs-lookup"><span data-stu-id="b2639-234">type</span></span>             | <span data-ttu-id="b2639-235">String</span><span class="sxs-lookup"><span data-stu-id="b2639-235">String</span></span>                                                   | <span data-ttu-id="b2639-236">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-236">Yes</span></span>                      | <span data-ttu-id="b2639-237">adminadd</span><span class="sxs-lookup"><span data-stu-id="b2639-237">AdminAdd</span></span> |
| <span data-ttu-id="b2639-238">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-238">reason</span></span>           | <span data-ttu-id="b2639-239">String</span><span class="sxs-lookup"><span data-stu-id="b2639-239">String</span></span>                                                   | <span data-ttu-id="b2639-240">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="b2639-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="b2639-241">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-241">schedule</span></span>         | [<span data-ttu-id="b2639-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-243">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="b2639-244">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-245">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="b2639-246">例 2: ユーザーが対象となる役割をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="b2639-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="b2639-247">この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="b2639-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="b2639-248">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-248">Property</span></span>         | <span data-ttu-id="b2639-249">型</span><span class="sxs-lookup"><span data-stu-id="b2639-249">Type</span></span>                                                     | <span data-ttu-id="b2639-250">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-250">Required</span></span>                 | <span data-ttu-id="b2639-251">値</span><span class="sxs-lookup"><span data-stu-id="b2639-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="b2639-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-252">resourceId</span></span>       | <span data-ttu-id="b2639-253">String</span><span class="sxs-lookup"><span data-stu-id="b2639-253">String</span></span>                                                   | <span data-ttu-id="b2639-254">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-254">Yes</span></span>                      | <span data-ttu-id="b2639-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-255">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-256">roleDefinitionId</span></span> | <span data-ttu-id="b2639-257">String</span><span class="sxs-lookup"><span data-stu-id="b2639-257">String</span></span>                                                   | <span data-ttu-id="b2639-258">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-258">Yes</span></span>                      | <span data-ttu-id="b2639-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-260">subjectId</span></span>        | <span data-ttu-id="b2639-261">String</span><span class="sxs-lookup"><span data-stu-id="b2639-261">String</span></span>                                                   | <span data-ttu-id="b2639-262">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-262">Yes</span></span>                      | <span data-ttu-id="b2639-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-263">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-264">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-264">assignmentState</span></span>  | <span data-ttu-id="b2639-265">String</span><span class="sxs-lookup"><span data-stu-id="b2639-265">String</span></span>                                                   | <span data-ttu-id="b2639-266">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-266">Yes</span></span>                      | <span data-ttu-id="b2639-267">アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-267">Active</span></span> |
| <span data-ttu-id="b2639-268">type</span><span class="sxs-lookup"><span data-stu-id="b2639-268">type</span></span>             | <span data-ttu-id="b2639-269">String</span><span class="sxs-lookup"><span data-stu-id="b2639-269">String</span></span>                                                   | <span data-ttu-id="b2639-270">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-270">Yes</span></span>                      | <span data-ttu-id="b2639-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="b2639-271">UserAdd</span></span> |
| <span data-ttu-id="b2639-272">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-272">reason</span></span>           | <span data-ttu-id="b2639-273">String</span><span class="sxs-lookup"><span data-stu-id="b2639-273">String</span></span>                                                   | <span data-ttu-id="b2639-274">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="b2639-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="b2639-275">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-275">schedule</span></span>         | [<span data-ttu-id="b2639-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-277">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="b2639-278">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-279">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="b2639-280">例 3: ユーザーが割り当てられた役割を非アクティブにする</span><span class="sxs-lookup"><span data-stu-id="b2639-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="b2639-281">この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="b2639-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="b2639-282">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-282">Property</span></span>         | <span data-ttu-id="b2639-283">型</span><span class="sxs-lookup"><span data-stu-id="b2639-283">Type</span></span>                                                     | <span data-ttu-id="b2639-284">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-284">Required</span></span> | <span data-ttu-id="b2639-285">値</span><span class="sxs-lookup"><span data-stu-id="b2639-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="b2639-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-286">resourceId</span></span>       | <span data-ttu-id="b2639-287">String</span><span class="sxs-lookup"><span data-stu-id="b2639-287">String</span></span>                                                   | <span data-ttu-id="b2639-288">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-288">Yes</span></span>      | <span data-ttu-id="b2639-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-289">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-290">roleDefinitionId</span></span> | <span data-ttu-id="b2639-291">String</span><span class="sxs-lookup"><span data-stu-id="b2639-291">String</span></span>                                                   | <span data-ttu-id="b2639-292">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-292">Yes</span></span>      | <span data-ttu-id="b2639-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-294">subjectId</span></span>        | <span data-ttu-id="b2639-295">String</span><span class="sxs-lookup"><span data-stu-id="b2639-295">String</span></span>                                                   | <span data-ttu-id="b2639-296">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-296">Yes</span></span>      | <span data-ttu-id="b2639-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-297">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-298">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-298">assignmentState</span></span>  | <span data-ttu-id="b2639-299">String</span><span class="sxs-lookup"><span data-stu-id="b2639-299">String</span></span>                                                   | <span data-ttu-id="b2639-300">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-300">Yes</span></span>      | <span data-ttu-id="b2639-301">アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-301">Active</span></span> |
| <span data-ttu-id="b2639-302">type</span><span class="sxs-lookup"><span data-stu-id="b2639-302">type</span></span>             | <span data-ttu-id="b2639-303">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-303">String</span></span>                                                   | <span data-ttu-id="b2639-304">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-304">Yes</span></span>      | <span data-ttu-id="b2639-305">userremove</span><span class="sxs-lookup"><span data-stu-id="b2639-305">UserRemove</span></span> |
| <span data-ttu-id="b2639-306">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-306">reason</span></span>           | <span data-ttu-id="b2639-307">String</span><span class="sxs-lookup"><span data-stu-id="b2639-307">String</span></span>                                                   | <span data-ttu-id="b2639-308">いいえ</span><span class="sxs-lookup"><span data-stu-id="b2639-308">No</span></span>       |   |
| <span data-ttu-id="b2639-309">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-309">schedule</span></span>         | [<span data-ttu-id="b2639-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-311">いいえ</span><span class="sxs-lookup"><span data-stu-id="b2639-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="b2639-312">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-313">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="b2639-314">例 4: 管理者が役割からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="b2639-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="b2639-315">この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="b2639-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="b2639-316">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2639-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b2639-317">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-317">Property</span></span>         | <span data-ttu-id="b2639-318">型</span><span class="sxs-lookup"><span data-stu-id="b2639-318">Type</span></span>                                                     | <span data-ttu-id="b2639-319">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-319">Required</span></span> | <span data-ttu-id="b2639-320">値</span><span class="sxs-lookup"><span data-stu-id="b2639-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="b2639-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-321">resourceId</span></span>       | <span data-ttu-id="b2639-322">String</span><span class="sxs-lookup"><span data-stu-id="b2639-322">String</span></span>                                                   | <span data-ttu-id="b2639-323">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-323">Yes</span></span>      | <span data-ttu-id="b2639-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-324">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-325">roleDefinitionId</span></span> | <span data-ttu-id="b2639-326">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-326">String</span></span>                                                   | <span data-ttu-id="b2639-327">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-327">Yes</span></span>      | <span data-ttu-id="b2639-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-329">subjectId</span></span>        | <span data-ttu-id="b2639-330">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-330">String</span></span>                                                   | <span data-ttu-id="b2639-331">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-331">Yes</span></span>      | <span data-ttu-id="b2639-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-332">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-333">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-333">assignmentState</span></span>  | <span data-ttu-id="b2639-334">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-334">String</span></span>                                                   | <span data-ttu-id="b2639-335">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-335">Yes</span></span>      | <span data-ttu-id="b2639-336">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-336">Eligible / Active</span></span> |
| <span data-ttu-id="b2639-337">type</span><span class="sxs-lookup"><span data-stu-id="b2639-337">type</span></span>             | <span data-ttu-id="b2639-338">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-338">String</span></span>                                                   | <span data-ttu-id="b2639-339">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-339">Yes</span></span>      | <span data-ttu-id="b2639-340">adminremove</span><span class="sxs-lookup"><span data-stu-id="b2639-340">AdminRemove</span></span> |
| <span data-ttu-id="b2639-341">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-341">reason</span></span>           | <span data-ttu-id="b2639-342">String</span><span class="sxs-lookup"><span data-stu-id="b2639-342">String</span></span>                                                   | <span data-ttu-id="b2639-343">いいえ</span><span class="sxs-lookup"><span data-stu-id="b2639-343">No</span></span>       |   |
| <span data-ttu-id="b2639-344">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-344">schedule</span></span>         | [<span data-ttu-id="b2639-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-346">いいえ</span><span class="sxs-lookup"><span data-stu-id="b2639-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="b2639-347">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-348">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="b2639-349">例 5: 管理者の更新の役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="b2639-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="b2639-350">この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。</span><span class="sxs-lookup"><span data-stu-id="b2639-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="b2639-351">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2639-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b2639-352">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-352">Property</span></span>         | <span data-ttu-id="b2639-353">型</span><span class="sxs-lookup"><span data-stu-id="b2639-353">Type</span></span>                                                     | <span data-ttu-id="b2639-354">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-354">Required</span></span>                | <span data-ttu-id="b2639-355">値</span><span class="sxs-lookup"><span data-stu-id="b2639-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="b2639-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-356">resourceId</span></span>       | <span data-ttu-id="b2639-357">String</span><span class="sxs-lookup"><span data-stu-id="b2639-357">String</span></span>                                                   | <span data-ttu-id="b2639-358">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-358">Yes</span></span>                     | <span data-ttu-id="b2639-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-359">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-360">roleDefinitionId</span></span> | <span data-ttu-id="b2639-361">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-361">String</span></span>                                                   | <span data-ttu-id="b2639-362">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-362">Yes</span></span>                     | <span data-ttu-id="b2639-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-364">subjectId</span></span>        | <span data-ttu-id="b2639-365">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-365">String</span></span>                                                   | <span data-ttu-id="b2639-366">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-366">Yes</span></span>                     | <span data-ttu-id="b2639-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-367">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-368">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-368">assignmentState</span></span>  | <span data-ttu-id="b2639-369">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-369">String</span></span>                                                   | <span data-ttu-id="b2639-370">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-370">Yes</span></span>                     | <span data-ttu-id="b2639-371">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-371">Eligible / Active</span></span> |
| <span data-ttu-id="b2639-372">type</span><span class="sxs-lookup"><span data-stu-id="b2639-372">type</span></span>             | <span data-ttu-id="b2639-373">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-373">String</span></span>                                                   | <span data-ttu-id="b2639-374">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-374">Yes</span></span>                     | <span data-ttu-id="b2639-375">adminupdate</span><span class="sxs-lookup"><span data-stu-id="b2639-375">AdminUpdate</span></span> |
| <span data-ttu-id="b2639-376">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-376">reason</span></span>           | <span data-ttu-id="b2639-377">String</span><span class="sxs-lookup"><span data-stu-id="b2639-377">String</span></span>                                                   | <span data-ttu-id="b2639-378">rolesettings に依存</span><span class="sxs-lookup"><span data-stu-id="b2639-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="b2639-379">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-379">schedule</span></span>         | [<span data-ttu-id="b2639-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-381">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="b2639-382">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-383">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="b2639-384">例 6: 管理者が期限切れの役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="b2639-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="b2639-385">この例では、user anucuser の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。</span><span class="sxs-lookup"><span data-stu-id="b2639-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="b2639-386">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2639-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b2639-387">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2639-387">Property</span></span>         | <span data-ttu-id="b2639-388">型</span><span class="sxs-lookup"><span data-stu-id="b2639-388">Type</span></span>                                                     | <span data-ttu-id="b2639-389">必須</span><span class="sxs-lookup"><span data-stu-id="b2639-389">Required</span></span>                | <span data-ttu-id="b2639-390">値</span><span class="sxs-lookup"><span data-stu-id="b2639-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="b2639-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="b2639-391">resourceId</span></span>       | <span data-ttu-id="b2639-392">String</span><span class="sxs-lookup"><span data-stu-id="b2639-392">String</span></span>                                                   | <span data-ttu-id="b2639-393">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-393">Yes</span></span>                     | <span data-ttu-id="b2639-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b2639-394">\<resourceId\></span></span> |
| <span data-ttu-id="b2639-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b2639-395">roleDefinitionId</span></span> | <span data-ttu-id="b2639-396">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-396">String</span></span>                                                   | <span data-ttu-id="b2639-397">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-397">Yes</span></span>                     | <span data-ttu-id="b2639-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b2639-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b2639-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="b2639-399">subjectId</span></span>        | <span data-ttu-id="b2639-400">文字列</span><span class="sxs-lookup"><span data-stu-id="b2639-400">String</span></span>                                                   | <span data-ttu-id="b2639-401">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-401">Yes</span></span>                     | <span data-ttu-id="b2639-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b2639-402">\<subjectId\></span></span> |
| <span data-ttu-id="b2639-403">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b2639-403">assignmentState</span></span>  | <span data-ttu-id="b2639-404">String</span><span class="sxs-lookup"><span data-stu-id="b2639-404">String</span></span>                                                   | <span data-ttu-id="b2639-405">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-405">Yes</span></span>                     | <span data-ttu-id="b2639-406">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="b2639-406">Eligible / Active</span></span> |
| <span data-ttu-id="b2639-407">type</span><span class="sxs-lookup"><span data-stu-id="b2639-407">type</span></span>             | <span data-ttu-id="b2639-408">String</span><span class="sxs-lookup"><span data-stu-id="b2639-408">String</span></span>                                                   | <span data-ttu-id="b2639-409">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-409">Yes</span></span>                     | <span data-ttu-id="b2639-410">adminextend</span><span class="sxs-lookup"><span data-stu-id="b2639-410">AdminExtend</span></span> |
| <span data-ttu-id="b2639-411">したがっ</span><span class="sxs-lookup"><span data-stu-id="b2639-411">reason</span></span>           | <span data-ttu-id="b2639-412">String</span><span class="sxs-lookup"><span data-stu-id="b2639-412">String</span></span>                                                   | <span data-ttu-id="b2639-413">rolesettings に依存</span><span class="sxs-lookup"><span data-stu-id="b2639-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="b2639-414">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="b2639-414">schedule</span></span>         | [<span data-ttu-id="b2639-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b2639-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b2639-416">はい</span><span class="sxs-lookup"><span data-stu-id="b2639-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="b2639-417">要求</span><span class="sxs-lookup"><span data-stu-id="b2639-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2639-418">応答</span><span class="sxs-lookup"><span data-stu-id="b2639-418">Response</span></span>

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
  "suppressions": []
}
-->
