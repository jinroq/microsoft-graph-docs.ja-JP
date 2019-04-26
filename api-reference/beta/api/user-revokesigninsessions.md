---
title: 'ユーザー: revokeSignInSessions'
description: '**signInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128ebec580fa97707c56d099f5a6e7c66fa3dfc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334524"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="07075-103">ユーザー: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="07075-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07075-104">**signInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="07075-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="07075-105">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="07075-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="07075-106">この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="07075-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="07075-107">アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="07075-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="07075-108">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="07075-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="07075-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07075-109">Permissions</span></span>
<span data-ttu-id="07075-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07075-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07075-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07075-112">Permission type</span></span>                        | <span data-ttu-id="07075-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07075-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="07075-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07075-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="07075-115">directory.accessasuser.all、またはすべてのディレクトリを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="07075-115">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07075-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07075-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07075-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07075-117">Not supported.</span></span> |
|<span data-ttu-id="07075-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07075-118">Application</span></span>                            | <span data-ttu-id="07075-119">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07075-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07075-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07075-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```
## <a name="request-headers"></a><span data-ttu-id="07075-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07075-121">Request headers</span></span>
| <span data-ttu-id="07075-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07075-122">Header</span></span>       | <span data-ttu-id="07075-123">値</span><span class="sxs-lookup"><span data-stu-id="07075-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07075-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="07075-124">Authorization</span></span>  | <span data-ttu-id="07075-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07075-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07075-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="07075-127">Request body</span></span>
<span data-ttu-id="07075-128">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="07075-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="07075-129">応答</span><span class="sxs-lookup"><span data-stu-id="07075-129">Response</span></span>

<span data-ttu-id="07075-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="07075-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07075-131">例</span><span class="sxs-lookup"><span data-stu-id="07075-131">Example</span></span>
<span data-ttu-id="07075-132">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="07075-132">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="07075-133">要求</span><span class="sxs-lookup"><span data-stu-id="07075-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="07075-134">応答</span><span class="sxs-lookup"><span data-stu-id="07075-134">Response</span></span>
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
  "suppressions": []
}
-->
