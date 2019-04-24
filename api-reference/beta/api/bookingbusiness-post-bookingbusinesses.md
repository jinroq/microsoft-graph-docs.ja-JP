---
title: bookingbusiness の作成
description: テナントに新しい Microsoft 予約ビジネスを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a9217392953d287689dca7a7b6f4c74fbe6383
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461765"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="2b2e5-103">bookingbusiness の作成</span><span class="sxs-lookup"><span data-stu-id="2b2e5-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b2e5-104">テナントに新しい Microsoft 予約ビジネスを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="2b2e5-105">これは、ビジネス表示名を指定する必要がある、予約ビジネスを設定するための最初の手順です。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="2b2e5-106">会社の住所、web サイトのアドレス、スケジュールポリシーなどのその他の情報を含めたり、後で**bookingbusiness**を[更新](bookingbusiness-update.md)してその情報を設定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b2e5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b2e5-107">Permissions</span></span>
<span data-ttu-id="2b2e5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b2e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b2e5-110">Permission type</span></span>      | <span data-ttu-id="2b2e5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b2e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b2e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b2e5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b2e5-113">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="2b2e5-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="2b2e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b2e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b2e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-115">Not supported.</span></span>   |
|<span data-ttu-id="2b2e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b2e5-116">Application</span></span> | <span data-ttu-id="2b2e5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b2e5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b2e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="2b2e5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b2e5-119">Request headers</span></span>
| <span data-ttu-id="2b2e5-120">名前</span><span class="sxs-lookup"><span data-stu-id="2b2e5-120">Name</span></span>       | <span data-ttu-id="2b2e5-121">説明</span><span class="sxs-lookup"><span data-stu-id="2b2e5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b2e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b2e5-122">Authorization</span></span>  | <span data-ttu-id="2b2e5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2b2e5-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b2e5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b2e5-124">Request body</span></span>
<span data-ttu-id="2b2e5-125">要求本文で、 [bookingbusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2b2e5-126">応答</span><span class="sxs-lookup"><span data-stu-id="2b2e5-126">Response</span></span>
<span data-ttu-id="2b2e5-127">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[bookingbusiness](../resources/bookingbusiness.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b2e5-128">例</span><span class="sxs-lookup"><span data-stu-id="2b2e5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b2e5-129">要求</span><span class="sxs-lookup"><span data-stu-id="2b2e5-129">Request</span></span>
<span data-ttu-id="2b2e5-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="2b2e5-131">要求本文で、 [bookingbusiness](../resources/bookingbusiness.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2b2e5-132">応答</span><span class="sxs-lookup"><span data-stu-id="2b2e5-132">Response</span></span>
<span data-ttu-id="2b2e5-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-133">The following is an example of the response.</span></span> <span data-ttu-id="2b2e5-134">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2b2e5-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2b2e5-135">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
