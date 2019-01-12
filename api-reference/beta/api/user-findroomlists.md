---
title: 'ユーザー: findRoomLists'
description: テナントで定義された部屋の一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f170b40689b09f54ea53632ca113018de1671b4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979293"
---
# <a name="user-findroomlists"></a><span data-ttu-id="4e9c0-103">ユーザー: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="4e9c0-103">user: findRoomLists</span></span>

> <span data-ttu-id="4e9c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e9c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e9c0-106">テナントで定義された部屋の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="4e9c0-107">テナントは、ルーム リストに会議室を整理できます。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="4e9c0-108">各会議室や部屋の一覧は、 [emailAddress](../resources/emailaddress.md)インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="4e9c0-109">テナント、テナント内の[すべての部屋を取得](user-findrooms.md)を、または[すべての会議室を取得する](user-findrooms.md)特定の会議室の一覧で [すべてのルーム一覧を取得できます。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="4e9c0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e9c0-110">Permissions</span></span>
<span data-ttu-id="4e9c0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e9c0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e9c0-113">Permission type</span></span>      | <span data-ttu-id="4e9c0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e9c0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e9c0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e9c0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4e9c0-116">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e9c0-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="4e9c0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e9c0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e9c0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-118">Not supported.</span></span>    |
|<span data-ttu-id="4e9c0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e9c0-119">Application</span></span> | <span data-ttu-id="4e9c0-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e9c0-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e9c0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e9c0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="4e9c0-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e9c0-122">Request headers</span></span>
| <span data-ttu-id="4e9c0-123">名前</span><span class="sxs-lookup"><span data-stu-id="4e9c0-123">Name</span></span>       | <span data-ttu-id="4e9c0-124">型</span><span class="sxs-lookup"><span data-stu-id="4e9c0-124">Type</span></span> | <span data-ttu-id="4e9c0-125">説明</span><span class="sxs-lookup"><span data-stu-id="4e9c0-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4e9c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e9c0-126">Authorization</span></span>  | <span data-ttu-id="4e9c0-127">string</span><span class="sxs-lookup"><span data-stu-id="4e9c0-127">string</span></span>  | <span data-ttu-id="4e9c0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e9c0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e9c0-130">Content-Type</span></span>  | <span data-ttu-id="4e9c0-131">string</span><span class="sxs-lookup"><span data-stu-id="4e9c0-131">string</span></span>  | <span data-ttu-id="4e9c0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4e9c0-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4e9c0-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e9c0-134">Request body</span></span>
<span data-ttu-id="4e9c0-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e9c0-136">応答</span><span class="sxs-lookup"><span data-stu-id="4e9c0-136">Response</span></span>

<span data-ttu-id="4e9c0-137">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードおよび[emailAddress](../resources/emailaddress.md)コレクション オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="4e9c0-138">テナントのリストが定義されていない場合は、空の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="4e9c0-139">例</span><span class="sxs-lookup"><span data-stu-id="4e9c0-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e9c0-140">要求</span><span class="sxs-lookup"><span data-stu-id="4e9c0-140">Request</span></span>

<span data-ttu-id="4e9c0-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="4e9c0-142">応答</span><span class="sxs-lookup"><span data-stu-id="4e9c0-142">Response</span></span>
<span data-ttu-id="4e9c0-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-143">Here is an example of the response.</span></span> 

<span data-ttu-id="4e9c0-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e9c0-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
