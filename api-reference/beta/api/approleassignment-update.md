---
title: Approleassignment を更新します。
description: Approleassignment オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 89147651b1a3ea182247cf3620efba9464c4b055
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572914"
---
# <a name="update-approleassignment"></a><span data-ttu-id="94f81-103">Approleassignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="94f81-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94f81-104">Approleassignment オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94f81-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94f81-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94f81-105">Permissions</span></span>
<span data-ttu-id="94f81-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f81-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94f81-108">Permission type</span></span>      | <span data-ttu-id="94f81-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94f81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94f81-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94f81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94f81-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94f81-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="94f81-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94f81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94f81-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f81-113">Not supported.</span></span>    |
|<span data-ttu-id="94f81-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94f81-114">Application</span></span> | <span data-ttu-id="94f81-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f81-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94f81-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94f81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94f81-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94f81-117">Request headers</span></span>
| <span data-ttu-id="94f81-118">名前</span><span class="sxs-lookup"><span data-stu-id="94f81-118">Name</span></span>       | <span data-ttu-id="94f81-119">型</span><span class="sxs-lookup"><span data-stu-id="94f81-119">Type</span></span> | <span data-ttu-id="94f81-120">説明</span><span class="sxs-lookup"><span data-stu-id="94f81-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94f81-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f81-121">Authorization</span></span>  | <span data-ttu-id="94f81-122">string</span><span class="sxs-lookup"><span data-stu-id="94f81-122">string</span></span>  | <span data-ttu-id="94f81-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94f81-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94f81-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="94f81-125">Request body</span></span>
<span data-ttu-id="94f81-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="94f81-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94f81-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94f81-129">Property</span></span>     | <span data-ttu-id="94f81-130">型</span><span class="sxs-lookup"><span data-stu-id="94f81-130">Type</span></span>   |<span data-ttu-id="94f81-131">説明</span><span class="sxs-lookup"><span data-stu-id="94f81-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94f81-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="94f81-132">creationTimestamp</span></span>|<span data-ttu-id="94f81-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94f81-133">DateTimeOffset</span></span>|<span data-ttu-id="94f81-134">交付が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="94f81-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="94f81-135">ID</span><span class="sxs-lookup"><span data-stu-id="94f81-135">id</span></span>|<span data-ttu-id="94f81-136">Guid</span><span class="sxs-lookup"><span data-stu-id="94f81-136">Guid</span></span>|<span data-ttu-id="94f81-137">プリンシパルに割り当てられたロールの id です。</span><span class="sxs-lookup"><span data-stu-id="94f81-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="94f81-138">この役割は、 **appRoles**プロパティにターゲットのリソース アプリケーション**引数 resourceId**で宣言されなければなりません。</span><span class="sxs-lookup"><span data-stu-id="94f81-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="94f81-139">リソースですべてのアクセス許可が宣言されていない場合は、デフォルトの id (GUID は 0) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="94f81-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="94f81-140">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="94f81-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="94f81-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="94f81-141">principalDisplayName</span></span>|<span data-ttu-id="94f81-142">String</span><span class="sxs-lookup"><span data-stu-id="94f81-142">String</span></span>|<span data-ttu-id="94f81-143">アクセス権を与えられたプリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="94f81-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="94f81-144">principalId</span><span class="sxs-lookup"><span data-stu-id="94f81-144">principalId</span></span>|<span data-ttu-id="94f81-145">Guid</span><span class="sxs-lookup"><span data-stu-id="94f81-145">Guid</span></span>|<span data-ttu-id="94f81-146">アクセスを付与されているプリンシパルの一意の識別子 (**オブジェクト Id**) です。</span><span class="sxs-lookup"><span data-stu-id="94f81-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="94f81-147">**メモ**: 必要です。</span><span class="sxs-lookup"><span data-stu-id="94f81-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="94f81-148">principalType</span><span class="sxs-lookup"><span data-stu-id="94f81-148">principalType</span></span>|<span data-ttu-id="94f81-149">String</span><span class="sxs-lookup"><span data-stu-id="94f81-149">String</span></span>|<span data-ttu-id="94f81-150">プリンシパルの種類。</span><span class="sxs-lookup"><span data-stu-id="94f81-150">The type of principal.</span></span>  <span data-ttu-id="94f81-151">「ユーザー」、「グループ」または"ServicePrincipal"指定できます。</span><span class="sxs-lookup"><span data-stu-id="94f81-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="94f81-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="94f81-152">resourceDisplayName</span></span>|<span data-ttu-id="94f81-153">String</span><span class="sxs-lookup"><span data-stu-id="94f81-153">String</span></span>|<span data-ttu-id="94f81-154">割り当てが作成するリソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="94f81-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="94f81-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="94f81-155">resourceId</span></span>|<span data-ttu-id="94f81-156">Guid</span><span class="sxs-lookup"><span data-stu-id="94f81-156">Guid</span></span>|<span data-ttu-id="94f81-157">割り当てが作成する対象のリソース (サービス主体) の一意の識別子 (**オブジェクト Id**) です。</span><span class="sxs-lookup"><span data-stu-id="94f81-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="94f81-158">応答</span><span class="sxs-lookup"><span data-stu-id="94f81-158">Response</span></span>

<span data-ttu-id="94f81-159">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[appRoleAssignment](../resources/approleassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="94f81-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94f81-160">例</span><span class="sxs-lookup"><span data-stu-id="94f81-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94f81-161">要求</span><span class="sxs-lookup"><span data-stu-id="94f81-161">Request</span></span>
<span data-ttu-id="94f81-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94f81-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{id}
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="94f81-163">応答</span><span class="sxs-lookup"><span data-stu-id="94f81-163">Response</span></span>
<span data-ttu-id="94f81-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94f81-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
