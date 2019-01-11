---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アクセス許可を変更する
localization_priority: Normal
ms.openlocfilehash: 44f98d559ab6dc4c81a4efede2f3f60020c2f944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859683"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="eb0c6-102">共有アクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="eb0c6-102">Update sharing permission</span></span>

> <span data-ttu-id="eb0c6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb0c6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb0c6-105">共有アクセス許可のプロパティを更新するには、アクセス許可リソースのパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="eb0c6-106">**roles** プロパティのみ、この方法で変更可能です。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb0c6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb0c6-107">Permissions</span></span>

<span data-ttu-id="eb0c6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb0c6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb0c6-110">Permission type</span></span>      | <span data-ttu-id="eb0c6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb0c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb0c6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb0c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb0c6-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0c6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb0c6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb0c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb0c6-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0c6-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb0c6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb0c6-116">Application</span></span> | <span data-ttu-id="eb0c6-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0c6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb0c6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb0c6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="eb0c6-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb0c6-119">Optional request headers</span></span>

| <span data-ttu-id="eb0c6-120">名前</span><span class="sxs-lookup"><span data-stu-id="eb0c6-120">Name</span></span>          | <span data-ttu-id="eb0c6-121">種類</span><span class="sxs-lookup"><span data-stu-id="eb0c6-121">Type</span></span>   | <span data-ttu-id="eb0c6-122">説明</span><span class="sxs-lookup"><span data-stu-id="eb0c6-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="eb0c6-123">if-match</span><span class="sxs-lookup"><span data-stu-id="eb0c6-123">if-match</span></span>      | <span data-ttu-id="eb0c6-124">文字列</span><span class="sxs-lookup"><span data-stu-id="eb0c6-124">string</span></span> | <span data-ttu-id="eb0c6-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb0c6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb0c6-126">Request body</span></span>

<span data-ttu-id="eb0c6-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="eb0c6-128">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="eb0c6-129">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eb0c6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb0c6-130">Property</span></span>     | <span data-ttu-id="eb0c6-131">種類</span><span class="sxs-lookup"><span data-stu-id="eb0c6-131">Type</span></span>   | <span data-ttu-id="eb0c6-132">説明</span><span class="sxs-lookup"><span data-stu-id="eb0c6-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="eb0c6-133">**roles**</span><span class="sxs-lookup"><span data-stu-id="eb0c6-133">**roles**</span></span>    | <span data-ttu-id="eb0c6-134">String</span><span class="sxs-lookup"><span data-stu-id="eb0c6-134">String</span></span> | <span data-ttu-id="eb0c6-135">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="eb0c6-136">応答</span><span class="sxs-lookup"><span data-stu-id="eb0c6-136">Response</span></span>

<span data-ttu-id="eb0c6-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb0c6-138">例</span><span class="sxs-lookup"><span data-stu-id="eb0c6-138">Example</span></span>

<span data-ttu-id="eb0c6-139">以下は、共有アクセス許可のロールを読み取り専用に変更する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="eb0c6-140">応答</span><span class="sxs-lookup"><span data-stu-id="eb0c6-140">Response</span></span>

<span data-ttu-id="eb0c6-141">成功した場合、このメソッドは、応答本文でアクセス許可の更新された状態を表す [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="eb0c6-141">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
