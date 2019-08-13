---
title: 'user: findRoomLists'
description: テナントで定義された部屋の一覧を取得します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c2d3fce0952864ef6eade0df81233be2e03bac0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362473"
---
# <a name="user-findroomlists"></a><span data-ttu-id="cc12e-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="cc12e-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc12e-104">[emailAddress](../resources/emailaddress.md) オブジェクトで表されるように、テナントに定義されている会議室一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc12e-104">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="cc12e-105">テナントは会議室を部屋の一覧に整理できます。</span><span class="sxs-lookup"><span data-stu-id="cc12e-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="cc12e-106">この API 内で、それぞれの会議室と部屋の一覧は、[emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="cc12e-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="cc12e-107">テナント内のすべての部屋の一覧を取得できます。また、テナント内の[すべての部屋を取得](user-findrooms.md)したり、または特定の部屋の一覧の[すべての部屋を取得](user-findrooms.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="cc12e-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="cc12e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc12e-108">Permissions</span></span>
<span data-ttu-id="cc12e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc12e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cc12e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc12e-111">Permission type</span></span>      | <span data-ttu-id="cc12e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc12e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc12e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc12e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cc12e-114">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc12e-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="cc12e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc12e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc12e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc12e-116">Not supported.</span></span>    |
|<span data-ttu-id="cc12e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc12e-117">Application</span></span> | <span data-ttu-id="cc12e-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc12e-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc12e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc12e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="cc12e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc12e-120">Request headers</span></span>
| <span data-ttu-id="cc12e-121">名前</span><span class="sxs-lookup"><span data-stu-id="cc12e-121">Name</span></span>       | <span data-ttu-id="cc12e-122">種類</span><span class="sxs-lookup"><span data-stu-id="cc12e-122">Type</span></span> | <span data-ttu-id="cc12e-123">説明</span><span class="sxs-lookup"><span data-stu-id="cc12e-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="cc12e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc12e-124">Authorization</span></span>  | <span data-ttu-id="cc12e-125">string</span><span class="sxs-lookup"><span data-stu-id="cc12e-125">string</span></span>  | <span data-ttu-id="cc12e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc12e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc12e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc12e-128">Content-Type</span></span>  | <span data-ttu-id="cc12e-129">string</span><span class="sxs-lookup"><span data-stu-id="cc12e-129">string</span></span>  | <span data-ttu-id="cc12e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc12e-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="cc12e-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc12e-132">Request body</span></span>
<span data-ttu-id="cc12e-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cc12e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc12e-134">応答</span><span class="sxs-lookup"><span data-stu-id="cc12e-134">Response</span></span>

<span data-ttu-id="cc12e-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [emailAddress](../resources/emailaddress.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cc12e-135">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="cc12e-136">テナントで定義されている一覧が存在しない場合は、空の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="cc12e-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="cc12e-137">例</span><span class="sxs-lookup"><span data-stu-id="cc12e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc12e-138">要求</span><span class="sxs-lookup"><span data-stu-id="cc12e-138">Request</span></span>

<span data-ttu-id="cc12e-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc12e-139">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cc12e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc12e-140">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc12e-141">C#</span><span class="sxs-lookup"><span data-stu-id="cc12e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc12e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc12e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc12e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc12e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc12e-144">Java</span><span class="sxs-lookup"><span data-stu-id="cc12e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-room-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cc12e-145">応答</span><span class="sxs-lookup"><span data-stu-id="cc12e-145">Response</span></span>
<span data-ttu-id="cc12e-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cc12e-146">Here is an example of the response.</span></span> 

<span data-ttu-id="cc12e-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc12e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
