---
title: identityProvider を一覧表示する
description: すべての identityProvider ディレクトリ内で取得します。
localization_priority: Normal
ms.openlocfilehash: c7ddabf8aef2a4d50f6ea133ecf696c8bdda922b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262665"
---
# <a name="list-identityproviders"></a><span data-ttu-id="6e7c7-103">identityProvider を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6e7c7-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e7c7-104">すべての [identityProvider](../resources/identityprovider.md) ディレクトリ内で取得します。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e7c7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e7c7-105">Permissions</span></span>

<span data-ttu-id="6e7c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e7c7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e7c7-108">Permission type</span></span>      | <span data-ttu-id="6e7c7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e7c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e7c7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e7c7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6e7c7-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e7c7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6e7c7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e7c7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6e7c7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-113">Not supported.</span></span>|
|<span data-ttu-id="6e7c7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e7c7-114">Application</span></span>|<span data-ttu-id="6e7c7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-115">Not supported.</span></span>|

<span data-ttu-id="6e7c7-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e7c7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e7c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="6e7c7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e7c7-118">Request headers</span></span>

|<span data-ttu-id="6e7c7-119">名前</span><span class="sxs-lookup"><span data-stu-id="6e7c7-119">Name</span></span>|<span data-ttu-id="6e7c7-120">説明</span><span class="sxs-lookup"><span data-stu-id="6e7c7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6e7c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e7c7-121">Authorization</span></span>|<span data-ttu-id="6e7c7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e7c7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e7c7-124">Request body</span></span>

<span data-ttu-id="6e7c7-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e7c7-126">応答</span><span class="sxs-lookup"><span data-stu-id="6e7c7-126">Response</span></span>

<span data-ttu-id="6e7c7-127">成功した場合、このメソッドは `200 OK` 応答コードと、JSON 表現の [identityProvider](../resources/identityprovider.md) のコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e7c7-128">例</span><span class="sxs-lookup"><span data-stu-id="6e7c7-128">Example</span></span>

<span data-ttu-id="6e7c7-129">次の例では、すべての **identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e7c7-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="6e7c7-130">要求</span><span class="sxs-lookup"><span data-stu-id="6e7c7-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="6e7c7-131">応答</span><span class="sxs-lookup"><span data-stu-id="6e7c7-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6e7c7-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="6e7c7-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6e7c7-133">C#</span><span class="sxs-lookup"><span data-stu-id="6e7c7-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e7c7-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e7c7-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6e7c7-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="6e7c7-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
