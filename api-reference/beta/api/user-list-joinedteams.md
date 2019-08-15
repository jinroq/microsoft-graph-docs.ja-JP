---
title: joinedTeams を一覧表示する
description: ユーザーがダイレクト メンバーになっている Microsoft Teams のチームを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db3bb194cb6c33f7afe9410c5ca28bdbe0c6e299
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408979"
---
# <a name="list-joinedteams"></a><span data-ttu-id="9a8bf-103">joinedTeams を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9a8bf-103">List joinedTeams</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a8bf-104">ユーザーがダイレクト メンバーになっている Microsoft Teams の[チーム](../resources/team.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="9a8bf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a8bf-105">Permissions</span></span>
<span data-ttu-id="9a8bf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a8bf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a8bf-108">Permission type</span></span>      | <span data-ttu-id="9a8bf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a8bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a8bf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a8bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a8bf-111">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8bf-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a8bf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a8bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a8bf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-113">Not supported.</span></span>    |
|<span data-ttu-id="9a8bf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a8bf-114">Application</span></span> | <span data-ttu-id="9a8bf-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8bf-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="9a8bf-116">現在、ユーザーに委任されたアクセス許可では、この操作は 'me' ユーザーに対してのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-116">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="9a8bf-117">アプリケーションのアクセス許可では、特定のユーザー ID を指定することにより、すべてのユーザーに対して機能します ('me' エイリアスはアプリケーションのアクセス許可ではサポートされていません)。詳細については、「[既知の問題](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-117">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="9a8bf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a8bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a8bf-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a8bf-119">Optional query parameters</span></span>
<span data-ttu-id="9a8bf-120">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a8bf-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a8bf-121">Request headers</span></span>
| <span data-ttu-id="9a8bf-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a8bf-122">Header</span></span>       | <span data-ttu-id="9a8bf-123">値</span><span class="sxs-lookup"><span data-stu-id="9a8bf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a8bf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a8bf-124">Authorization</span></span>  | <span data-ttu-id="9a8bf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9a8bf-127">承諾</span><span class="sxs-lookup"><span data-stu-id="9a8bf-127">Accept</span></span>  | <span data-ttu-id="9a8bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a8bf-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a8bf-129">Request body</span></span>
<span data-ttu-id="9a8bf-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a8bf-131">応答</span><span class="sxs-lookup"><span data-stu-id="9a8bf-131">Response</span></span>

<span data-ttu-id="9a8bf-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [team](../resources/team.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/team.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8bf-133">例</span><span class="sxs-lookup"><span data-stu-id="9a8bf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a8bf-134">要求</span><span class="sxs-lookup"><span data-stu-id="9a8bf-134">Request</span></span>
<span data-ttu-id="9a8bf-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a8bf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8bf-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a8bf-137">C#</span><span class="sxs-lookup"><span data-stu-id="9a8bf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a8bf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a8bf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a8bf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a8bf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a8bf-140">応答</span><span class="sxs-lookup"><span data-stu-id="9a8bf-140">Response</span></span>
<span data-ttu-id="9a8bf-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a8bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="9a8bf-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a8bf-144">See also</span></span>
[<span data-ttu-id="9a8bf-145">すべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="9a8bf-145">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
