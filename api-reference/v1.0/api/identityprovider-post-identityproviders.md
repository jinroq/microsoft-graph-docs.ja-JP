---
title: identityProvider を作成する
description: 新しい identityProvider を作成する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ffd1f600395a1c72f2ab4c72ef1c3d3a358e387
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016154"
---
# <a name="create-identityprovider"></a><span data-ttu-id="066dc-103">identityProvider を作成する</span><span class="sxs-lookup"><span data-stu-id="066dc-103">Create identityProvider</span></span>

<span data-ttu-id="066dc-104">表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい [ identityProvider ](../resources/identityprovider.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="066dc-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="066dc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="066dc-105">Permissions</span></span>

<span data-ttu-id="066dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="066dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066dc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="066dc-108">Permission type</span></span>      | <span data-ttu-id="066dc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="066dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066dc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="066dc-110">Delegated (work or school account)</span></span>|<span data-ttu-id="066dc-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="066dc-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="066dc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="066dc-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="066dc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066dc-113">Not supported.</span></span>|
|<span data-ttu-id="066dc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="066dc-114">Application</span></span>|<span data-ttu-id="066dc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066dc-115">Not supported.</span></span>|

<span data-ttu-id="066dc-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="066dc-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="066dc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="066dc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="066dc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="066dc-118">Request headers</span></span>

|<span data-ttu-id="066dc-119">名前</span><span class="sxs-lookup"><span data-stu-id="066dc-119">Name</span></span>|<span data-ttu-id="066dc-120">説明</span><span class="sxs-lookup"><span data-stu-id="066dc-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="066dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="066dc-121">Authorization</span></span>|<span data-ttu-id="066dc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="066dc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="066dc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="066dc-124">Content-Type</span></span>|<span data-ttu-id="066dc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="066dc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="066dc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="066dc-127">Request body</span></span>

<span data-ttu-id="066dc-128">要求本文で、[identityProvider](../resources/identityprovider.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="066dc-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="066dc-129">次の表に示す、すべてのプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="066dc-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="066dc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="066dc-130">Property</span></span>|<span data-ttu-id="066dc-131">型</span><span class="sxs-lookup"><span data-stu-id="066dc-131">Type</span></span>|<span data-ttu-id="066dc-132">説明</span><span class="sxs-lookup"><span data-stu-id="066dc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="066dc-133">clientId</span><span class="sxs-lookup"><span data-stu-id="066dc-133">clientId</span></span>|<span data-ttu-id="066dc-134">String</span><span class="sxs-lookup"><span data-stu-id="066dc-134">String</span></span>|<span data-ttu-id="066dc-135">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="066dc-135">The client ID for the application.</span></span> <span data-ttu-id="066dc-136">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="066dc-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="066dc-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="066dc-137">clientSecret</span></span>|<span data-ttu-id="066dc-138">String</span><span class="sxs-lookup"><span data-stu-id="066dc-138">String</span></span>|<span data-ttu-id="066dc-139">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="066dc-139">The client secret for the application.</span></span> <span data-ttu-id="066dc-140">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="066dc-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="066dc-141">name</span><span class="sxs-lookup"><span data-stu-id="066dc-141">name</span></span>|<span data-ttu-id="066dc-142">String</span><span class="sxs-lookup"><span data-stu-id="066dc-142">String</span></span>|<span data-ttu-id="066dc-143">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="066dc-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="066dc-144">type</span><span class="sxs-lookup"><span data-stu-id="066dc-144">type</span></span>|<span data-ttu-id="066dc-145">String</span><span class="sxs-lookup"><span data-stu-id="066dc-145">String</span></span>|<span data-ttu-id="066dc-146">ID プロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="066dc-146">The identity provider type.</span></span> <span data-ttu-id="066dc-147">B2C シナリオでは、この型は次のいずれかの値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="066dc-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="066dc-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="066dc-148">Microsoft</span></span><li/><span data-ttu-id="066dc-149">Google</span><span class="sxs-lookup"><span data-stu-id="066dc-149">Google</span></span><li/><span data-ttu-id="066dc-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="066dc-150">Amazon</span></span><li/><span data-ttu-id="066dc-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="066dc-151">LinkedIn</span></span><li/><span data-ttu-id="066dc-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="066dc-152">Facebook</span></span><li/><span data-ttu-id="066dc-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="066dc-153">GitHub</span></span><li/><span data-ttu-id="066dc-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="066dc-154">Twitter</span></span><li/><span data-ttu-id="066dc-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="066dc-155">Weibo</span></span><li/><span data-ttu-id="066dc-156">QQ</span><span class="sxs-lookup"><span data-stu-id="066dc-156">QQ</span></span><li/><span data-ttu-id="066dc-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="066dc-157">WeChat</span></span></ul><span data-ttu-id="066dc-158">B2B には Google のみ</span><span class="sxs-lookup"><span data-stu-id="066dc-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="066dc-159">応答</span><span class="sxs-lookup"><span data-stu-id="066dc-159">Response</span></span>

<span data-ttu-id="066dc-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [identityProvider](../resources/identityprovider.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="066dc-160">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="066dc-161">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="066dc-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="066dc-162">例</span><span class="sxs-lookup"><span data-stu-id="066dc-162">Example</span></span>

<span data-ttu-id="066dc-163">次の例では、**identityProvider** を作成します。</span><span class="sxs-lookup"><span data-stu-id="066dc-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="066dc-164">要求</span><span class="sxs-lookup"><span data-stu-id="066dc-164">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="066dc-165">応答</span><span class="sxs-lookup"><span data-stu-id="066dc-165">Response</span></span>

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


