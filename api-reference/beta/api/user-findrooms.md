---
title: 'user: findRooms'
description: 'ユーザーのテナント内、または特定の部屋の一覧内のすべての会議室を取得します。 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5784824fe0e6c174935d12b8b22052709a61f69d
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637379"
---
# <a name="user-findrooms"></a><span data-ttu-id="81a63-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="81a63-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a63-104">ユーザーのテナント内、または特定の部屋の一覧内のすべての会議室を取得します。</span><span class="sxs-lookup"><span data-stu-id="81a63-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="81a63-105">テナントは会議室を部屋の一覧に整理できます。</span><span class="sxs-lookup"><span data-stu-id="81a63-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="81a63-106">それぞれの会議室と部屋の一覧は、[emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="81a63-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="81a63-107">テナント内の[すべての部屋の一覧を取得](user-findroomlists.md)できます。また、テナント内のすべての部屋を取得したり、または特定の部屋の一覧のすべての部屋を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="81a63-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="81a63-108">テナント内の最初の 100 部屋まで取得できます。</span><span class="sxs-lookup"><span data-stu-id="81a63-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="81a63-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81a63-109">Permissions</span></span>
<span data-ttu-id="81a63-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81a63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="81a63-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81a63-112">Permission type</span></span>      | <span data-ttu-id="81a63-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81a63-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81a63-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81a63-114">Delegated (work or school account)</span></span> | <span data-ttu-id="81a63-115">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a63-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="81a63-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81a63-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81a63-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81a63-117">Not supported.</span></span>    |
|<span data-ttu-id="81a63-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81a63-118">Application</span></span> | <span data-ttu-id="81a63-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a63-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81a63-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81a63-120">HTTP request</span></span>

<span data-ttu-id="81a63-121">テナント内のすべての部屋を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="81a63-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="81a63-122">テナントの特定の部屋の一覧にある部屋をすべて取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="81a63-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="81a63-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="81a63-123">Query parameters</span></span>

| <span data-ttu-id="81a63-124">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="81a63-124">Query parameter</span></span>       | <span data-ttu-id="81a63-125">種類</span><span class="sxs-lookup"><span data-stu-id="81a63-125">Type</span></span> | <span data-ttu-id="81a63-126">説明</span><span class="sxs-lookup"><span data-stu-id="81a63-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="81a63-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="81a63-127">RoomList</span></span> | <span data-ttu-id="81a63-128">string</span><span class="sxs-lookup"><span data-stu-id="81a63-128">string</span></span> | <span data-ttu-id="81a63-p103">部屋の一覧に関連付けられている SMTP アドレス。それぞれの部屋の一覧は、SMTP アドレスを含んでいる [emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="81a63-p103">The SMTP address associated with the room list. Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="81a63-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81a63-131">Request headers</span></span>
| <span data-ttu-id="81a63-132">名前</span><span class="sxs-lookup"><span data-stu-id="81a63-132">Name</span></span>       | <span data-ttu-id="81a63-133">型</span><span class="sxs-lookup"><span data-stu-id="81a63-133">Type</span></span> | <span data-ttu-id="81a63-134">説明</span><span class="sxs-lookup"><span data-stu-id="81a63-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="81a63-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a63-135">Authorization</span></span>  | <span data-ttu-id="81a63-136">string</span><span class="sxs-lookup"><span data-stu-id="81a63-136">string</span></span>  | <span data-ttu-id="81a63-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81a63-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81a63-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81a63-139">Content-Type</span></span>  | <span data-ttu-id="81a63-140">string</span><span class="sxs-lookup"><span data-stu-id="81a63-140">string</span></span>  | <span data-ttu-id="81a63-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="81a63-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="81a63-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="81a63-143">Request body</span></span>
<span data-ttu-id="81a63-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="81a63-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81a63-145">応答</span><span class="sxs-lookup"><span data-stu-id="81a63-145">Response</span></span>

<span data-ttu-id="81a63-146">成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [emailAddress](../resources/emailaddress.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81a63-146">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="81a63-147">例</span><span class="sxs-lookup"><span data-stu-id="81a63-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="81a63-148">要求 1</span><span class="sxs-lookup"><span data-stu-id="81a63-148">Request 1</span></span>

<span data-ttu-id="81a63-149">最初の例では、サインインしているユーザーのテナントで定義されている部屋をすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="81a63-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="81a63-150">応答 1</span><span class="sxs-lookup"><span data-stu-id="81a63-150">Response 1</span></span>
<span data-ttu-id="81a63-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="81a63-151">Here is an example of the response.</span></span> 

<span data-ttu-id="81a63-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81a63-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
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
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="81a63-154">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="81a63-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="81a63-155">C#</span><span class="sxs-lookup"><span data-stu-id="81a63-155">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81a63-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="81a63-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="81a63-157">要求 2</span><span class="sxs-lookup"><span data-stu-id="81a63-157">Request 2</span></span>

<span data-ttu-id="81a63-158">2 番目の例では、電子メール アドレス Building2Rooms@contoso.onmicrosoft.com で識別される特定の部屋の一覧の部屋を取得します。</span><span class="sxs-lookup"><span data-stu-id="81a63-158">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="81a63-159">応答 2</span><span class="sxs-lookup"><span data-stu-id="81a63-159">Response 2</span></span>
<span data-ttu-id="81a63-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="81a63-160">Here is an example of the response.</span></span> 

<span data-ttu-id="81a63-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81a63-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
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
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="81a63-163">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="81a63-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="81a63-164">C#</span><span class="sxs-lookup"><span data-stu-id="81a63-164">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81a63-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="81a63-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
