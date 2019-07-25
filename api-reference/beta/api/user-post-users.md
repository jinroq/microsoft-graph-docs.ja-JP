---
title: user の作成
description: 新しいユーザーを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b14b07c1c252cc58cabcdb152c64d3303ef9cc66
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866794"
---
# <a name="create-user"></a><span data-ttu-id="77af6-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="77af6-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77af6-104">新しい[ユーザー](../resources/user.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="77af6-104">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="77af6-105">要求本文に、作成するユーザーを含めます。</span><span class="sxs-lookup"><span data-stu-id="77af6-105">The request body contains the user to create.</span></span> <span data-ttu-id="77af6-106">少なくとも、ユーザーについての必須プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77af6-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="77af6-107">必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="77af6-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="77af6-108">外部ユーザーを作成するには、[招待 API](invitation-post.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="77af6-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="77af6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77af6-109">Permissions</span></span>

<span data-ttu-id="77af6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77af6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77af6-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77af6-112">Permission type</span></span>      | <span data-ttu-id="77af6-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77af6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77af6-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77af6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="77af6-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77af6-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77af6-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77af6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77af6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77af6-117">Not supported.</span></span>    |
|<span data-ttu-id="77af6-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77af6-118">Application</span></span> | <span data-ttu-id="77af6-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77af6-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77af6-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77af6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="77af6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77af6-121">Request headers</span></span>
| <span data-ttu-id="77af6-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77af6-122">Header</span></span>       | <span data-ttu-id="77af6-123">値</span><span class="sxs-lookup"><span data-stu-id="77af6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77af6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77af6-124">Authorization</span></span>  | <span data-ttu-id="77af6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77af6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="77af6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77af6-127">Content-Type</span></span>  | <span data-ttu-id="77af6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77af6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77af6-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="77af6-129">Request body</span></span>

<span data-ttu-id="77af6-130">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77af6-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="77af6-131">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="77af6-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="77af6-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="77af6-132">Parameter</span></span> | <span data-ttu-id="77af6-133">型</span><span class="sxs-lookup"><span data-stu-id="77af6-133">Type</span></span> | <span data-ttu-id="77af6-134">説明</span><span class="sxs-lookup"><span data-stu-id="77af6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77af6-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="77af6-135">accountEnabled</span></span> |<span data-ttu-id="77af6-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="77af6-136">Boolean</span></span> |<span data-ttu-id="77af6-137">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="77af6-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="77af6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="77af6-138">displayName</span></span> |<span data-ttu-id="77af6-139">string</span><span class="sxs-lookup"><span data-stu-id="77af6-139">string</span></span> |<span data-ttu-id="77af6-140">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="77af6-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="77af6-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="77af6-141">onPremisesImmutableId</span></span> |<span data-ttu-id="77af6-142">string</span><span class="sxs-lookup"><span data-stu-id="77af6-142">string</span></span> |<span data-ttu-id="77af6-143">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="77af6-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="77af6-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="77af6-144">mailNickname</span></span> |<span data-ttu-id="77af6-145">string</span><span class="sxs-lookup"><span data-stu-id="77af6-145">string</span></span> |<span data-ttu-id="77af6-146">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="77af6-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="77af6-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="77af6-147">passwordProfile</span></span>|[<span data-ttu-id="77af6-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="77af6-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="77af6-149">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="77af6-149">The password profile for the user.</span></span>|
|<span data-ttu-id="77af6-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="77af6-150">userPrincipalName</span></span> |<span data-ttu-id="77af6-151">string</span><span class="sxs-lookup"><span data-stu-id="77af6-151">string</span></span> |<span data-ttu-id="77af6-152">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="77af6-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="77af6-153">**ユーザー**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`POST` 、操作を使用して、作成中にユーザーインスタンスにカスタムプロパティを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="77af6-153">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="77af6-154">この API を使用して作成されたフェデレーションユーザーには、既定で12時間ごとにサインインすることが強制されます。</span><span class="sxs-lookup"><span data-stu-id="77af6-154">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="77af6-155">これを変更する方法の詳細については、「[トークンの有効期間の例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77af6-155">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="77af6-156">応答</span><span class="sxs-lookup"><span data-stu-id="77af6-156">Response</span></span>

<span data-ttu-id="77af6-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77af6-157">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77af6-158">例</span><span class="sxs-lookup"><span data-stu-id="77af6-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77af6-159">要求</span><span class="sxs-lookup"><span data-stu-id="77af6-159">Request</span></span>
<span data-ttu-id="77af6-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77af6-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77af6-161">プロトコル</span><span class="sxs-lookup"><span data-stu-id="77af6-161">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77af6-162">C#</span><span class="sxs-lookup"><span data-stu-id="77af6-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77af6-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="77af6-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77af6-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="77af6-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77af6-165">Java</span><span class="sxs-lookup"><span data-stu-id="77af6-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="77af6-166">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77af6-166">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="77af6-167">応答</span><span class="sxs-lookup"><span data-stu-id="77af6-167">Response</span></span>
<span data-ttu-id="77af6-168">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="77af6-168">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="77af6-169">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="77af6-169">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77af6-170">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="77af6-170">All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="77af6-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="77af6-171">See also</span></span>

- [<span data-ttu-id="77af6-172">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="77af6-172">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="77af6-173">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="77af6-173">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="77af6-174">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="77af6-174">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
  ]
}
-->
