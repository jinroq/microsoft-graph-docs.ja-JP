---
title: プレースを一覧表示する
description: Place オブジェクトのリストを取得します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 27835ec7eea8c1bd40fd07be41900171465da3e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876784"
---
# <a name="list-places"></a><span data-ttu-id="1c07a-103">プレースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1c07a-103">List places</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c07a-104">テナントで定義されている、指定された種類の[プレース](../resources/place.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-104">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="1c07a-105">たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1c07a-105">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="1c07a-106">**Place**オブジェクトには、次の種類のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="1c07a-106">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="1c07a-107">ルーム[](../resources/room.md)には、会議室の電子メールアドレスなどの豊富なプロパティと、アクセシビリティ、容量、デバイスのサポートが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c07a-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="1c07a-108">会議室リストのメールアドレスが含まれる[会議室一覧](../resources/roomlist.md)と、会議室一覧の会議室のインスタンスのコレクションを取得するナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1c07a-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="1c07a-109">**Room**と**roomList**の両方が**place**オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-109">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="1c07a-110">この操作は、 [Fin/oms](../api/user-findrooms.md)および[fin/omlists](../api/user-findroomlists.md)関数と比較して、ルームおよび会議室のリストに関する豊富なペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-110">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="1c07a-111">その違いについては、「[詳細](../resources/place.md#using-the-places-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c07a-111">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c07a-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c07a-112">Permissions</span></span>

<span data-ttu-id="1c07a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c07a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c07a-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c07a-115">Permission type</span></span>                        | <span data-ttu-id="1c07a-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c07a-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c07a-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c07a-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c07a-118">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="1c07a-118">Place.Read.All</span></span> |
| <span data-ttu-id="1c07a-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c07a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c07a-120">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1c07a-120">Not supported</span></span> |
| <span data-ttu-id="1c07a-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c07a-121">Application</span></span>                            | <span data-ttu-id="1c07a-122">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="1c07a-122">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c07a-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c07a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="1c07a-124">テナント内のすべてのルームを取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1c07a-124">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="1c07a-125">テナント内のすべての会議室一覧を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1c07a-125">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="1c07a-126">指定した会議室一覧のすべての会議室を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1c07a-126">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="1c07a-127">**注**: 会議室一覧の会議室を取得するには、その**id**ではなく、 **emailAddress**プロパティで会議室一覧を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c07a-127">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="1c07a-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c07a-128">Optional query parameters</span></span>

<span data-ttu-id="1c07a-129">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1c07a-129">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1c07a-130">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c07a-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c07a-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c07a-131">Request headers</span></span>

| <span data-ttu-id="1c07a-132">名前</span><span class="sxs-lookup"><span data-stu-id="1c07a-132">Name</span></span>          | <span data-ttu-id="1c07a-133">説明</span><span class="sxs-lookup"><span data-stu-id="1c07a-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1c07a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c07a-134">Authorization</span></span> | <span data-ttu-id="1c07a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c07a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c07a-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c07a-137">Request body</span></span>

<span data-ttu-id="1c07a-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c07a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c07a-139">応答</span><span class="sxs-lookup"><span data-stu-id="1c07a-139">Response</span></span>

<span data-ttu-id="1c07a-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[place](../resources/place.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-140">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c07a-141">例</span><span class="sxs-lookup"><span data-stu-id="1c07a-141">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="1c07a-142">例 1: テナントで定義されているすべてのルームを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1c07a-142">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1c07a-143">要求</span><span class="sxs-lookup"><span data-stu-id="1c07a-143">Request</span></span>

<span data-ttu-id="1c07a-144">次の例は、テナント内のすべての[room](../resources/room.md)オブジェクトを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1c07a-144">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c07a-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c07a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c07a-146">C#</span><span class="sxs-lookup"><span data-stu-id="1c07a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c07a-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c07a-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c07a-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c07a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c07a-149">Java</span><span class="sxs-lookup"><span data-stu-id="1c07a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c07a-150">応答</span><span class="sxs-lookup"><span data-stu-id="1c07a-150">Response</span></span>

<span data-ttu-id="1c07a-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-151">The following is an example of the response.</span></span>

><span data-ttu-id="1c07a-152">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1c07a-152">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c07a-153">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1c07a-153">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_rooms",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.room",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
      "emailAddress": "cf100@contoso.com",
      "displayName": "Conf Room 100",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488626,
        "longitude": -122.1293731033803
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "100",
      "capacity": "50",
      "building": "1",
      "floorNumber": 1,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "bean bags"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    },
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="1c07a-154">例 2: テナントで定義されているすべての会議室一覧を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1c07a-154">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1c07a-155">要求</span><span class="sxs-lookup"><span data-stu-id="1c07a-155">Request</span></span>

<span data-ttu-id="1c07a-156">次の例は、テナント内のすべての[roomList](../resources/roomlist.md)オブジェクトを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1c07a-156">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c07a-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c07a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c07a-158">C#</span><span class="sxs-lookup"><span data-stu-id="1c07a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c07a-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c07a-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c07a-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c07a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c07a-161">Java</span><span class="sxs-lookup"><span data-stu-id="1c07a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c07a-162">応答</span><span class="sxs-lookup"><span data-stu-id="1c07a-162">Response</span></span>

<span data-ttu-id="1c07a-163">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-163">The following is an example of the response.</span></span>

><span data-ttu-id="1c07a-164">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1c07a-164">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c07a-165">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1c07a-165">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_roomlists",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.roomList",
  "value": [
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
      "displayName": "Building 1",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg1@contoso.com"
    },
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1706",
      "displayName": "Building 2",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg2@contoso.com"
    }
  ]
}
```

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="1c07a-166">例 3: ルームリストに含まれているルームのリスト</span><span class="sxs-lookup"><span data-stu-id="1c07a-166">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="1c07a-167">要求</span><span class="sxs-lookup"><span data-stu-id="1c07a-167">Request</span></span>

<span data-ttu-id="1c07a-168">次の例は、 **roomList**に含まれる[room](../resources/room.md)オブジェクトの一覧を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1c07a-168">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="1c07a-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c07a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c07a-170">C#</span><span class="sxs-lookup"><span data-stu-id="1c07a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c07a-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c07a-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c07a-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c07a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c07a-173">Java</span><span class="sxs-lookup"><span data-stu-id="1c07a-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c07a-174">応答</span><span class="sxs-lookup"><span data-stu-id="1c07a-174">Response</span></span>

<span data-ttu-id="1c07a-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c07a-175">The following is an example of the response.</span></span>

><span data-ttu-id="1c07a-176">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1c07a-176">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c07a-177">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1c07a-177">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_rooms_in_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List places",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Malformed function params 'id-of-roomlist'"
  ]
}-->
