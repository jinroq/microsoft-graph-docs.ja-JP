---
title: 参加チームのリストを作成する
description: ユーザーの直接のメンバーでは、マイクロソフトのチームで、チームを取得します。
author: dkershaw10
ms.openlocfilehash: 1fdc3ac9f2f09e31af71cdb4707dd84adf2c74a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343842"
---
# <a name="list-joinedteams"></a><span data-ttu-id="c871b-103">参加チームのリストを作成する</span><span class="sxs-lookup"><span data-stu-id="c871b-103">List joinedTeams</span></span>

> <span data-ttu-id="c871b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c871b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c871b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c871b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c871b-106">ユーザーの直接のメンバーでは、マイクロソフトのチームで[チーム](../resources/team.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="c871b-106">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="c871b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c871b-107">Permissions</span></span>
<span data-ttu-id="c871b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c871b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c871b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c871b-110">Permission type</span></span>      | <span data-ttu-id="c871b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c871b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c871b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c871b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c871b-113">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c871b-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="c871b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c871b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c871b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c871b-115">Not supported.</span></span>    |
|<span data-ttu-id="c871b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c871b-116">Application</span></span> | <span data-ttu-id="c871b-117">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c871b-117">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="c871b-118">現在、委任されたユーザーのアクセス許可を持つこの操作だけが、'me' ユーザーです。</span><span class="sxs-lookup"><span data-stu-id="c871b-118">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="c871b-119">アプリケーションのアクセス許可を持つ機能のすべてのユーザーによって特定のユーザー id を指定します。('me' エイリアスはアプリケーションのアクセス許可)詳細については、[既知の問題](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c871b-119">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="c871b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c871b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c871b-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c871b-121">Optional query parameters</span></span>
<span data-ttu-id="c871b-122">[OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c871b-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c871b-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c871b-123">Request headers</span></span>
| <span data-ttu-id="c871b-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c871b-124">Header</span></span>       | <span data-ttu-id="c871b-125">値</span><span class="sxs-lookup"><span data-stu-id="c871b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c871b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c871b-126">Authorization</span></span>  | <span data-ttu-id="c871b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c871b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c871b-129">承諾</span><span class="sxs-lookup"><span data-stu-id="c871b-129">Accept</span></span>  | <span data-ttu-id="c871b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c871b-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c871b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c871b-131">Request body</span></span>
<span data-ttu-id="c871b-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c871b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c871b-133">応答</span><span class="sxs-lookup"><span data-stu-id="c871b-133">Response</span></span>

<span data-ttu-id="c871b-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c871b-134">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c871b-135">例</span><span class="sxs-lookup"><span data-stu-id="c871b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c871b-136">要求</span><span class="sxs-lookup"><span data-stu-id="c871b-136">Request</span></span>
<span data-ttu-id="c871b-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c871b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="c871b-138">応答</span><span class="sxs-lookup"><span data-stu-id="c871b-138">Response</span></span>
<span data-ttu-id="c871b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c871b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c871b-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="c871b-142">See also</span></span>
[<span data-ttu-id="c871b-143">すべてのチームをリストします。</span><span class="sxs-lookup"><span data-stu-id="c871b-143">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
