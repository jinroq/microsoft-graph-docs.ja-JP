---
title: 場所を取得する
description: Place オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 41487c2b8a474de125a70634427402f97bfeb445
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342384"
---
# <a name="get-place"></a><span data-ttu-id="6fea8-103">場所を取得する</span><span class="sxs-lookup"><span data-stu-id="6fea8-103">Get place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6fea8-104">ID または電子メールアドレスのいずれかで指定された[place](../resources/place.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="6fea8-104">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="6fea8-105">**Place**オブジェクトには、次のいずれかの種類を指定できます。</span><span class="sxs-lookup"><span data-stu-id="6fea8-105">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="6fea8-106">ルーム[](../resources/room.md)には、会議室の電子メールアドレスなどの豊富なプロパティと、アクセシビリティ、容量、デバイスのサポートが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fea8-106">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="6fea8-107">会議室一覧の電子メールアドレスが含まれている[会議室一覧](../resources/roomlist.md)、およびその会議室一覧の**会議室**のインスタンスのコレクションを取得するナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="6fea8-107">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="6fea8-108">**Room**と**roomList**の両方が[place](../resources/place.md)オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="6fea8-108">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6fea8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6fea8-109">Permissions</span></span>

<span data-ttu-id="6fea8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fea8-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fea8-112">Permission type</span></span>                        | <span data-ttu-id="6fea8-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fea8-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6fea8-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fea8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fea8-115">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="6fea8-115">Place.Read.All</span></span> |
| <span data-ttu-id="6fea8-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fea8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fea8-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6fea8-117">Not supported</span></span> |
| <span data-ttu-id="6fea8-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fea8-118">Application</span></span>                            | <span data-ttu-id="6fea8-119">すべてをお読みください。</span><span class="sxs-lookup"><span data-stu-id="6fea8-119">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fea8-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fea8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fea8-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6fea8-121">Optional query parameters</span></span>

<span data-ttu-id="6fea8-122">このメソッドは、応答をカスタマイズするために、次のクエリパラメーターをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6fea8-122">This method supports the following query parameters to help customize the response:</span></span>
* <span data-ttu-id="6fea8-123">$filter</span><span class="sxs-lookup"><span data-stu-id="6fea8-123">$filter</span></span>
* <span data-ttu-id="6fea8-124">$select</span><span class="sxs-lookup"><span data-stu-id="6fea8-124">$select</span></span>
* <span data-ttu-id="6fea8-125">$top</span><span class="sxs-lookup"><span data-stu-id="6fea8-125">$top</span></span>

<span data-ttu-id="6fea8-126">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fea8-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fea8-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fea8-127">Request headers</span></span>

| <span data-ttu-id="6fea8-128">名前</span><span class="sxs-lookup"><span data-stu-id="6fea8-128">Name</span></span>          | <span data-ttu-id="6fea8-129">説明</span><span class="sxs-lookup"><span data-stu-id="6fea8-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6fea8-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fea8-130">Authorization</span></span> | <span data-ttu-id="6fea8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6fea8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fea8-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fea8-133">Request body</span></span>

<span data-ttu-id="6fea8-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6fea8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fea8-135">応答</span><span class="sxs-lookup"><span data-stu-id="6fea8-135">Response</span></span>

<span data-ttu-id="6fea8-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[place](../resources/place.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6fea8-136">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fea8-137">例</span><span class="sxs-lookup"><span data-stu-id="6fea8-137">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="6fea8-138">例 1: ルームを取得する</span><span class="sxs-lookup"><span data-stu-id="6fea8-138">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="6fea8-139">要求</span><span class="sxs-lookup"><span data-stu-id="6fea8-139">Request</span></span>

<span data-ttu-id="6fea8-140">次の例では、プロパティを取得する**ルーム**の**id**を指定しています。</span><span class="sxs-lookup"><span data-stu-id="6fea8-140">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fea8-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6fea8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```http
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fea8-142">C#</span><span class="sxs-lookup"><span data-stu-id="6fea8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fea8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fea8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fea8-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="6fea8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6fea8-145">Java</span><span class="sxs-lookup"><span data-stu-id="6fea8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6fea8-146">応答</span><span class="sxs-lookup"><span data-stu-id="6fea8-146">Response</span></span>

<span data-ttu-id="6fea8-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6fea8-147">The following is an example of the response.</span></span>

><span data-ttu-id="6fea8-148">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="6fea8-148">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6fea8-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6fea8-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_room",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
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
}
```

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="6fea8-150">例 2: 会議室一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="6fea8-150">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="6fea8-151">要求</span><span class="sxs-lookup"><span data-stu-id="6fea8-151">Request</span></span>

<span data-ttu-id="6fea8-152">次の例では、プロパティを取得する**roomList**の**emailAddress**を指定しています。</span><span class="sxs-lookup"><span data-stu-id="6fea8-152">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fea8-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6fea8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fea8-154">C#</span><span class="sxs-lookup"><span data-stu-id="6fea8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fea8-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fea8-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fea8-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="6fea8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6fea8-157">Java</span><span class="sxs-lookup"><span data-stu-id="6fea8-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6fea8-158">応答</span><span class="sxs-lookup"><span data-stu-id="6fea8-158">Response</span></span>

<span data-ttu-id="6fea8-159">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6fea8-159">The following is an example of the response.</span></span>

><span data-ttu-id="6fea8-160">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="6fea8-160">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6fea8-161">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6fea8-161">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
