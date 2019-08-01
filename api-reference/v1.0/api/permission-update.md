---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アクセス許可の変更
localization_priority: Normal
description: 共有アクセス許可のプロパティを更新するには、アクセス許可リソースのパッチを適用します。
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a4c679c117630a78092e0d99a9e2aab2e8785ffd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022538"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="a935d-103">共有アクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="a935d-103">Update sharing permission</span></span>

<span data-ttu-id="a935d-104">共有アクセス許可のプロパティを更新するには、アクセス許可リソースのパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="a935d-104">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="a935d-105">**roles** プロパティのみ、この方法で変更可能です。</span><span class="sxs-lookup"><span data-stu-id="a935d-105">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="a935d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a935d-106">Permissions</span></span>

<span data-ttu-id="a935d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a935d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a935d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a935d-109">Permission type</span></span>      | <span data-ttu-id="a935d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a935d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a935d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a935d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a935d-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a935d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a935d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a935d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a935d-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a935d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a935d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a935d-115">Application</span></span> | <span data-ttu-id="a935d-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a935d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a935d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a935d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a935d-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a935d-118">Optional request headers</span></span>

| <span data-ttu-id="a935d-119">名前</span><span class="sxs-lookup"><span data-stu-id="a935d-119">Name</span></span>          | <span data-ttu-id="a935d-120">型</span><span class="sxs-lookup"><span data-stu-id="a935d-120">Type</span></span>   | <span data-ttu-id="a935d-121">説明</span><span class="sxs-lookup"><span data-stu-id="a935d-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a935d-122">if-match</span><span class="sxs-lookup"><span data-stu-id="a935d-122">if-match</span></span>      | <span data-ttu-id="a935d-123">string</span><span class="sxs-lookup"><span data-stu-id="a935d-123">string</span></span> | <span data-ttu-id="a935d-124">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="a935d-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a935d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a935d-125">Request body</span></span>

<span data-ttu-id="a935d-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a935d-126">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="a935d-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="a935d-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="a935d-128">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a935d-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a935d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a935d-129">Property</span></span> | <span data-ttu-id="a935d-130">型</span><span class="sxs-lookup"><span data-stu-id="a935d-130">Type</span></span>              | <span data-ttu-id="a935d-131">説明</span><span class="sxs-lookup"><span data-stu-id="a935d-131">Description</span></span>                   |
|:---------|:------------------|:------------------------------|
| <span data-ttu-id="a935d-132">roles</span><span class="sxs-lookup"><span data-stu-id="a935d-132">roles</span></span>    | <span data-ttu-id="a935d-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a935d-133">String collection</span></span> | <span data-ttu-id="a935d-134">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="a935d-134">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="a935d-135">応答</span><span class="sxs-lookup"><span data-stu-id="a935d-135">Response</span></span>

<span data-ttu-id="a935d-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a935d-136">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a935d-137">例</span><span class="sxs-lookup"><span data-stu-id="a935d-137">Example</span></span>

<span data-ttu-id="a935d-138">以下は、共有アクセス許可のロールを読み取り専用に変更する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a935d-138">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a935d-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a935d-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a935d-140">C#</span><span class="sxs-lookup"><span data-stu-id="a935d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a935d-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="a935d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a935d-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="a935d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a935d-143">Java</span><span class="sxs-lookup"><span data-stu-id="a935d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a935d-144">応答</span><span class="sxs-lookup"><span data-stu-id="a935d-144">Response</span></span>

<span data-ttu-id="a935d-145">成功した場合、このメソッドは、応答本文でアクセス許可の更新された状態を表す [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="a935d-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

## <a name="error-responses"></a><span data-ttu-id="a935d-146">エラー応答</span><span class="sxs-lookup"><span data-stu-id="a935d-146">Error responses</span></span>

<span data-ttu-id="a935d-147">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a935d-147">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission",
  "suppressions": [
  ]
} -->
