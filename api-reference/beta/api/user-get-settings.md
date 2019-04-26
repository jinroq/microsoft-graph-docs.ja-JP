---
title: 設定を取得する
description: ユーザーと組織の設定オブジェクトを読み取ります。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dcd9079956b4db8b349ba6b81bd85d8472630643
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334913"
---
# <a name="get-settings"></a><span data-ttu-id="d603c-103">設定を取得する</span><span class="sxs-lookup"><span data-stu-id="d603c-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d603c-104">ユーザーと組織の[設定](../resources/user-settings.md)オブジェクトを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d603c-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="d603c-105">[settings](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、「[ユーザーの設定を更新](user-update-settings.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d603c-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d603c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d603c-106">Permissions</span></span>

<span data-ttu-id="d603c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d603c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d603c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d603c-109">Permission type</span></span>      | <span data-ttu-id="d603c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d603c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d603c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d603c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d603c-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d603c-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="d603c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d603c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d603c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d603c-114">Not supported.</span></span>    |
|<span data-ttu-id="d603c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d603c-115">Application</span></span> | <span data-ttu-id="d603c-116">user。すべてのユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d603c-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d603c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d603c-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="d603c-118">' user id ' または ' userPrincipalName ' を持つ要求は、ユーザーまたはすべてのアクセス許可を持つユーザーのみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d603c-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="d603c-119">詳細については、「 [Permissions](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d603c-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="d603c-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="d603c-120">Request body</span></span>

<span data-ttu-id="d603c-121">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d603c-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d603c-122">応答</span><span class="sxs-lookup"><span data-stu-id="d603c-122">Response</span></span>

<span data-ttu-id="d603c-123">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[ユーザー設定](../resources/user-settings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d603c-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d603c-124">例</span><span class="sxs-lookup"><span data-stu-id="d603c-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d603c-125">要求</span><span class="sxs-lookup"><span data-stu-id="d603c-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="d603c-126">応答</span><span class="sxs-lookup"><span data-stu-id="d603c-126">Response</span></span>

<span data-ttu-id="d603c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d603c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
