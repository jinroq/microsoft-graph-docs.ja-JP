---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "アクセス許可を変更する"
ms.openlocfilehash: ead6babf88b7efc578ef8be6d11cc9fb59dd5fdd
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="update-sharing-permission"></a><span data-ttu-id="b56f2-102">共有アクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="b56f2-102">Update sharing permission</span></span>

<span data-ttu-id="b56f2-103">共有アクセス許可のプロパティを更新するには、アクセス許可リソースのパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="b56f2-103">Update the properties of a permission by patching the resource.</span></span>

<span data-ttu-id="b56f2-104">**roles** プロパティのみ、この方法で変更可能です。</span><span class="sxs-lookup"><span data-stu-id="b56f2-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="b56f2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b56f2-105">Permissions</span></span>

<span data-ttu-id="b56f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b56f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b56f2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b56f2-108">Permission type</span></span>      | <span data-ttu-id="b56f2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b56f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b56f2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b56f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b56f2-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b56f2-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b56f2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b56f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b56f2-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b56f2-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b56f2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b56f2-114">Application</span></span> | <span data-ttu-id="b56f2-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b56f2-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b56f2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b56f2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b56f2-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b56f2-117">Optional request headers</span></span>

| <span data-ttu-id="b56f2-118">名前</span><span class="sxs-lookup"><span data-stu-id="b56f2-118">Name</span></span>          | <span data-ttu-id="b56f2-119">型</span><span class="sxs-lookup"><span data-stu-id="b56f2-119">Type</span></span>   | <span data-ttu-id="b56f2-120">説明</span><span class="sxs-lookup"><span data-stu-id="b56f2-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b56f2-121">if-match</span><span class="sxs-lookup"><span data-stu-id="b56f2-121">if-match</span></span>      | <span data-ttu-id="b56f2-122">string</span><span class="sxs-lookup"><span data-stu-id="b56f2-122">string</span></span> | <span data-ttu-id="b56f2-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="b56f2-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b56f2-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b56f2-124">Request body</span></span>

<span data-ttu-id="b56f2-125">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b56f2-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="b56f2-126">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="b56f2-126">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
<span data-ttu-id="b56f2-127">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b56f2-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b56f2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b56f2-128">Property</span></span>     | <span data-ttu-id="b56f2-129">型</span><span class="sxs-lookup"><span data-stu-id="b56f2-129">Type</span></span>   | <span data-ttu-id="b56f2-130">説明</span><span class="sxs-lookup"><span data-stu-id="b56f2-130">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="b56f2-131">**roles**</span><span class="sxs-lookup"><span data-stu-id="b56f2-131">**roles**</span></span>    | <span data-ttu-id="b56f2-132">String</span><span class="sxs-lookup"><span data-stu-id="b56f2-132">String</span></span> | <span data-ttu-id="b56f2-133">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="b56f2-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="b56f2-134">応答</span><span class="sxs-lookup"><span data-stu-id="b56f2-134">Response</span></span>

<span data-ttu-id="b56f2-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b56f2-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b56f2-136">例</span><span class="sxs-lookup"><span data-stu-id="b56f2-136">Example</span></span>

<span data-ttu-id="b56f2-137">以下は、共有アクセス許可のロールを読み取り専用に変更する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b56f2-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="b56f2-138">応答</span><span class="sxs-lookup"><span data-stu-id="b56f2-138">Response</span></span>

<span data-ttu-id="b56f2-139">成功した場合、このメソッドは、応答本文で更新されたアクセス許可の状態を表す [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="b56f2-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="b56f2-140">エラー応答</span><span class="sxs-lookup"><span data-stu-id="b56f2-140">Error responses</span></span>

<span data-ttu-id="b56f2-141">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b56f2-141">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
