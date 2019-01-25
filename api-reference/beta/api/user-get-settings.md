---
title: 設定を取得します。
description: ユーザーと組織の設定オブジェクトを参照してください。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507482"
---
# <a name="get-settings"></a><span data-ttu-id="dc18f-103">設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="dc18f-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc18f-104">ユーザーと組織の[設定](../resources/user-settings.md)オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc18f-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="dc18f-105">[設定](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定の更新](user-update-settings.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc18f-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc18f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc18f-106">Permissions</span></span>

<span data-ttu-id="dc18f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc18f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc18f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc18f-109">Permission type</span></span>      | <span data-ttu-id="dc18f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc18f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc18f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc18f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc18f-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc18f-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc18f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc18f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc18f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc18f-114">Not supported.</span></span>    |
|<span data-ttu-id="dc18f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc18f-115">Application</span></span> | <span data-ttu-id="dc18f-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc18f-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc18f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc18f-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="dc18f-118">'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。</span><span class="sxs-lookup"><span data-stu-id="dc18f-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="dc18f-119">詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc18f-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="dc18f-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc18f-120">Request body</span></span>

<span data-ttu-id="dc18f-121">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc18f-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc18f-122">応答</span><span class="sxs-lookup"><span data-stu-id="dc18f-122">Response</span></span>

<span data-ttu-id="dc18f-123">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[ユーザー設定](../resources/user-settings.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dc18f-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc18f-124">例</span><span class="sxs-lookup"><span data-stu-id="dc18f-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc18f-125">要求</span><span class="sxs-lookup"><span data-stu-id="dc18f-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="dc18f-126">応答</span><span class="sxs-lookup"><span data-stu-id="dc18f-126">Response</span></span>

<span data-ttu-id="dc18f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc18f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
