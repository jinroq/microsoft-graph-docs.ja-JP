---
title: governanceRoleAssignmentRequest を作成する
description: 役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。 次の表に、操作の一覧を示します。
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503283"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="24a68-104">governanceRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="24a68-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24a68-105">役割の割り当てに対して必要な操作を表すための役割の割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="24a68-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="24a68-106">次の表に、操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="24a68-106">The following table lists the operations.</span></span>

| <span data-ttu-id="24a68-107">操作</span><span class="sxs-lookup"><span data-stu-id="24a68-107">Operation</span></span>                                   | <span data-ttu-id="24a68-108">型</span><span class="sxs-lookup"><span data-stu-id="24a68-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="24a68-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="24a68-109">Assign a role assignment</span></span>                    | <span data-ttu-id="24a68-110">adminadd</span><span class="sxs-lookup"><span data-stu-id="24a68-110">AdminAdd</span></span>    |
| <span data-ttu-id="24a68-111">適格な役割の割り当てをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="24a68-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="24a68-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="24a68-112">UserAdd</span></span>     |
| <span data-ttu-id="24a68-113">アクティブ化された役割の割り当てを無効にする</span><span class="sxs-lookup"><span data-stu-id="24a68-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="24a68-114">userremove</span><span class="sxs-lookup"><span data-stu-id="24a68-114">UserRemove</span></span>  |
| <span data-ttu-id="24a68-115">役割の割り当てを削除する</span><span class="sxs-lookup"><span data-stu-id="24a68-115">Remove a role assignment</span></span>                    | <span data-ttu-id="24a68-116">adminremove</span><span class="sxs-lookup"><span data-stu-id="24a68-116">AdminRemove</span></span> |
| <span data-ttu-id="24a68-117">役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="24a68-117">Update a role assignment</span></span>                    | <span data-ttu-id="24a68-118">adminupdate</span><span class="sxs-lookup"><span data-stu-id="24a68-118">AdminUpdate</span></span> |
| <span data-ttu-id="24a68-119">自分の役割の割り当てを拡張するための要求</span><span class="sxs-lookup"><span data-stu-id="24a68-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="24a68-120">userextend</span><span class="sxs-lookup"><span data-stu-id="24a68-120">UserExtend</span></span>  |
| <span data-ttu-id="24a68-121">役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="24a68-121">Extend a role assignment</span></span>                    | <span data-ttu-id="24a68-122">adminextend</span><span class="sxs-lookup"><span data-stu-id="24a68-122">AdminExtend</span></span> |
| <span data-ttu-id="24a68-123">期限切れの役割の割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="24a68-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="24a68-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="24a68-124">UserRenew</span></span>   |
| <span data-ttu-id="24a68-125">期限切れの役割の割り当てを更新する</span><span class="sxs-lookup"><span data-stu-id="24a68-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="24a68-126">adminrenew</span><span class="sxs-lookup"><span data-stu-id="24a68-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="24a68-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24a68-127">Permissions</span></span>

<span data-ttu-id="24a68-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24a68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24a68-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24a68-130">Permission type</span></span>                        | <span data-ttu-id="24a68-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24a68-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="24a68-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24a68-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="24a68-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="24a68-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="24a68-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24a68-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24a68-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24a68-135">Not supported.</span></span>                            |
| <span data-ttu-id="24a68-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24a68-136">Application</span></span>                            | <span data-ttu-id="24a68-137">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="24a68-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="24a68-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24a68-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="24a68-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24a68-139">Request headers</span></span>

| <span data-ttu-id="24a68-140">名前</span><span class="sxs-lookup"><span data-stu-id="24a68-140">Name</span></span>          | <span data-ttu-id="24a68-141">説明</span><span class="sxs-lookup"><span data-stu-id="24a68-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="24a68-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="24a68-142">Authorization</span></span> | <span data-ttu-id="24a68-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="24a68-143">Bearer {code}</span></span>    |
| <span data-ttu-id="24a68-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="24a68-144">Content-type</span></span>  | <span data-ttu-id="24a68-145">application/json</span><span class="sxs-lookup"><span data-stu-id="24a68-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24a68-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="24a68-146">Request body</span></span>

