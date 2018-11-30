---
title: IdentityProvider を更新します。
description: 既存の identityProvider プロパティを更新します。
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069175"
---
# <a name="update-identityprovider"></a><span data-ttu-id="147aa-103">IdentityProvider を更新します。</span><span class="sxs-lookup"><span data-stu-id="147aa-103">Update identityProvider</span></span>

> <span data-ttu-id="147aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="147aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="147aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="147aa-106">既存の[identityProvider](../resources/identityprovider.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="147aa-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="147aa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="147aa-107">Permissions</span></span>

<span data-ttu-id="147aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="147aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="147aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="147aa-110">Permission type</span></span>      | <span data-ttu-id="147aa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="147aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="147aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="147aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="147aa-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="147aa-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="147aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="147aa-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="147aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147aa-115">Not supported.</span></span>|
|<span data-ttu-id="147aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="147aa-116">Application</span></span>|<span data-ttu-id="147aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147aa-117">Not supported.</span></span>|

<span data-ttu-id="147aa-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="147aa-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="147aa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="147aa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="147aa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="147aa-120">Request headers</span></span>

|<span data-ttu-id="147aa-121">名前</span><span class="sxs-lookup"><span data-stu-id="147aa-121">Name</span></span>|<span data-ttu-id="147aa-122">説明</span><span class="sxs-lookup"><span data-stu-id="147aa-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="147aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="147aa-123">Authorization</span></span>|<span data-ttu-id="147aa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="147aa-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="147aa-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="147aa-126">Content-Type</span></span>|<span data-ttu-id="147aa-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="147aa-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="147aa-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="147aa-129">Request body</span></span>

<span data-ttu-id="147aa-130">要求の本文には、更新する必要がある 1 つまたは複数のプロパティを使用して JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="147aa-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="147aa-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="147aa-131">Property</span></span>|<span data-ttu-id="147aa-132">型</span><span class="sxs-lookup"><span data-stu-id="147aa-132">Type</span></span>|<span data-ttu-id="147aa-133">説明</span><span class="sxs-lookup"><span data-stu-id="147aa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="147aa-134">clientId</span><span class="sxs-lookup"><span data-stu-id="147aa-134">clientId</span></span>|<span data-ttu-id="147aa-135">String</span><span class="sxs-lookup"><span data-stu-id="147aa-135">String</span></span>|<span data-ttu-id="147aa-136">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="147aa-136">The client ID for the application.</span></span> <span data-ttu-id="147aa-137">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="147aa-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="147aa-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="147aa-138">clientSecret</span></span>|<span data-ttu-id="147aa-139">String</span><span class="sxs-lookup"><span data-stu-id="147aa-139">String</span></span>|<span data-ttu-id="147aa-140">アプリケーションのクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="147aa-140">The client secret for the application.</span></span> <span data-ttu-id="147aa-141">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="147aa-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="147aa-142">名前</span><span class="sxs-lookup"><span data-stu-id="147aa-142">name</span></span>|<span data-ttu-id="147aa-143">String</span><span class="sxs-lookup"><span data-stu-id="147aa-143">String</span></span>|<span data-ttu-id="147aa-144">Id プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="147aa-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="147aa-145">応答</span><span class="sxs-lookup"><span data-stu-id="147aa-145">Response</span></span>

<span data-ttu-id="147aa-146">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="147aa-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="147aa-147">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="147aa-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="147aa-148">使用例</span><span class="sxs-lookup"><span data-stu-id="147aa-148">Example</span></span>

<span data-ttu-id="147aa-149">次の例では、トークンの有効期間の**identityProvider**の定義を更新し、組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="147aa-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="147aa-150">要求</span><span class="sxs-lookup"><span data-stu-id="147aa-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a><span data-ttu-id="147aa-151">応答</span><span class="sxs-lookup"><span data-stu-id="147aa-151">Response</span></span>

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
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->