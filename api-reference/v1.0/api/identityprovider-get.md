---
title: identityProvider を入手する
description: 既存の identityProvider のプロパティを取得する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25b3e2733c3dcd9261f2b8ef59a4a98e96cfb401
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880920"
---
# <a name="get-identityprovider"></a><span data-ttu-id="9664b-103">identityProvider を入手する</span><span class="sxs-lookup"><span data-stu-id="9664b-103">Get identityProvider</span></span>

<span data-ttu-id="9664b-104">既存の [identityProvider](../resources/identityprovider.md) のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9664b-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9664b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9664b-105">Permissions</span></span>

<span data-ttu-id="9664b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9664b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9664b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9664b-108">Permission type</span></span>      | <span data-ttu-id="9664b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9664b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9664b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9664b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9664b-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9664b-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9664b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9664b-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9664b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9664b-113">Not supported.</span></span>|
|<span data-ttu-id="9664b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9664b-114">Application</span></span>|<span data-ttu-id="9664b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9664b-115">Not supported.</span></span>|

<span data-ttu-id="9664b-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9664b-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9664b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9664b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9664b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9664b-118">Request headers</span></span>

|<span data-ttu-id="9664b-119">名前</span><span class="sxs-lookup"><span data-stu-id="9664b-119">Name</span></span>|<span data-ttu-id="9664b-120">説明</span><span class="sxs-lookup"><span data-stu-id="9664b-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9664b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9664b-121">Authorization</span></span>|<span data-ttu-id="9664b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9664b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9664b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9664b-124">Request body</span></span>

<span data-ttu-id="9664b-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9664b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9664b-126">応答</span><span class="sxs-lookup"><span data-stu-id="9664b-126">Response</span></span>

<span data-ttu-id="9664b-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [identityProvider](../resources/identityprovider.md) の JSON 表現を返します。</span><span class="sxs-lookup"><span data-stu-id="9664b-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9664b-128">例</span><span class="sxs-lookup"><span data-stu-id="9664b-128">Example</span></span>

<span data-ttu-id="9664b-129">次の例では、特定の**identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="9664b-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="9664b-130">要求</span><span class="sxs-lookup"><span data-stu-id="9664b-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9664b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9664b-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9664b-132">C#</span><span class="sxs-lookup"><span data-stu-id="9664b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9664b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9664b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9664b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9664b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9664b-135">Java</span><span class="sxs-lookup"><span data-stu-id="9664b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9664b-136">応答</span><span class="sxs-lookup"><span data-stu-id="9664b-136">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
