---
title: 'user: findRooms'
description: 'ユーザーのテナント内、または特定の部屋の一覧内のすべての会議室を取得します。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebfa5ad0c308cc2d4936c6e3a2a410a9656c3794
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421135"
---
# <a name="user-findrooms"></a><span data-ttu-id="8c9ea-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="8c9ea-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9ea-104">ユーザーのテナントまたは特定の部屋の一覧内にあるすべての会議室を表す [emailAddress](../resources/emailaddress.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="8c9ea-105">テナントは会議室を部屋の一覧に整理できます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="8c9ea-106">この API 内で、それぞれの会議室と部屋の一覧は、[emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="8c9ea-107">テナント内の[すべての部屋の一覧を取得](user-findroomlists.md)できます。また、テナント内のすべての部屋を取得したり、または特定の部屋の一覧のすべての部屋を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="8c9ea-108">テナント内の最初の 100 部屋まで取得できます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c9ea-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c9ea-109">Permissions</span></span>
<span data-ttu-id="8c9ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c9ea-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c9ea-112">Permission type</span></span>      | <span data-ttu-id="8c9ea-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c9ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c9ea-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c9ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8c9ea-115">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c9ea-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="8c9ea-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c9ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c9ea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-117">Not supported.</span></span>    |
|<span data-ttu-id="8c9ea-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c9ea-118">Application</span></span> | <span data-ttu-id="8c9ea-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c9ea-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c9ea-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c9ea-120">HTTP request</span></span>

<span data-ttu-id="8c9ea-121">テナント内のすべての部屋を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="8c9ea-122">テナントの特定の部屋の一覧にある部屋をすべて取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="8c9ea-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c9ea-123">Query parameters</span></span>

| <span data-ttu-id="8c9ea-124">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c9ea-124">Query parameter</span></span>       | <span data-ttu-id="8c9ea-125">種類</span><span class="sxs-lookup"><span data-stu-id="8c9ea-125">Type</span></span> | <span data-ttu-id="8c9ea-126">説明</span><span class="sxs-lookup"><span data-stu-id="8c9ea-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8c9ea-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="8c9ea-127">RoomList</span></span> | <span data-ttu-id="8c9ea-128">string</span><span class="sxs-lookup"><span data-stu-id="8c9ea-128">string</span></span> | <span data-ttu-id="8c9ea-p103">部屋の一覧に関連付けられている SMTP アドレス。それぞれの部屋の一覧は、SMTP アドレスを含んでいる [emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p103">The SMTP address associated with the room list. Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8c9ea-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c9ea-131">Request headers</span></span>
| <span data-ttu-id="8c9ea-132">名前</span><span class="sxs-lookup"><span data-stu-id="8c9ea-132">Name</span></span>       | <span data-ttu-id="8c9ea-133">種類</span><span class="sxs-lookup"><span data-stu-id="8c9ea-133">Type</span></span> | <span data-ttu-id="8c9ea-134">説明</span><span class="sxs-lookup"><span data-stu-id="8c9ea-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8c9ea-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c9ea-135">Authorization</span></span>  | <span data-ttu-id="8c9ea-136">string</span><span class="sxs-lookup"><span data-stu-id="8c9ea-136">string</span></span>  | <span data-ttu-id="8c9ea-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c9ea-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c9ea-139">Content-Type</span></span>  | <span data-ttu-id="8c9ea-140">string</span><span class="sxs-lookup"><span data-stu-id="8c9ea-140">string</span></span>  | <span data-ttu-id="8c9ea-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8c9ea-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c9ea-143">Request body</span></span>
<span data-ttu-id="8c9ea-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c9ea-145">応答</span><span class="sxs-lookup"><span data-stu-id="8c9ea-145">Response</span></span>

<span data-ttu-id="8c9ea-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [emailAddress](../resources/emailaddress.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="8c9ea-147">例</span><span class="sxs-lookup"><span data-stu-id="8c9ea-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="8c9ea-148">要求 1</span><span class="sxs-lookup"><span data-stu-id="8c9ea-148">Request 1</span></span>

<span data-ttu-id="8c9ea-149">最初の例では、サインインしているユーザーのテナントで定義されているすべての部屋を表す [emailAddress](../resources/emailaddress.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c9ea-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9ea-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c9ea-151">C#</span><span class="sxs-lookup"><span data-stu-id="8c9ea-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c9ea-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9ea-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c9ea-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c9ea-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="8c9ea-154">応答 1</span><span class="sxs-lookup"><span data-stu-id="8c9ea-154">Response 1</span></span>
<span data-ttu-id="8c9ea-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-155">Here is an example of the response.</span></span> 

<span data-ttu-id="8c9ea-p106">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="8c9ea-158">要求 2</span><span class="sxs-lookup"><span data-stu-id="8c9ea-158">Request 2</span></span>

<span data-ttu-id="8c9ea-159">2 番目の例では、メール アドレス Building2Rooms@contoso.onmicrosoft.com で識別される特定の部屋の一覧の部屋を表す [emailAddress](../resources/emailaddress.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c9ea-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9ea-160">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c9ea-161">C#</span><span class="sxs-lookup"><span data-stu-id="8c9ea-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c9ea-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9ea-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c9ea-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c9ea-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="8c9ea-164">応答 2</span><span class="sxs-lookup"><span data-stu-id="8c9ea-164">Response 2</span></span>
<span data-ttu-id="8c9ea-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-165">Here is an example of the response.</span></span> 

<span data-ttu-id="8c9ea-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c9ea-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
