---
title: identityProvider を一覧表示する
description: すべての identityProvider ディレクトリ内で取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 4000be4ce44ed38c40b739313a80ad84aa880feb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420566"
---
# <a name="list-identityproviders"></a><span data-ttu-id="802ae-103">identityProvider を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="802ae-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="802ae-104">すべての [identityProvider](../resources/identityprovider.md) ディレクトリ内で取得します。</span><span class="sxs-lookup"><span data-stu-id="802ae-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="802ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="802ae-105">Permissions</span></span>

<span data-ttu-id="802ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="802ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="802ae-108">Permission type</span></span>      | <span data-ttu-id="802ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="802ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="802ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="802ae-110">Delegated (work or school account)</span></span>|<span data-ttu-id="802ae-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802ae-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="802ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="802ae-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="802ae-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="802ae-113">Not supported.</span></span>|
|<span data-ttu-id="802ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="802ae-114">Application</span></span>|<span data-ttu-id="802ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="802ae-115">Not supported.</span></span>|

<span data-ttu-id="802ae-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="802ae-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="802ae-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="802ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="802ae-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="802ae-118">Request headers</span></span>

|<span data-ttu-id="802ae-119">名前</span><span class="sxs-lookup"><span data-stu-id="802ae-119">Name</span></span>|<span data-ttu-id="802ae-120">説明</span><span class="sxs-lookup"><span data-stu-id="802ae-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="802ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="802ae-121">Authorization</span></span>|<span data-ttu-id="802ae-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="802ae-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="802ae-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="802ae-124">Request body</span></span>

<span data-ttu-id="802ae-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="802ae-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="802ae-126">応答</span><span class="sxs-lookup"><span data-stu-id="802ae-126">Response</span></span>

<span data-ttu-id="802ae-127">成功した場合、このメソッドは `200 OK` 応答コードと、JSON 表現の [identityProvider](../resources/identityprovider.md) のコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="802ae-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802ae-128">例</span><span class="sxs-lookup"><span data-stu-id="802ae-128">Example</span></span>

<span data-ttu-id="802ae-129">次の例では、すべての **identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="802ae-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="802ae-130">要求</span><span class="sxs-lookup"><span data-stu-id="802ae-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="802ae-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="802ae-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="802ae-132">C#</span><span class="sxs-lookup"><span data-stu-id="802ae-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="802ae-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="802ae-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="802ae-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="802ae-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="802ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="802ae-135">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
