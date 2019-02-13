---
title: GovernanceRoleAssignmentRequest を作成します。
description: 役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。 次の表に、操作をします。
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967222"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="1ed5d-104">GovernanceRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ed5d-105">役割の割り当てで必要な操作を表すロールの割り当て要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="1ed5d-106">次の表に、操作をします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-106">The following table lists the operations.</span></span>

| <span data-ttu-id="1ed5d-107">Operation</span><span class="sxs-lookup"><span data-stu-id="1ed5d-107">Operation</span></span>                                   | <span data-ttu-id="1ed5d-108">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="1ed5d-109">役割の割り当てを割り当てる</span><span class="sxs-lookup"><span data-stu-id="1ed5d-109">Assign a role assignment</span></span>                    | <span data-ttu-id="1ed5d-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="1ed5d-110">AdminAdd</span></span>    |
| <span data-ttu-id="1ed5d-111">対象のロール割り当てを有効化します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="1ed5d-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="1ed5d-112">UserAdd</span></span>     |
| <span data-ttu-id="1ed5d-113">アクティブ化されたロール割り当てを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="1ed5d-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="1ed5d-114">UserRemove</span></span>  |
| <span data-ttu-id="1ed5d-115">役割の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-115">Remove a role assignment</span></span>                    | <span data-ttu-id="1ed5d-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="1ed5d-116">AdminRemove</span></span> |
| <span data-ttu-id="1ed5d-117">役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-117">Update a role assignment</span></span>                    | <span data-ttu-id="1ed5d-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="1ed5d-118">AdminUpdate</span></span> |
| <span data-ttu-id="1ed5d-119">自分の役割の割り当てを拡張する要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="1ed5d-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="1ed5d-120">UserExtend</span></span>  |
| <span data-ttu-id="1ed5d-121">役割の割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-121">Extend a role assignment</span></span>                    | <span data-ttu-id="1ed5d-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="1ed5d-122">AdminExtend</span></span> |
| <span data-ttu-id="1ed5d-123">[期限切れのロールの割り当てを更新する要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="1ed5d-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="1ed5d-124">UserRenew</span></span>   |
| <span data-ttu-id="1ed5d-125">期限切れのロール割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="1ed5d-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="1ed5d-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="1ed5d-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ed5d-127">Permissions</span></span>

<span data-ttu-id="1ed5d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ed5d-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ed5d-130">Permission type</span></span>                        | <span data-ttu-id="1ed5d-131">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ed5d-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="1ed5d-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ed5d-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ed5d-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1ed5d-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="1ed5d-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ed5d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ed5d-135">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-135">Not supported.</span></span>                            |
| <span data-ttu-id="1ed5d-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ed5d-136">Application</span></span>                            | <span data-ttu-id="1ed5d-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1ed5d-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ed5d-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="1ed5d-139">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ed5d-139">Request headers</span></span>

| <span data-ttu-id="1ed5d-140">名前</span><span class="sxs-lookup"><span data-stu-id="1ed5d-140">Name</span></span>          | <span data-ttu-id="1ed5d-141">説明</span><span class="sxs-lookup"><span data-stu-id="1ed5d-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="1ed5d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ed5d-142">Authorization</span></span> | <span data-ttu-id="1ed5d-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ed5d-143">Bearer {code}</span></span>    |
| <span data-ttu-id="1ed5d-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-144">Content-type</span></span>  | <span data-ttu-id="1ed5d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed5d-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ed5d-146">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ed5d-146">Request body</span></span>

<span data-ttu-id="1ed5d-147">要求の本文には、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="1ed5d-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-148">Property</span></span>         | <span data-ttu-id="1ed5d-149">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-149">Type</span></span>                                                     | <span data-ttu-id="1ed5d-150">説明</span><span class="sxs-lookup"><span data-stu-id="1ed5d-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="1ed5d-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-151">resourceId</span></span>       | <span data-ttu-id="1ed5d-152">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-152">String</span></span>                                                   | <span data-ttu-id="1ed5d-153">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-153">The ID of the resource.</span></span> <span data-ttu-id="1ed5d-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-154">Required.</span></span> |
| <span data-ttu-id="1ed5d-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-155">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-156">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-156">String</span></span>                                                   | <span data-ttu-id="1ed5d-157">役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-157">The ID of the role definition.</span></span> <span data-ttu-id="1ed5d-158">必須です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-158">Required.</span></span> |
| <span data-ttu-id="1ed5d-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-159">subjectId</span></span>        | <span data-ttu-id="1ed5d-160">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-160">String</span></span>                                                   | <span data-ttu-id="1ed5d-161">サブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-161">The ID of the subject.</span></span> <span data-ttu-id="1ed5d-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-162">Required.</span></span> |
| <span data-ttu-id="1ed5d-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-163">assignmentState</span></span>  | <span data-ttu-id="1ed5d-164">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-164">String</span></span>                                                   | <span data-ttu-id="1ed5d-165">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-165">The state of assignment.</span></span> <span data-ttu-id="1ed5d-166">値は、`Eligible`と`Active`。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="1ed5d-167">必須。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-167">Required.</span></span> |
| <span data-ttu-id="1ed5d-168">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-168">type</span></span>             | <span data-ttu-id="1ed5d-169">文字列</span><span class="sxs-lookup"><span data-stu-id="1ed5d-169">String</span></span>                                                   | <span data-ttu-id="1ed5d-170">要求の種類。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-170">The request type.</span></span> <span data-ttu-id="1ed5d-171">値は、 `AdminAdd`、 `UserAdd`、 `AdminUpdate`、 `AdminRemove`、 `UserRemove`、 `UserExtend`、 `UserRenew`、`AdminRenew`と`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="1ed5d-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-172">Required.</span></span> |
| <span data-ttu-id="1ed5d-173">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-173">reason</span></span>           | <span data-ttu-id="1ed5d-174">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-174">String</span></span>                                                   | <span data-ttu-id="1ed5d-175">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="1ed5d-176">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-176">schedule</span></span>         | [<span data-ttu-id="1ed5d-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-178">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="1ed5d-179">要求の種類の`UserAdd`、 `AdminAdd`、`AdminUpdate`と`AdminExtend`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="1ed5d-180">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-180">Response</span></span>

<span data-ttu-id="1ed5d-181">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="1ed5d-182">エラー コード</span><span class="sxs-lookup"><span data-stu-id="1ed5d-182">Error codes</span></span>

<span data-ttu-id="1ed5d-183">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="1ed5d-184">さらに、また次の表に記載されているエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="1ed5d-185">エラー コード</span><span class="sxs-lookup"><span data-stu-id="1ed5d-185">Error code</span></span>     | <span data-ttu-id="1ed5d-186">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-186">Error message</span></span>                               | <span data-ttu-id="1ed5d-187">詳細</span><span class="sxs-lookup"><span data-stu-id="1ed5d-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="1ed5d-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-188">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="1ed5d-189">RoleNotFound</span></span>                                | <span data-ttu-id="1ed5d-190">`roleDefinitionId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="1ed5d-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-191">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="1ed5d-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="1ed5d-193">状態の要求の本文に記載されているリソースは、`Locked`と、役割の割り当て要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="1ed5d-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-194">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="1ed5d-195">SubjectNotFound</span></span>                             | <span data-ttu-id="1ed5d-196">`subjectId` 、要求の本文が見つかりません指定します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="1ed5d-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-197">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="1ed5d-199">あるシステムで保留中の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を既に存在します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="1ed5d-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-200">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="1ed5d-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="1ed5d-202">既に要求された[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="1ed5d-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-203">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="1ed5d-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="1ed5d-205">更新または拡張するように要求した[governanceRoleAssignment](../resources/governanceroleassignment.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="1ed5d-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1ed5d-206">400 BadRequest</span></span> | <span data-ttu-id="1ed5d-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="1ed5d-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="1ed5d-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)は、社内ポリシーを満たしていないと、作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="1ed5d-209">例</span><span class="sxs-lookup"><span data-stu-id="1ed5d-209">Examples</span></span>

<span data-ttu-id="1ed5d-210">次の例では、この API を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="1ed5d-211">例 1: 管理者のユーザーに割り当てるロール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="1ed5d-212">この例では、管理者は、課金情報の閲覧者の役割をユーザー nawu@fimdev.net を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="1ed5d-213">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="1ed5d-214">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-214">Property</span></span>         | <span data-ttu-id="1ed5d-215">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-215">Type</span></span>                                                     | <span data-ttu-id="1ed5d-216">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-216">Required</span></span>                 | <span data-ttu-id="1ed5d-217">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="1ed5d-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-218">resourceId</span></span>       | <span data-ttu-id="1ed5d-219">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-219">String</span></span>                                                   | <span data-ttu-id="1ed5d-220">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-220">Yes</span></span>                      | <span data-ttu-id="1ed5d-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-221">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-222">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-223">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-223">String</span></span>                                                   | <span data-ttu-id="1ed5d-224">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-224">Yes</span></span>                      | <span data-ttu-id="1ed5d-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-226">subjectId</span></span>        | <span data-ttu-id="1ed5d-227">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-227">String</span></span>                                                   | <span data-ttu-id="1ed5d-228">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-228">Yes</span></span>                      | <span data-ttu-id="1ed5d-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-229">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-230">assignmentState</span></span>  | <span data-ttu-id="1ed5d-231">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-231">String</span></span>                                                   | <span data-ttu-id="1ed5d-232">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-232">Yes</span></span>                      | <span data-ttu-id="1ed5d-233">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-233">Eligible / Active</span></span> |
| <span data-ttu-id="1ed5d-234">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-234">type</span></span>             | <span data-ttu-id="1ed5d-235">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-235">String</span></span>                                                   | <span data-ttu-id="1ed5d-236">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-236">Yes</span></span>                      | <span data-ttu-id="1ed5d-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="1ed5d-237">AdminAdd</span></span> |
| <span data-ttu-id="1ed5d-238">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-238">reason</span></span>           | <span data-ttu-id="1ed5d-239">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-239">String</span></span>                                                   | <span data-ttu-id="1ed5d-240">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="1ed5d-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="1ed5d-241">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-241">schedule</span></span>         | [<span data-ttu-id="1ed5d-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-243">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-244">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-245">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="1ed5d-246">例 2: ユーザーは対象となるロールをアクティブにします</span><span class="sxs-lookup"><span data-stu-id="1ed5d-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="1ed5d-247">この例では、ユーザー nawu@fimdev.net は、対象となる請求のリーダーの役割をアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="1ed5d-248">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-248">Property</span></span>         | <span data-ttu-id="1ed5d-249">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-249">Type</span></span>                                                     | <span data-ttu-id="1ed5d-250">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-250">Required</span></span>                 | <span data-ttu-id="1ed5d-251">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="1ed5d-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-252">resourceId</span></span>       | <span data-ttu-id="1ed5d-253">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-253">String</span></span>                                                   | <span data-ttu-id="1ed5d-254">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-254">Yes</span></span>                      | <span data-ttu-id="1ed5d-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-255">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-256">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-257">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-257">String</span></span>                                                   | <span data-ttu-id="1ed5d-258">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-258">Yes</span></span>                      | <span data-ttu-id="1ed5d-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-260">subjectId</span></span>        | <span data-ttu-id="1ed5d-261">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-261">String</span></span>                                                   | <span data-ttu-id="1ed5d-262">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-262">Yes</span></span>                      | <span data-ttu-id="1ed5d-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-263">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-264">assignmentState</span></span>  | <span data-ttu-id="1ed5d-265">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-265">String</span></span>                                                   | <span data-ttu-id="1ed5d-266">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-266">Yes</span></span>                      | <span data-ttu-id="1ed5d-267">Active</span><span class="sxs-lookup"><span data-stu-id="1ed5d-267">Active</span></span> |
| <span data-ttu-id="1ed5d-268">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-268">type</span></span>             | <span data-ttu-id="1ed5d-269">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-269">String</span></span>                                                   | <span data-ttu-id="1ed5d-270">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-270">Yes</span></span>                      | <span data-ttu-id="1ed5d-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="1ed5d-271">UserAdd</span></span> |
| <span data-ttu-id="1ed5d-272">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-272">reason</span></span>           | <span data-ttu-id="1ed5d-273">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-273">String</span></span>                                                   | <span data-ttu-id="1ed5d-274">ロールの設定によって異なります</span><span class="sxs-lookup"><span data-stu-id="1ed5d-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="1ed5d-275">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-275">schedule</span></span>         | [<span data-ttu-id="1ed5d-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-277">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-278">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-279">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="1ed5d-280">例 3: ユーザーが割り当て済みのロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="1ed5d-281">この例では、ユーザー nawu@fimdev.net には、作業中の課金情報の閲覧者の役割が無効になります。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="1ed5d-282">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-282">Property</span></span>         | <span data-ttu-id="1ed5d-283">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-283">Type</span></span>                                                     | <span data-ttu-id="1ed5d-284">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-284">Required</span></span> | <span data-ttu-id="1ed5d-285">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="1ed5d-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-286">resourceId</span></span>       | <span data-ttu-id="1ed5d-287">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-287">String</span></span>                                                   | <span data-ttu-id="1ed5d-288">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-288">Yes</span></span>      | <span data-ttu-id="1ed5d-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-289">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-290">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-291">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-291">String</span></span>                                                   | <span data-ttu-id="1ed5d-292">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-292">Yes</span></span>      | <span data-ttu-id="1ed5d-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-294">subjectId</span></span>        | <span data-ttu-id="1ed5d-295">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-295">String</span></span>                                                   | <span data-ttu-id="1ed5d-296">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-296">Yes</span></span>      | <span data-ttu-id="1ed5d-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-297">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-298">assignmentState</span></span>  | <span data-ttu-id="1ed5d-299">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-299">String</span></span>                                                   | <span data-ttu-id="1ed5d-300">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-300">Yes</span></span>      | <span data-ttu-id="1ed5d-301">Active</span><span class="sxs-lookup"><span data-stu-id="1ed5d-301">Active</span></span> |
| <span data-ttu-id="1ed5d-302">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-302">type</span></span>             | <span data-ttu-id="1ed5d-303">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-303">String</span></span>                                                   | <span data-ttu-id="1ed5d-304">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-304">Yes</span></span>      | <span data-ttu-id="1ed5d-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="1ed5d-305">UserRemove</span></span> |
| <span data-ttu-id="1ed5d-306">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-306">reason</span></span>           | <span data-ttu-id="1ed5d-307">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-307">String</span></span>                                                   | <span data-ttu-id="1ed5d-308">いいえ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-308">No</span></span>       |   |
| <span data-ttu-id="1ed5d-309">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-309">schedule</span></span>         | [<span data-ttu-id="1ed5d-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-311">いいえ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-312">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-313">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="1ed5d-314">例 4: 管理者ユーザー ロールから削除します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="1ed5d-315">この例では、管理者は、課金情報の閲覧者の役割からユーザー nawu@fimdev.net を削除します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="1ed5d-316">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="1ed5d-317">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-317">Property</span></span>         | <span data-ttu-id="1ed5d-318">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-318">Type</span></span>                                                     | <span data-ttu-id="1ed5d-319">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-319">Required</span></span> | <span data-ttu-id="1ed5d-320">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="1ed5d-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-321">resourceId</span></span>       | <span data-ttu-id="1ed5d-322">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-322">String</span></span>                                                   | <span data-ttu-id="1ed5d-323">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-323">Yes</span></span>      | <span data-ttu-id="1ed5d-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-324">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-325">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-326">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-326">String</span></span>                                                   | <span data-ttu-id="1ed5d-327">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-327">Yes</span></span>      | <span data-ttu-id="1ed5d-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-329">subjectId</span></span>        | <span data-ttu-id="1ed5d-330">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-330">String</span></span>                                                   | <span data-ttu-id="1ed5d-331">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-331">Yes</span></span>      | <span data-ttu-id="1ed5d-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-332">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-333">assignmentState</span></span>  | <span data-ttu-id="1ed5d-334">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-334">String</span></span>                                                   | <span data-ttu-id="1ed5d-335">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-335">Yes</span></span>      | <span data-ttu-id="1ed5d-336">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-336">Eligible / Active</span></span> |
| <span data-ttu-id="1ed5d-337">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-337">type</span></span>             | <span data-ttu-id="1ed5d-338">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-338">String</span></span>                                                   | <span data-ttu-id="1ed5d-339">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-339">Yes</span></span>      | <span data-ttu-id="1ed5d-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="1ed5d-340">AdminRemove</span></span> |
| <span data-ttu-id="1ed5d-341">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-341">reason</span></span>           | <span data-ttu-id="1ed5d-342">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-342">String</span></span>                                                   | <span data-ttu-id="1ed5d-343">いいえ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-343">No</span></span>       |   |
| <span data-ttu-id="1ed5d-344">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-344">schedule</span></span>         | [<span data-ttu-id="1ed5d-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-346">いいえ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-347">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-348">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="1ed5d-349">例 5: 管理者が役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="1ed5d-350">この例では、管理者は、所有者をユーザー nawu@fimdev.net の役割の割り当てを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="1ed5d-351">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="1ed5d-352">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-352">Property</span></span>         | <span data-ttu-id="1ed5d-353">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-353">Type</span></span>                                                     | <span data-ttu-id="1ed5d-354">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-354">Required</span></span>                | <span data-ttu-id="1ed5d-355">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="1ed5d-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-356">resourceId</span></span>       | <span data-ttu-id="1ed5d-357">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-357">String</span></span>                                                   | <span data-ttu-id="1ed5d-358">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-358">Yes</span></span>                     | <span data-ttu-id="1ed5d-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-359">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-360">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-361">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-361">String</span></span>                                                   | <span data-ttu-id="1ed5d-362">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-362">Yes</span></span>                     | <span data-ttu-id="1ed5d-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-364">subjectId</span></span>        | <span data-ttu-id="1ed5d-365">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-365">String</span></span>                                                   | <span data-ttu-id="1ed5d-366">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-366">Yes</span></span>                     | <span data-ttu-id="1ed5d-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-367">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-368">assignmentState</span></span>  | <span data-ttu-id="1ed5d-369">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-369">String</span></span>                                                   | <span data-ttu-id="1ed5d-370">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-370">Yes</span></span>                     | <span data-ttu-id="1ed5d-371">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-371">Eligible / Active</span></span> |
| <span data-ttu-id="1ed5d-372">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-372">type</span></span>             | <span data-ttu-id="1ed5d-373">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-373">String</span></span>                                                   | <span data-ttu-id="1ed5d-374">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-374">Yes</span></span>                     | <span data-ttu-id="1ed5d-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="1ed5d-375">AdminUpdate</span></span> |
| <span data-ttu-id="1ed5d-376">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-376">reason</span></span>           | <span data-ttu-id="1ed5d-377">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-377">String</span></span>                                                   | <span data-ttu-id="1ed5d-378">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="1ed5d-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="1ed5d-379">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-379">schedule</span></span>         | [<span data-ttu-id="1ed5d-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-381">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-382">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-383">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="1ed5d-384">例 6: 管理者は、期限切れのロールの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="1ed5d-385">次の使用例は、API の管理サービスの共同作成者に ANUJCUSER のユーザーの有効期限切れのロールの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="1ed5d-386">**注:** だけでなく、アクセス許可が、次の使用例が必要です、依頼者の少なくとも 1 つ`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="1ed5d-387">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-387">Property</span></span>         | <span data-ttu-id="1ed5d-388">型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-388">Type</span></span>                                                     | <span data-ttu-id="1ed5d-389">必須</span><span class="sxs-lookup"><span data-stu-id="1ed5d-389">Required</span></span>                | <span data-ttu-id="1ed5d-390">値</span><span class="sxs-lookup"><span data-stu-id="1ed5d-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="1ed5d-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-391">resourceId</span></span>       | <span data-ttu-id="1ed5d-392">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-392">String</span></span>                                                   | <span data-ttu-id="1ed5d-393">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-393">Yes</span></span>                     | <span data-ttu-id="1ed5d-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-394">\<resourceId\></span></span> |
| <span data-ttu-id="1ed5d-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-395">roleDefinitionId</span></span> | <span data-ttu-id="1ed5d-396">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-396">String</span></span>                                                   | <span data-ttu-id="1ed5d-397">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-397">Yes</span></span>                     | <span data-ttu-id="1ed5d-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="1ed5d-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="1ed5d-399">subjectId</span></span>        | <span data-ttu-id="1ed5d-400">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-400">String</span></span>                                                   | <span data-ttu-id="1ed5d-401">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-401">Yes</span></span>                     | <span data-ttu-id="1ed5d-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="1ed5d-402">\<subjectId\></span></span> |
| <span data-ttu-id="1ed5d-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="1ed5d-403">assignmentState</span></span>  | <span data-ttu-id="1ed5d-404">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-404">String</span></span>                                                   | <span data-ttu-id="1ed5d-405">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-405">Yes</span></span>                     | <span data-ttu-id="1ed5d-406">対象となる/アクティブ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-406">Eligible / Active</span></span> |
| <span data-ttu-id="1ed5d-407">type</span><span class="sxs-lookup"><span data-stu-id="1ed5d-407">type</span></span>             | <span data-ttu-id="1ed5d-408">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-408">String</span></span>                                                   | <span data-ttu-id="1ed5d-409">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-409">Yes</span></span>                     | <span data-ttu-id="1ed5d-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="1ed5d-410">AdminExtend</span></span> |
| <span data-ttu-id="1ed5d-411">理由</span><span class="sxs-lookup"><span data-stu-id="1ed5d-411">reason</span></span>           | <span data-ttu-id="1ed5d-412">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-412">String</span></span>                                                   | <span data-ttu-id="1ed5d-413">roleSettings によって異なります</span><span class="sxs-lookup"><span data-stu-id="1ed5d-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="1ed5d-414">スケジュール</span><span class="sxs-lookup"><span data-stu-id="1ed5d-414">schedule</span></span>         | [<span data-ttu-id="1ed5d-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1ed5d-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="1ed5d-416">はい</span><span class="sxs-lookup"><span data-stu-id="1ed5d-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="1ed5d-417">要求</span><span class="sxs-lookup"><span data-stu-id="1ed5d-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1ed5d-418">応答</span><span class="sxs-lookup"><span data-stu-id="1ed5d-418">Response</span></span>

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
