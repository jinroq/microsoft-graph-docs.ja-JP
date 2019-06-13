---
title: user の作成
description: 新しいユーザーを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62c57763c41c034b6c93a8e0e40780a9f0ccc69b
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914680"
---
# <a name="create-user"></a><span data-ttu-id="073f7-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="073f7-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="073f7-104">新しいユーザーを作成します。</span><span class="sxs-lookup"><span data-stu-id="073f7-104">Create a new user.</span></span>
<span data-ttu-id="073f7-105">要求本文に、作成するユーザーを含めます。</span><span class="sxs-lookup"><span data-stu-id="073f7-105">The request body contains the user to create.</span></span> <span data-ttu-id="073f7-106">少なくとも、ユーザーについての必須プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="073f7-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="073f7-107">必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="073f7-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="073f7-108">外部ユーザーは、招待状を使用して作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="073f7-108">External users must be created through an invitation.</span></span> <span data-ttu-id="073f7-109">外部ユーザーの作成を有効にする必要がある場合は、「[招待](../resources/invitation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="073f7-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="073f7-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="073f7-110">Permissions</span></span>

<span data-ttu-id="073f7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="073f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="073f7-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="073f7-113">Permission type</span></span>      | <span data-ttu-id="073f7-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="073f7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="073f7-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="073f7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="073f7-116">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="073f7-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="073f7-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="073f7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="073f7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="073f7-118">Not supported.</span></span>    |
|<span data-ttu-id="073f7-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="073f7-119">Application</span></span> | <span data-ttu-id="073f7-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073f7-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="073f7-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="073f7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="073f7-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="073f7-122">Request headers</span></span>
| <span data-ttu-id="073f7-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="073f7-123">Header</span></span>       | <span data-ttu-id="073f7-124">値</span><span class="sxs-lookup"><span data-stu-id="073f7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="073f7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="073f7-125">Authorization</span></span>  | <span data-ttu-id="073f7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="073f7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="073f7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="073f7-128">Content-Type</span></span>  | <span data-ttu-id="073f7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="073f7-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="073f7-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="073f7-130">Request body</span></span>

<span data-ttu-id="073f7-131">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="073f7-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="073f7-132">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="073f7-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="073f7-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="073f7-133">Parameter</span></span> | <span data-ttu-id="073f7-134">型</span><span class="sxs-lookup"><span data-stu-id="073f7-134">Type</span></span> | <span data-ttu-id="073f7-135">説明</span><span class="sxs-lookup"><span data-stu-id="073f7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="073f7-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="073f7-136">accountEnabled</span></span> |<span data-ttu-id="073f7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="073f7-137">Boolean</span></span> |<span data-ttu-id="073f7-138">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="073f7-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="073f7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="073f7-139">displayName</span></span> |<span data-ttu-id="073f7-140">string</span><span class="sxs-lookup"><span data-stu-id="073f7-140">string</span></span> |<span data-ttu-id="073f7-141">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="073f7-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="073f7-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="073f7-142">onPremisesImmutableId</span></span> |<span data-ttu-id="073f7-143">string</span><span class="sxs-lookup"><span data-stu-id="073f7-143">string</span></span> |<span data-ttu-id="073f7-144">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="073f7-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="073f7-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="073f7-145">mailNickname</span></span> |<span data-ttu-id="073f7-146">string</span><span class="sxs-lookup"><span data-stu-id="073f7-146">string</span></span> |<span data-ttu-id="073f7-147">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="073f7-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="073f7-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="073f7-148">passwordProfile</span></span>|[<span data-ttu-id="073f7-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="073f7-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="073f7-150">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="073f7-150">The password profile for the user.</span></span>|
|<span data-ttu-id="073f7-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="073f7-151">userPrincipalName</span></span> |<span data-ttu-id="073f7-152">string</span><span class="sxs-lookup"><span data-stu-id="073f7-152">string</span></span> |<span data-ttu-id="073f7-153">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="073f7-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="073f7-154">**ユーザー**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`POST` 、操作を使用して、作成中にユーザーインスタンスにカスタムプロパティを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="073f7-154">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="073f7-155">この API を使用して作成されたフェデレーションユーザーには、既定で12時間ごとにサインインすることが強制されます。</span><span class="sxs-lookup"><span data-stu-id="073f7-155">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="073f7-156">これを変更する方法の詳細については、「[トークンの有効期間の例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="073f7-156">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="073f7-157">応答</span><span class="sxs-lookup"><span data-stu-id="073f7-157">Response</span></span>

<span data-ttu-id="073f7-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="073f7-158">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073f7-159">例</span><span class="sxs-lookup"><span data-stu-id="073f7-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="073f7-160">要求</span><span class="sxs-lookup"><span data-stu-id="073f7-160">Request</span></span>
<span data-ttu-id="073f7-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="073f7-161">Here is an example of the request.</span></span>
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="073f7-162">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="073f7-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="073f7-163">応答</span><span class="sxs-lookup"><span data-stu-id="073f7-163">Response</span></span>
<span data-ttu-id="073f7-164">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="073f7-164">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="073f7-165">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="073f7-165">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="073f7-166">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="073f7-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="073f7-167">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="073f7-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="073f7-168">C#</span><span class="sxs-lookup"><span data-stu-id="073f7-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="073f7-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="073f7-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="073f7-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="073f7-170">See also</span></span>

- [<span data-ttu-id="073f7-171">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="073f7-171">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="073f7-172">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="073f7-172">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="073f7-173">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="073f7-173">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
