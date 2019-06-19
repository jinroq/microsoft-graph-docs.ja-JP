---
title: 'ユーザー: revokeSignInSessions'
description: '**SignInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ab60a38e404dc13dbbc58b1103931cfe0b16c44
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001637"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="6c524-103">ユーザー: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="6c524-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="6c524-104">**SignInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="6c524-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="6c524-105">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="6c524-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="6c524-106">この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="6c524-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="6c524-107">アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6c524-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="6c524-108">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6c524-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="6c524-109">**RevokeSignInSessions**を呼び出した後、トークンが取り消されるまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c524-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c524-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c524-110">Permissions</span></span>

<span data-ttu-id="6c524-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c524-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c524-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c524-113">Permission type</span></span>                        | <span data-ttu-id="6c524-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c524-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c524-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c524-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c524-116">Directory.accessasuser.all、またはすべてのディレクトリを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c524-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6c524-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c524-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c524-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c524-118">Not supported.</span></span> |
|<span data-ttu-id="6c524-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c524-119">Application</span></span>                            | <span data-ttu-id="6c524-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c524-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c524-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c524-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="6c524-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c524-122">Request headers</span></span>
| <span data-ttu-id="6c524-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c524-123">Header</span></span>       | <span data-ttu-id="6c524-124">値</span><span class="sxs-lookup"><span data-stu-id="6c524-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c524-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c524-125">Authorization</span></span>  | <span data-ttu-id="6c524-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c524-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c524-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c524-128">Request body</span></span>
<span data-ttu-id="6c524-129">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="6c524-129">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="6c524-130">応答</span><span class="sxs-lookup"><span data-stu-id="6c524-130">Response</span></span>

<span data-ttu-id="6c524-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6c524-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c524-132">例</span><span class="sxs-lookup"><span data-stu-id="6c524-132">Example</span></span>
<span data-ttu-id="6c524-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c524-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c524-134">要求</span><span class="sxs-lookup"><span data-stu-id="6c524-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="6c524-135">応答</span><span class="sxs-lookup"><span data-stu-id="6c524-135">Response</span></span>
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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->