<span data-ttu-id="24a68-147">要求本文で、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24a68-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="24a68-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-148">Property</span></span>         | <span data-ttu-id="24a68-149">型</span><span class="sxs-lookup"><span data-stu-id="24a68-149">Type</span></span>                                                     | <span data-ttu-id="24a68-150">説明</span><span class="sxs-lookup"><span data-stu-id="24a68-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="24a68-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-151">resourceId</span></span>       | <span data-ttu-id="24a68-152">String</span><span class="sxs-lookup"><span data-stu-id="24a68-152">String</span></span>                                                   | <span data-ttu-id="24a68-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="24a68-153">The ID of the resource.</span></span> <span data-ttu-id="24a68-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="24a68-154">Required.</span></span> |
| <span data-ttu-id="24a68-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-155">roleDefinitionId</span></span> | <span data-ttu-id="24a68-156">String</span><span class="sxs-lookup"><span data-stu-id="24a68-156">String</span></span>                                                   | <span data-ttu-id="24a68-157">ロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="24a68-157">The ID of the role definition.</span></span> <span data-ttu-id="24a68-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="24a68-158">Required.</span></span> |
| <span data-ttu-id="24a68-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-159">subjectId</span></span>        | <span data-ttu-id="24a68-160">String</span><span class="sxs-lookup"><span data-stu-id="24a68-160">String</span></span>                                                   | <span data-ttu-id="24a68-161">件名の ID。</span><span class="sxs-lookup"><span data-stu-id="24a68-161">The ID of the subject.</span></span> <span data-ttu-id="24a68-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="24a68-162">Required.</span></span> |
| <span data-ttu-id="24a68-163">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-163">assignmentState</span></span>  | <span data-ttu-id="24a68-164">String</span><span class="sxs-lookup"><span data-stu-id="24a68-164">String</span></span>                                                   | <span data-ttu-id="24a68-165">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="24a68-165">The state of assignment.</span></span> <span data-ttu-id="24a68-166">値には、 `Eligible`および`Active`を指定できます。</span><span class="sxs-lookup"><span data-stu-id="24a68-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="24a68-167">必須。</span><span class="sxs-lookup"><span data-stu-id="24a68-167">Required.</span></span> |
| <span data-ttu-id="24a68-168">type</span><span class="sxs-lookup"><span data-stu-id="24a68-168">type</span></span>             | <span data-ttu-id="24a68-169">String</span><span class="sxs-lookup"><span data-stu-id="24a68-169">String</span></span>                                                   | <span data-ttu-id="24a68-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="24a68-170">The request type.</span></span> <span data-ttu-id="24a68-171">値には、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、 `AdminRenew`を`AdminExtend`使用できます。</span><span class="sxs-lookup"><span data-stu-id="24a68-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="24a68-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="24a68-172">Required.</span></span> |
| <span data-ttu-id="24a68-173">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-173">reason</span></span>           | <span data-ttu-id="24a68-174">String</span><span class="sxs-lookup"><span data-stu-id="24a68-174">String</span></span>                                                   | <span data-ttu-id="24a68-175">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="24a68-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="24a68-176">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-176">schedule</span></span>         | [<span data-ttu-id="24a68-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-178">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="24a68-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="24a68-179">、 `UserAdd` `AdminAdd`、、および`AdminExtend`の要求の種類には、が必要です。 `AdminUpdate`</span><span class="sxs-lookup"><span data-stu-id="24a68-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="24a68-180">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-180">Response</span></span>

<span data-ttu-id="24a68-181">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24a68-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="24a68-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="24a68-182">Error codes</span></span>

