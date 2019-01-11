---
title: 設定を取得します。
description: ユーザーと組織の設定オブジェクトを参照してください。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 30217d43ac453c9e3502b00ece22ac01edf0abfb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852403"
---
# <a name="get-settings"></a><span data-ttu-id="4d9ba-103">設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-103">Get settings</span></span>

> <span data-ttu-id="4d9ba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d9ba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d9ba-106">ユーザーと組織の[設定](../resources/user-settings.md)オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="4d9ba-107">[設定](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定の更新](user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d9ba-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d9ba-108">Permissions</span></span>

<span data-ttu-id="4d9ba-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d9ba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d9ba-111">Permission type</span></span>      | <span data-ttu-id="4d9ba-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d9ba-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d9ba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d9ba-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4d9ba-114">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d9ba-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d9ba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d9ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d9ba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-116">Not supported.</span></span>    |
|<span data-ttu-id="4d9ba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d9ba-117">Application</span></span> | <span data-ttu-id="4d9ba-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d9ba-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d9ba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d9ba-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="4d9ba-120">'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="4d9ba-121">詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="4d9ba-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d9ba-122">Request body</span></span>

<span data-ttu-id="4d9ba-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d9ba-124">応答</span><span class="sxs-lookup"><span data-stu-id="4d9ba-124">Response</span></span>

<span data-ttu-id="4d9ba-125">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[ユーザー設定](../resources/user-settings.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d9ba-126">例</span><span class="sxs-lookup"><span data-stu-id="4d9ba-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d9ba-127">要求</span><span class="sxs-lookup"><span data-stu-id="4d9ba-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="4d9ba-128">応答</span><span class="sxs-lookup"><span data-stu-id="4d9ba-128">Response</span></span>

<span data-ttu-id="4d9ba-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d9ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
