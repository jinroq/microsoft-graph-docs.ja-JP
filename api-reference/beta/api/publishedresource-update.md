---
title: PublishedResource の更新
description: '[Publishedresource](../resources/publishedresource.md)オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8876dc513a196f24dd2c5a695c0158720e87522b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309214"
---
# <a name="update-publishedresource"></a><span data-ttu-id="4027c-103">PublishedResource の更新</span><span class="sxs-lookup"><span data-stu-id="4027c-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4027c-104">Publishedresource [Publishedresource](../resources/publishedresource.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4027c-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4027c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4027c-105">Permissions</span></span>

<span data-ttu-id="4027c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4027c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4027c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4027c-108">Permission type</span></span>                        | <span data-ttu-id="4027c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4027c-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="4027c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4027c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4027c-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="4027c-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="4027c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4027c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4027c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4027c-113">Not supported.</span></span> |
| <span data-ttu-id="4027c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4027c-114">Application</span></span>                            | <span data-ttu-id="4027c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4027c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4027c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4027c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="4027c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4027c-117">Request headers</span></span>

| <span data-ttu-id="4027c-118">名前</span><span class="sxs-lookup"><span data-stu-id="4027c-118">Name</span></span>       | <span data-ttu-id="4027c-119">説明</span><span class="sxs-lookup"><span data-stu-id="4027c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4027c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4027c-120">Authorization</span></span> | <span data-ttu-id="4027c-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="4027c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4027c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="4027c-122">Request body</span></span>

<span data-ttu-id="4027c-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4027c-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="4027c-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="4027c-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4027c-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4027c-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4027c-126">次の表に、更新できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4027c-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="4027c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4027c-127">Property</span></span>     | <span data-ttu-id="4027c-128">型</span><span class="sxs-lookup"><span data-stu-id="4027c-128">Type</span></span>        | <span data-ttu-id="4027c-129">説明</span><span class="sxs-lookup"><span data-stu-id="4027c-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4027c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4027c-130">displayName</span></span>|<span data-ttu-id="4027c-131">String</span><span class="sxs-lookup"><span data-stu-id="4027c-131">String</span></span>|<span data-ttu-id="4027c-132">オンプレミスで発行されたリソース名を表します。</span><span class="sxs-lookup"><span data-stu-id="4027c-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="4027c-133">応答</span><span class="sxs-lookup"><span data-stu-id="4027c-133">Response</span></span>

<span data-ttu-id="4027c-134">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4027c-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4027c-135">例</span><span class="sxs-lookup"><span data-stu-id="4027c-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4027c-136">要求</span><span class="sxs-lookup"><span data-stu-id="4027c-136">Request</span></span>

<span data-ttu-id="4027c-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4027c-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4027c-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4027c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d

{
    "displayName": "Demo provisioning (updated)"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4027c-139">C#</span><span class="sxs-lookup"><span data-stu-id="4027c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4027c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4027c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4027c-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="4027c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4027c-142">Java</span><span class="sxs-lookup"><span data-stu-id="4027c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4027c-143">応答</span><span class="sxs-lookup"><span data-stu-id="4027c-143">Response</span></span>

<span data-ttu-id="4027c-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4027c-144">The following is an example of the response.</span></span>

> <span data-ttu-id="4027c-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4027c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
