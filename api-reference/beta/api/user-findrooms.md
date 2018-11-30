---
title: 'ユーザー: findRooms'
description: 'すべての会議室ユーザーのテナントや、特定の場所] ボックスの一覧を取得します。 '
ms.openlocfilehash: 3169202f83af0696cbd2aaadd83d3beb9a3c01d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071827"
---
# <a name="user-findrooms"></a><span data-ttu-id="79cd1-103">ユーザー: findRooms</span><span class="sxs-lookup"><span data-stu-id="79cd1-103">user: findRooms</span></span>

> <span data-ttu-id="79cd1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79cd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79cd1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79cd1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79cd1-106">すべての会議室ユーザーのテナントや、特定の場所] ボックスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="79cd1-107">テナントは、ルーム リストに会議室を整理できます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="79cd1-108">各会議室や部屋の一覧は、 [emailAddress](../resources/emailaddress.md)インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="79cd1-109">[ルームのすべてのリストを取得](user-findroomlists.md)することができます、テナント、テナント内のすべての部屋を取得または特定の会議室の一覧内のすべての会議室を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="79cd1-110">テナントの最初の 100 室取得できます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="79cd1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79cd1-111">Permissions</span></span>
<span data-ttu-id="79cd1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79cd1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="79cd1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79cd1-114">Permission type</span></span>      | <span data-ttu-id="79cd1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79cd1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79cd1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79cd1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="79cd1-117">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79cd1-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="79cd1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79cd1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79cd1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79cd1-119">Not supported.</span></span>    |
|<span data-ttu-id="79cd1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79cd1-120">Application</span></span> | <span data-ttu-id="79cd1-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="79cd1-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79cd1-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79cd1-122">HTTP request</span></span>

<span data-ttu-id="79cd1-123">テナント内のすべての部屋を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="79cd1-124">テナントの特定の会議室の一覧内のすべての会議室を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="79cd1-125">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79cd1-125">Query parameters</span></span>

| <span data-ttu-id="79cd1-126">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79cd1-126">Query parameter</span></span>       | <span data-ttu-id="79cd1-127">種類</span><span class="sxs-lookup"><span data-stu-id="79cd1-127">Type</span></span> | <span data-ttu-id="79cd1-128">説明</span><span class="sxs-lookup"><span data-stu-id="79cd1-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="79cd1-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="79cd1-129">RoomList</span></span> | <span data-ttu-id="79cd1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="79cd1-130">string</span></span> | <span data-ttu-id="79cd1-131">ルームのリストに関連付けられている SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="79cd1-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="79cd1-132">[EmailAddress](../resources/emailaddress.md)インスタンス、SMTP アドレスが含まれている各部屋の一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="79cd1-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79cd1-133">Request headers</span></span>
| <span data-ttu-id="79cd1-134">名前</span><span class="sxs-lookup"><span data-stu-id="79cd1-134">Name</span></span>       | <span data-ttu-id="79cd1-135">型</span><span class="sxs-lookup"><span data-stu-id="79cd1-135">Type</span></span> | <span data-ttu-id="79cd1-136">説明</span><span class="sxs-lookup"><span data-stu-id="79cd1-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="79cd1-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="79cd1-137">Authorization</span></span>  | <span data-ttu-id="79cd1-138">string</span><span class="sxs-lookup"><span data-stu-id="79cd1-138">string</span></span>  | <span data-ttu-id="79cd1-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79cd1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79cd1-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79cd1-141">Content-Type</span></span>  | <span data-ttu-id="79cd1-142">string</span><span class="sxs-lookup"><span data-stu-id="79cd1-142">string</span></span>  | <span data-ttu-id="79cd1-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="79cd1-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="79cd1-145">要求本文</span><span class="sxs-lookup"><span data-stu-id="79cd1-145">Request body</span></span>
<span data-ttu-id="79cd1-146">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79cd1-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79cd1-147">応答</span><span class="sxs-lookup"><span data-stu-id="79cd1-147">Response</span></span>

<span data-ttu-id="79cd1-148">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードおよび[emailAddress](../resources/emailaddress.md)コレクション オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="79cd1-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="79cd1-149">例</span><span class="sxs-lookup"><span data-stu-id="79cd1-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="79cd1-150">要求 1</span><span class="sxs-lookup"><span data-stu-id="79cd1-150">Request 1</span></span>

<span data-ttu-id="79cd1-151">最初の例では、サインインしているユーザーのテナント型で定義されているすべての部屋を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="79cd1-152">応答 1</span><span class="sxs-lookup"><span data-stu-id="79cd1-152">Response 1</span></span>
<span data-ttu-id="79cd1-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="79cd1-153">Here is an example of the response.</span></span> 

<span data-ttu-id="79cd1-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="79cd1-156">要求 2</span><span class="sxs-lookup"><span data-stu-id="79cd1-156">Request 2</span></span>

<span data-ttu-id="79cd1-157">2 番目の例では、Building2Rooms@contoso.onmicrosoft.com の電子メール アドレスで識別される領域を指定したボックスの一覧で 2 つの部屋を取得します。</span><span class="sxs-lookup"><span data-stu-id="79cd1-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="79cd1-158">応答 2</span><span class="sxs-lookup"><span data-stu-id="79cd1-158">Response 2</span></span>
<span data-ttu-id="79cd1-159">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="79cd1-159">Here is an example of the response.</span></span> 

<span data-ttu-id="79cd1-p108">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79cd1-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->