---
title: 'ユーザー: invalidateAllRefreshTokens'
description: '**Refreshtokensvalidfromdatetime**ユーザープロパティを現在の日付/時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。 通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。  この操作を実行すると、ユーザーが最初にサインインする必要がなく、デバイス上のアプリケーションを介してアクセスされる組織のデータにアクセスできなくなります。 実際、この操作を実行すると、デバイスに関係なく、以前に同意していたすべてのアプリケーションに対して、ユーザーが再度サインインすることになります。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55e556bdcd810d040d022df481ae437eb90a5921
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996456"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="281dd-106">ユーザー: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="281dd-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="281dd-107">**Refreshtokensvalidfromdatetime**ユーザープロパティを現在の日付/時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="281dd-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="281dd-108">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="281dd-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="281dd-109">この操作を実行すると、ユーザーが最初にサインインする必要がなく、デバイス上のアプリケーションを介してアクセスされる組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="281dd-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="281dd-110">実際、この操作を実行すると、デバイスに関係なく、以前に同意していたすべてのアプリケーションに対して、ユーザーが再度サインインすることになります。</span><span class="sxs-lookup"><span data-stu-id="281dd-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="281dd-111">開発者にとって、アプリケーションが無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行した場合、アプリケーションでエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="281dd-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="281dd-112">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="281dd-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="281dd-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="281dd-113">Permissions</span></span>
<span data-ttu-id="281dd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="281dd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="281dd-116">アプリケーションで、サインインしているユーザーが同意のアプリケーションを無効にできるようにするには、Directory.accessasuser.all のようにします。</span><span class="sxs-lookup"><span data-stu-id="281dd-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="281dd-117">管理者が同意、Directory.accessasuser.all のいずれかのユーザーがアプリケーションを無効にすることを許可するアプリケーションの場合。</span><span class="sxs-lookup"><span data-stu-id="281dd-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="281dd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="281dd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="281dd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="281dd-119">Request headers</span></span>
| <span data-ttu-id="281dd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="281dd-120">Header</span></span>       | <span data-ttu-id="281dd-121">値</span><span class="sxs-lookup"><span data-stu-id="281dd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="281dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="281dd-122">Authorization</span></span>  | <span data-ttu-id="281dd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="281dd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="281dd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="281dd-125">Request body</span></span>
<span data-ttu-id="281dd-126">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="281dd-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="281dd-127">応答</span><span class="sxs-lookup"><span data-stu-id="281dd-127">Response</span></span>

<span data-ttu-id="281dd-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="281dd-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="281dd-129">例</span><span class="sxs-lookup"><span data-stu-id="281dd-129">Example</span></span>
<span data-ttu-id="281dd-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="281dd-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="281dd-131">要求</span><span class="sxs-lookup"><span data-stu-id="281dd-131">Request</span></span>
<span data-ttu-id="281dd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="281dd-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="281dd-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="281dd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="281dd-134">C#</span><span class="sxs-lookup"><span data-stu-id="281dd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="281dd-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="281dd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="281dd-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="281dd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="281dd-137">Java</span><span class="sxs-lookup"><span data-stu-id="281dd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="281dd-138">応答</span><span class="sxs-lookup"><span data-stu-id="281dd-138">Response</span></span>
<span data-ttu-id="281dd-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="281dd-139">Here is an example of the response.</span></span> 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
