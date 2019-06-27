---
title: identityProvider を入手する
description: 既存の identityProvider のプロパティを取得する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90c9cec4d7a3a0dff47de37b461e087103ed7081
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277134"
---
# <a name="get-identityprovider"></a><span data-ttu-id="158af-103">identityProvider を入手する</span><span class="sxs-lookup"><span data-stu-id="158af-103">Get identityProvider</span></span>

<span data-ttu-id="158af-104">既存の [identityProvider](../resources/identityprovider.md) のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="158af-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="158af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="158af-105">Permissions</span></span>

<span data-ttu-id="158af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="158af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="158af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="158af-108">Permission type</span></span>      | <span data-ttu-id="158af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="158af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="158af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="158af-110">Delegated (work or school account)</span></span>|<span data-ttu-id="158af-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="158af-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="158af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="158af-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="158af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="158af-113">Not supported.</span></span>|
|<span data-ttu-id="158af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="158af-114">Application</span></span>|<span data-ttu-id="158af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="158af-115">Not supported.</span></span>|

<span data-ttu-id="158af-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="158af-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="158af-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="158af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="158af-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="158af-118">Request headers</span></span>

|<span data-ttu-id="158af-119">名前</span><span class="sxs-lookup"><span data-stu-id="158af-119">Name</span></span>|<span data-ttu-id="158af-120">説明</span><span class="sxs-lookup"><span data-stu-id="158af-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="158af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="158af-121">Authorization</span></span>|<span data-ttu-id="158af-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="158af-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="158af-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="158af-124">Request body</span></span>

<span data-ttu-id="158af-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="158af-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="158af-126">応答</span><span class="sxs-lookup"><span data-stu-id="158af-126">Response</span></span>

<span data-ttu-id="158af-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [identityProvider](../resources/identityprovider.md) の JSON 表現を返します。</span><span class="sxs-lookup"><span data-stu-id="158af-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="158af-128">例</span><span class="sxs-lookup"><span data-stu-id="158af-128">Example</span></span>

<span data-ttu-id="158af-129">次の例では、特定の**identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="158af-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="158af-130">要求</span><span class="sxs-lookup"><span data-stu-id="158af-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="158af-131">応答</span><span class="sxs-lookup"><span data-stu-id="158af-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="158af-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="158af-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="158af-133">C#</span><span class="sxs-lookup"><span data-stu-id="158af-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="158af-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="158af-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-identityprovider-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="158af-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="158af-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-identityprovider-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
