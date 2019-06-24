---
title: ApplicationTemplates のリスト
description: Applicationtemplate オブジェクトのリストを取得します。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac8ad3a8b4a7a396c0cb35c1c72c2d1a2e309184
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147923"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="9cb6e-103">ApplicationTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="9cb6e-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb6e-104">Azure AD アプリケーションギャラリーから[Applicationtemplate](../resources/applicationtemplate.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cb6e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9cb6e-105">Permissions</span></span>

<span data-ttu-id="9cb6e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cb6e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9cb6e-108">Permission type</span></span>                        | <span data-ttu-id="9cb6e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9cb6e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9cb6e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9cb6e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cb6e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-111">None.</span></span> |
| <span data-ttu-id="9cb6e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9cb6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb6e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-113">Not supported.</span></span> |
| <span data-ttu-id="9cb6e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9cb6e-114">Application</span></span>                            | <span data-ttu-id="9cb6e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-115">None.</span></span> |

<span data-ttu-id="9cb6e-116">アプリケーションが Microsoft Graph を呼び出すための有効なアクセストークンを持っていれば、この API を呼び出すために追加のアクセス許可は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="9cb6e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9cb6e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cb6e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9cb6e-118">Optional query parameters</span></span>

<span data-ttu-id="9cb6e-119">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="9cb6e-120">パラメーターは`$filter`限定的な方法で使用できます。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="9cb6e-121">**DisplayName**または**カテゴリ**でのみフィルターを適用できます。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="9cb6e-122">たとえば、 `$filter=contains(displayName, 'salesf')` または `$filter=categories/any(c:contains(c, 'myCategory'))` などです。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="9cb6e-123">を使用`$orderby`して`$top,` `$skip` 、任意の GET 要求でパラメーターをクエリできます。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="9cb6e-124">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cb6e-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cb6e-125">Request headers</span></span>

| <span data-ttu-id="9cb6e-126">名前</span><span class="sxs-lookup"><span data-stu-id="9cb6e-126">Name</span></span>      |<span data-ttu-id="9cb6e-127">説明</span><span class="sxs-lookup"><span data-stu-id="9cb6e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cb6e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb6e-128">Authorization</span></span> | <span data-ttu-id="9cb6e-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9cb6e-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cb6e-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9cb6e-130">Request body</span></span>

<span data-ttu-id="9cb6e-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cb6e-132">応答</span><span class="sxs-lookup"><span data-stu-id="9cb6e-132">Response</span></span>

<span data-ttu-id="9cb6e-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationtemplate](../resources/applicationtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cb6e-134">例</span><span class="sxs-lookup"><span data-stu-id="9cb6e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cb6e-135">要求</span><span class="sxs-lookup"><span data-stu-id="9cb6e-135">Request</span></span>

<span data-ttu-id="9cb6e-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### <a name="response"></a><span data-ttu-id="9cb6e-137">応答</span><span class="sxs-lookup"><span data-stu-id="9cb6e-137">Response</span></span>

<span data-ttu-id="9cb6e-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9cb6e-139">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9cb6e-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9cb6e-140">All the properties will be returned from an actual call.</span></span>

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
