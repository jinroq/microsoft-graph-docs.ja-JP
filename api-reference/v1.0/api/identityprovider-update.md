---
title: identityProvider を更新する
description: 既存の identityProvider のプロパティを更新する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3831045172c7c3b6a0d116bd28f5dfc4462ec582
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613284"
---
# <a name="update-identityprovider"></a><span data-ttu-id="c0688-103">identityProvider を更新する</span><span class="sxs-lookup"><span data-stu-id="c0688-103">Update identityProvider</span></span>

<span data-ttu-id="c0688-104">既存の [identityProvider](../resources/identityprovider.md) のプロパティを更新する。</span><span class="sxs-lookup"><span data-stu-id="c0688-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0688-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0688-105">Permissions</span></span>

<span data-ttu-id="c0688-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0688-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0688-108">Permission type</span></span>      | <span data-ttu-id="c0688-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0688-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0688-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0688-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c0688-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0688-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c0688-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0688-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c0688-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0688-113">Not supported.</span></span>|
|<span data-ttu-id="c0688-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0688-114">Application</span></span>|<span data-ttu-id="c0688-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0688-115">Not supported.</span></span>|

<span data-ttu-id="c0688-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0688-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c0688-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0688-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0688-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0688-118">Request headers</span></span>

|<span data-ttu-id="c0688-119">名前</span><span class="sxs-lookup"><span data-stu-id="c0688-119">Name</span></span>|<span data-ttu-id="c0688-120">説明</span><span class="sxs-lookup"><span data-stu-id="c0688-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c0688-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0688-121">Authorization</span></span>|<span data-ttu-id="c0688-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0688-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c0688-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0688-124">Content-Type</span></span>|<span data-ttu-id="c0688-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c0688-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0688-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0688-127">Request body</span></span>

<span data-ttu-id="c0688-128">要求本文で、更新が必要なプロパティを 1 つまたは複数持つ JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="c0688-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="c0688-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0688-129">Property</span></span>|<span data-ttu-id="c0688-130">型</span><span class="sxs-lookup"><span data-stu-id="c0688-130">Type</span></span>|<span data-ttu-id="c0688-131">説明</span><span class="sxs-lookup"><span data-stu-id="c0688-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0688-132">clientId</span><span class="sxs-lookup"><span data-stu-id="c0688-132">clientId</span></span>|<span data-ttu-id="c0688-133">String</span><span class="sxs-lookup"><span data-stu-id="c0688-133">String</span></span>|<span data-ttu-id="c0688-134">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="c0688-134">The client ID for the application.</span></span> <span data-ttu-id="c0688-135">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="c0688-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c0688-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="c0688-136">clientSecret</span></span>|<span data-ttu-id="c0688-137">String</span><span class="sxs-lookup"><span data-stu-id="c0688-137">String</span></span>|<span data-ttu-id="c0688-138">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="c0688-138">The client secret for the application.</span></span> <span data-ttu-id="c0688-139">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="c0688-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c0688-140">name</span><span class="sxs-lookup"><span data-stu-id="c0688-140">name</span></span>|<span data-ttu-id="c0688-141">String</span><span class="sxs-lookup"><span data-stu-id="c0688-141">String</span></span>|<span data-ttu-id="c0688-142">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c0688-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="c0688-143">応答</span><span class="sxs-lookup"><span data-stu-id="c0688-143">Response</span></span>

<span data-ttu-id="c0688-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c0688-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="c0688-145">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="c0688-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c0688-146">例</span><span class="sxs-lookup"><span data-stu-id="c0688-146">Example</span></span>

<span data-ttu-id="c0688-147">次の例では、トークンの有効期間の定義 **identityProvider** を更新し、それを組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="c0688-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="c0688-148">要求</span><span class="sxs-lookup"><span data-stu-id="c0688-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a><span data-ttu-id="c0688-149">応答</span><span class="sxs-lookup"><span data-stu-id="c0688-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c0688-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c0688-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c0688-151">C#</span><span class="sxs-lookup"><span data-stu-id="c0688-151">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0688-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0688-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-identityprovider-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
