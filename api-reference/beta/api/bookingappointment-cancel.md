---
title: 'bookingAppointment: キャンセル'
description: 指定した bookingappointment で指定された bookingAppointment を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d7be27f56ce9ab6aeed9feb539fbda1e297860d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945285"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="46545-103">bookingAppointment: キャンセル</span><span class="sxs-lookup"><span data-stu-id="46545-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46545-104">指定した[bookingappointment](../resources/bookingbusiness.md)で指定された[bookingappointment](../resources/bookingappointment.md)を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="46545-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="46545-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46545-105">Permissions</span></span>
<span data-ttu-id="46545-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46545-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46545-108">Permission type</span></span>      | <span data-ttu-id="46545-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46545-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46545-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46545-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="46545-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="46545-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="46545-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46545-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46545-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46545-113">Not supported.</span></span>   |
|<span data-ttu-id="46545-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46545-114">Application</span></span> | <span data-ttu-id="46545-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46545-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="46545-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46545-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="46545-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46545-117">Request headers</span></span>
| <span data-ttu-id="46545-118">名前</span><span class="sxs-lookup"><span data-stu-id="46545-118">Name</span></span>       | <span data-ttu-id="46545-119">説明</span><span class="sxs-lookup"><span data-stu-id="46545-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46545-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="46545-120">Authorization</span></span>  | <span data-ttu-id="46545-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="46545-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="46545-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="46545-122">Request body</span></span>
<span data-ttu-id="46545-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="46545-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46545-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="46545-124">Parameter</span></span>    | <span data-ttu-id="46545-125">型</span><span class="sxs-lookup"><span data-stu-id="46545-125">Type</span></span>   |<span data-ttu-id="46545-126">説明</span><span class="sxs-lookup"><span data-stu-id="46545-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46545-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="46545-127">cancellationMessage</span></span>|<span data-ttu-id="46545-128">String</span><span class="sxs-lookup"><span data-stu-id="46545-128">String</span></span>|<span data-ttu-id="46545-129">予定がキャンセルされたことをお客様に通知するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="46545-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="46545-130">応答</span><span class="sxs-lookup"><span data-stu-id="46545-130">Response</span></span>
<span data-ttu-id="46545-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="46545-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="46545-133">Exisit でない予定を取り消しようとすると、このメソッドはを`HTTP 404 Not found`返します。</span><span class="sxs-lookup"><span data-stu-id="46545-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="46545-134">例</span><span class="sxs-lookup"><span data-stu-id="46545-134">Example</span></span>
<span data-ttu-id="46545-135">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46545-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46545-136">要求</span><span class="sxs-lookup"><span data-stu-id="46545-136">Request</span></span>
<span data-ttu-id="46545-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46545-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46545-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="46545-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="46545-139">C#</span><span class="sxs-lookup"><span data-stu-id="46545-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46545-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="46545-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46545-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="46545-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46545-142">Java</span><span class="sxs-lookup"><span data-stu-id="46545-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46545-143">応答</span><span class="sxs-lookup"><span data-stu-id="46545-143">Response</span></span>
<span data-ttu-id="46545-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46545-144">The following is an example of the response.</span></span>
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
