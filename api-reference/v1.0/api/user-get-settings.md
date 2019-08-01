---
title: 設定を取得する
description: ユーザーおよび組織の設定 オブジェクトを読み取ります。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64ecf4c4f44cf59bf3c6344edda7510a6997d813
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027077"
---
# <a name="get-settings"></a><span data-ttu-id="bd95d-103">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="bd95d-103">Get settings</span></span>

<span data-ttu-id="bd95d-104">ユーザーおよび組織の[設定](../resources/user-settings.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd95d-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="bd95d-105">[設定](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定を更新する](user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd95d-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd95d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd95d-106">Permissions</span></span>

<span data-ttu-id="bd95d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd95d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd95d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd95d-109">Permission type</span></span>      | <span data-ttu-id="bd95d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd95d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd95d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd95d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd95d-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd95d-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd95d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd95d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd95d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd95d-114">Not supported.</span></span>    |
|<span data-ttu-id="bd95d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd95d-115">Application</span></span> | <span data-ttu-id="bd95d-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd95d-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd95d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd95d-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="bd95d-118">「user id」または「userPrincipalName」を持つリクエストは、ユーザーまたは User.ReadWrite.All 権限を持つユーザーのみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="bd95d-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="bd95d-119">詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd95d-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="bd95d-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd95d-120">Request body</span></span>

<span data-ttu-id="bd95d-121">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bd95d-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd95d-122">応答</span><span class="sxs-lookup"><span data-stu-id="bd95d-122">Response</span></span>

<span data-ttu-id="bd95d-123">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user-settings.md)設定 オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bd95d-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd95d-124">例</span><span class="sxs-lookup"><span data-stu-id="bd95d-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bd95d-125">要求</span><span class="sxs-lookup"><span data-stu-id="bd95d-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="bd95d-126">応答</span><span class="sxs-lookup"><span data-stu-id="bd95d-126">Response</span></span>

<span data-ttu-id="bd95d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd95d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

