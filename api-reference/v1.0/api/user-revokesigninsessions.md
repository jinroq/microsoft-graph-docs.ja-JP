---
title: 'ユーザー: revokeSignInSessions'
description: '**SignInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a39c7af37cd5ab94a33a06a7dd4c91c0c4b55600
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449009"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="971e4-103">ユーザー: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="971e4-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="971e4-104">**SignInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="971e4-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="971e4-105">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="971e4-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="971e4-106">この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="971e4-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="971e4-107">アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="971e4-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="971e4-108">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="971e4-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="971e4-109">**RevokeSignInSessions**を呼び出した後、トークンが取り消されるまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="971e4-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="971e4-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="971e4-110">Permissions</span></span>

<span data-ttu-id="971e4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="971e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="971e4-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="971e4-113">Permission type</span></span>                        | <span data-ttu-id="971e4-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="971e4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="971e4-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="971e4-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="971e4-116">Directory.accessasuser.all、またはすべてのディレクトリを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="971e4-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="971e4-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="971e4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="971e4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="971e4-118">Not supported.</span></span> |
|<span data-ttu-id="971e4-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="971e4-119">Application</span></span>                            | <span data-ttu-id="971e4-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="971e4-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="971e4-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="971e4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="971e4-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="971e4-122">Request headers</span></span>
| <span data-ttu-id="971e4-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="971e4-123">Header</span></span>       | <span data-ttu-id="971e4-124">値</span><span class="sxs-lookup"><span data-stu-id="971e4-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="971e4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="971e4-125">Authorization</span></span>  | <span data-ttu-id="971e4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="971e4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="971e4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="971e4-128">Request body</span></span>
<span data-ttu-id="971e4-129">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="971e4-129">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="971e4-130">応答</span><span class="sxs-lookup"><span data-stu-id="971e4-130">Response</span></span>

<span data-ttu-id="971e4-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="971e4-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="971e4-132">例</span><span class="sxs-lookup"><span data-stu-id="971e4-132">Example</span></span>
<span data-ttu-id="971e4-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="971e4-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="971e4-134">要求</span><span class="sxs-lookup"><span data-stu-id="971e4-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="971e4-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="971e4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="971e4-136">C#</span><span class="sxs-lookup"><span data-stu-id="971e4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="971e4-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="971e4-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="971e4-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="971e4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="971e4-139">応答</span><span class="sxs-lookup"><span data-stu-id="971e4-139">Response</span></span>
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
