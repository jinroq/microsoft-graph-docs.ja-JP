---
title: IdentityProvider を取得します。
description: 既存の identityProvider のプロパティを取得します。
ms.openlocfilehash: 238e222c820e62685fa7c9e7ca50f5efb33693cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069488"
---
# <a name="get-identityprovider"></a><span data-ttu-id="6a993-103">IdentityProvider を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a993-103">Get identityProvider</span></span>

> <span data-ttu-id="6a993-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a993-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a993-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a993-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a993-106">既存の[identityProvider](../resources/identityprovider.md)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a993-106">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a993-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a993-107">Permissions</span></span>

<span data-ttu-id="6a993-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a993-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a993-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a993-110">Permission type</span></span>      | <span data-ttu-id="6a993-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a993-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a993-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a993-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a993-113">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a993-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6a993-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a993-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6a993-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a993-115">Not supported.</span></span>|
|<span data-ttu-id="6a993-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a993-116">Application</span></span>|<span data-ttu-id="6a993-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a993-117">Not supported.</span></span>|

<span data-ttu-id="6a993-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a993-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a993-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a993-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a993-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a993-120">Request headers</span></span>

|<span data-ttu-id="6a993-121">名前</span><span class="sxs-lookup"><span data-stu-id="6a993-121">Name</span></span>|<span data-ttu-id="6a993-122">説明</span><span class="sxs-lookup"><span data-stu-id="6a993-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6a993-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a993-123">Authorization</span></span>|<span data-ttu-id="6a993-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a993-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a993-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a993-126">Request body</span></span>

<span data-ttu-id="6a993-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a993-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a993-128">応答</span><span class="sxs-lookup"><span data-stu-id="6a993-128">Response</span></span>

<span data-ttu-id="6a993-129">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[identityProvider](../resources/identityprovider.md)の JSON 形式です。</span><span class="sxs-lookup"><span data-stu-id="6a993-129">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a993-130">使用例</span><span class="sxs-lookup"><span data-stu-id="6a993-130">Example</span></span>

<span data-ttu-id="6a993-131">次の例では、特定の**identityProvider**を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a993-131">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="6a993-132">要求</span><span class="sxs-lookup"><span data-stu-id="6a993-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="6a993-133">応答</span><span class="sxs-lookup"><span data-stu-id="6a993-133">Response</span></span>

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
  "tocPath": ""
}-->