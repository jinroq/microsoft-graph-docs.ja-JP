---
title: BookingBusiness を作成します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: aa5c4b9eaa2426736d23f42856d19ab14e6a1a43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922320"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="a7ed3-104">BookingBusiness を作成します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-104">Create bookingBusiness</span></span>

 > <span data-ttu-id="a7ed3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7ed3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a7ed3-107">テナント内には、新しい Microsoft 予約ビジネスを作成します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-107">Create a new Microsoft Bookings business in a tenant.</span></span> 

<span data-ttu-id="a7ed3-108">これは、ビジネスの表示名を指定する必要があります予約のビジネスのセットアップの最初のステップです。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-108">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="a7ed3-109">会社の住所、web サイトのアドレス、およびスケジュー リング ポリシーは、他の情報が含まれます。 または情報の設定を後で[更新](bookingbusiness-update.md)することで**bookingBusiness**できます。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-109">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7ed3-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7ed3-110">Permissions</span></span>
<span data-ttu-id="a7ed3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ed3-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7ed3-113">Permission type</span></span>      | <span data-ttu-id="a7ed3-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7ed3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7ed3-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7ed3-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="a7ed3-116">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a7ed3-116">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="a7ed3-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7ed3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7ed3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-118">Not supported.</span></span>   |
|<span data-ttu-id="a7ed3-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7ed3-119">Application</span></span> | <span data-ttu-id="a7ed3-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a7ed3-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7ed3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="a7ed3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7ed3-122">Request headers</span></span>
| <span data-ttu-id="a7ed3-123">名前</span><span class="sxs-lookup"><span data-stu-id="a7ed3-123">Name</span></span>       | <span data-ttu-id="a7ed3-124">説明</span><span class="sxs-lookup"><span data-stu-id="a7ed3-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7ed3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7ed3-125">Authorization</span></span>  | <span data-ttu-id="a7ed3-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a7ed3-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ed3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7ed3-127">Request body</span></span>
<span data-ttu-id="a7ed3-128">要求の本文には、 [bookingBusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-128">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a7ed3-129">応答</span><span class="sxs-lookup"><span data-stu-id="a7ed3-129">Response</span></span>
<span data-ttu-id="a7ed3-130">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingBusiness](../resources/bookingbusiness.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-130">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ed3-131">例</span><span class="sxs-lookup"><span data-stu-id="a7ed3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7ed3-132">要求</span><span class="sxs-lookup"><span data-stu-id="a7ed3-132">Request</span></span>
<span data-ttu-id="a7ed3-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-133">The following is an example of the request.</span></span>
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
<span data-ttu-id="a7ed3-134">要求の本文には、 [bookingBusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-134">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7ed3-135">応答</span><span class="sxs-lookup"><span data-stu-id="a7ed3-135">Response</span></span>
<span data-ttu-id="a7ed3-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-136">The following is an example of the response.</span></span> <span data-ttu-id="a7ed3-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a7ed3-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a7ed3-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
