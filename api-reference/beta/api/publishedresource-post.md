---
title: PublishedResource の作成
description: 新しい**Publishedresource**オブジェクトを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75e560ac96a5d8979cd5b0b7c9f76e9ba2d42b90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309220"
---
# <a name="create-publishedresource"></a><span data-ttu-id="792ec-103">PublishedResource の作成</span><span class="sxs-lookup"><span data-stu-id="792ec-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="792ec-104">新しい[Publishedresource](../resources/publishedresource.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="792ec-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="792ec-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="792ec-105">Permissions</span></span>

<span data-ttu-id="792ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="792ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="792ec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="792ec-108">Permission type</span></span>                        | <span data-ttu-id="792ec-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="792ec-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="792ec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="792ec-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="792ec-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="792ec-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="792ec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="792ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="792ec-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ec-113">Not supported.</span></span> |
| <span data-ttu-id="792ec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="792ec-114">Application</span></span>                            | <span data-ttu-id="792ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="792ec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="792ec-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="792ec-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="792ec-117">Request headers</span></span>

| <span data-ttu-id="792ec-118">名前</span><span class="sxs-lookup"><span data-stu-id="792ec-118">Name</span></span>      |<span data-ttu-id="792ec-119">説明</span><span class="sxs-lookup"><span data-stu-id="792ec-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="792ec-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="792ec-120">Authorization</span></span> | <span data-ttu-id="792ec-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="792ec-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="792ec-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="792ec-122">Request body</span></span>

<span data-ttu-id="792ec-123">要求本文で、 [Publishedresource](../resources/publishedresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="792ec-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="792ec-124">次のプロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="792ec-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="792ec-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="792ec-125">Property</span></span>     | <span data-ttu-id="792ec-126">型</span><span class="sxs-lookup"><span data-stu-id="792ec-126">Type</span></span>        | <span data-ttu-id="792ec-127">説明</span><span class="sxs-lookup"><span data-stu-id="792ec-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="792ec-128">displayName</span><span class="sxs-lookup"><span data-stu-id="792ec-128">displayName</span></span>|<span data-ttu-id="792ec-129">String</span><span class="sxs-lookup"><span data-stu-id="792ec-129">String</span></span>|<span data-ttu-id="792ec-130">PublishedResource の表示名。</span><span class="sxs-lookup"><span data-stu-id="792ec-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="792ec-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="792ec-131">resourceName</span></span>|<span data-ttu-id="792ec-132">String</span><span class="sxs-lookup"><span data-stu-id="792ec-132">String</span></span>|<span data-ttu-id="792ec-133">PublishedResource の名前。</span><span class="sxs-lookup"><span data-stu-id="792ec-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="792ec-134">応答</span><span class="sxs-lookup"><span data-stu-id="792ec-134">Response</span></span>

<span data-ttu-id="792ec-135">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[publishedresource](../resources/publishedresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="792ec-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="792ec-136">例</span><span class="sxs-lookup"><span data-stu-id="792ec-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="792ec-137">要求</span><span class="sxs-lookup"><span data-stu-id="792ec-137">Request</span></span>

<span data-ttu-id="792ec-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="792ec-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="792ec-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="792ec-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources
Content-Type: application/json

{
    "displayName": "New provisioning",
    "resourceName": "domain1.contoso.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="792ec-140">C#</span><span class="sxs-lookup"><span data-stu-id="792ec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="792ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="792ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="792ec-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="792ec-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="792ec-143">Java</span><span class="sxs-lookup"><span data-stu-id="792ec-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="792ec-144">応答</span><span class="sxs-lookup"><span data-stu-id="792ec-144">Response</span></span>

<span data-ttu-id="792ec-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="792ec-145">The following is an example of the response.</span></span>

> <span data-ttu-id="792ec-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="792ec-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 201 Created

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "publishingType": "provisioning",
    "displayName": "New provisionin",
    "resourceName": "domain1.contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
