---
title: ユーザーを作成する
description: この API を使用して、新しいユーザーを作成します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b65a12336073c2206867bf9540933df0b8d9fec5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449023"
---
# <a name="create-user"></a><span data-ttu-id="72633-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="72633-103">Create User</span></span>

<span data-ttu-id="72633-p101">新しい[ユーザー](../resources/user.md)を作成します。要求本文に、作成するユーザーを含めます。少なくとも、ユーザーについての必須プロパティを指定する必要があります。必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="72633-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="72633-108">外部ユーザーを作成するには、[招待 API](invitation-post.md) を使用します。</span><span class="sxs-lookup"><span data-stu-id="72633-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72633-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72633-109">Permissions</span></span>

<span data-ttu-id="72633-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72633-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72633-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72633-112">Permission type</span></span>      | <span data-ttu-id="72633-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72633-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72633-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72633-114">Delegated (work or school account)</span></span> | <span data-ttu-id="72633-115">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72633-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72633-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72633-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72633-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72633-117">Not supported.</span></span>    |
|<span data-ttu-id="72633-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72633-118">Application</span></span> | <span data-ttu-id="72633-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72633-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72633-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72633-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="72633-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72633-121">Request headers</span></span>

| <span data-ttu-id="72633-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72633-122">Header</span></span>       | <span data-ttu-id="72633-123">値</span><span class="sxs-lookup"><span data-stu-id="72633-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72633-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72633-124">Authorization</span></span>  | <span data-ttu-id="72633-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72633-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72633-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72633-127">Content-Type</span></span>  | <span data-ttu-id="72633-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72633-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72633-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="72633-129">Request body</span></span>

<span data-ttu-id="72633-130">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="72633-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="72633-131">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="72633-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="72633-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="72633-132">Parameter</span></span> | <span data-ttu-id="72633-133">型</span><span class="sxs-lookup"><span data-stu-id="72633-133">Type</span></span> | <span data-ttu-id="72633-134">説明</span><span class="sxs-lookup"><span data-stu-id="72633-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72633-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="72633-135">accountEnabled</span></span> |<span data-ttu-id="72633-136">boolean</span><span class="sxs-lookup"><span data-stu-id="72633-136">boolean</span></span> |<span data-ttu-id="72633-137">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="72633-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="72633-138">displayName</span><span class="sxs-lookup"><span data-stu-id="72633-138">displayName</span></span> |<span data-ttu-id="72633-139">string</span><span class="sxs-lookup"><span data-stu-id="72633-139">string</span></span> |<span data-ttu-id="72633-140">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="72633-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="72633-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="72633-141">onPremisesImmutableId</span></span> |<span data-ttu-id="72633-142">string</span><span class="sxs-lookup"><span data-stu-id="72633-142">string</span></span> |<span data-ttu-id="72633-143">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="72633-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="72633-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="72633-144">mailNickname</span></span> |<span data-ttu-id="72633-145">string</span><span class="sxs-lookup"><span data-stu-id="72633-145">string</span></span> |<span data-ttu-id="72633-146">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="72633-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="72633-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="72633-147">passwordProfile</span></span>|[<span data-ttu-id="72633-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="72633-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="72633-149">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="72633-149">The password profile for the user.</span></span>|
|<span data-ttu-id="72633-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72633-150">userPrincipalName</span></span> |<span data-ttu-id="72633-151">string</span><span class="sxs-lookup"><span data-stu-id="72633-151">string</span></span> |<span data-ttu-id="72633-152">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="72633-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="72633-153">**ユーザー** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにユーザー インスタンスに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="72633-153">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="72633-154">この API を使用して作成されたフェデレーション ユーザーは、既定で 12 時間ごとに強制サインインされます。</span><span class="sxs-lookup"><span data-stu-id="72633-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="72633-155">この設定を変更する方法の詳細については、「[トークンの有効期間の例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72633-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="72633-156">応答</span><span class="sxs-lookup"><span data-stu-id="72633-156">Response</span></span>

<span data-ttu-id="72633-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72633-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72633-158">例</span><span class="sxs-lookup"><span data-stu-id="72633-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="72633-159">要求</span><span class="sxs-lookup"><span data-stu-id="72633-159">Request</span></span>

<span data-ttu-id="72633-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72633-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="72633-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="72633-161">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="72633-162">C#</span><span class="sxs-lookup"><span data-stu-id="72633-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72633-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="72633-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72633-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72633-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="72633-165">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="72633-165">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="72633-166">応答</span><span class="sxs-lookup"><span data-stu-id="72633-166">Response</span></span>

<span data-ttu-id="72633-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72633-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
