---
title: 'bookingAppointment: キャンセル'
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: ffb800b5084177b05b62e1ba14b475b8a760d766
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844479"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="a26a8-104">bookingAppointment: キャンセル</span><span class="sxs-lookup"><span data-stu-id="a26a8-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="a26a8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a26a8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a26a8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a26a8-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a26a8-107">指定された[bookingbusiness](../resources/bookingbusiness.md)では、指定された[bookingAppointment](../resources/bookingappointment.md)をキャンセルし、関連する顧客とスタッフのメンバーにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="a26a8-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a26a8-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a26a8-108">Permissions</span></span>
<span data-ttu-id="a26a8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a26a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26a8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a26a8-111">Permission type</span></span>      | <span data-ttu-id="a26a8-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a26a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a26a8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a26a8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="a26a8-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a26a8-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a26a8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a26a8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a26a8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a26a8-116">Not supported.</span></span>   |
|<span data-ttu-id="a26a8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a26a8-117">Application</span></span> | <span data-ttu-id="a26a8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a26a8-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="a26a8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a26a8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="a26a8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a26a8-120">Request headers</span></span>
| <span data-ttu-id="a26a8-121">名前</span><span class="sxs-lookup"><span data-stu-id="a26a8-121">Name</span></span>       | <span data-ttu-id="a26a8-122">説明</span><span class="sxs-lookup"><span data-stu-id="a26a8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a26a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a26a8-123">Authorization</span></span>  | <span data-ttu-id="a26a8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a26a8-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a26a8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a26a8-125">Request body</span></span>
<span data-ttu-id="a26a8-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a26a8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a26a8-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a26a8-127">Parameter</span></span>    | <span data-ttu-id="a26a8-128">Type</span><span class="sxs-lookup"><span data-stu-id="a26a8-128">Type</span></span>   |<span data-ttu-id="a26a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="a26a8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a26a8-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="a26a8-130">cancellationMessage</span></span>|<span data-ttu-id="a26a8-131">String</span><span class="sxs-lookup"><span data-stu-id="a26a8-131">String</span></span>|<span data-ttu-id="a26a8-132">予定が取り消されましたことをお客様と確認のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="a26a8-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="a26a8-133">応答</span><span class="sxs-lookup"><span data-stu-id="a26a8-133">Response</span></span>
<span data-ttu-id="a26a8-p104">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a26a8-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="a26a8-136">Exisit ではありませんが、予定をキャンセルしようかどうか、このメソッドを返します`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="a26a8-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="a26a8-137">例</span><span class="sxs-lookup"><span data-stu-id="a26a8-137">Example</span></span>
<span data-ttu-id="a26a8-138">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="a26a8-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a26a8-139">要求</span><span class="sxs-lookup"><span data-stu-id="a26a8-139">Request</span></span>
<span data-ttu-id="a26a8-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a26a8-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

##### <a name="response"></a><span data-ttu-id="a26a8-141">応答</span><span class="sxs-lookup"><span data-stu-id="a26a8-141">Response</span></span>
<span data-ttu-id="a26a8-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a26a8-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
