---
title: identityProvider を更新する
description: '既存の identityprovider.readwrite.all: のプロパティを更新します。'
localization_priority: Normal
ms.openlocfilehash: c73a96a5447a9f6dc8408b7abbb52dc5b7ee68a6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328596"
---
# <a name="update-identityprovider"></a><span data-ttu-id="598b7-103">identityProvider を更新する</span><span class="sxs-lookup"><span data-stu-id="598b7-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="598b7-104">既存の [identityProvider](../resources/identityprovider.md) のプロパティを更新する。</span><span class="sxs-lookup"><span data-stu-id="598b7-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="598b7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="598b7-105">Permissions</span></span>

<span data-ttu-id="598b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="598b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="598b7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="598b7-108">Permission type</span></span>      | <span data-ttu-id="598b7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="598b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="598b7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="598b7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="598b7-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598b7-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="598b7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="598b7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="598b7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="598b7-113">Not supported.</span></span>|
|<span data-ttu-id="598b7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="598b7-114">Application</span></span>|<span data-ttu-id="598b7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="598b7-115">Not supported.</span></span>|

<span data-ttu-id="598b7-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="598b7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="598b7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="598b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="598b7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="598b7-118">Request headers</span></span>

|<span data-ttu-id="598b7-119">名前</span><span class="sxs-lookup"><span data-stu-id="598b7-119">Name</span></span>|<span data-ttu-id="598b7-120">説明</span><span class="sxs-lookup"><span data-stu-id="598b7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="598b7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="598b7-121">Authorization</span></span>|<span data-ttu-id="598b7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="598b7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="598b7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="598b7-124">Content-Type</span></span>|<span data-ttu-id="598b7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="598b7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="598b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="598b7-127">Request body</span></span>

<span data-ttu-id="598b7-128">要求本文で、更新が必要なプロパティを 1 つまたは複数持つ JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="598b7-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="598b7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="598b7-129">Property</span></span>|<span data-ttu-id="598b7-130">型</span><span class="sxs-lookup"><span data-stu-id="598b7-130">Type</span></span>|<span data-ttu-id="598b7-131">説明</span><span class="sxs-lookup"><span data-stu-id="598b7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="598b7-132">clientId</span><span class="sxs-lookup"><span data-stu-id="598b7-132">clientId</span></span>|<span data-ttu-id="598b7-133">String</span><span class="sxs-lookup"><span data-stu-id="598b7-133">String</span></span>|<span data-ttu-id="598b7-134">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="598b7-134">The client ID for the application.</span></span> <span data-ttu-id="598b7-135">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="598b7-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="598b7-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="598b7-136">clientSecret</span></span>|<span data-ttu-id="598b7-137">String</span><span class="sxs-lookup"><span data-stu-id="598b7-137">String</span></span>|<span data-ttu-id="598b7-138">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="598b7-138">The client secret for the application.</span></span> <span data-ttu-id="598b7-139">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="598b7-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="598b7-140">name</span><span class="sxs-lookup"><span data-stu-id="598b7-140">name</span></span>|<span data-ttu-id="598b7-141">String</span><span class="sxs-lookup"><span data-stu-id="598b7-141">String</span></span>|<span data-ttu-id="598b7-142">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="598b7-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="598b7-143">応答</span><span class="sxs-lookup"><span data-stu-id="598b7-143">Response</span></span>

<span data-ttu-id="598b7-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="598b7-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="598b7-145">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="598b7-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="598b7-146">例</span><span class="sxs-lookup"><span data-stu-id="598b7-146">Example</span></span>

<span data-ttu-id="598b7-147">次の例では、トークンの有効期間の定義 **identityProvider** を更新し、それを組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="598b7-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="598b7-148">要求</span><span class="sxs-lookup"><span data-stu-id="598b7-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="598b7-149">応答</span><span class="sxs-lookup"><span data-stu-id="598b7-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
