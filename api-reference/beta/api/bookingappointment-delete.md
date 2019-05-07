---
title: BookingAppointment の削除
description: 指定した bookingappointment の書店の予定を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4a0dc3276128a9e0a6c3efda1ab3c96bbb3c5db8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636248"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="b9921-103">BookingAppointment の削除</span><span class="sxs-lookup"><span data-stu-id="b9921-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9921-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[書店の予定](../resources/bookingappointment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b9921-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b9921-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b9921-105">Permissions</span></span>
<span data-ttu-id="b9921-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9921-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9921-108">Permission type</span></span>      | <span data-ttu-id="b9921-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9921-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9921-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9921-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9921-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="b9921-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b9921-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9921-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9921-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9921-113">Not supported.</span></span>   |
|<span data-ttu-id="b9921-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9921-114">Application</span></span> | <span data-ttu-id="b9921-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9921-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b9921-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9921-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b9921-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9921-117">Request headers</span></span>
| <span data-ttu-id="b9921-118">名前</span><span class="sxs-lookup"><span data-stu-id="b9921-118">Name</span></span>       | <span data-ttu-id="b9921-119">説明</span><span class="sxs-lookup"><span data-stu-id="b9921-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9921-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9921-120">Authorization</span></span>  | <span data-ttu-id="b9921-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9921-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9921-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9921-122">Request body</span></span>
<span data-ttu-id="b9921-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9921-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b9921-124">応答</span><span class="sxs-lookup"><span data-stu-id="b9921-124">Response</span></span>
<span data-ttu-id="b9921-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b9921-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9921-127">例</span><span class="sxs-lookup"><span data-stu-id="b9921-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9921-128">要求</span><span class="sxs-lookup"><span data-stu-id="b9921-128">Request</span></span>
<span data-ttu-id="b9921-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9921-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="b9921-130">応答</span><span class="sxs-lookup"><span data-stu-id="b9921-130">Response</span></span>
<span data-ttu-id="b9921-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9921-131">The following is an example of the response.</span></span> <span data-ttu-id="b9921-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b9921-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b9921-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b9921-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b9921-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b9921-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9921-135">Visual</span><span class="sxs-lookup"><span data-stu-id="b9921-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9921-136">Java</span><span class="sxs-lookup"><span data-stu-id="b9921-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingappointment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
