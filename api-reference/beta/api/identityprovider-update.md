---
title: IdentityProvider を更新します。
description: 既存の identityProvider プロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: d98bc5d0bd7a8f165f33c89548a69805039cdf07
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525746"
---
# <a name="update-identityprovider"></a><span data-ttu-id="7b43a-103">IdentityProvider を更新します。</span><span class="sxs-lookup"><span data-stu-id="7b43a-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b43a-104">既存の[identityProvider](../resources/identityprovider.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b43a-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b43a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b43a-105">Permissions</span></span>

<span data-ttu-id="7b43a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b43a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b43a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b43a-108">Permission type</span></span>      | <span data-ttu-id="7b43a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b43a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b43a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b43a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7b43a-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b43a-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7b43a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b43a-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7b43a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b43a-113">Not supported.</span></span>|
|<span data-ttu-id="7b43a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b43a-114">Application</span></span>|<span data-ttu-id="7b43a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b43a-115">Not supported.</span></span>|

<span data-ttu-id="7b43a-116">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b43a-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="7b43a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b43a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b43a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b43a-118">Request headers</span></span>

|<span data-ttu-id="7b43a-119">名前</span><span class="sxs-lookup"><span data-stu-id="7b43a-119">Name</span></span>|<span data-ttu-id="7b43a-120">説明</span><span class="sxs-lookup"><span data-stu-id="7b43a-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7b43a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b43a-121">Authorization</span></span>|<span data-ttu-id="7b43a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b43a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7b43a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b43a-124">Content-Type</span></span>|<span data-ttu-id="7b43a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7b43a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b43a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b43a-127">Request body</span></span>

<span data-ttu-id="7b43a-128">要求の本文には、更新する必要がある 1 つまたは複数のプロパティを使用して JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="7b43a-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="7b43a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b43a-129">Property</span></span>|<span data-ttu-id="7b43a-130">型</span><span class="sxs-lookup"><span data-stu-id="7b43a-130">Type</span></span>|<span data-ttu-id="7b43a-131">説明</span><span class="sxs-lookup"><span data-stu-id="7b43a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b43a-132">clientId</span><span class="sxs-lookup"><span data-stu-id="7b43a-132">clientId</span></span>|<span data-ttu-id="7b43a-133">String</span><span class="sxs-lookup"><span data-stu-id="7b43a-133">String</span></span>|<span data-ttu-id="7b43a-134">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="7b43a-134">The client ID for the application.</span></span> <span data-ttu-id="7b43a-135">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="7b43a-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7b43a-136">client_secret</span><span class="sxs-lookup"><span data-stu-id="7b43a-136">clientSecret</span></span>|<span data-ttu-id="7b43a-137">String</span><span class="sxs-lookup"><span data-stu-id="7b43a-137">String</span></span>|<span data-ttu-id="7b43a-138">アプリケーションのクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="7b43a-138">The client secret for the application.</span></span> <span data-ttu-id="7b43a-139">これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。</span><span class="sxs-lookup"><span data-stu-id="7b43a-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7b43a-140">name</span><span class="sxs-lookup"><span data-stu-id="7b43a-140">name</span></span>|<span data-ttu-id="7b43a-141">String</span><span class="sxs-lookup"><span data-stu-id="7b43a-141">String</span></span>|<span data-ttu-id="7b43a-142">Id プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="7b43a-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="7b43a-143">応答</span><span class="sxs-lookup"><span data-stu-id="7b43a-143">Response</span></span>

<span data-ttu-id="7b43a-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7b43a-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7b43a-145">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="7b43a-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7b43a-146">例</span><span class="sxs-lookup"><span data-stu-id="7b43a-146">Example</span></span>

<span data-ttu-id="7b43a-147">次の例では、トークンの有効期間の**identityProvider**の定義を更新し、組織の既定値として設定します。</span><span class="sxs-lookup"><span data-stu-id="7b43a-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7b43a-148">要求</span><span class="sxs-lookup"><span data-stu-id="7b43a-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="7b43a-149">応答</span><span class="sxs-lookup"><span data-stu-id="7b43a-149">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
