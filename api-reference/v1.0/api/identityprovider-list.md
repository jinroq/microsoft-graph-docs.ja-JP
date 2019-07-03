---
title: identityProvider を一覧表示する
description: identityProvider をすべて取得する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 756578bd61e034972f9b500091ab54c0c7a7dd5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444651"
---
# <a name="list-identityproviders"></a><span data-ttu-id="99bf7-103">identityProvider を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="99bf7-103">List identityProviders</span></span>

<span data-ttu-id="99bf7-104">すべての [identityProvider](../resources/identityprovider.md) ディレクトリ内で取得します。</span><span class="sxs-lookup"><span data-stu-id="99bf7-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="99bf7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99bf7-105">Permissions</span></span>

<span data-ttu-id="99bf7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99bf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99bf7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99bf7-108">Permission type</span></span>      | <span data-ttu-id="99bf7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99bf7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99bf7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99bf7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="99bf7-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99bf7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="99bf7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99bf7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="99bf7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99bf7-113">Not supported.</span></span>|
|<span data-ttu-id="99bf7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99bf7-114">Application</span></span>|<span data-ttu-id="99bf7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99bf7-115">Not supported.</span></span>|

<span data-ttu-id="99bf7-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="99bf7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="99bf7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99bf7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="99bf7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99bf7-118">Request headers</span></span>

|<span data-ttu-id="99bf7-119">名前</span><span class="sxs-lookup"><span data-stu-id="99bf7-119">Name</span></span>|<span data-ttu-id="99bf7-120">説明</span><span class="sxs-lookup"><span data-stu-id="99bf7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="99bf7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99bf7-121">Authorization</span></span>|<span data-ttu-id="99bf7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99bf7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99bf7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="99bf7-124">Request body</span></span>

<span data-ttu-id="99bf7-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99bf7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99bf7-126">応答</span><span class="sxs-lookup"><span data-stu-id="99bf7-126">Response</span></span>

<span data-ttu-id="99bf7-127">成功した場合、このメソッドは `200 OK` 応答コードと、JSON 表現の [identityProvider](../resources/identityprovider.md) のコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="99bf7-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99bf7-128">例</span><span class="sxs-lookup"><span data-stu-id="99bf7-128">Example</span></span>

<span data-ttu-id="99bf7-129">次の例では、すべての **identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="99bf7-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="99bf7-130">要求</span><span class="sxs-lookup"><span data-stu-id="99bf7-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="99bf7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="99bf7-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99bf7-132">C#</span><span class="sxs-lookup"><span data-stu-id="99bf7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99bf7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="99bf7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99bf7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99bf7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99bf7-135">応答</span><span class="sxs-lookup"><span data-stu-id="99bf7-135">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
