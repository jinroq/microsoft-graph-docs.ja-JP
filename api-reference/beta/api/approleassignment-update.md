---
title: Approleassignment を更新します。
description: Approleassignment オブジェクトのプロパティを更新します。
ms.openlocfilehash: 3c861afde396d9cab2f745c15c7de1d9a81c5dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067044"
---
# <a name="update-approleassignment"></a><span data-ttu-id="3af33-103">Approleassignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="3af33-103">Update approleassignment</span></span>

> <span data-ttu-id="3af33-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3af33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3af33-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3af33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3af33-106">Approleassignment オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3af33-106">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3af33-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3af33-107">Permissions</span></span>
<span data-ttu-id="3af33-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3af33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af33-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3af33-110">Permission type</span></span>      | <span data-ttu-id="3af33-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3af33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3af33-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3af33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3af33-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3af33-113">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="3af33-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3af33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3af33-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3af33-115">Not supported.</span></span>    |
|<span data-ttu-id="3af33-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3af33-116">Application</span></span> | <span data-ttu-id="3af33-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3af33-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3af33-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3af33-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3af33-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3af33-119">Request headers</span></span>
| <span data-ttu-id="3af33-120">名前</span><span class="sxs-lookup"><span data-stu-id="3af33-120">Name</span></span>       | <span data-ttu-id="3af33-121">型</span><span class="sxs-lookup"><span data-stu-id="3af33-121">Type</span></span> | <span data-ttu-id="3af33-122">説明</span><span class="sxs-lookup"><span data-stu-id="3af33-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3af33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3af33-123">Authorization</span></span>  | <span data-ttu-id="3af33-124">string</span><span class="sxs-lookup"><span data-stu-id="3af33-124">string</span></span>  | <span data-ttu-id="3af33-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3af33-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3af33-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3af33-127">Request body</span></span>
<span data-ttu-id="3af33-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3af33-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3af33-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af33-131">Property</span></span>     | <span data-ttu-id="3af33-132">型</span><span class="sxs-lookup"><span data-stu-id="3af33-132">Type</span></span>   |<span data-ttu-id="3af33-133">説明</span><span class="sxs-lookup"><span data-stu-id="3af33-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3af33-134">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="3af33-134">creationTimestamp</span></span>|<span data-ttu-id="3af33-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3af33-135">DateTimeOffset</span></span>|<span data-ttu-id="3af33-136">交付が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="3af33-136">The time when the grant was created.</span></span>|
|<span data-ttu-id="3af33-137">ID</span><span class="sxs-lookup"><span data-stu-id="3af33-137">id</span></span>|<span data-ttu-id="3af33-138">Guid</span><span class="sxs-lookup"><span data-stu-id="3af33-138">Guid</span></span>|<span data-ttu-id="3af33-139">プリンシパルに割り当てられたロールの id です。</span><span class="sxs-lookup"><span data-stu-id="3af33-139">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="3af33-140">この役割は、 **appRoles**プロパティにターゲットのリソース アプリケーション**引数 resourceId**で宣言されなければなりません。</span><span class="sxs-lookup"><span data-stu-id="3af33-140">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="3af33-141">リソースですべてのアクセス許可が宣言されていない場合は、デフォルトの id (GUID は 0) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="3af33-141">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="3af33-142">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="3af33-142">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="3af33-143">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="3af33-143">principalDisplayName</span></span>|<span data-ttu-id="3af33-144">String</span><span class="sxs-lookup"><span data-stu-id="3af33-144">String</span></span>|<span data-ttu-id="3af33-145">アクセス権を与えられたプリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="3af33-145">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="3af33-146">principalId</span><span class="sxs-lookup"><span data-stu-id="3af33-146">principalId</span></span>|<span data-ttu-id="3af33-147">Guid</span><span class="sxs-lookup"><span data-stu-id="3af33-147">Guid</span></span>|<span data-ttu-id="3af33-148">アクセスを付与されているプリンシパルの一意の識別子 (**オブジェクト Id**) です。</span><span class="sxs-lookup"><span data-stu-id="3af33-148">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="3af33-149">**メモ**: 必要です。</span><span class="sxs-lookup"><span data-stu-id="3af33-149">**Notes**: required.</span></span>            |
|<span data-ttu-id="3af33-150">principalType</span><span class="sxs-lookup"><span data-stu-id="3af33-150">principalType</span></span>|<span data-ttu-id="3af33-151">String</span><span class="sxs-lookup"><span data-stu-id="3af33-151">String</span></span>|<span data-ttu-id="3af33-152">プリンシパルの種類。</span><span class="sxs-lookup"><span data-stu-id="3af33-152">The type of principal.</span></span>  <span data-ttu-id="3af33-153">「ユーザー」、「グループ」または"ServicePrincipal"指定できます。</span><span class="sxs-lookup"><span data-stu-id="3af33-153">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="3af33-154">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3af33-154">resourceDisplayName</span></span>|<span data-ttu-id="3af33-155">String</span><span class="sxs-lookup"><span data-stu-id="3af33-155">String</span></span>|<span data-ttu-id="3af33-156">割り当てが作成するリソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="3af33-156">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="3af33-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="3af33-157">resourceId</span></span>|<span data-ttu-id="3af33-158">Guid</span><span class="sxs-lookup"><span data-stu-id="3af33-158">Guid</span></span>|<span data-ttu-id="3af33-159">割り当てが作成する対象のリソース (サービス主体) の一意の識別子 (**オブジェクト Id**) です。</span><span class="sxs-lookup"><span data-stu-id="3af33-159">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="3af33-160">応答</span><span class="sxs-lookup"><span data-stu-id="3af33-160">Response</span></span>

<span data-ttu-id="3af33-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[appRoleAssignment](../resources/approleassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3af33-161">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3af33-162">例</span><span class="sxs-lookup"><span data-stu-id="3af33-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3af33-163">要求</span><span class="sxs-lookup"><span data-stu-id="3af33-163">Request</span></span>
<span data-ttu-id="3af33-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3af33-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3af33-165">応答</span><span class="sxs-lookup"><span data-stu-id="3af33-165">Response</span></span>
<span data-ttu-id="3af33-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3af33-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->