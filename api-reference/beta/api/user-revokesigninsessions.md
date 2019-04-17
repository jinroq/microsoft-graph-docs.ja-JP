---
title: 'ユーザー: revokeSignInSessions'
description: '**signInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 607b89201958ec2c8062109e2e02b1749b1c96ef
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890573"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="5d956-103">ユーザー: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="5d956-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d956-104">**signInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="5d956-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="5d956-105">通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。</span><span class="sxs-lookup"><span data-stu-id="5d956-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="5d956-106">この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="5d956-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="5d956-107">アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="5d956-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="5d956-108">このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="5d956-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d956-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d956-109">Permissions</span></span>
<span data-ttu-id="5d956-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d956-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d956-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d956-112">Permission type</span></span>                        | <span data-ttu-id="5d956-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d956-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d956-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d956-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d956-115">directory.accessasuser.all、またはすべてのディレクトリを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5d956-115">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5d956-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d956-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d956-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d956-117">Not supported.</span></span> |
|<span data-ttu-id="5d956-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d956-118">Application</span></span>                            | <span data-ttu-id="5d956-119">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d956-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d956-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d956-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```
## <a name="request-headers"></a><span data-ttu-id="5d956-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d956-121">Request headers</span></span>
| <span data-ttu-id="5d956-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d956-122">Header</span></span>       | <span data-ttu-id="5d956-123">値</span><span class="sxs-lookup"><span data-stu-id="5d956-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d956-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d956-124">Authorization</span></span>  | <span data-ttu-id="5d956-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d956-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d956-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d956-127">Request body</span></span>
<span data-ttu-id="5d956-128">この操作には、要求コンテンツはありません。</span><span class="sxs-lookup"><span data-stu-id="5d956-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="5d956-129">応答</span><span class="sxs-lookup"><span data-stu-id="5d956-129">Response</span></span>

<span data-ttu-id="5d956-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5d956-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5d956-131">例</span><span class="sxs-lookup"><span data-stu-id="5d956-131">Example</span></span>
<span data-ttu-id="5d956-132">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d956-132">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5d956-133">要求</span><span class="sxs-lookup"><span data-stu-id="5d956-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="5d956-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d956-134">Response</span></span>
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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
