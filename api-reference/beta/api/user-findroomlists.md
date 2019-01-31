---
title: 'user: findRoomLists'
description: テナントで定義された部屋の一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cc26367c9cecd16604f7cfefb3be5ce265e3c2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520579"
---
# <a name="user-findroomlists"></a><span data-ttu-id="cb689-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="cb689-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb689-104">テナントで定義された部屋の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="cb689-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="cb689-105">テナントは会議室を部屋の一覧に整理できます。</span><span class="sxs-lookup"><span data-stu-id="cb689-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="cb689-106">それぞれの会議室と部屋の一覧は、[emailAddress](../resources/emailaddress.md) インスタンスによって表されます。</span><span class="sxs-lookup"><span data-stu-id="cb689-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="cb689-107">テナント内のすべての部屋の一覧を取得できます。また、テナント内の[すべての部屋を取得](user-findrooms.md)したり、または特定の部屋の一覧の[すべての部屋を取得](user-findrooms.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="cb689-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="cb689-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb689-108">Permissions</span></span>
<span data-ttu-id="cb689-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb689-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cb689-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb689-111">Permission type</span></span>      | <span data-ttu-id="cb689-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb689-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb689-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb689-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cb689-114">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb689-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb689-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb689-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb689-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb689-116">Not supported.</span></span>    |
|<span data-ttu-id="cb689-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb689-117">Application</span></span> | <span data-ttu-id="cb689-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb689-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb689-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb689-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="cb689-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb689-120">Request headers</span></span>
| <span data-ttu-id="cb689-121">名前</span><span class="sxs-lookup"><span data-stu-id="cb689-121">Name</span></span>       | <span data-ttu-id="cb689-122">型</span><span class="sxs-lookup"><span data-stu-id="cb689-122">Type</span></span> | <span data-ttu-id="cb689-123">説明</span><span class="sxs-lookup"><span data-stu-id="cb689-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="cb689-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb689-124">Authorization</span></span>  | <span data-ttu-id="cb689-125">string</span><span class="sxs-lookup"><span data-stu-id="cb689-125">string</span></span>  | <span data-ttu-id="cb689-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb689-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb689-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb689-128">Content-Type</span></span>  | <span data-ttu-id="cb689-129">string</span><span class="sxs-lookup"><span data-stu-id="cb689-129">string</span></span>  | <span data-ttu-id="cb689-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb689-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="cb689-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb689-132">Request body</span></span>
<span data-ttu-id="cb689-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cb689-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb689-134">応答</span><span class="sxs-lookup"><span data-stu-id="cb689-134">Response</span></span>

<span data-ttu-id="cb689-135">成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [emailAddress](../resources/emailaddress.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb689-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="cb689-136">テナントで定義されている一覧が存在しない場合は、空の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="cb689-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="cb689-137">例</span><span class="sxs-lookup"><span data-stu-id="cb689-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb689-138">要求</span><span class="sxs-lookup"><span data-stu-id="cb689-138">Request</span></span>

<span data-ttu-id="cb689-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb689-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="cb689-140">応答</span><span class="sxs-lookup"><span data-stu-id="cb689-140">Response</span></span>
<span data-ttu-id="cb689-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cb689-141">Here is an example of the response.</span></span> 

<span data-ttu-id="cb689-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb689-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
