---
title: identityProvider を入手する
description: 既存の identityProvider のプロパティを取得する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc06d4f8dcab8bf07d2dc0a9ff8130b305b8217c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649427"
---
# <a name="get-identityprovider"></a><span data-ttu-id="bef6a-103">identityProvider を入手する</span><span class="sxs-lookup"><span data-stu-id="bef6a-103">Get identityProvider</span></span>

<span data-ttu-id="bef6a-104">既存の [identityProvider](../resources/identityprovider.md) のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="bef6a-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bef6a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bef6a-105">Permissions</span></span>

<span data-ttu-id="bef6a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bef6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef6a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bef6a-108">Permission type</span></span>      | <span data-ttu-id="bef6a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bef6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bef6a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bef6a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bef6a-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef6a-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="bef6a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bef6a-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bef6a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bef6a-113">Not supported.</span></span>|
|<span data-ttu-id="bef6a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bef6a-114">Application</span></span>|<span data-ttu-id="bef6a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bef6a-115">Not supported.</span></span>|

<span data-ttu-id="bef6a-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="bef6a-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="bef6a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bef6a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bef6a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bef6a-118">Request headers</span></span>

|<span data-ttu-id="bef6a-119">名前</span><span class="sxs-lookup"><span data-stu-id="bef6a-119">Name</span></span>|<span data-ttu-id="bef6a-120">説明</span><span class="sxs-lookup"><span data-stu-id="bef6a-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bef6a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bef6a-121">Authorization</span></span>|<span data-ttu-id="bef6a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bef6a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef6a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="bef6a-124">Request body</span></span>

<span data-ttu-id="bef6a-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bef6a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bef6a-126">応答</span><span class="sxs-lookup"><span data-stu-id="bef6a-126">Response</span></span>

<span data-ttu-id="bef6a-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [identityProvider](../resources/identityProvider.md) の JSON 表現を返します。</span><span class="sxs-lookup"><span data-stu-id="bef6a-127">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/identityProvider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef6a-128">例</span><span class="sxs-lookup"><span data-stu-id="bef6a-128">Example</span></span>

<span data-ttu-id="bef6a-129">次の例では、特定の**identityProvider** を取得します。</span><span class="sxs-lookup"><span data-stu-id="bef6a-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="bef6a-130">要求</span><span class="sxs-lookup"><span data-stu-id="bef6a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="bef6a-131">応答</span><span class="sxs-lookup"><span data-stu-id="bef6a-131">Response</span></span>

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
