---
title: identityProvider を削除する
description: 既存の identityProvider を削除する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a09018011e87da383371ba41b1a046ddeb9002b5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649425"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="68325-103">identityProvider を削除する</span><span class="sxs-lookup"><span data-stu-id="68325-103">Delete identityProvider</span></span>

<span data-ttu-id="68325-104">既存の [identityProvider](../resources/identityprovider.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="68325-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68325-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68325-105">Permissions</span></span>

<span data-ttu-id="68325-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68325-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68325-108">Permission type</span></span>      | <span data-ttu-id="68325-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68325-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68325-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68325-110">Delegated (work or school account)</span></span>|<span data-ttu-id="68325-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68325-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="68325-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68325-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="68325-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68325-113">Not supported.</span></span>|
|<span data-ttu-id="68325-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68325-114">Application</span></span>|<span data-ttu-id="68325-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68325-115">Not supported.</span></span>|

<span data-ttu-id="68325-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="68325-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="68325-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68325-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68325-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68325-118">Request headers</span></span>

|<span data-ttu-id="68325-119">名前</span><span class="sxs-lookup"><span data-stu-id="68325-119">Name</span></span>|<span data-ttu-id="68325-120">説明</span><span class="sxs-lookup"><span data-stu-id="68325-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="68325-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="68325-121">Authorization</span></span>|<span data-ttu-id="68325-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="68325-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68325-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="68325-124">Request body</span></span>

<span data-ttu-id="68325-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="68325-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68325-126">応答</span><span class="sxs-lookup"><span data-stu-id="68325-126">Response</span></span>

<span data-ttu-id="68325-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="68325-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68325-128">例</span><span class="sxs-lookup"><span data-stu-id="68325-128">Example</span></span>

<span data-ttu-id="68325-129">次の例では、\*\* identityProvider \*\* を削除します。</span><span class="sxs-lookup"><span data-stu-id="68325-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="68325-130">要求</span><span class="sxs-lookup"><span data-stu-id="68325-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="68325-131">応答</span><span class="sxs-lookup"><span data-stu-id="68325-131">Response</span></span>

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
