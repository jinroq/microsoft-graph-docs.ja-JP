---
title: 'ユーザー: invalidateAllRefreshTokens'
description: '**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。 通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。  この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。 実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 740829e4ebd3b64308e514ab1c7633db7f35e7d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950180"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="43a85-106">ユーザー: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="43a85-106">user: invalidateAllRefreshTokens</span></span>

> <span data-ttu-id="43a85-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43a85-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43a85-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43a85-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43a85-109">**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。</span><span class="sxs-lookup"><span data-stu-id="43a85-109">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="43a85-110">通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。</span><span class="sxs-lookup"><span data-stu-id="43a85-110">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="43a85-111">この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。</span><span class="sxs-lookup"><span data-stu-id="43a85-111">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="43a85-112">実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。</span><span class="sxs-lookup"><span data-stu-id="43a85-112">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="43a85-113">開発者は、アプリケーションによって、無効な更新トークンを使用してこのユーザーの委任されたアクセス トークンを償還しようとする場合、アプリケーション エラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="43a85-113">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="43a85-114">このような場合は、アプリケーションが承認の端点にサインインするユーザーを強制的に実行を要求することによって、新しい更新のトークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43a85-114">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="43a85-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43a85-115">Permissions</span></span>
<span data-ttu-id="43a85-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43a85-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="43a85-118">アプリケーションを無効にするユーザーに、署名を許可するアプリケーションに同意した: User.ReadWrite、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43a85-118">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="43a85-119">同意したユーザーのアプリケーションを無効にする管理者を許可するアプリケーション: Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43a85-119">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="43a85-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43a85-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="43a85-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43a85-121">Request headers</span></span>
| <span data-ttu-id="43a85-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43a85-122">Header</span></span>       | <span data-ttu-id="43a85-123">値</span><span class="sxs-lookup"><span data-stu-id="43a85-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="43a85-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43a85-124">Authorization</span></span>  | <span data-ttu-id="43a85-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="43a85-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43a85-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="43a85-127">Request body</span></span>
<span data-ttu-id="43a85-128">この操作には、要求のコンテンツがありません。</span><span class="sxs-lookup"><span data-stu-id="43a85-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="43a85-129">応答</span><span class="sxs-lookup"><span data-stu-id="43a85-129">Response</span></span>

<span data-ttu-id="43a85-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="43a85-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43a85-131">例</span><span class="sxs-lookup"><span data-stu-id="43a85-131">Example</span></span>
<span data-ttu-id="43a85-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="43a85-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="43a85-133">要求</span><span class="sxs-lookup"><span data-stu-id="43a85-133">Request</span></span>
<span data-ttu-id="43a85-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43a85-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="43a85-135">応答</span><span class="sxs-lookup"><span data-stu-id="43a85-135">Response</span></span>
<span data-ttu-id="43a85-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="43a85-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
