---
title: BookingCustomer を作成します。
description: 新しい bookingCustomer オブジェクトを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4557d65edf4727659fdae94599c0796fc940ed1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523961"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="df4a6-103">BookingCustomer を作成します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df4a6-104">新しい[bookingCustomer](../resources/bookingcustomer.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="df4a6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df4a6-105">Permissions</span></span>
<span data-ttu-id="df4a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df4a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4a6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df4a6-108">Permission type</span></span>      | <span data-ttu-id="df4a6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="df4a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df4a6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df4a6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="df4a6-111">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="df4a6-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="df4a6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df4a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df4a6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df4a6-113">Not supported.</span></span>   |
|<span data-ttu-id="df4a6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df4a6-114">Application</span></span> | <span data-ttu-id="df4a6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df4a6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="df4a6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df4a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="df4a6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df4a6-117">Request headers</span></span>
| <span data-ttu-id="df4a6-118">名前</span><span class="sxs-lookup"><span data-stu-id="df4a6-118">Name</span></span>       | <span data-ttu-id="df4a6-119">説明</span><span class="sxs-lookup"><span data-stu-id="df4a6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df4a6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="df4a6-120">Authorization</span></span>  | <span data-ttu-id="df4a6-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="df4a6-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4a6-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="df4a6-122">Request body</span></span>
<span data-ttu-id="df4a6-123">要求の本文には、 [bookingCustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="df4a6-124">応答</span><span class="sxs-lookup"><span data-stu-id="df4a6-124">Response</span></span>
<span data-ttu-id="df4a6-125">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingCustomer](../resources/bookingcustomer.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="df4a6-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df4a6-126">例</span><span class="sxs-lookup"><span data-stu-id="df4a6-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df4a6-127">要求</span><span class="sxs-lookup"><span data-stu-id="df4a6-127">Request</span></span>
<span data-ttu-id="df4a6-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers

Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="df4a6-129">要求の本文には、 [bookingCustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="df4a6-130">応答</span><span class="sxs-lookup"><span data-stu-id="df4a6-130">Response</span></span>
<span data-ttu-id="df4a6-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df4a6-131">The following is an example of the response.</span></span> <span data-ttu-id="df4a6-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="df4a6-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="df4a6-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="df4a6-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
