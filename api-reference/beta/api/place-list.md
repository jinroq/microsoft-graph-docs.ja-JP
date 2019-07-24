---
title: プレースを一覧表示する
description: Place オブジェクトのリストを取得します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 173273bac942e8c2b2084109a1a50af3da579a53
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841053"
---
# <a name="list-places"></a><span data-ttu-id="8b706-103">プレースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8b706-103">List places</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b706-104">テナントで定義されている、指定された種類の[プレース](../resources/place.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8b706-104">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="8b706-105">たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8b706-105">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="8b706-106">**Place**オブジェクトには、次の種類のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="8b706-106">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="8b706-107">ルーム[](../resources/room.md)には、会議室の電子メールアドレスなどの豊富なプロパティと、アクセシビリティ、容量、デバイスのサポートが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8b706-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="8b706-108">会議室リストのメールアドレスが含まれる[会議室一覧](../resources/roomlist.md)と、会議室一覧の会議室のインスタンスのコレクションを取得するナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="8b706-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="8b706-109">**Room**と**roomList**の両方が**place**オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="8b706-109">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="8b706-110">この操作は、 [Fin/oms](../api/user-findrooms.md)および[fin/omlists](../api/user-findroomlists.md)関数と比較して、ルームおよび会議室のリストに関する豊富なペイロードを返します。</span><span class="sxs-lookup"><span data-stu-id="8b706-110">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="8b706-111">その違いについては、「[詳細](../resources/place.md#using-the-places-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b706-111">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b706-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b706-112">Permissions</span></span>

<span data-ttu-id="8b706-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b706-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b706-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b706-115">Permission type</span></span>                        | <span data-ttu-id="8b706-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b706-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b706-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b706-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b706-118">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="8b706-118">Place.Read.All</span></span> |
| <span data-ttu-id="8b706-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b706-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b706-120">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="8b706-120">Not supported</span></span> |
| <span data-ttu-id="8b706-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b706-121">Application</span></span>                            | <span data-ttu-id="8b706-122">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="8b706-122">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b706-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b706-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8b706-124">テナント内のすべてのルームを取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8b706-124">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="8b706-125">テナント内のすべての会議室一覧を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8b706-125">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="8b706-126">指定した会議室一覧のすべての会議室を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8b706-126">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="8b706-127">**注**: 会議室一覧の会議室を取得するには、その**id**ではなく、 **emailAddress**プロパティで会議室一覧を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b706-127">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="8b706-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b706-128">Optional query parameters</span></span>

<span data-ttu-id="8b706-129">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8b706-129">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8b706-130">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b706-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b706-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b706-131">Request headers</span></span>

| <span data-ttu-id="8b706-132">名前</span><span class="sxs-lookup"><span data-stu-id="8b706-132">Name</span></span>          | <span data-ttu-id="8b706-133">説明</span><span class="sxs-lookup"><span data-stu-id="8b706-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8b706-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b706-134">Authorization</span></span> | <span data-ttu-id="8b706-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b706-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b706-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b706-137">Request body</span></span>

<span data-ttu-id="8b706-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8b706-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b706-139">応答</span><span class="sxs-lookup"><span data-stu-id="8b706-139">Response</span></span>

<span data-ttu-id="8b706-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[place](../resources/place.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8b706-140">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b706-141">例</span><span class="sxs-lookup"><span data-stu-id="8b706-141">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="8b706-142">例 1: テナントで定義されているすべてのルームを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8b706-142">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8b706-143">要求</span><span class="sxs-lookup"><span data-stu-id="8b706-143">Request</span></span>

<span data-ttu-id="8b706-144">次の例は、テナント内のすべての[room](../resources/room.md)オブジェクトを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8b706-144">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```

#### <a name="response"></a><span data-ttu-id="8b706-145">応答</span><span class="sxs-lookup"><span data-stu-id="8b706-145">Response</span></span>

<span data-ttu-id="8b706-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b706-146">The following is an example of the response.</span></span>

><span data-ttu-id="8b706-147">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b706-147">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b706-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b706-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="8b706-149">例 2: テナントで定義されているすべての会議室一覧を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8b706-149">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8b706-150">要求</span><span class="sxs-lookup"><span data-stu-id="8b706-150">Request</span></span>

<span data-ttu-id="8b706-151">次の例は、テナント内のすべての[roomList](../resources/roomlist.md)オブジェクトを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8b706-151">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```

#### <a name="response"></a><span data-ttu-id="8b706-152">応答</span><span class="sxs-lookup"><span data-stu-id="8b706-152">Response</span></span>

<span data-ttu-id="8b706-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b706-153">The following is an example of the response.</span></span>

><span data-ttu-id="8b706-154">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b706-154">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b706-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b706-155">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="8b706-156">例 3: ルームリストに含まれているルームのリスト</span><span class="sxs-lookup"><span data-stu-id="8b706-156">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="8b706-157">要求</span><span class="sxs-lookup"><span data-stu-id="8b706-157">Request</span></span>

<span data-ttu-id="8b706-158">次の例は、 **roomList**に含まれる[room](../resources/room.md)オブジェクトの一覧を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8b706-158">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```

#### <a name="response"></a><span data-ttu-id="8b706-159">応答</span><span class="sxs-lookup"><span data-stu-id="8b706-159">Response</span></span>

<span data-ttu-id="8b706-160">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b706-160">The following is an example of the response.</span></span>

><span data-ttu-id="8b706-161">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b706-161">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b706-162">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b706-162">All the properties will be returned from an actual call.</span></span>

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
