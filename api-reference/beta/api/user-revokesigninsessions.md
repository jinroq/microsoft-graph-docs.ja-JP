---
title: 'ユーザー: revokeSignInSessions'
description: '**SignInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c945eeefaad03ec08e062fe8db80573c5ef6469
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421835"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="3f313-103">ユーザー: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="3f313-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f313-104">**SignInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="3f313-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="3f313-105">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="3f313-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="3f313-106">この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="3f313-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="3f313-107">アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="3f313-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="3f313-108">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="3f313-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="3f313-109">**RevokeSignInSessions**を呼び出した後、トークンが取り消されるまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3f313-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f313-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f313-110">Permissions</span></span>

<span data-ttu-id="3f313-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f313-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f313-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f313-113">Permission type</span></span>                        | <span data-ttu-id="3f313-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f313-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f313-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f313-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f313-116">Directory.accessasuser.all、またはすべてのディレクトリを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3f313-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3f313-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f313-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f313-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f313-118">Not supported.</span></span> |
|<span data-ttu-id="3f313-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f313-119">Application</span></span>                            | <span data-ttu-id="3f313-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f313-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f313-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f313-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="3f313-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f313-122">Request headers</span></span>
| <span data-ttu-id="3f313-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f313-123">Header</span></span>       | <span data-ttu-id="3f313-124">値</span><span class="sxs-lookup"><span data-stu-id="3f313-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f313-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f313-125">Authorization</span></span>  | <span data-ttu-id="3f313-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f313-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3f313-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f313-128">Content-Type</span></span>  | <span data-ttu-id="3f313-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3f313-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f313-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f313-130">Request body</span></span>
<span data-ttu-id="3f313-131">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="3f313-131">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="3f313-132">応答</span><span class="sxs-lookup"><span data-stu-id="3f313-132">Response</span></span>

<span data-ttu-id="3f313-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3f313-133">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="3f313-134">この API には[既知の問題](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)があります。</span><span class="sxs-lookup"><span data-stu-id="3f313-134">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="3f313-135">このメソッドは、異なる HTTP 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3f313-135">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f313-136">例</span><span class="sxs-lookup"><span data-stu-id="3f313-136">Example</span></span>
<span data-ttu-id="3f313-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3f313-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3f313-138">要求</span><span class="sxs-lookup"><span data-stu-id="3f313-138">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f313-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3f313-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f313-140">C#</span><span class="sxs-lookup"><span data-stu-id="3f313-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f313-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f313-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f313-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="3f313-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f313-143">応答</span><span class="sxs-lookup"><span data-stu-id="3f313-143">Response</span></span>
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
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
