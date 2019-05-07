---
title: joinedTeams を一覧表示する
description: ユーザーがダイレクト メンバーになっている Microsoft Teams のチームを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82fa29b1756b70d6b2ef9c0cc7051c5f9befcd10
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637259"
---
# <a name="list-joinedteams"></a><span data-ttu-id="4d53f-103">joinedTeams を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4d53f-103">List joinedTeams</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d53f-104">ユーザーがダイレクト メンバーになっている Microsoft Teams の[チーム](../resources/team.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="4d53f-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="4d53f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d53f-105">Permissions</span></span>
<span data-ttu-id="4d53f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d53f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d53f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d53f-108">Permission type</span></span>      | <span data-ttu-id="4d53f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d53f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d53f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d53f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d53f-111">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d53f-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d53f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d53f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d53f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d53f-113">Not supported.</span></span>    |
|<span data-ttu-id="4d53f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d53f-114">Application</span></span> | <span data-ttu-id="4d53f-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d53f-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="4d53f-116">現在、ユーザーに委任されたアクセス許可では、この操作は 'me' ユーザーに対してのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="4d53f-116">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="4d53f-117">アプリケーションのアクセス許可では、特定のユーザー ID を指定することにより、すべてのユーザーに対して機能します ('me' エイリアスはアプリケーションのアクセス許可ではサポートされていません)。詳細については、「[既知の問題](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d53f-117">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="4d53f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d53f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d53f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4d53f-119">Optional query parameters</span></span>
<span data-ttu-id="4d53f-120">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d53f-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d53f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d53f-121">Request headers</span></span>
| <span data-ttu-id="4d53f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d53f-122">Header</span></span>       | <span data-ttu-id="4d53f-123">値</span><span class="sxs-lookup"><span data-stu-id="4d53f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d53f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d53f-124">Authorization</span></span>  | <span data-ttu-id="4d53f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d53f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4d53f-127">承諾</span><span class="sxs-lookup"><span data-stu-id="4d53f-127">Accept</span></span>  | <span data-ttu-id="4d53f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4d53f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d53f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d53f-129">Request body</span></span>
<span data-ttu-id="4d53f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4d53f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d53f-131">応答</span><span class="sxs-lookup"><span data-stu-id="4d53f-131">Response</span></span>

<span data-ttu-id="4d53f-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4d53f-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d53f-133">例</span><span class="sxs-lookup"><span data-stu-id="4d53f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d53f-134">要求</span><span class="sxs-lookup"><span data-stu-id="4d53f-134">Request</span></span>
<span data-ttu-id="4d53f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d53f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="4d53f-136">応答</span><span class="sxs-lookup"><span data-stu-id="4d53f-136">Response</span></span>
<span data-ttu-id="4d53f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d53f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d53f-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="4d53f-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d53f-141">C#</span><span class="sxs-lookup"><span data-stu-id="4d53f-141">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_joinedteams-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d53f-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d53f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_joinedteams-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="4d53f-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d53f-143">See also</span></span>
[<span data-ttu-id="4d53f-144">すべてのチームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="4d53f-144">List all teams</span></span>](/graph/teams-list-all-teams)

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
    "Error: /api-reference/beta/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
