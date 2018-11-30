---
title: リスト identityProviders
description: ディレクトリ内のすべての identityProviders を取得します。
ms.openlocfilehash: fd5662690b644bc7a34587a5bdfc519188a3d4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072621"
---
# <a name="list-identityproviders"></a><span data-ttu-id="fadbe-103">リスト identityProviders</span><span class="sxs-lookup"><span data-stu-id="fadbe-103">List identityProviders</span></span>

> <span data-ttu-id="fadbe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fadbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fadbe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fadbe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fadbe-106">ディレクトリ内のすべての[identityProviders](../resources/identityprovider.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="fadbe-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="fadbe-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fadbe-107">Permissions</span></span>

<span data-ttu-id="fadbe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fadbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fadbe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fadbe-110">Permission type</span></span>      | <span data-ttu-id="fadbe-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fadbe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fadbe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fadbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fadbe-113">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fadbe-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fadbe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fadbe-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fadbe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fadbe-115">Not supported.</span></span>|
|<span data-ttu-id="fadbe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fadbe-116">Application</span></span>|<span data-ttu-id="fadbe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fadbe-117">Not supported.</span></span>|

<span data-ttu-id="fadbe-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="fadbe-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="fadbe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fadbe-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="fadbe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fadbe-120">Request headers</span></span>

|<span data-ttu-id="fadbe-121">名前</span><span class="sxs-lookup"><span data-stu-id="fadbe-121">Name</span></span>|<span data-ttu-id="fadbe-122">説明</span><span class="sxs-lookup"><span data-stu-id="fadbe-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fadbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fadbe-123">Authorization</span></span>|<span data-ttu-id="fadbe-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fadbe-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fadbe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fadbe-126">Request body</span></span>

<span data-ttu-id="fadbe-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fadbe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fadbe-128">応答</span><span class="sxs-lookup"><span data-stu-id="fadbe-128">Response</span></span>

<span data-ttu-id="fadbe-129">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に JSON 形式で[identityProviders](../resources/identityprovider.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="fadbe-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fadbe-130">使用例</span><span class="sxs-lookup"><span data-stu-id="fadbe-130">Example</span></span>

<span data-ttu-id="fadbe-131">次の例では、すべての**identityProvider**を取得します。</span><span class="sxs-lookup"><span data-stu-id="fadbe-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="fadbe-132">要求</span><span class="sxs-lookup"><span data-stu-id="fadbe-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="fadbe-133">応答</span><span class="sxs-lookup"><span data-stu-id="fadbe-133">Response</span></span>

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
  "tocPath": ""
}-->