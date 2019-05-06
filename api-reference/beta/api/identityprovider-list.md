---
title: identityProvider を一覧表示する
description: すべての identityProvider ディレクトリ内で取得します。
localization_priority: Normal
ms.openlocfilehash: 483594fc9075e11f872f80303bd42b8c59b91053
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592226"
---
# <a name="list-identityproviders"></a><span data-ttu-id="d7b53-103">identityProvider を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d7b53-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b53-104">すべての [identityProvider](../resources/identityprovider.md) ディレクトリ内で取得します。</span><span class="sxs-lookup"><span data-stu-id="d7b53-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7b53-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7b53-105">Permissions</span></span>

<span data-ttu-id="d7b53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b53-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7b53-108">Permission type</span></span>      | <span data-ttu-id="d7b53-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7b53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7b53-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b53-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d7b53-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7b53-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d7b53-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b53-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d7b53-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b53-113">Not supported.</span></span>|
|<span data-ttu-id="d7b53-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7b53-114">Application</span></span>|<span data-ttu-id="d7b53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b53-115">Not supported.</span></span>|

<span data-ttu-id="d7b53-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7b53-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d7b53-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7b53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="d7b53-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b53-118">Request headers</span></span>

|<span data-ttu-id="d7b53-119">名前</span><span class="sxs-lookup"><span data-stu-id="d7b53-119">Name</span></span>|<span data-ttu-id="d7b53-120">説明</span><span class="sxs-lookup"><span data-stu-id="d7b53-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d7b53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b53-121">Authorization</span></span>|<span data-ttu-id="d7b53-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7b53-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7b53-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7b53-124">Request body</span></span>

<span data-ttu-id="d7b53-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7b53-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7b53-126">応答</span><span class="sxs-lookup"><span data-stu-id="d7b53-126">Response</span></span>

<span data-ttu-id="d7b53-127">成功した場合、このメソッドは `200 OK` 応答コードと、JSON 表現の [identityProvider](../resources/identityprovider.md) のコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d7b53-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7b53-128">例</span><span class="sxs-lookup"><span data-stu-id="d7b53-128">Example</span></span>

<span data-ttu-id="d7b53-129">次の例では、すべての **identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="d7b53-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d7b53-130">要求</span><span class="sxs-lookup"><span data-stu-id="d7b53-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="d7b53-131">応答</span><span class="sxs-lookup"><span data-stu-id="d7b53-131">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7b53-132">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d7b53-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7b53-133">Visual</span><span class="sxs-lookup"><span data-stu-id="d7b53-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7b53-134">Java</span><span class="sxs-lookup"><span data-stu-id="d7b53-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityproviders-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
