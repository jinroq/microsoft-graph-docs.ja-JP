---
title: approleassignment を更新する
description: Approleassignment オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 50b9e1add1a873226d61ea3795ecbac917a14b0a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318538"
---
# <a name="update-approleassignment"></a><span data-ttu-id="31b06-103">approleassignment を更新する</span><span class="sxs-lookup"><span data-stu-id="31b06-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b06-104">Approleassignment オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31b06-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="31b06-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="31b06-105">Permissions</span></span>
<span data-ttu-id="31b06-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31b06-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31b06-108">Permission type</span></span>      | <span data-ttu-id="31b06-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="31b06-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31b06-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31b06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31b06-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31b06-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="31b06-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31b06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b06-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31b06-113">Not supported.</span></span>    |
|<span data-ttu-id="31b06-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31b06-114">Application</span></span> | <span data-ttu-id="31b06-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31b06-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31b06-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31b06-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="31b06-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31b06-117">Request headers</span></span>
| <span data-ttu-id="31b06-118">名前</span><span class="sxs-lookup"><span data-stu-id="31b06-118">Name</span></span>       | <span data-ttu-id="31b06-119">型</span><span class="sxs-lookup"><span data-stu-id="31b06-119">Type</span></span> | <span data-ttu-id="31b06-120">説明</span><span class="sxs-lookup"><span data-stu-id="31b06-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="31b06-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31b06-121">Authorization</span></span>  | <span data-ttu-id="31b06-122">string</span><span class="sxs-lookup"><span data-stu-id="31b06-122">string</span></span>  | <span data-ttu-id="31b06-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="31b06-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31b06-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="31b06-125">Request body</span></span>
<span data-ttu-id="31b06-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="31b06-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="31b06-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31b06-129">Property</span></span>     | <span data-ttu-id="31b06-130">型</span><span class="sxs-lookup"><span data-stu-id="31b06-130">Type</span></span>   |<span data-ttu-id="31b06-131">説明</span><span class="sxs-lookup"><span data-stu-id="31b06-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31b06-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="31b06-132">creationTimestamp</span></span>|<span data-ttu-id="31b06-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31b06-133">DateTimeOffset</span></span>|<span data-ttu-id="31b06-134">許可が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="31b06-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="31b06-135">id</span><span class="sxs-lookup"><span data-stu-id="31b06-135">id</span></span>|<span data-ttu-id="31b06-136">Guid</span><span class="sxs-lookup"><span data-stu-id="31b06-136">Guid</span></span>|<span data-ttu-id="31b06-137">プリンシパルに割り当てられたロール ID です。</span><span class="sxs-lookup"><span data-stu-id="31b06-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="31b06-138">このロールは、**appRoles** プロパティのターゲット リソース アプリケーション **resourceId** によって宣言される必要があります。</span><span class="sxs-lookup"><span data-stu-id="31b06-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="31b06-139">リソースがアクセス許可を宣言していない場合は、既存の ID (ゼロ GUID) を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="31b06-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="31b06-140">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="31b06-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="31b06-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="31b06-141">principalDisplayName</span></span>|<span data-ttu-id="31b06-142">String</span><span class="sxs-lookup"><span data-stu-id="31b06-142">String</span></span>|<span data-ttu-id="31b06-143">アクセス権が付与されているプリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="31b06-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="31b06-144">principalId</span><span class="sxs-lookup"><span data-stu-id="31b06-144">principalId</span></span>|<span data-ttu-id="31b06-145">Guid</span><span class="sxs-lookup"><span data-stu-id="31b06-145">Guid</span></span>|<span data-ttu-id="31b06-146">アクセスが許可されているプリンシパルの一意識別子 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="31b06-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="31b06-147">**メモ**: 必須。</span><span class="sxs-lookup"><span data-stu-id="31b06-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="31b06-148">principalType</span><span class="sxs-lookup"><span data-stu-id="31b06-148">principalType</span></span>|<span data-ttu-id="31b06-149">String</span><span class="sxs-lookup"><span data-stu-id="31b06-149">String</span></span>|<span data-ttu-id="31b06-150">プリンシパルの種類。</span><span class="sxs-lookup"><span data-stu-id="31b06-150">The type of principal.</span></span>  <span data-ttu-id="31b06-151">"User"、"Group"、"ServicePrincipal" のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="31b06-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="31b06-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="31b06-152">resourceDisplayName</span></span>|<span data-ttu-id="31b06-153">String</span><span class="sxs-lookup"><span data-stu-id="31b06-153">String</span></span>|<span data-ttu-id="31b06-154">割り当てが作成されたリソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="31b06-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="31b06-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="31b06-155">resourceId</span></span>|<span data-ttu-id="31b06-156">Guid</span><span class="sxs-lookup"><span data-stu-id="31b06-156">Guid</span></span>|<span data-ttu-id="31b06-157">割り当てが行われたターゲットリソース (サービスプリンシパル) の一意識別子 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="31b06-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="31b06-158">応答</span><span class="sxs-lookup"><span data-stu-id="31b06-158">Response</span></span>

<span data-ttu-id="31b06-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[approleassignment](../resources/approleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31b06-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31b06-160">例</span><span class="sxs-lookup"><span data-stu-id="31b06-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31b06-161">要求</span><span class="sxs-lookup"><span data-stu-id="31b06-161">Request</span></span>
<span data-ttu-id="31b06-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31b06-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31b06-163">プロトコル</span><span class="sxs-lookup"><span data-stu-id="31b06-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="31b06-164">C#</span><span class="sxs-lookup"><span data-stu-id="31b06-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31b06-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31b06-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31b06-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="31b06-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="31b06-167">Java</span><span class="sxs-lookup"><span data-stu-id="31b06-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31b06-168">応答</span><span class="sxs-lookup"><span data-stu-id="31b06-168">Response</span></span>
<span data-ttu-id="31b06-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31b06-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
