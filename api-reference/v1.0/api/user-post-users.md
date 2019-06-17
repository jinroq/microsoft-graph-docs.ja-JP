---
title: ユーザーを作成する
description: この API を使用して、新しいユーザーを作成します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f023c8882600952feeacffea62b90dc167cf58a
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914687"
---
# <a name="create-user"></a><span data-ttu-id="d19ca-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="d19ca-103">Create User</span></span>

<span data-ttu-id="d19ca-p101">新しいユーザーを作成します。要求本文に、作成するユーザーを含めます。少なくとも、ユーザーについての必須プロパティを指定する必要があります。必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="d19ca-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="d19ca-108">招待状を通して外部ユーザーを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d19ca-108">External users must be created through an invitation.</span></span> <span data-ttu-id="d19ca-109">外部ユーザーの作成を有効にする必要がある場合は、「[招待](../resources/invitation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d19ca-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d19ca-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d19ca-110">Permissions</span></span>

<span data-ttu-id="d19ca-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d19ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d19ca-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d19ca-113">Permission type</span></span>      | <span data-ttu-id="d19ca-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d19ca-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d19ca-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d19ca-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d19ca-116">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d19ca-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d19ca-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d19ca-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d19ca-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d19ca-118">Not supported.</span></span>    |
|<span data-ttu-id="d19ca-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d19ca-119">Application</span></span> | <span data-ttu-id="d19ca-120">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d19ca-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d19ca-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d19ca-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="d19ca-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d19ca-122">Request headers</span></span>

| <span data-ttu-id="d19ca-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d19ca-123">Header</span></span>       | <span data-ttu-id="d19ca-124">値</span><span class="sxs-lookup"><span data-stu-id="d19ca-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d19ca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d19ca-125">Authorization</span></span>  | <span data-ttu-id="d19ca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d19ca-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d19ca-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d19ca-128">Content-Type</span></span>  | <span data-ttu-id="d19ca-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d19ca-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d19ca-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="d19ca-130">Request body</span></span>

<span data-ttu-id="d19ca-131">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d19ca-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="d19ca-132">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d19ca-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="d19ca-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d19ca-133">Parameter</span></span> | <span data-ttu-id="d19ca-134">型</span><span class="sxs-lookup"><span data-stu-id="d19ca-134">Type</span></span> | <span data-ttu-id="d19ca-135">説明</span><span class="sxs-lookup"><span data-stu-id="d19ca-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d19ca-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="d19ca-136">accountEnabled</span></span> |<span data-ttu-id="d19ca-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d19ca-137">boolean</span></span> |<span data-ttu-id="d19ca-138">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="d19ca-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="d19ca-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d19ca-139">displayName</span></span> |<span data-ttu-id="d19ca-140">string</span><span class="sxs-lookup"><span data-stu-id="d19ca-140">string</span></span> |<span data-ttu-id="d19ca-141">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="d19ca-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="d19ca-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="d19ca-142">onPremisesImmutableId</span></span> |<span data-ttu-id="d19ca-143">string</span><span class="sxs-lookup"><span data-stu-id="d19ca-143">string</span></span> |<span data-ttu-id="d19ca-144">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="d19ca-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="d19ca-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d19ca-145">mailNickname</span></span> |<span data-ttu-id="d19ca-146">string</span><span class="sxs-lookup"><span data-stu-id="d19ca-146">string</span></span> |<span data-ttu-id="d19ca-147">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="d19ca-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="d19ca-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d19ca-148">passwordProfile</span></span>|[<span data-ttu-id="d19ca-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="d19ca-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="d19ca-150">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="d19ca-150">The password profile for the user.</span></span>|
|<span data-ttu-id="d19ca-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d19ca-151">userPrincipalName</span></span> |<span data-ttu-id="d19ca-152">string</span><span class="sxs-lookup"><span data-stu-id="d19ca-152">string</span></span> |<span data-ttu-id="d19ca-153">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="d19ca-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="d19ca-154">**ユーザー** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにユーザー インスタンスに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="d19ca-154">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="d19ca-155">この API を使用して作成されたフェデレーション ユーザーは、既定で 12 時間ごとに強制サインインされます。</span><span class="sxs-lookup"><span data-stu-id="d19ca-155">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="d19ca-156">この設定を変更する方法の詳細については、「[トークンの有効期間の例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d19ca-156">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="d19ca-157">応答</span><span class="sxs-lookup"><span data-stu-id="d19ca-157">Response</span></span>

<span data-ttu-id="d19ca-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d19ca-158">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d19ca-159">例</span><span class="sxs-lookup"><span data-stu-id="d19ca-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d19ca-160">要求</span><span class="sxs-lookup"><span data-stu-id="d19ca-160">Request</span></span>

<span data-ttu-id="d19ca-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d19ca-161">Here is an example of the request.</span></span>
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

<span data-ttu-id="d19ca-162">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d19ca-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d19ca-163">応答</span><span class="sxs-lookup"><span data-stu-id="d19ca-163">Response</span></span>

<span data-ttu-id="d19ca-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d19ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="d19ca-167">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d19ca-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d19ca-168">C#</span><span class="sxs-lookup"><span data-stu-id="d19ca-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d19ca-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="d19ca-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
