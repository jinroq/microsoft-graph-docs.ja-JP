---
title: BookingAppointment の削除
description: 指定した bookingappointment の書店の予定を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0727ade214a493397202a15970c227ab1432721d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857287"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="4bc62-103">BookingAppointment の削除</span><span class="sxs-lookup"><span data-stu-id="4bc62-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bc62-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[書店の予定](../resources/bookingappointment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="4bc62-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4bc62-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4bc62-105">Permissions</span></span>
<span data-ttu-id="4bc62-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc62-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bc62-108">Permission type</span></span>      | <span data-ttu-id="4bc62-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bc62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bc62-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bc62-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4bc62-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="4bc62-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4bc62-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bc62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc62-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bc62-113">Not supported.</span></span>   |
|<span data-ttu-id="4bc62-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bc62-114">Application</span></span> | <span data-ttu-id="4bc62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bc62-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4bc62-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bc62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4bc62-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bc62-117">Request headers</span></span>
| <span data-ttu-id="4bc62-118">名前</span><span class="sxs-lookup"><span data-stu-id="4bc62-118">Name</span></span>       | <span data-ttu-id="4bc62-119">説明</span><span class="sxs-lookup"><span data-stu-id="4bc62-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bc62-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc62-120">Authorization</span></span>  | <span data-ttu-id="4bc62-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4bc62-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc62-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bc62-122">Request body</span></span>
<span data-ttu-id="4bc62-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4bc62-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4bc62-124">応答</span><span class="sxs-lookup"><span data-stu-id="4bc62-124">Response</span></span>
<span data-ttu-id="4bc62-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4bc62-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc62-127">例</span><span class="sxs-lookup"><span data-stu-id="4bc62-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bc62-128">要求</span><span class="sxs-lookup"><span data-stu-id="4bc62-128">Request</span></span>
<span data-ttu-id="4bc62-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bc62-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4bc62-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4bc62-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4bc62-131">C#</span><span class="sxs-lookup"><span data-stu-id="4bc62-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4bc62-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="4bc62-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4bc62-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="4bc62-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4bc62-134">Java</span><span class="sxs-lookup"><span data-stu-id="4bc62-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4bc62-135">応答</span><span class="sxs-lookup"><span data-stu-id="4bc62-135">Response</span></span>
<span data-ttu-id="4bc62-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bc62-136">The following is an example of the response.</span></span> <span data-ttu-id="4bc62-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4bc62-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4bc62-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4bc62-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
