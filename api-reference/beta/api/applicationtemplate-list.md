---
title: ApplicationTemplates のリスト
description: Applicationtemplate オブジェクトのリストを取得します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e58a2f679aac51a94b90ec3c81835663c148e54d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318594"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="1aec4-103">ApplicationTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="1aec4-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aec4-104">Azure AD アプリケーションギャラリーから[Applicationtemplate](../resources/applicationtemplate.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1aec4-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aec4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1aec4-105">Permissions</span></span>

<span data-ttu-id="1aec4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1aec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1aec4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1aec4-108">Permission type</span></span>                        | <span data-ttu-id="1aec4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1aec4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1aec4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1aec4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1aec4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1aec4-111">None.</span></span> |
| <span data-ttu-id="1aec4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1aec4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aec4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1aec4-113">Not supported.</span></span> |
| <span data-ttu-id="1aec4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1aec4-114">Application</span></span>                            | <span data-ttu-id="1aec4-115">なし。</span><span class="sxs-lookup"><span data-stu-id="1aec4-115">None.</span></span> |

<span data-ttu-id="1aec4-116">アプリケーションが Microsoft Graph を呼び出すための有効なアクセストークンを持っていれば、この API を呼び出すために追加のアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1aec4-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="1aec4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1aec4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1aec4-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1aec4-118">Optional query parameters</span></span>

<span data-ttu-id="1aec4-119">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1aec4-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="1aec4-120">パラメーターは`$filter`限定的な方法で使用できます。</span><span class="sxs-lookup"><span data-stu-id="1aec4-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="1aec4-121">**DisplayName**または**カテゴリ**でのみフィルターを適用できます。</span><span class="sxs-lookup"><span data-stu-id="1aec4-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="1aec4-122">たとえば、 `$filter=contains(displayName, 'salesf')` または `$filter=categories/any(c:contains(c, 'myCategory'))` などです。</span><span class="sxs-lookup"><span data-stu-id="1aec4-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="1aec4-123">を使用`$orderby`して`$top,` `$skip` 、任意の GET 要求でパラメーターをクエリできます。</span><span class="sxs-lookup"><span data-stu-id="1aec4-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="1aec4-124">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1aec4-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1aec4-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1aec4-125">Request headers</span></span>

| <span data-ttu-id="1aec4-126">名前</span><span class="sxs-lookup"><span data-stu-id="1aec4-126">Name</span></span>      |<span data-ttu-id="1aec4-127">説明</span><span class="sxs-lookup"><span data-stu-id="1aec4-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1aec4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aec4-128">Authorization</span></span> | <span data-ttu-id="1aec4-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1aec4-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aec4-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="1aec4-130">Request body</span></span>

<span data-ttu-id="1aec4-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1aec4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aec4-132">応答</span><span class="sxs-lookup"><span data-stu-id="1aec4-132">Response</span></span>

<span data-ttu-id="1aec4-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationtemplate](../resources/applicationtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1aec4-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1aec4-134">例</span><span class="sxs-lookup"><span data-stu-id="1aec4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1aec4-135">要求</span><span class="sxs-lookup"><span data-stu-id="1aec4-135">Request</span></span>

<span data-ttu-id="1aec4-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1aec4-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1aec4-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1aec4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1aec4-138">C#</span><span class="sxs-lookup"><span data-stu-id="1aec4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1aec4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1aec4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1aec4-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="1aec4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1aec4-141">Java</span><span class="sxs-lookup"><span data-stu-id="1aec4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1aec4-142">応答</span><span class="sxs-lookup"><span data-stu-id="1aec4-142">Response</span></span>

<span data-ttu-id="1aec4-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1aec4-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1aec4-144">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1aec4-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1aec4-145">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1aec4-145">All the properties will be returned from an actual call.</span></span>

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
