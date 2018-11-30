---
title: IdentityProvider を作成します。
description: 新しい identityProvider を作成するには、表示名、identityProvider の種類、クライアント ID とクライアント シークレットを指定します。
ms.openlocfilehash: 8786cbf6676567a0c6aaef5bf497f50cff1ce9a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071025"
---
# <a name="create-identityprovider"></a><span data-ttu-id="1f894-103">IdentityProvider を作成します。</span><span class="sxs-lookup"><span data-stu-id="1f894-103">Create identityProvider</span></span>

> <span data-ttu-id="1f894-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f894-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f894-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f894-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f894-106">新しい[identityProvider](../resources/identityprovider.md)を作成するには、表示名、identityProvider の種類、クライアント ID とクライアント シークレットを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f894-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f894-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f894-107">Permissions</span></span>

<span data-ttu-id="1f894-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f894-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f894-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f894-110">Permission type</span></span>      | <span data-ttu-id="1f894-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f894-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f894-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f894-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f894-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f894-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1f894-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f894-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1f894-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f894-115">Not supported.</span></span>|
|<span data-ttu-id="1f894-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f894-116">Application</span></span>|<span data-ttu-id="1f894-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f894-117">Not supported.</span></span>|

<span data-ttu-id="1f894-118">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f894-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1f894-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f894-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="1f894-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f894-120">Request headers</span></span>

|<span data-ttu-id="1f894-121">名前</span><span class="sxs-lookup"><span data-stu-id="1f894-121">Name</span></span>|<span data-ttu-id="1f894-122">説明</span><span class="sxs-lookup"><span data-stu-id="1f894-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1f894-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f894-123">Authorization</span></span>|<span data-ttu-id="1f894-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f894-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f894-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f894-126">Content-Type</span></span>|<span data-ttu-id="1f894-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1f894-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f894-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f894-129">Request body</span></span>

<span data-ttu-id="1f894-130">要求の本文には、 [identityProvider](../resources/identityprovider.md)オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="1f894-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="1f894-131">次の表に記載されているすべてのプロパティは、必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f894-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="1f894-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f894-132">Property</span></span>|<span data-ttu-id="1f894-133">型</span><span class="sxs-lookup"><span data-stu-id="1f894-133">Type</span></span>|<span data-ttu-id="1f894-134">説明</span><span class="sxs-lookup"><span data-stu-id="1f894-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f894-135">clientId</span><span class="sxs-lookup"><span data-stu-id="1f894-135">clientId</span></span>|<span data-ttu-id="1f894-136">String</span><span class="sxs-lookup"><span data-stu-id="1f894-136">String</span></span>|<span data-ttu-id="1f894-137">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="1f894-137">The client ID for the application.</span></span> <span data-ttu-id="1f894-138">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="1f894-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="1f894-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="1f894-139">clientSecret</span></span>|<span data-ttu-id="1f894-140">String</span><span class="sxs-lookup"><span data-stu-id="1f894-140">String</span></span>|<span data-ttu-id="1f894-141">アプリケーションのクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="1f894-141">The client secret for the application.</span></span> <span data-ttu-id="1f894-142">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="1f894-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="1f894-143">名前</span><span class="sxs-lookup"><span data-stu-id="1f894-143">name</span></span>|<span data-ttu-id="1f894-144">String</span><span class="sxs-lookup"><span data-stu-id="1f894-144">String</span></span>|<span data-ttu-id="1f894-145">Id プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1f894-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="1f894-146">type</span><span class="sxs-lookup"><span data-stu-id="1f894-146">type</span></span>|<span data-ttu-id="1f894-147">String</span><span class="sxs-lookup"><span data-stu-id="1f894-147">String</span></span>|<span data-ttu-id="1f894-148">Id プロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="1f894-148">The identity provider type.</span></span> <span data-ttu-id="1f894-149">次の値のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f894-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="1f894-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="1f894-150">Microsoft</span></span><li/><span data-ttu-id="1f894-151">Google</span><span class="sxs-lookup"><span data-stu-id="1f894-151">Google</span></span><li/><span data-ttu-id="1f894-152">アマゾン</span><span class="sxs-lookup"><span data-stu-id="1f894-152">Amazon</span></span><li/><span data-ttu-id="1f894-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="1f894-153">LinkedIn</span></span><li/><span data-ttu-id="1f894-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="1f894-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="1f894-155">応答</span><span class="sxs-lookup"><span data-stu-id="1f894-155">Response</span></span>

<span data-ttu-id="1f894-156">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[identityProvider](../resources/identityprovider.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1f894-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="1f894-157">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="1f894-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1f894-158">使用例</span><span class="sxs-lookup"><span data-stu-id="1f894-158">Example</span></span>

<span data-ttu-id="1f894-159">次の使用例は、 **identityProvider**を作成します。</span><span class="sxs-lookup"><span data-stu-id="1f894-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="1f894-160">要求</span><span class="sxs-lookup"><span data-stu-id="1f894-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="1f894-161">応答</span><span class="sxs-lookup"><span data-stu-id="1f894-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
