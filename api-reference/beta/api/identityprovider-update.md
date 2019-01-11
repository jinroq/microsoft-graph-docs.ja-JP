---
title: IdentityProvider を更新します。
description: 既存の identityProvider プロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: ebe49fb562f77004edfa3504130fbf50f4d40003
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832810"
---
# <a name="update-identityprovider"></a><span data-ttu-id="d0a5a-103">IdentityProvider を更新します。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-103">Update identityProvider</span></span>

> <span data-ttu-id="d0a5a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0a5a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0a5a-106">既存の[identityProvider](../resources/identityprovider.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0a5a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0a5a-107">Permissions</span></span>

<span data-ttu-id="d0a5a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0a5a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0a5a-110">Permission type</span></span>      | <span data-ttu-id="d0a5a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0a5a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0a5a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0a5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0a5a-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a5a-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d0a5a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0a5a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d0a5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-115">Not supported.</span></span>|
|<span data-ttu-id="d0a5a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0a5a-116">Application</span></span>|<span data-ttu-id="d0a5a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-117">Not supported.</span></span>|

<span data-ttu-id="d0a5a-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0a5a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0a5a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d0a5a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0a5a-120">Request headers</span></span>

|<span data-ttu-id="d0a5a-121">名前</span><span class="sxs-lookup"><span data-stu-id="d0a5a-121">Name</span></span>|<span data-ttu-id="d0a5a-122">説明</span><span class="sxs-lookup"><span data-stu-id="d0a5a-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d0a5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0a5a-123">Authorization</span></span>|<span data-ttu-id="d0a5a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0a5a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0a5a-126">Content-Type</span></span>|<span data-ttu-id="d0a5a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d0a5a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0a5a-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0a5a-129">Request body</span></span>

<span data-ttu-id="d0a5a-130">要求の本文には、更新する必要がある 1 つまたは複数のプロパティを使用して JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="d0a5a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0a5a-131">Property</span></span>|<span data-ttu-id="d0a5a-132">種類</span><span class="sxs-lookup"><span data-stu-id="d0a5a-132">Type</span></span>|<span data-ttu-id="d0a5a-133">説明</span><span class="sxs-lookup"><span data-stu-id="d0a5a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0a5a-134">clientId</span><span class="sxs-lookup"><span data-stu-id="d0a5a-134">clientId</span></span>|<span data-ttu-id="d0a5a-135">String</span><span class="sxs-lookup"><span data-stu-id="d0a5a-135">String</span></span>|<span data-ttu-id="d0a5a-136">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-136">The client ID for the application.</span></span> <span data-ttu-id="d0a5a-137">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="d0a5a-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d0a5a-138">clientSecret</span></span>|<span data-ttu-id="d0a5a-139">String</span><span class="sxs-lookup"><span data-stu-id="d0a5a-139">String</span></span>|<span data-ttu-id="d0a5a-140">アプリケーションのクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-140">The client secret for the application.</span></span> <span data-ttu-id="d0a5a-141">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="d0a5a-142">名前</span><span class="sxs-lookup"><span data-stu-id="d0a5a-142">name</span></span>|<span data-ttu-id="d0a5a-143">String</span><span class="sxs-lookup"><span data-stu-id="d0a5a-143">String</span></span>|<span data-ttu-id="d0a5a-144">Id プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="d0a5a-145">応答</span><span class="sxs-lookup"><span data-stu-id="d0a5a-145">Response</span></span>

<span data-ttu-id="d0a5a-146">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d0a5a-147">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d0a5a-148">例</span><span class="sxs-lookup"><span data-stu-id="d0a5a-148">Example</span></span>

<span data-ttu-id="d0a5a-149">次の例では、トークンの有効期間の**identityProvider**の定義を更新し、組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="d0a5a-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="d0a5a-150">要求</span><span class="sxs-lookup"><span data-stu-id="d0a5a-150">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d0a5a-151">応答</span><span class="sxs-lookup"><span data-stu-id="d0a5a-151">Response</span></span>

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