<span data-ttu-id="24a68-183">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="24a68-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="24a68-184">また、次の表に示されているエラーコードも返します。</span><span class="sxs-lookup"><span data-stu-id="24a68-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="24a68-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="24a68-185">Error code</span></span>     | <span data-ttu-id="24a68-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="24a68-186">Error message</span></span>                               | <span data-ttu-id="24a68-187">詳細</span><span class="sxs-lookup"><span data-stu-id="24a68-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="24a68-188">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-188">400 BadRequest</span></span> | <span data-ttu-id="24a68-189">rolenotfound</span><span class="sxs-lookup"><span data-stu-id="24a68-189">RoleNotFound</span></span>                                | <span data-ttu-id="24a68-190">要求`roleDefinitionId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="24a68-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="24a68-191">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-191">400 BadRequest</span></span> | <span data-ttu-id="24a68-192">resourceislocked</span><span class="sxs-lookup"><span data-stu-id="24a68-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="24a68-193">要求本文で指定されたリソースはの状態`Locked`にあり、役割の割り当て要求を作成できません。</span><span class="sxs-lookup"><span data-stu-id="24a68-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="24a68-194">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-194">400 BadRequest</span></span> | <span data-ttu-id="24a68-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="24a68-195">SubjectNotFound</span></span>                             | <span data-ttu-id="24a68-196">要求`subjectId`本文で指定されたが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="24a68-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="24a68-197">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-197">400 BadRequest</span></span> | <span data-ttu-id="24a68-198">pendingrole割り当て要求</span><span class="sxs-lookup"><span data-stu-id="24a68-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="24a68-199">保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)がシステムに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="24a68-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="24a68-200">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-200">400 BadRequest</span></span> | <span data-ttu-id="24a68-201">role割り当てが存在する</span><span class="sxs-lookup"><span data-stu-id="24a68-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="24a68-202">作成するよう要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに既に存在しています。</span><span class="sxs-lookup"><span data-stu-id="24a68-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="24a68-203">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-203">400 BadRequest</span></span> | <span data-ttu-id="24a68-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="24a68-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="24a68-205">更新または拡張が要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="24a68-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="24a68-206">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="24a68-206">400 BadRequest</span></span> | <span data-ttu-id="24a68-207">role割り当て要求 policyvalidationfailed</span><span class="sxs-lookup"><span data-stu-id="24a68-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="24a68-208">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は内部ポリシーを満たしていないため、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="24a68-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="24a68-209">例</span><span class="sxs-lookup"><span data-stu-id="24a68-209">Examples</span></span>

<span data-ttu-id="24a68-210">次の例は、この API の使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="24a68-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="24a68-211">例 1: 管理者がユーザーを役割に割り当てる</span><span class="sxs-lookup"><span data-stu-id="24a68-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="24a68-212">この例では、管理者がユーザー nawu@fimdev.net を課金閲覧者の役割に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="24a68-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="24a68-213">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24a68-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="24a68-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-214">Property</span></span>         | <span data-ttu-id="24a68-215">型</span><span class="sxs-lookup"><span data-stu-id="24a68-215">Type</span></span>                                                     | <span data-ttu-id="24a68-216">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-216">Required</span></span>                 | <span data-ttu-id="24a68-217">値</span><span class="sxs-lookup"><span data-stu-id="24a68-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="24a68-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-218">resourceId</span></span>       | <span data-ttu-id="24a68-219">String</span><span class="sxs-lookup"><span data-stu-id="24a68-219">String</span></span>                                                   | <span data-ttu-id="24a68-220">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-220">Yes</span></span>                      | <span data-ttu-id="24a68-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-221">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-222">roleDefinitionId</span></span> | <span data-ttu-id="24a68-223">String</span><span class="sxs-lookup"><span data-stu-id="24a68-223">String</span></span>                                                   | <span data-ttu-id="24a68-224">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-224">Yes</span></span>                      | <span data-ttu-id="24a68-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-226">subjectId</span></span>        | <span data-ttu-id="24a68-227">String</span><span class="sxs-lookup"><span data-stu-id="24a68-227">String</span></span>                                                   | <span data-ttu-id="24a68-228">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-228">Yes</span></span>                      | <span data-ttu-id="24a68-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-229">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-230">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-230">assignmentState</span></span>  | <span data-ttu-id="24a68-231">String</span><span class="sxs-lookup"><span data-stu-id="24a68-231">String</span></span>                                                   | <span data-ttu-id="24a68-232">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-232">Yes</span></span>                      | <span data-ttu-id="24a68-233">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="24a68-233">Eligible / Active</span></span> |
| <span data-ttu-id="24a68-234">type</span><span class="sxs-lookup"><span data-stu-id="24a68-234">type</span></span>             | <span data-ttu-id="24a68-235">String</span><span class="sxs-lookup"><span data-stu-id="24a68-235">String</span></span>                                                   | <span data-ttu-id="24a68-236">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-236">Yes</span></span>                      | <span data-ttu-id="24a68-237">adminadd</span><span class="sxs-lookup"><span data-stu-id="24a68-237">AdminAdd</span></span> |
| <span data-ttu-id="24a68-238">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-238">reason</span></span>           | <span data-ttu-id="24a68-239">String</span><span class="sxs-lookup"><span data-stu-id="24a68-239">String</span></span>                                                   | <span data-ttu-id="24a68-240">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="24a68-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="24a68-241">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-241">schedule</span></span>         | [<span data-ttu-id="24a68-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-243">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="24a68-244">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-245">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="24a68-246">例 2: ユーザーが対象となる役割をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="24a68-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="24a68-247">この例では、ユーザー nawu@fimdev.net が対象となる請求リーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="24a68-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="24a68-248">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-248">Property</span></span>         | <span data-ttu-id="24a68-249">型</span><span class="sxs-lookup"><span data-stu-id="24a68-249">Type</span></span>                                                     | <span data-ttu-id="24a68-250">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-250">Required</span></span>                 | <span data-ttu-id="24a68-251">値</span><span class="sxs-lookup"><span data-stu-id="24a68-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="24a68-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-252">resourceId</span></span>       | <span data-ttu-id="24a68-253">String</span><span class="sxs-lookup"><span data-stu-id="24a68-253">String</span></span>                                                   | <span data-ttu-id="24a68-254">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-254">Yes</span></span>                      | <span data-ttu-id="24a68-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-255">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-256">roleDefinitionId</span></span> | <span data-ttu-id="24a68-257">String</span><span class="sxs-lookup"><span data-stu-id="24a68-257">String</span></span>                                                   | <span data-ttu-id="24a68-258">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-258">Yes</span></span>                      | <span data-ttu-id="24a68-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-260">subjectId</span></span>        | <span data-ttu-id="24a68-261">String</span><span class="sxs-lookup"><span data-stu-id="24a68-261">String</span></span>                                                   | <span data-ttu-id="24a68-262">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-262">Yes</span></span>                      | <span data-ttu-id="24a68-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-263">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-264">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-264">assignmentState</span></span>  | <span data-ttu-id="24a68-265">String</span><span class="sxs-lookup"><span data-stu-id="24a68-265">String</span></span>                                                   | <span data-ttu-id="24a68-266">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-266">Yes</span></span>                      | <span data-ttu-id="24a68-267">Active</span><span class="sxs-lookup"><span data-stu-id="24a68-267">Active</span></span> |
| <span data-ttu-id="24a68-268">type</span><span class="sxs-lookup"><span data-stu-id="24a68-268">type</span></span>             | <span data-ttu-id="24a68-269">String</span><span class="sxs-lookup"><span data-stu-id="24a68-269">String</span></span>                                                   | <span data-ttu-id="24a68-270">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-270">Yes</span></span>                      | <span data-ttu-id="24a68-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="24a68-271">UserAdd</span></span> |
| <span data-ttu-id="24a68-272">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-272">reason</span></span>           | <span data-ttu-id="24a68-273">String</span><span class="sxs-lookup"><span data-stu-id="24a68-273">String</span></span>                                                   | <span data-ttu-id="24a68-274">役割の設定によって異なる</span><span class="sxs-lookup"><span data-stu-id="24a68-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="24a68-275">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-275">schedule</span></span>         | [<span data-ttu-id="24a68-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-277">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="24a68-278">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-279">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="24a68-280">例 3: ユーザーが割り当てられた役割を非アクティブにする</span><span class="sxs-lookup"><span data-stu-id="24a68-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="24a68-281">この例では、ユーザー nawu@fimdev.net がアクティブな課金閲覧者の役割を非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="24a68-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="24a68-282">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-282">Property</span></span>         | <span data-ttu-id="24a68-283">型</span><span class="sxs-lookup"><span data-stu-id="24a68-283">Type</span></span>                                                     | <span data-ttu-id="24a68-284">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-284">Required</span></span> | <span data-ttu-id="24a68-285">値</span><span class="sxs-lookup"><span data-stu-id="24a68-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="24a68-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-286">resourceId</span></span>       | <span data-ttu-id="24a68-287">String</span><span class="sxs-lookup"><span data-stu-id="24a68-287">String</span></span>                                                   | <span data-ttu-id="24a68-288">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-288">Yes</span></span>      | <span data-ttu-id="24a68-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-289">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-290">roleDefinitionId</span></span> | <span data-ttu-id="24a68-291">String</span><span class="sxs-lookup"><span data-stu-id="24a68-291">String</span></span>                                                   | <span data-ttu-id="24a68-292">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-292">Yes</span></span>      | <span data-ttu-id="24a68-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-294">subjectId</span></span>        | <span data-ttu-id="24a68-295">String</span><span class="sxs-lookup"><span data-stu-id="24a68-295">String</span></span>                                                   | <span data-ttu-id="24a68-296">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-296">Yes</span></span>      | <span data-ttu-id="24a68-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-297">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-298">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-298">assignmentState</span></span>  | <span data-ttu-id="24a68-299">String</span><span class="sxs-lookup"><span data-stu-id="24a68-299">String</span></span>                                                   | <span data-ttu-id="24a68-300">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-300">Yes</span></span>      | <span data-ttu-id="24a68-301">Active</span><span class="sxs-lookup"><span data-stu-id="24a68-301">Active</span></span> |
| <span data-ttu-id="24a68-302">type</span><span class="sxs-lookup"><span data-stu-id="24a68-302">type</span></span>             | <span data-ttu-id="24a68-303">String</span><span class="sxs-lookup"><span data-stu-id="24a68-303">String</span></span>                                                   | <span data-ttu-id="24a68-304">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-304">Yes</span></span>      | <span data-ttu-id="24a68-305">userremove</span><span class="sxs-lookup"><span data-stu-id="24a68-305">UserRemove</span></span> |
| <span data-ttu-id="24a68-306">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-306">reason</span></span>           | <span data-ttu-id="24a68-307">String</span><span class="sxs-lookup"><span data-stu-id="24a68-307">String</span></span>                                                   | <span data-ttu-id="24a68-308">いいえ</span><span class="sxs-lookup"><span data-stu-id="24a68-308">No</span></span>       |   |
| <span data-ttu-id="24a68-309">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-309">schedule</span></span>         | [<span data-ttu-id="24a68-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-311">いいえ</span><span class="sxs-lookup"><span data-stu-id="24a68-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="24a68-312">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-313">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="24a68-314">例 4: 管理者が役割からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="24a68-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="24a68-315">この例では、管理者が Billing Reader ロールからユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="24a68-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="24a68-316">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24a68-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="24a68-317">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-317">Property</span></span>         | <span data-ttu-id="24a68-318">型</span><span class="sxs-lookup"><span data-stu-id="24a68-318">Type</span></span>                                                     | <span data-ttu-id="24a68-319">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-319">Required</span></span> | <span data-ttu-id="24a68-320">値</span><span class="sxs-lookup"><span data-stu-id="24a68-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="24a68-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-321">resourceId</span></span>       | <span data-ttu-id="24a68-322">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-322">String</span></span>                                                   | <span data-ttu-id="24a68-323">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-323">Yes</span></span>      | <span data-ttu-id="24a68-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-324">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-325">roleDefinitionId</span></span> | <span data-ttu-id="24a68-326">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-326">String</span></span>                                                   | <span data-ttu-id="24a68-327">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-327">Yes</span></span>      | <span data-ttu-id="24a68-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-329">subjectId</span></span>        | <span data-ttu-id="24a68-330">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-330">String</span></span>                                                   | <span data-ttu-id="24a68-331">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-331">Yes</span></span>      | <span data-ttu-id="24a68-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-332">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-333">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-333">assignmentState</span></span>  | <span data-ttu-id="24a68-334">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-334">String</span></span>                                                   | <span data-ttu-id="24a68-335">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-335">Yes</span></span>      | <span data-ttu-id="24a68-336">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="24a68-336">Eligible / Active</span></span> |
| <span data-ttu-id="24a68-337">type</span><span class="sxs-lookup"><span data-stu-id="24a68-337">type</span></span>             | <span data-ttu-id="24a68-338">String</span><span class="sxs-lookup"><span data-stu-id="24a68-338">String</span></span>                                                   | <span data-ttu-id="24a68-339">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-339">Yes</span></span>      | <span data-ttu-id="24a68-340">adminremove</span><span class="sxs-lookup"><span data-stu-id="24a68-340">AdminRemove</span></span> |
| <span data-ttu-id="24a68-341">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-341">reason</span></span>           | <span data-ttu-id="24a68-342">String</span><span class="sxs-lookup"><span data-stu-id="24a68-342">String</span></span>                                                   | <span data-ttu-id="24a68-343">いいえ</span><span class="sxs-lookup"><span data-stu-id="24a68-343">No</span></span>       |   |
| <span data-ttu-id="24a68-344">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-344">schedule</span></span>         | [<span data-ttu-id="24a68-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-346">いいえ</span><span class="sxs-lookup"><span data-stu-id="24a68-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="24a68-347">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-348">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="24a68-349">例 5: 管理者の更新の役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="24a68-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="24a68-350">この例では、管理者がユーザー nawu@fimdev.net の役割の割り当てを所有者に更新します。</span><span class="sxs-lookup"><span data-stu-id="24a68-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="24a68-351">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24a68-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="24a68-352">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-352">Property</span></span>         | <span data-ttu-id="24a68-353">型</span><span class="sxs-lookup"><span data-stu-id="24a68-353">Type</span></span>                                                     | <span data-ttu-id="24a68-354">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-354">Required</span></span>                | <span data-ttu-id="24a68-355">値</span><span class="sxs-lookup"><span data-stu-id="24a68-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="24a68-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-356">resourceId</span></span>       | <span data-ttu-id="24a68-357">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-357">String</span></span>                                                   | <span data-ttu-id="24a68-358">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-358">Yes</span></span>                     | <span data-ttu-id="24a68-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-359">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-360">roleDefinitionId</span></span> | <span data-ttu-id="24a68-361">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-361">String</span></span>                                                   | <span data-ttu-id="24a68-362">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-362">Yes</span></span>                     | <span data-ttu-id="24a68-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-364">subjectId</span></span>        | <span data-ttu-id="24a68-365">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-365">String</span></span>                                                   | <span data-ttu-id="24a68-366">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-366">Yes</span></span>                     | <span data-ttu-id="24a68-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-367">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-368">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-368">assignmentState</span></span>  | <span data-ttu-id="24a68-369">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-369">String</span></span>                                                   | <span data-ttu-id="24a68-370">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-370">Yes</span></span>                     | <span data-ttu-id="24a68-371">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="24a68-371">Eligible / Active</span></span> |
| <span data-ttu-id="24a68-372">type</span><span class="sxs-lookup"><span data-stu-id="24a68-372">type</span></span>             | <span data-ttu-id="24a68-373">String</span><span class="sxs-lookup"><span data-stu-id="24a68-373">String</span></span>                                                   | <span data-ttu-id="24a68-374">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-374">Yes</span></span>                     | <span data-ttu-id="24a68-375">adminupdate</span><span class="sxs-lookup"><span data-stu-id="24a68-375">AdminUpdate</span></span> |
| <span data-ttu-id="24a68-376">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-376">reason</span></span>           | <span data-ttu-id="24a68-377">String</span><span class="sxs-lookup"><span data-stu-id="24a68-377">String</span></span>                                                   | <span data-ttu-id="24a68-378">rolesettings に依存</span><span class="sxs-lookup"><span data-stu-id="24a68-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="24a68-379">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-379">schedule</span></span>         | [<span data-ttu-id="24a68-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-381">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="24a68-382">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-383">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="24a68-384">例 6: 管理者が期限切れの役割の割り当てを拡張する</span><span class="sxs-lookup"><span data-stu-id="24a68-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="24a68-385">この例では、user anucuser の期限切れのロール割り当てを API Management Service 共同作成者に拡張します。</span><span class="sxs-lookup"><span data-stu-id="24a68-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="24a68-386">**注:** この例では、アクセス許可に加えて、リソースに対して少なく`Active`とも1つ`owner`の`user access administrator`管理者ロールの割り当て (または) が要求者に割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24a68-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="24a68-387">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a68-387">Property</span></span>         | <span data-ttu-id="24a68-388">型</span><span class="sxs-lookup"><span data-stu-id="24a68-388">Type</span></span>                                                     | <span data-ttu-id="24a68-389">必須</span><span class="sxs-lookup"><span data-stu-id="24a68-389">Required</span></span>                | <span data-ttu-id="24a68-390">値</span><span class="sxs-lookup"><span data-stu-id="24a68-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="24a68-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="24a68-391">resourceId</span></span>       | <span data-ttu-id="24a68-392">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-392">String</span></span>                                                   | <span data-ttu-id="24a68-393">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-393">Yes</span></span>                     | <span data-ttu-id="24a68-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="24a68-394">\<resourceId\></span></span> |
| <span data-ttu-id="24a68-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24a68-395">roleDefinitionId</span></span> | <span data-ttu-id="24a68-396">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-396">String</span></span>                                                   | <span data-ttu-id="24a68-397">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-397">Yes</span></span>                     | <span data-ttu-id="24a68-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="24a68-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="24a68-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="24a68-399">subjectId</span></span>        | <span data-ttu-id="24a68-400">文字列</span><span class="sxs-lookup"><span data-stu-id="24a68-400">String</span></span>                                                   | <span data-ttu-id="24a68-401">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-401">Yes</span></span>                     | <span data-ttu-id="24a68-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="24a68-402">\<subjectId\></span></span> |
| <span data-ttu-id="24a68-403">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="24a68-403">assignmentState</span></span>  | <span data-ttu-id="24a68-404">String</span><span class="sxs-lookup"><span data-stu-id="24a68-404">String</span></span>                                                   | <span data-ttu-id="24a68-405">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-405">Yes</span></span>                     | <span data-ttu-id="24a68-406">対象/アクティブ</span><span class="sxs-lookup"><span data-stu-id="24a68-406">Eligible / Active</span></span> |
| <span data-ttu-id="24a68-407">type</span><span class="sxs-lookup"><span data-stu-id="24a68-407">type</span></span>             | <span data-ttu-id="24a68-408">String</span><span class="sxs-lookup"><span data-stu-id="24a68-408">String</span></span>                                                   | <span data-ttu-id="24a68-409">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-409">Yes</span></span>                     | <span data-ttu-id="24a68-410">adminextend</span><span class="sxs-lookup"><span data-stu-id="24a68-410">AdminExtend</span></span> |
| <span data-ttu-id="24a68-411">したがっ</span><span class="sxs-lookup"><span data-stu-id="24a68-411">reason</span></span>           | <span data-ttu-id="24a68-412">String</span><span class="sxs-lookup"><span data-stu-id="24a68-412">String</span></span>                                                   | <span data-ttu-id="24a68-413">rolesettings に依存</span><span class="sxs-lookup"><span data-stu-id="24a68-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="24a68-414">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="24a68-414">schedule</span></span>         | [<span data-ttu-id="24a68-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24a68-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="24a68-416">はい</span><span class="sxs-lookup"><span data-stu-id="24a68-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="24a68-417">要求</span><span class="sxs-lookup"><span data-stu-id="24a68-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="24a68-418">応答</span><span class="sxs-lookup"><span data-stu-id="24a68-418">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
