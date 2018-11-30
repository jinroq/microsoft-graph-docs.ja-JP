---
title: 'bookingAppointment: キャンセル'
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 4cd7b511f997f32c134f70a976cd94c2ed910fb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066424"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="9ad2e-104">bookingAppointment: キャンセル</span><span class="sxs-lookup"><span data-stu-id="9ad2e-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="9ad2e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ad2e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9ad2e-107">指定された[bookingbusiness](../resources/bookingbusiness.md)では、指定された[bookingAppointment](../resources/bookingappointment.md)をキャンセルし、関連する顧客とスタッフのメンバーにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ad2e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ad2e-108">Permissions</span></span>
<span data-ttu-id="9ad2e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad2e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ad2e-111">Permission type</span></span>      | <span data-ttu-id="9ad2e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ad2e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ad2e-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9ad2e-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9ad2e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad2e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-116">Not supported.</span></span>   |
|<span data-ttu-id="9ad2e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ad2e-117">Application</span></span> | <span data-ttu-id="9ad2e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="9ad2e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ad2e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="9ad2e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ad2e-120">Request headers</span></span>
| <span data-ttu-id="9ad2e-121">名前</span><span class="sxs-lookup"><span data-stu-id="9ad2e-121">Name</span></span>       | <span data-ttu-id="9ad2e-122">説明</span><span class="sxs-lookup"><span data-stu-id="9ad2e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ad2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ad2e-123">Authorization</span></span>  | <span data-ttu-id="9ad2e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9ad2e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ad2e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ad2e-125">Request body</span></span>
<span data-ttu-id="9ad2e-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ad2e-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9ad2e-127">Parameter</span></span>    | <span data-ttu-id="9ad2e-128">型</span><span class="sxs-lookup"><span data-stu-id="9ad2e-128">Type</span></span>   |<span data-ttu-id="9ad2e-129">説明</span><span class="sxs-lookup"><span data-stu-id="9ad2e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ad2e-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="9ad2e-130">cancellationMessage</span></span>|<span data-ttu-id="9ad2e-131">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-131">String</span></span>|<span data-ttu-id="9ad2e-132">予定が取り消されましたことをお客様と確認のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="9ad2e-133">応答</span><span class="sxs-lookup"><span data-stu-id="9ad2e-133">Response</span></span>
<span data-ttu-id="9ad2e-p104">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="9ad2e-136">Exisit ではありませんが、予定をキャンセルしようかどうか、このメソッドを返します`HTTP 404 Not found`。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="9ad2e-137">例</span><span class="sxs-lookup"><span data-stu-id="9ad2e-137">Example</span></span>
<span data-ttu-id="9ad2e-138">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ad2e-139">要求</span><span class="sxs-lookup"><span data-stu-id="9ad2e-139">Request</span></span>
<span data-ttu-id="9ad2e-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-140">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9ad2e-141">応答</span><span class="sxs-lookup"><span data-stu-id="9ad2e-141">Response</span></span>
<span data-ttu-id="9ad2e-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ad2e-142">The following is an example of the response.</span></span> 
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