---
title: 'bookingAppointment: キャンセル'
description: 指定した bookingappointment で指定された bookingAppointment を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f4ea71b02e798b47c3f133078a352402f9f52267
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415688"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="91d6a-103">bookingAppointment: キャンセル</span><span class="sxs-lookup"><span data-stu-id="91d6a-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d6a-104">指定した[bookingappointment](../resources/bookingbusiness.md)で指定された[bookingappointment](../resources/bookingappointment.md)を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="91d6a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91d6a-105">Permissions</span></span>
<span data-ttu-id="91d6a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91d6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d6a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91d6a-108">Permission type</span></span>      | <span data-ttu-id="91d6a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91d6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d6a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91d6a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="91d6a-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="91d6a-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="91d6a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91d6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d6a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d6a-113">Not supported.</span></span>   |
|<span data-ttu-id="91d6a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91d6a-114">Application</span></span> | <span data-ttu-id="91d6a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d6a-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="91d6a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91d6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="91d6a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91d6a-117">Request headers</span></span>
| <span data-ttu-id="91d6a-118">名前</span><span class="sxs-lookup"><span data-stu-id="91d6a-118">Name</span></span>       | <span data-ttu-id="91d6a-119">説明</span><span class="sxs-lookup"><span data-stu-id="91d6a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91d6a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d6a-120">Authorization</span></span>  | <span data-ttu-id="91d6a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="91d6a-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="91d6a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="91d6a-122">Request body</span></span>
<span data-ttu-id="91d6a-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91d6a-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="91d6a-124">Parameter</span></span>    | <span data-ttu-id="91d6a-125">型</span><span class="sxs-lookup"><span data-stu-id="91d6a-125">Type</span></span>   |<span data-ttu-id="91d6a-126">説明</span><span class="sxs-lookup"><span data-stu-id="91d6a-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d6a-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="91d6a-127">cancellationMessage</span></span>|<span data-ttu-id="91d6a-128">String</span><span class="sxs-lookup"><span data-stu-id="91d6a-128">String</span></span>|<span data-ttu-id="91d6a-129">予定がキャンセルされたことをお客様に通知するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="91d6a-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="91d6a-130">応答</span><span class="sxs-lookup"><span data-stu-id="91d6a-130">Response</span></span>
<span data-ttu-id="91d6a-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="91d6a-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="91d6a-133">Exisit でない予定を取り消しようとすると、このメソッドはを`HTTP 404 Not found`返します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="91d6a-134">例</span><span class="sxs-lookup"><span data-stu-id="91d6a-134">Example</span></span>
<span data-ttu-id="91d6a-135">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91d6a-136">要求</span><span class="sxs-lookup"><span data-stu-id="91d6a-136">Request</span></span>
<span data-ttu-id="91d6a-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91d6a-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="91d6a-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="91d6a-139">C#</span><span class="sxs-lookup"><span data-stu-id="91d6a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91d6a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91d6a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91d6a-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="91d6a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91d6a-142">応答</span><span class="sxs-lookup"><span data-stu-id="91d6a-142">Response</span></span>
<span data-ttu-id="91d6a-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d6a-143">The following is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
