---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アクセス許可の変更
localization_priority: Normal
ms.openlocfilehash: f2bc5954380836af12382ec02f4d04f9fa4c29c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876994"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="23863-102">共有アクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="23863-102">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23863-103">共有アクセス許可のプロパティを更新するには、アクセス許可リソースのパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="23863-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="23863-104">**roles** プロパティのみ、この方法で変更可能です。</span><span class="sxs-lookup"><span data-stu-id="23863-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="23863-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="23863-105">Permissions</span></span>

<span data-ttu-id="23863-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23863-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23863-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23863-108">Permission type</span></span>      | <span data-ttu-id="23863-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="23863-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23863-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23863-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23863-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23863-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="23863-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23863-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23863-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23863-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="23863-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23863-114">Application</span></span> | <span data-ttu-id="23863-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23863-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23863-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23863-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="23863-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23863-117">Optional request headers</span></span>

| <span data-ttu-id="23863-118">名前</span><span class="sxs-lookup"><span data-stu-id="23863-118">Name</span></span>          | <span data-ttu-id="23863-119">型</span><span class="sxs-lookup"><span data-stu-id="23863-119">Type</span></span>   | <span data-ttu-id="23863-120">説明</span><span class="sxs-lookup"><span data-stu-id="23863-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="23863-121">if-match</span><span class="sxs-lookup"><span data-stu-id="23863-121">if-match</span></span>      | <span data-ttu-id="23863-122">string</span><span class="sxs-lookup"><span data-stu-id="23863-122">string</span></span> | <span data-ttu-id="23863-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="23863-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23863-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="23863-124">Request body</span></span>

<span data-ttu-id="23863-125">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="23863-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="23863-126">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="23863-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="23863-127">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="23863-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="23863-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23863-128">Property</span></span>     | <span data-ttu-id="23863-129">型</span><span class="sxs-lookup"><span data-stu-id="23863-129">Type</span></span>   | <span data-ttu-id="23863-130">説明</span><span class="sxs-lookup"><span data-stu-id="23863-130">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="23863-131">**roles**</span><span class="sxs-lookup"><span data-stu-id="23863-131">**roles**</span></span>    | <span data-ttu-id="23863-132">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="23863-132">String collection</span></span> | <span data-ttu-id="23863-133">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="23863-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="23863-134">応答</span><span class="sxs-lookup"><span data-stu-id="23863-134">Response</span></span>

<span data-ttu-id="23863-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23863-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23863-136">例</span><span class="sxs-lookup"><span data-stu-id="23863-136">Example</span></span>

<span data-ttu-id="23863-137">以下は、共有アクセス許可のロールを読み取り専用に変更する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23863-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23863-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="23863-138">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23863-139">C#</span><span class="sxs-lookup"><span data-stu-id="23863-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23863-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="23863-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23863-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="23863-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23863-142">Java</span><span class="sxs-lookup"><span data-stu-id="23863-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23863-143">応答</span><span class="sxs-lookup"><span data-stu-id="23863-143">Response</span></span>

<span data-ttu-id="23863-144">成功した場合、このメソッドは、応答本文でアクセス許可の更新された状態を表す [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="23863-144">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission",
  "suppressions": [
  ]
}
-->
