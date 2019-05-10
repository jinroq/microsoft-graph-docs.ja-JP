---
title: 'user: findRoomLists'
description: テナントで定義された部屋の一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19bd8c7caca4aa2dc4d30c431d115dede0426e23
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637389"
---
# <a name="user-findroomlists"></a><span data-ttu-id="72e68-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="72e68-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e68-104">テナントで定義された部屋の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="72e68-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="72e68-105">テナントは会議室を部屋の一覧に整理できます。</span><span class="sxs-lookup"><span data-stu-id="72e68-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="72e68-106">それぞれの会議室と部屋の一覧は、[emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="72e68-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="72e68-107">テナント内のすべての部屋の一覧を取得できます。また、テナント内の[すべての部屋を取得](user-findrooms.md)したり、または特定の部屋の一覧の[すべての部屋を取得](user-findrooms.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="72e68-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="72e68-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72e68-108">Permissions</span></span>
<span data-ttu-id="72e68-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72e68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72e68-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72e68-111">Permission type</span></span>      | <span data-ttu-id="72e68-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72e68-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72e68-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72e68-113">Delegated (work or school account)</span></span> | <span data-ttu-id="72e68-114">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e68-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="72e68-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72e68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72e68-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72e68-116">Not supported.</span></span>    |
|<span data-ttu-id="72e68-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72e68-117">Application</span></span> | <span data-ttu-id="72e68-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e68-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72e68-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72e68-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="72e68-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72e68-120">Request headers</span></span>
| <span data-ttu-id="72e68-121">名前</span><span class="sxs-lookup"><span data-stu-id="72e68-121">Name</span></span>       | <span data-ttu-id="72e68-122">型</span><span class="sxs-lookup"><span data-stu-id="72e68-122">Type</span></span> | <span data-ttu-id="72e68-123">説明</span><span class="sxs-lookup"><span data-stu-id="72e68-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="72e68-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e68-124">Authorization</span></span>  | <span data-ttu-id="72e68-125">string</span><span class="sxs-lookup"><span data-stu-id="72e68-125">string</span></span>  | <span data-ttu-id="72e68-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72e68-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72e68-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72e68-128">Content-Type</span></span>  | <span data-ttu-id="72e68-129">string</span><span class="sxs-lookup"><span data-stu-id="72e68-129">string</span></span>  | <span data-ttu-id="72e68-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="72e68-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="72e68-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="72e68-132">Request body</span></span>
<span data-ttu-id="72e68-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="72e68-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72e68-134">応答</span><span class="sxs-lookup"><span data-stu-id="72e68-134">Response</span></span>

<span data-ttu-id="72e68-135">成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [emailAddress](../resources/emailaddress.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72e68-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="72e68-136">テナントで定義されている一覧が存在しない場合は、空の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="72e68-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="72e68-137">例</span><span class="sxs-lookup"><span data-stu-id="72e68-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72e68-138">要求</span><span class="sxs-lookup"><span data-stu-id="72e68-138">Request</span></span>

<span data-ttu-id="72e68-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72e68-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="72e68-140">応答</span><span class="sxs-lookup"><span data-stu-id="72e68-140">Response</span></span>
<span data-ttu-id="72e68-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="72e68-141">Here is an example of the response.</span></span> 

<span data-ttu-id="72e68-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72e68-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="72e68-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="72e68-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72e68-145">C#</span><span class="sxs-lookup"><span data-stu-id="72e68-145">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_room_lists-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72e68-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="72e68-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_room_lists-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
