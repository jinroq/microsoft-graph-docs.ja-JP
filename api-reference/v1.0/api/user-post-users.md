---
title: ユーザーを作成する
description: 新しいユーザーを作成するのにには、この API を使用します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66499d47fc2458debc8d2c234738e6a7b0a18c64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945595"
---
# <a name="create-user"></a><span data-ttu-id="e180c-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="e180c-103">Create User</span></span>

<span data-ttu-id="e180c-p101">この API を使用して、新しいユーザーを作成します。要求本文に、作成するユーザーを含めます。少なくとも、ユーザーについての必須プロパティを指定する必要があります。必要に応じて、その他の書き込み可能なプロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="e180c-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="e180c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e180c-108">Permissions</span></span>
<span data-ttu-id="e180c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e180c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e180c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e180c-111">Permission type</span></span>      | <span data-ttu-id="e180c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e180c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e180c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e180c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e180c-114">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e180c-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e180c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e180c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e180c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e180c-116">Not supported.</span></span>    |
|<span data-ttu-id="e180c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e180c-117">Application</span></span> | <span data-ttu-id="e180c-118">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e180c-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e180c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e180c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="e180c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e180c-120">Request headers</span></span>
| <span data-ttu-id="e180c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e180c-121">Header</span></span>       | <span data-ttu-id="e180c-122">値</span><span class="sxs-lookup"><span data-stu-id="e180c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e180c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e180c-123">Authorization</span></span>  | <span data-ttu-id="e180c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e180c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e180c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e180c-126">Content-Type</span></span>  | <span data-ttu-id="e180c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e180c-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e180c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e180c-128">Request body</span></span>
<span data-ttu-id="e180c-129">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e180c-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="e180c-130">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e180c-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="e180c-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e180c-131">Parameter</span></span> | <span data-ttu-id="e180c-132">型</span><span class="sxs-lookup"><span data-stu-id="e180c-132">Type</span></span> | <span data-ttu-id="e180c-133">説明</span><span class="sxs-lookup"><span data-stu-id="e180c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e180c-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e180c-134">accountEnabled</span></span> |<span data-ttu-id="e180c-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="e180c-135">boolean</span></span> |<span data-ttu-id="e180c-136">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="e180c-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="e180c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e180c-137">displayName</span></span> |<span data-ttu-id="e180c-138">string</span><span class="sxs-lookup"><span data-stu-id="e180c-138">string</span></span> |<span data-ttu-id="e180c-139">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="e180c-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="e180c-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="e180c-140">onPremisesImmutableId</span></span> |<span data-ttu-id="e180c-141">文字列</span><span class="sxs-lookup"><span data-stu-id="e180c-141">string</span></span> |<span data-ttu-id="e180c-142">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="e180c-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="e180c-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e180c-143">mailNickname</span></span> |<span data-ttu-id="e180c-144">文字列</span><span class="sxs-lookup"><span data-stu-id="e180c-144">string</span></span> |<span data-ttu-id="e180c-145">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="e180c-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="e180c-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e180c-146">passwordProfile</span></span>|[<span data-ttu-id="e180c-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="e180c-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="e180c-148">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="e180c-148">The password profile for the user.</span></span>|
|<span data-ttu-id="e180c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e180c-149">userPrincipalName</span></span> |<span data-ttu-id="e180c-150">文字列</span><span class="sxs-lookup"><span data-stu-id="e180c-150">string</span></span> |<span data-ttu-id="e180c-151">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="e180c-151">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="e180c-152">応答</span><span class="sxs-lookup"><span data-stu-id="e180c-152">Response</span></span>

<span data-ttu-id="e180c-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e180c-153">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e180c-154">例</span><span class="sxs-lookup"><span data-stu-id="e180c-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e180c-155">要求</span><span class="sxs-lookup"><span data-stu-id="e180c-155">Request</span></span>
<span data-ttu-id="e180c-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e180c-156">Here is an example of the request.</span></span>
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
<span data-ttu-id="e180c-157">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e180c-157">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e180c-158">応答</span><span class="sxs-lookup"><span data-stu-id="e180c-158">Response</span></span>
<span data-ttu-id="e180c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e180c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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
  "tocPath": ""
}-->
