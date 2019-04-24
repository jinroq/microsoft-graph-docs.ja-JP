---
title: identityProvider を作成する
description: 表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい  identityProvider  を作成します。
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501274"
---
# <a name="create-identityprovider"></a><span data-ttu-id="7014f-103">identityProvider を作成する</span><span class="sxs-lookup"><span data-stu-id="7014f-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7014f-104">表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい [ identityProvider ](../resources/identityprovider.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="7014f-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="7014f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7014f-105">Permissions</span></span>

<span data-ttu-id="7014f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7014f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7014f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7014f-108">Permission type</span></span>      | <span data-ttu-id="7014f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7014f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7014f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7014f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7014f-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7014f-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7014f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7014f-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7014f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7014f-113">Not supported.</span></span>|
|<span data-ttu-id="7014f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7014f-114">Application</span></span>|<span data-ttu-id="7014f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7014f-115">Not supported.</span></span>|

<span data-ttu-id="7014f-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="7014f-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="7014f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7014f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="7014f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7014f-118">Request headers</span></span>

|<span data-ttu-id="7014f-119">名前</span><span class="sxs-lookup"><span data-stu-id="7014f-119">Name</span></span>|<span data-ttu-id="7014f-120">説明</span><span class="sxs-lookup"><span data-stu-id="7014f-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7014f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7014f-121">Authorization</span></span>|<span data-ttu-id="7014f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7014f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7014f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7014f-124">Content-Type</span></span>|<span data-ttu-id="7014f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7014f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7014f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7014f-127">Request body</span></span>

<span data-ttu-id="7014f-128">要求本文で、[identityProvider](../resources/identityprovider.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="7014f-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="7014f-129">次の表に示す、すべてのプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="7014f-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="7014f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7014f-130">Property</span></span>|<span data-ttu-id="7014f-131">型</span><span class="sxs-lookup"><span data-stu-id="7014f-131">Type</span></span>|<span data-ttu-id="7014f-132">説明</span><span class="sxs-lookup"><span data-stu-id="7014f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7014f-133">clientId</span><span class="sxs-lookup"><span data-stu-id="7014f-133">clientId</span></span>|<span data-ttu-id="7014f-134">String</span><span class="sxs-lookup"><span data-stu-id="7014f-134">String</span></span>|<span data-ttu-id="7014f-135">アプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="7014f-135">The client ID for the application.</span></span> <span data-ttu-id="7014f-136">アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="7014f-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7014f-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="7014f-137">clientSecret</span></span>|<span data-ttu-id="7014f-138">String</span><span class="sxs-lookup"><span data-stu-id="7014f-138">String</span></span>|<span data-ttu-id="7014f-139">アプリケーションでのクライアント シークレット。</span><span class="sxs-lookup"><span data-stu-id="7014f-139">The client secret for the application.</span></span> <span data-ttu-id="7014f-140">アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。</span><span class="sxs-lookup"><span data-stu-id="7014f-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7014f-141">name</span><span class="sxs-lookup"><span data-stu-id="7014f-141">name</span></span>|<span data-ttu-id="7014f-142">String</span><span class="sxs-lookup"><span data-stu-id="7014f-142">String</span></span>|<span data-ttu-id="7014f-143">ID プロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="7014f-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="7014f-144">type</span><span class="sxs-lookup"><span data-stu-id="7014f-144">type</span></span>|<span data-ttu-id="7014f-145">String</span><span class="sxs-lookup"><span data-stu-id="7014f-145">String</span></span>|<span data-ttu-id="7014f-146">ID プロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="7014f-146">The identity provider type.</span></span> <span data-ttu-id="7014f-147">次のいずれかの値であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="7014f-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="7014f-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="7014f-148">Microsoft</span></span><li/><span data-ttu-id="7014f-149">Google</span><span class="sxs-lookup"><span data-stu-id="7014f-149">Google</span></span><li/><span data-ttu-id="7014f-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="7014f-150">Amazon</span></span><li/><span data-ttu-id="7014f-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="7014f-151">LinkedIn</span></span><li/><span data-ttu-id="7014f-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="7014f-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="7014f-153">応答</span><span class="sxs-lookup"><span data-stu-id="7014f-153">Response</span></span>

<span data-ttu-id="7014f-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [identityProvider](../resources/identityprovider.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7014f-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="7014f-155">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="7014f-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7014f-156">例</span><span class="sxs-lookup"><span data-stu-id="7014f-156">Example</span></span>

<span data-ttu-id="7014f-157">次の例では、**identityProvider** を作成します。</span><span class="sxs-lookup"><span data-stu-id="7014f-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="7014f-158">要求</span><span class="sxs-lookup"><span data-stu-id="7014f-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="7014f-159">応答</span><span class="sxs-lookup"><span data-stu-id="7014f-159">Response</span></span>

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
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
