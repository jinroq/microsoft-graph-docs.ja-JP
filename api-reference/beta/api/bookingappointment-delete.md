---
title: bookingappointment の削除
description: 指定した bookingappointment の書店の予定を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a8abe1961be7e3caf36c9d690497347f42c83fde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461116"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="c830c-103">bookingappointment の削除</span><span class="sxs-lookup"><span data-stu-id="c830c-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c830c-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[書店の予定](../resources/bookingappointment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c830c-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c830c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c830c-105">Permissions</span></span>
<span data-ttu-id="c830c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c830c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c830c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c830c-108">Permission type</span></span>      | <span data-ttu-id="c830c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c830c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c830c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c830c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c830c-111">bookingsappointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="c830c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c830c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c830c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c830c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c830c-113">Not supported.</span></span>   |
|<span data-ttu-id="c830c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c830c-114">Application</span></span> | <span data-ttu-id="c830c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c830c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c830c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c830c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c830c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c830c-117">Request headers</span></span>
| <span data-ttu-id="c830c-118">名前</span><span class="sxs-lookup"><span data-stu-id="c830c-118">Name</span></span>       | <span data-ttu-id="c830c-119">説明</span><span class="sxs-lookup"><span data-stu-id="c830c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c830c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c830c-120">Authorization</span></span>  | <span data-ttu-id="c830c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c830c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c830c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c830c-122">Request body</span></span>
<span data-ttu-id="c830c-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c830c-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c830c-124">応答</span><span class="sxs-lookup"><span data-stu-id="c830c-124">Response</span></span>
<span data-ttu-id="c830c-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c830c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c830c-127">例</span><span class="sxs-lookup"><span data-stu-id="c830c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c830c-128">要求</span><span class="sxs-lookup"><span data-stu-id="c830c-128">Request</span></span>
<span data-ttu-id="c830c-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c830c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="c830c-130">応答</span><span class="sxs-lookup"><span data-stu-id="c830c-130">Response</span></span>
<span data-ttu-id="c830c-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c830c-131">The following is an example of the response.</span></span> <span data-ttu-id="c830c-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c830c-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c830c-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c830c-133">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
