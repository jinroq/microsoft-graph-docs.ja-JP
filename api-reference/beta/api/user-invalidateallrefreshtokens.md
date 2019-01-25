---
title: 'ユーザー: invalidateAllRefreshTokens'
description: '**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。 通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。  この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。 実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524528"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="f2cfd-106">ユーザー: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="f2cfd-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2cfd-107">**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="f2cfd-108">通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="f2cfd-109">この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="f2cfd-110">実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="f2cfd-111">開発者は、アプリケーションによって、無効な更新トークンを使用してこのユーザーの委任されたアクセス トークンを償還しようとする場合、アプリケーション エラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="f2cfd-112">このような場合は、アプリケーションが承認の端点にサインインするユーザーを強制的に実行を要求することによって、新しい更新のトークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2cfd-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2cfd-113">Permissions</span></span>
<span data-ttu-id="f2cfd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="f2cfd-116">アプリケーションを無効にするユーザーに、署名を許可するアプリケーションに同意した: User.ReadWrite、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2cfd-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="f2cfd-117">同意したユーザーのアプリケーションを無効にする管理者を許可するアプリケーション: Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2cfd-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f2cfd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2cfd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="f2cfd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2cfd-119">Request headers</span></span>
| <span data-ttu-id="f2cfd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2cfd-120">Header</span></span>       | <span data-ttu-id="f2cfd-121">値</span><span class="sxs-lookup"><span data-stu-id="f2cfd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2cfd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2cfd-122">Authorization</span></span>  | <span data-ttu-id="f2cfd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2cfd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2cfd-125">Request body</span></span>
<span data-ttu-id="f2cfd-126">この操作には、要求のコンテンツがありません。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="f2cfd-127">応答</span><span class="sxs-lookup"><span data-stu-id="f2cfd-127">Response</span></span>

<span data-ttu-id="f2cfd-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2cfd-129">例</span><span class="sxs-lookup"><span data-stu-id="f2cfd-129">Example</span></span>
<span data-ttu-id="f2cfd-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f2cfd-131">要求</span><span class="sxs-lookup"><span data-stu-id="f2cfd-131">Request</span></span>
<span data-ttu-id="f2cfd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="f2cfd-133">応答</span><span class="sxs-lookup"><span data-stu-id="f2cfd-133">Response</span></span>
<span data-ttu-id="f2cfd-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f2cfd-134">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
