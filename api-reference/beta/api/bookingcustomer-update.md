---
title: bookingcustomer を更新する
description: bookingcustomer オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 90de81666335c1825e1d134f9b898ee4b6561664
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461732"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="8d3ac-103">bookingcustomer を更新する</span><span class="sxs-lookup"><span data-stu-id="8d3ac-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d3ac-104">[bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d3ac-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d3ac-105">Permissions</span></span>
<span data-ttu-id="8d3ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3ac-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d3ac-108">Permission type</span></span>      | <span data-ttu-id="8d3ac-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d3ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d3ac-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d3ac-111">bookingsappointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="8d3ac-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8d3ac-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3ac-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-113">Not supported.</span></span>   |
|<span data-ttu-id="8d3ac-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d3ac-114">Application</span></span> | <span data-ttu-id="8d3ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8d3ac-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d3ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8d3ac-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d3ac-117">Optional request headers</span></span>
| <span data-ttu-id="8d3ac-118">名前</span><span class="sxs-lookup"><span data-stu-id="8d3ac-118">Name</span></span>       | <span data-ttu-id="8d3ac-119">説明</span><span class="sxs-lookup"><span data-stu-id="8d3ac-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8d3ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3ac-120">Authorization</span></span>  | <span data-ttu-id="8d3ac-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8d3ac-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d3ac-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d3ac-122">Request body</span></span>
<span data-ttu-id="8d3ac-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8d3ac-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d3ac-126">Property</span></span>     | <span data-ttu-id="8d3ac-127">型</span><span class="sxs-lookup"><span data-stu-id="8d3ac-127">Type</span></span>   |<span data-ttu-id="8d3ac-128">説明</span><span class="sxs-lookup"><span data-stu-id="8d3ac-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d3ac-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8d3ac-129">displayName</span></span>|<span data-ttu-id="8d3ac-130">String</span><span class="sxs-lookup"><span data-stu-id="8d3ac-130">String</span></span>|<span data-ttu-id="8d3ac-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-131">The name of the customer.</span></span>|
|<span data-ttu-id="8d3ac-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8d3ac-132">emailAddress</span></span>|<span data-ttu-id="8d3ac-133">String</span><span class="sxs-lookup"><span data-stu-id="8d3ac-133">String</span></span>|<span data-ttu-id="8d3ac-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="8d3ac-135">応答</span><span class="sxs-lookup"><span data-stu-id="8d3ac-135">Response</span></span>
<span data-ttu-id="8d3ac-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d3ac-137">例</span><span class="sxs-lookup"><span data-stu-id="8d3ac-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d3ac-138">要求</span><span class="sxs-lookup"><span data-stu-id="8d3ac-138">Request</span></span>
<span data-ttu-id="8d3ac-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="8d3ac-140">応答</span><span class="sxs-lookup"><span data-stu-id="8d3ac-140">Response</span></span>
<span data-ttu-id="8d3ac-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-141">The following is an example of the response.</span></span> <span data-ttu-id="8d3ac-142">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8d3ac-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d3ac-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
