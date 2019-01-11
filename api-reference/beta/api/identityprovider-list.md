---
title: リスト identityProviders
description: ディレクトリ内のすべての identityProviders を取得します。
localization_priority: Normal
ms.openlocfilehash: 43442a0bf354816c8c104d57d9720940d83bc0d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837969"
---
# <a name="list-identityproviders"></a><span data-ttu-id="625f8-103">リスト identityProviders</span><span class="sxs-lookup"><span data-stu-id="625f8-103">List identityProviders</span></span>

> <span data-ttu-id="625f8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="625f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="625f8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="625f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="625f8-106">ディレクトリ内のすべての[identityProviders](../resources/identityprovider.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="625f8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="625f8-107">Permissions</span></span>

<span data-ttu-id="625f8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="625f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625f8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="625f8-110">Permission type</span></span>      | <span data-ttu-id="625f8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="625f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="625f8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="625f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="625f8-113">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625f8-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="625f8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="625f8-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="625f8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="625f8-115">Not supported.</span></span>|
|<span data-ttu-id="625f8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="625f8-116">Application</span></span>|<span data-ttu-id="625f8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="625f8-117">Not supported.</span></span>|

<span data-ttu-id="625f8-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="625f8-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="625f8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="625f8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="625f8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="625f8-120">Request headers</span></span>

|<span data-ttu-id="625f8-121">名前</span><span class="sxs-lookup"><span data-stu-id="625f8-121">Name</span></span>|<span data-ttu-id="625f8-122">説明</span><span class="sxs-lookup"><span data-stu-id="625f8-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="625f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="625f8-123">Authorization</span></span>|<span data-ttu-id="625f8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="625f8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="625f8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="625f8-126">Request body</span></span>

<span data-ttu-id="625f8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="625f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="625f8-128">応答</span><span class="sxs-lookup"><span data-stu-id="625f8-128">Response</span></span>

<span data-ttu-id="625f8-129">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に JSON 形式で[identityProviders](../resources/identityprovider.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="625f8-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625f8-130">例</span><span class="sxs-lookup"><span data-stu-id="625f8-130">Example</span></span>

<span data-ttu-id="625f8-131">次の例では、すべての**identityProvider**を取得します。</span><span class="sxs-lookup"><span data-stu-id="625f8-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="625f8-132">要求</span><span class="sxs-lookup"><span data-stu-id="625f8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="625f8-133">応答</span><span class="sxs-lookup"><span data-stu-id="625f8-133">Response</span></span>

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
