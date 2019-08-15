---
title: BookingBusiness の作成
description: テナントに新しい Microsoft 予約ビジネスを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 552780d9c869750db225d2a32852145e0f8776e7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415522"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="0bfef-103">BookingBusiness の作成</span><span class="sxs-lookup"><span data-stu-id="0bfef-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bfef-104">テナントに新しい Microsoft 予約ビジネスを作成します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="0bfef-105">これは、ビジネス表示名を指定する必要がある、予約ビジネスを設定するための最初の手順です。</span><span class="sxs-lookup"><span data-stu-id="0bfef-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="0bfef-106">会社の住所、web サイトのアドレス、スケジュールポリシーなどのその他の情報を含めたり、後で**Bookingbusiness**を[更新](bookingbusiness-update.md)してその情報を設定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="0bfef-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="0bfef-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0bfef-107">Permissions</span></span>
<span data-ttu-id="0bfef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bfef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bfef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bfef-110">Permission type</span></span>      | <span data-ttu-id="0bfef-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bfef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bfef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bfef-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0bfef-113">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="0bfef-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="0bfef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bfef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bfef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bfef-115">Not supported.</span></span>   |
|<span data-ttu-id="0bfef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bfef-116">Application</span></span> | <span data-ttu-id="0bfef-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bfef-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bfef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bfef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="0bfef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bfef-119">Request headers</span></span>
| <span data-ttu-id="0bfef-120">名前</span><span class="sxs-lookup"><span data-stu-id="0bfef-120">Name</span></span>       | <span data-ttu-id="0bfef-121">説明</span><span class="sxs-lookup"><span data-stu-id="0bfef-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0bfef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bfef-122">Authorization</span></span>  | <span data-ttu-id="0bfef-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0bfef-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bfef-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bfef-124">Request body</span></span>
<span data-ttu-id="0bfef-125">要求本文で、 [Bookingbusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0bfef-126">応答</span><span class="sxs-lookup"><span data-stu-id="0bfef-126">Response</span></span>
<span data-ttu-id="0bfef-127">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[bookingbusiness](../resources/bookingbusiness.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bfef-128">例</span><span class="sxs-lookup"><span data-stu-id="0bfef-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bfef-129">要求</span><span class="sxs-lookup"><span data-stu-id="0bfef-129">Request</span></span>
<span data-ttu-id="0bfef-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0bfef-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0bfef-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json

{
    "displayName":"Fourth Coffee",
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bfef-132">C#</span><span class="sxs-lookup"><span data-stu-id="0bfef-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bfef-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bfef-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bfef-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="0bfef-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0bfef-135">要求本文で、 [Bookingbusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-135">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0bfef-136">応答</span><span class="sxs-lookup"><span data-stu-id="0bfef-136">Response</span></span>
<span data-ttu-id="0bfef-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0bfef-137">The following is an example of the response.</span></span> <span data-ttu-id="0bfef-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0bfef-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0bfef-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0bfef-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"fourthcoffee@M365B489948.onmicrosoft.com",
    "displayName":"Fourth Coffee",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
