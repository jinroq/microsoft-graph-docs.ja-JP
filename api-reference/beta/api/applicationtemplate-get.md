---
title: ApplicationTemplate の取得
description: Applicationtemplate オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 498eaf8b33916cbaa493f211dab8b99889e14a59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439540"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="738a6-103">ApplicationTemplate の取得</span><span class="sxs-lookup"><span data-stu-id="738a6-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="738a6-104">[Applicationtemplate](../resources/applicationtemplate.md)オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="738a6-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="738a6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="738a6-105">Permissions</span></span>

<span data-ttu-id="738a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="738a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="738a6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="738a6-108">Permission type</span></span>                        | <span data-ttu-id="738a6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="738a6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="738a6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="738a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="738a6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="738a6-111">None.</span></span> |
| <span data-ttu-id="738a6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="738a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="738a6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="738a6-113">Not supported.</span></span> |
| <span data-ttu-id="738a6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="738a6-114">Application</span></span>                            | <span data-ttu-id="738a6-115">なし。</span><span class="sxs-lookup"><span data-stu-id="738a6-115">None.</span></span> |

<span data-ttu-id="738a6-116">アプリケーションが Microsoft Graph を呼び出すための有効なアクセストークンを持っていれば、この API を呼び出すために追加のアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="738a6-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="738a6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="738a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="738a6-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="738a6-118">Optional query parameters</span></span>

<span data-ttu-id="738a6-119">`$select`クエリパラメーターを使用して、最適なパフォーマンスを得るために必要なプロパティのみを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="738a6-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="738a6-120">**Id**プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="738a6-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="738a6-121">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="738a6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="738a6-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="738a6-122">Request headers</span></span>

| <span data-ttu-id="738a6-123">名前</span><span class="sxs-lookup"><span data-stu-id="738a6-123">Name</span></span>      |<span data-ttu-id="738a6-124">説明</span><span class="sxs-lookup"><span data-stu-id="738a6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="738a6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="738a6-125">Authorization</span></span> | <span data-ttu-id="738a6-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="738a6-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="738a6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="738a6-127">Request body</span></span>

<span data-ttu-id="738a6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="738a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="738a6-129">応答</span><span class="sxs-lookup"><span data-stu-id="738a6-129">Response</span></span>

<span data-ttu-id="738a6-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[applicationtemplate](../resources/applicationtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="738a6-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="738a6-131">例</span><span class="sxs-lookup"><span data-stu-id="738a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="738a6-132">要求</span><span class="sxs-lookup"><span data-stu-id="738a6-132">Request</span></span>

<span data-ttu-id="738a6-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="738a6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="738a6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="738a6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="738a6-135">C#</span><span class="sxs-lookup"><span data-stu-id="738a6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="738a6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="738a6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="738a6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="738a6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="738a6-138">応答</span><span class="sxs-lookup"><span data-stu-id="738a6-138">Response</span></span>

<span data-ttu-id="738a6-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="738a6-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="738a6-140">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="738a6-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="738a6-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="738a6-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
