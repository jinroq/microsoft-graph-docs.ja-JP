---
title: ユーザーを作成する
description: この API を使用して、新しいユーザーを作成します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e81ecd9b31ab5f2836e40e3b461a4974e161eb60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981462"
---
# <a name="create-user"></a><span data-ttu-id="51457-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="51457-103">Create User</span></span>

<span data-ttu-id="51457-p101">新しい[ユーザー](../resources/user.md)を作成します。要求本文に、作成するユーザーを含めます。少なくとも、ユーザーについての必須プロパティを指定する必要があります。必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="51457-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="51457-108">外部ユーザーを作成するには、[招待 API](invitation-post.md) を使用します。</span><span class="sxs-lookup"><span data-stu-id="51457-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="51457-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51457-109">Permissions</span></span>

<span data-ttu-id="51457-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51457-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51457-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51457-112">Permission type</span></span>      | <span data-ttu-id="51457-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51457-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51457-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51457-114">Delegated (work or school account)</span></span> | <span data-ttu-id="51457-115">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51457-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51457-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51457-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51457-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51457-117">Not supported.</span></span>    |
|<span data-ttu-id="51457-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51457-118">Application</span></span> | <span data-ttu-id="51457-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51457-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51457-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51457-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="51457-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51457-121">Request headers</span></span>

| <span data-ttu-id="51457-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51457-122">Header</span></span>       | <span data-ttu-id="51457-123">値</span><span class="sxs-lookup"><span data-stu-id="51457-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51457-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="51457-124">Authorization</span></span>  | <span data-ttu-id="51457-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="51457-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51457-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51457-127">Content-Type</span></span>  | <span data-ttu-id="51457-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51457-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51457-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="51457-129">Request body</span></span>

<span data-ttu-id="51457-130">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51457-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="51457-131">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51457-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="51457-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="51457-132">Parameter</span></span> | <span data-ttu-id="51457-133">型</span><span class="sxs-lookup"><span data-stu-id="51457-133">Type</span></span> | <span data-ttu-id="51457-134">説明</span><span class="sxs-lookup"><span data-stu-id="51457-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51457-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="51457-135">accountEnabled</span></span> |<span data-ttu-id="51457-136">boolean</span><span class="sxs-lookup"><span data-stu-id="51457-136">boolean</span></span> |<span data-ttu-id="51457-137">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="51457-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="51457-138">displayName</span><span class="sxs-lookup"><span data-stu-id="51457-138">displayName</span></span> |<span data-ttu-id="51457-139">string</span><span class="sxs-lookup"><span data-stu-id="51457-139">string</span></span> |<span data-ttu-id="51457-140">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="51457-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="51457-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="51457-141">onPremisesImmutableId</span></span> |<span data-ttu-id="51457-142">string</span><span class="sxs-lookup"><span data-stu-id="51457-142">string</span></span> |<span data-ttu-id="51457-143">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="51457-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="51457-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="51457-144">mailNickname</span></span> |<span data-ttu-id="51457-145">string</span><span class="sxs-lookup"><span data-stu-id="51457-145">string</span></span> |<span data-ttu-id="51457-146">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="51457-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="51457-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="51457-147">passwordProfile</span></span>|[<span data-ttu-id="51457-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="51457-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="51457-149">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="51457-149">The password profile for the user.</span></span>|
|<span data-ttu-id="51457-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51457-150">userPrincipalName</span></span> |<span data-ttu-id="51457-151">string</span><span class="sxs-lookup"><span data-stu-id="51457-151">string</span></span> |<span data-ttu-id="51457-152">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="51457-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="51457-153">**ユーザー** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにユーザー インスタンスに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="51457-153">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="51457-154">この API を使用して作成されたフェデレーション ユーザーは、既定で 12 時間ごとに強制サインインされます。</span><span class="sxs-lookup"><span data-stu-id="51457-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="51457-155">この設定を変更する方法の詳細については、「[トークンの有効期間の例外](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51457-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="51457-156">応答</span><span class="sxs-lookup"><span data-stu-id="51457-156">Response</span></span>

<span data-ttu-id="51457-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51457-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51457-158">例</span><span class="sxs-lookup"><span data-stu-id="51457-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51457-159">要求</span><span class="sxs-lookup"><span data-stu-id="51457-159">Request</span></span>

<span data-ttu-id="51457-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51457-160">Here is an example of the request.</span></span>
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

<span data-ttu-id="51457-161">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51457-161">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="51457-162">応答</span><span class="sxs-lookup"><span data-stu-id="51457-162">Response</span></span>

<span data-ttu-id="51457-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51457-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="51457-166">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="51457-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="51457-167">C#</span><span class="sxs-lookup"><span data-stu-id="51457-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51457-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="51457-168">Javascript</span></span>](#tab/javascript)
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
