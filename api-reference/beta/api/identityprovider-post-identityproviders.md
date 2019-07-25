---
title: identityProvider を作成する
description: 表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい  identityProvider  を作成します。
localization_priority: Normal
ms.openlocfilehash: 66f6b9bc009f207ca0eeef096791ce2877d1e45b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857590"
---
# <a name="create-identityprovider"></a><span data-ttu-id="2a63a-103">identityProvider を作成する</span><span class="sxs-lookup"><span data-stu-id="2a63a-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a63a-104">表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい [ identityProvider ](../resources/identityprovider.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="2a63a-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a63a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a63a-105">Permissions</span></span>

<span data-ttu-id="2a63a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a63a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a63a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a63a-108">Permission type</span></span>      | <span data-ttu-id="2a63a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a63a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a63a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a63a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2a63a-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a63a-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="2a63a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a63a-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2a63a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a63a-113">Not supported.</span></span>|
|<span data-ttu-id="2a63a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a63a-114">Application</span></span>|<span data-ttu-id="2a63a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a63a-115">Not supported.</span></span>|

<span data-ttu-id="2a63a-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a63a-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="2a63a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a63a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="2a63a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a63a-118">Request headers</span></span>

|<span data-ttu-id="2a63a-119">名前</span><span class="sxs-lookup"><span data-stu-id="2a63a-119">Name</span></span>|<span data-ttu-id="2a63a-120">説明</span><span class="sxs-lookup"><span data-stu-id="2a63a-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2a63a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a63a-121">Authorization</span></span>|<span data-ttu-id="2a63a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a63a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a63a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a63a-124">Content-Type</span></span>|<span data-ttu-id="2a63a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2a63a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a63a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a63a-127">Request body</span></span>

<span data-ttu-id="2a63a-128">要求本文で、[identityProvider](../resources/identityprovider.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a63a-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="2a63a-129">次の表に示す、すべてのプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="2a63a-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="2a63a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a63a-130">Property</span></span>|<span data-ttu-id="2a63a-131">型</span><span class="sxs-lookup"><span data-stu-id="2a63a-131">Type</span></span>|<span data-ttu-id="2a63a-132">説明</span><span class="sxs-lookup"><span data-stu-id="2a63a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a63a-133">clientId</span><span class="sxs-lookup"><span data-stu-id="2a63a-133">clientId</span></span>|<span data-ttu-id="2a63a-134">String</span><span class="sxs-lookup"><span data-stu-id="2a63a-134">String</span></span>|<span data-ttu-id="2a63a-135">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="2a63a-135">The client ID for the application.</span></span> <span data-ttu-id="2a63a-136">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="2a63a-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="2a63a-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="2a63a-137">clientSecret</span></span>|<span data-ttu-id="2a63a-138">String</span><span class="sxs-lookup"><span data-stu-id="2a63a-138">String</span></span>|<span data-ttu-id="2a63a-139">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="2a63a-139">The client secret for the application.</span></span> <span data-ttu-id="2a63a-140">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="2a63a-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="2a63a-141">name</span><span class="sxs-lookup"><span data-stu-id="2a63a-141">name</span></span>|<span data-ttu-id="2a63a-142">String</span><span class="sxs-lookup"><span data-stu-id="2a63a-142">String</span></span>|<span data-ttu-id="2a63a-143">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2a63a-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="2a63a-144">type</span><span class="sxs-lookup"><span data-stu-id="2a63a-144">type</span></span>|<span data-ttu-id="2a63a-145">String</span><span class="sxs-lookup"><span data-stu-id="2a63a-145">String</span></span>|<span data-ttu-id="2a63a-146">ID プロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="2a63a-146">The identity provider type.</span></span> <span data-ttu-id="2a63a-147">次のいずれかの値であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="2a63a-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="2a63a-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="2a63a-148">Microsoft</span></span><li/><span data-ttu-id="2a63a-149">Google</span><span class="sxs-lookup"><span data-stu-id="2a63a-149">Google</span></span><li/><span data-ttu-id="2a63a-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="2a63a-150">Amazon</span></span><li/><span data-ttu-id="2a63a-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="2a63a-151">LinkedIn</span></span><li/><span data-ttu-id="2a63a-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="2a63a-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="2a63a-153">応答</span><span class="sxs-lookup"><span data-stu-id="2a63a-153">Response</span></span>

<span data-ttu-id="2a63a-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [identityProvider](../resources/identityprovider.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2a63a-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="2a63a-155">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="2a63a-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2a63a-156">例</span><span class="sxs-lookup"><span data-stu-id="2a63a-156">Example</span></span>

<span data-ttu-id="2a63a-157">次の例では、**identityProvider** を作成します。</span><span class="sxs-lookup"><span data-stu-id="2a63a-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="2a63a-158">要求</span><span class="sxs-lookup"><span data-stu-id="2a63a-158">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2a63a-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2a63a-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a63a-160">C#</span><span class="sxs-lookup"><span data-stu-id="2a63a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a63a-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a63a-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a63a-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="2a63a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a63a-163">Java</span><span class="sxs-lookup"><span data-stu-id="2a63a-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a63a-164">応答</span><span class="sxs-lookup"><span data-stu-id="2a63a-164">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
