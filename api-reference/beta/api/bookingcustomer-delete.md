---
title: bookingcustomer の削除
description: 指定した bookingcustomer オブジェクトを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 5ff8d9f276164b9b6c1c5b582668123c3dd4eb02
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322380"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="1197f-103">bookingcustomer の削除</span><span class="sxs-lookup"><span data-stu-id="1197f-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1197f-104">指定した[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1197f-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1197f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1197f-105">Permissions</span></span>
<span data-ttu-id="1197f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1197f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1197f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1197f-108">Permission type</span></span>      | <span data-ttu-id="1197f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1197f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1197f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1197f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1197f-111">bookingsappointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="1197f-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1197f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1197f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1197f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1197f-113">Not supported.</span></span>   |
|<span data-ttu-id="1197f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1197f-114">Application</span></span> | <span data-ttu-id="1197f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1197f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1197f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1197f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1197f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1197f-117">Request headers</span></span>
| <span data-ttu-id="1197f-118">名前</span><span class="sxs-lookup"><span data-stu-id="1197f-118">Name</span></span>       | <span data-ttu-id="1197f-119">説明</span><span class="sxs-lookup"><span data-stu-id="1197f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1197f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1197f-120">Authorization</span></span>  | <span data-ttu-id="1197f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1197f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1197f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="1197f-122">Request body</span></span>
<span data-ttu-id="1197f-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1197f-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1197f-124">応答</span><span class="sxs-lookup"><span data-stu-id="1197f-124">Response</span></span>
<span data-ttu-id="1197f-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1197f-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1197f-127">例</span><span class="sxs-lookup"><span data-stu-id="1197f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1197f-128">要求</span><span class="sxs-lookup"><span data-stu-id="1197f-128">Request</span></span>
<span data-ttu-id="1197f-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1197f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="1197f-130">応答</span><span class="sxs-lookup"><span data-stu-id="1197f-130">Response</span></span>
<span data-ttu-id="1197f-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1197f-131">The following is an example of the response.</span></span> <span data-ttu-id="1197f-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1197f-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1197f-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1197f-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
