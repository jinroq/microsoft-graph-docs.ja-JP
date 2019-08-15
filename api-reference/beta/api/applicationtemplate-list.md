---
title: ApplicationTemplates のリスト
description: Applicationtemplate オブジェクトのリストを取得します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 63465f12b60c0b25aec59c9915e7d5aeba134985
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415716"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="62c84-103">ApplicationTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="62c84-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c84-104">Azure AD アプリケーションギャラリーから[Applicationtemplate](../resources/applicationtemplate.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="62c84-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="62c84-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="62c84-105">Permissions</span></span>

<span data-ttu-id="62c84-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62c84-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62c84-108">Permission type</span></span>                        | <span data-ttu-id="62c84-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="62c84-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62c84-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62c84-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62c84-111">なし。</span><span class="sxs-lookup"><span data-stu-id="62c84-111">None.</span></span> |
| <span data-ttu-id="62c84-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62c84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c84-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62c84-113">Not supported.</span></span> |
| <span data-ttu-id="62c84-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62c84-114">Application</span></span>                            | <span data-ttu-id="62c84-115">なし。</span><span class="sxs-lookup"><span data-stu-id="62c84-115">None.</span></span> |

<span data-ttu-id="62c84-116">アプリケーションが Microsoft Graph を呼び出すための有効なアクセストークンを持っていれば、この API を呼び出すために追加のアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="62c84-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="62c84-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62c84-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62c84-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="62c84-118">Optional query parameters</span></span>

<span data-ttu-id="62c84-119">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="62c84-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="62c84-120">パラメーターは`$filter`限定的な方法で使用できます。</span><span class="sxs-lookup"><span data-stu-id="62c84-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="62c84-121">**DisplayName**または**カテゴリ**でのみフィルターを適用できます。</span><span class="sxs-lookup"><span data-stu-id="62c84-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="62c84-122">たとえば、 `$filter=contains(displayName, 'salesf')` または `$filter=categories/any(c:contains(c, 'myCategory'))` などです。</span><span class="sxs-lookup"><span data-stu-id="62c84-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="62c84-123">を使用`$orderby`して`$top,` `$skip` 、任意の GET 要求でパラメーターをクエリできます。</span><span class="sxs-lookup"><span data-stu-id="62c84-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="62c84-124">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62c84-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62c84-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62c84-125">Request headers</span></span>

| <span data-ttu-id="62c84-126">名前</span><span class="sxs-lookup"><span data-stu-id="62c84-126">Name</span></span>      |<span data-ttu-id="62c84-127">説明</span><span class="sxs-lookup"><span data-stu-id="62c84-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62c84-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="62c84-128">Authorization</span></span> | <span data-ttu-id="62c84-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="62c84-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="62c84-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="62c84-130">Request body</span></span>

<span data-ttu-id="62c84-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="62c84-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62c84-132">応答</span><span class="sxs-lookup"><span data-stu-id="62c84-132">Response</span></span>

<span data-ttu-id="62c84-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationtemplate](../resources/applicationtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="62c84-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62c84-134">例</span><span class="sxs-lookup"><span data-stu-id="62c84-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62c84-135">要求</span><span class="sxs-lookup"><span data-stu-id="62c84-135">Request</span></span>

<span data-ttu-id="62c84-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62c84-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="62c84-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="62c84-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62c84-138">C#</span><span class="sxs-lookup"><span data-stu-id="62c84-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62c84-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62c84-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62c84-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="62c84-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62c84-141">応答</span><span class="sxs-lookup"><span data-stu-id="62c84-141">Response</span></span>

<span data-ttu-id="62c84-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62c84-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="62c84-143">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="62c84-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62c84-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="62c84-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applicationTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
