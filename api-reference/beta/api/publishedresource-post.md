---
title: PublishedResource の作成
description: 新しい**Publishedresource**オブジェクトを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8823d80a3786ea8a8d3b1b3e1f7a1ef467e7384c
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840976"
---
# <a name="create-publishedresource"></a><span data-ttu-id="2b225-103">PublishedResource の作成</span><span class="sxs-lookup"><span data-stu-id="2b225-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b225-104">新しい[Publishedresource](../resources/publishedresource.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b225-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b225-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b225-105">Permissions</span></span>

<span data-ttu-id="2b225-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b225-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b225-108">Permission type</span></span>                        | <span data-ttu-id="2b225-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b225-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b225-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b225-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b225-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="2b225-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2b225-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b225-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b225-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b225-113">Not supported.</span></span> |
| <span data-ttu-id="2b225-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b225-114">Application</span></span>                            | <span data-ttu-id="2b225-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b225-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b225-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b225-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="2b225-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b225-117">Request headers</span></span>

| <span data-ttu-id="2b225-118">名前</span><span class="sxs-lookup"><span data-stu-id="2b225-118">Name</span></span>      |<span data-ttu-id="2b225-119">説明</span><span class="sxs-lookup"><span data-stu-id="2b225-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b225-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b225-120">Authorization</span></span> | <span data-ttu-id="2b225-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="2b225-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b225-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b225-122">Request body</span></span>

<span data-ttu-id="2b225-123">要求本文で、 [Publishedresource](../resources/publishedresource.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b225-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="2b225-124">次のプロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b225-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="2b225-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b225-125">Property</span></span>     | <span data-ttu-id="2b225-126">型</span><span class="sxs-lookup"><span data-stu-id="2b225-126">Type</span></span>        | <span data-ttu-id="2b225-127">説明</span><span class="sxs-lookup"><span data-stu-id="2b225-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b225-128">displayName</span><span class="sxs-lookup"><span data-stu-id="2b225-128">displayName</span></span>|<span data-ttu-id="2b225-129">String</span><span class="sxs-lookup"><span data-stu-id="2b225-129">String</span></span>|<span data-ttu-id="2b225-130">PublishedResource の表示名。</span><span class="sxs-lookup"><span data-stu-id="2b225-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="2b225-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="2b225-131">resourceName</span></span>|<span data-ttu-id="2b225-132">String</span><span class="sxs-lookup"><span data-stu-id="2b225-132">String</span></span>|<span data-ttu-id="2b225-133">PublishedResource の名前。</span><span class="sxs-lookup"><span data-stu-id="2b225-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="2b225-134">応答</span><span class="sxs-lookup"><span data-stu-id="2b225-134">Response</span></span>

<span data-ttu-id="2b225-135">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[publishedresource](../resources/publishedresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2b225-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b225-136">例</span><span class="sxs-lookup"><span data-stu-id="2b225-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b225-137">要求</span><span class="sxs-lookup"><span data-stu-id="2b225-137">Request</span></span>

<span data-ttu-id="2b225-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b225-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b225-139">応答</span><span class="sxs-lookup"><span data-stu-id="2b225-139">Response</span></span>

<span data-ttu-id="2b225-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b225-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2b225-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2b225-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
