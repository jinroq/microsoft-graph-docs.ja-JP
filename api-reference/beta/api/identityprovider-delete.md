---
title: IdentityProvider を削除します。
description: 既存の identityProvider を削除します。
localization_priority: Normal
ms.openlocfilehash: 35689037d4f6a564ee3e1e40d18401ef793ef474
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808296"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="c341f-103">IdentityProvider を削除します。</span><span class="sxs-lookup"><span data-stu-id="c341f-103">Delete identityProvider</span></span>

> <span data-ttu-id="c341f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c341f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c341f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c341f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c341f-106">既存の[identityProvider](../resources/identityprovider.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c341f-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c341f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c341f-107">Permissions</span></span>

<span data-ttu-id="c341f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c341f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c341f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c341f-110">Permission type</span></span>      | <span data-ttu-id="c341f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c341f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c341f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c341f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c341f-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c341f-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c341f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c341f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c341f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c341f-115">Not supported.</span></span>|
|<span data-ttu-id="c341f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c341f-116">Application</span></span>|<span data-ttu-id="c341f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c341f-117">Not supported.</span></span>|

<span data-ttu-id="c341f-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c341f-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c341f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c341f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c341f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c341f-120">Request headers</span></span>

|<span data-ttu-id="c341f-121">名前</span><span class="sxs-lookup"><span data-stu-id="c341f-121">Name</span></span>|<span data-ttu-id="c341f-122">説明</span><span class="sxs-lookup"><span data-stu-id="c341f-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c341f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c341f-123">Authorization</span></span>|<span data-ttu-id="c341f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c341f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c341f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c341f-126">Request body</span></span>

<span data-ttu-id="c341f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c341f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c341f-128">応答</span><span class="sxs-lookup"><span data-stu-id="c341f-128">Response</span></span>

<span data-ttu-id="c341f-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c341f-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c341f-130">例</span><span class="sxs-lookup"><span data-stu-id="c341f-130">Example</span></span>

<span data-ttu-id="c341f-131">次の使用例は、 **identityProvider**を削除します。</span><span class="sxs-lookup"><span data-stu-id="c341f-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c341f-132">要求</span><span class="sxs-lookup"><span data-stu-id="c341f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="c341f-133">応答</span><span class="sxs-lookup"><span data-stu-id="c341f-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
