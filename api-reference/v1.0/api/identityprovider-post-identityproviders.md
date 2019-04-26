---
title: identityProvider を作成する
description: 新しい identityProvider を作成する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a33354c35903fedc3efedb84e9f2ed7bc20c9506
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577659"
---
# <a name="create-identityprovider"></a><span data-ttu-id="4b5e4-103">identityProvider を作成する</span><span class="sxs-lookup"><span data-stu-id="4b5e4-103">Create identityProvider</span></span>

<span data-ttu-id="4b5e4-104">表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい [ identityProvider ](../resources/identityprovider.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b5e4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4b5e4-105">Permissions</span></span>

<span data-ttu-id="4b5e4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5e4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b5e4-108">Permission type</span></span>      | <span data-ttu-id="4b5e4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b5e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b5e4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b5e4-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4b5e4-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5e4-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5e4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b5e4-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4b5e4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-113">Not supported.</span></span>|
|<span data-ttu-id="4b5e4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b5e4-114">Application</span></span>|<span data-ttu-id="4b5e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-115">Not supported.</span></span>|

<span data-ttu-id="4b5e4-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b5e4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b5e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="4b5e4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b5e4-118">Request headers</span></span>

|<span data-ttu-id="4b5e4-119">名前</span><span class="sxs-lookup"><span data-stu-id="4b5e4-119">Name</span></span>|<span data-ttu-id="4b5e4-120">説明</span><span class="sxs-lookup"><span data-stu-id="4b5e4-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4b5e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b5e4-121">Authorization</span></span>|<span data-ttu-id="4b5e4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4b5e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b5e4-124">Content-Type</span></span>|<span data-ttu-id="4b5e4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4b5e4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5e4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b5e4-127">Request body</span></span>

<span data-ttu-id="4b5e4-128">要求本文で、[identityProvider](../resources/identityProvider.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityProvider.md) object.</span></span> <span data-ttu-id="4b5e4-129">次の表に示す、すべてのプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="4b5e4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5e4-130">Property</span></span>|<span data-ttu-id="4b5e4-131">型</span><span class="sxs-lookup"><span data-stu-id="4b5e4-131">Type</span></span>|<span data-ttu-id="4b5e4-132">説明</span><span class="sxs-lookup"><span data-stu-id="4b5e4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b5e4-133">clientId</span><span class="sxs-lookup"><span data-stu-id="4b5e4-133">clientId</span></span>|<span data-ttu-id="4b5e4-134">String</span><span class="sxs-lookup"><span data-stu-id="4b5e4-134">String</span></span>|<span data-ttu-id="4b5e4-135">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-135">The client ID for the application.</span></span> <span data-ttu-id="4b5e4-136">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4b5e4-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="4b5e4-137">clientSecret</span></span>|<span data-ttu-id="4b5e4-138">String</span><span class="sxs-lookup"><span data-stu-id="4b5e4-138">String</span></span>|<span data-ttu-id="4b5e4-139">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-139">The client secret for the application.</span></span> <span data-ttu-id="4b5e4-140">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4b5e4-141">name</span><span class="sxs-lookup"><span data-stu-id="4b5e4-141">name</span></span>|<span data-ttu-id="4b5e4-142">String</span><span class="sxs-lookup"><span data-stu-id="4b5e4-142">String</span></span>|<span data-ttu-id="4b5e4-143">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="4b5e4-144">type</span><span class="sxs-lookup"><span data-stu-id="4b5e4-144">type</span></span>|<span data-ttu-id="4b5e4-145">String</span><span class="sxs-lookup"><span data-stu-id="4b5e4-145">String</span></span>|<span data-ttu-id="4b5e4-146">ID プロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-146">The identity provider type.</span></span> <span data-ttu-id="4b5e4-147">B2C シナリオでは、この型は次のいずれかの値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="4b5e4-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="4b5e4-148">Microsoft</span></span><li/><span data-ttu-id="4b5e4-149">Google</span><span class="sxs-lookup"><span data-stu-id="4b5e4-149">Google</span></span><li/><span data-ttu-id="4b5e4-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="4b5e4-150">Amazon</span></span><li/><span data-ttu-id="4b5e4-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="4b5e4-151">LinkedIn</span></span><li/><span data-ttu-id="4b5e4-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="4b5e4-152">Facebook</span></span><li/><span data-ttu-id="4b5e4-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="4b5e4-153">GitHub</span></span><li/><span data-ttu-id="4b5e4-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="4b5e4-154">Twitter</span></span><li/><span data-ttu-id="4b5e4-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="4b5e4-155">Weibo</span></span><li/><span data-ttu-id="4b5e4-156">QQ</span><span class="sxs-lookup"><span data-stu-id="4b5e4-156">QQ</span></span><li/><span data-ttu-id="4b5e4-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="4b5e4-157">WeChat</span></span></ul><span data-ttu-id="4b5e4-158">B2B には Google のみ</span><span class="sxs-lookup"><span data-stu-id="4b5e4-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="4b5e4-159">応答</span><span class="sxs-lookup"><span data-stu-id="4b5e4-159">Response</span></span>

<span data-ttu-id="4b5e4-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [identityProvider](../resources/identityProvider.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-160">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityProvider.md) object in the response body.</span></span> <span data-ttu-id="4b5e4-161">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="4b5e4-162">例</span><span class="sxs-lookup"><span data-stu-id="4b5e4-162">Example</span></span>

<span data-ttu-id="4b5e4-163">次の例では、**identityProvider** を作成します。</span><span class="sxs-lookup"><span data-stu-id="4b5e4-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="4b5e4-164">要求</span><span class="sxs-lookup"><span data-stu-id="4b5e4-164">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="4b5e4-165">応答</span><span class="sxs-lookup"><span data-stu-id="4b5e4-165">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


