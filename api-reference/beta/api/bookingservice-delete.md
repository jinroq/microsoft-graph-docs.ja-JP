---
title: BookingService を削除します。
description: 指定された bookingbusiness で、bookingService オブジェクトを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a541796fbfa500cc6d99205598042818b4aa47ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517037"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="5211e-103">BookingService を削除します。</span><span class="sxs-lookup"><span data-stu-id="5211e-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5211e-104">指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingService](../resources/bookingservice.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="5211e-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5211e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5211e-105">Permissions</span></span>
<span data-ttu-id="5211e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5211e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5211e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5211e-108">Permission type</span></span>      | <span data-ttu-id="5211e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5211e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5211e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5211e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5211e-111">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5211e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5211e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5211e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5211e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5211e-113">Not supported.</span></span>   |
|<span data-ttu-id="5211e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5211e-114">Application</span></span> | <span data-ttu-id="5211e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5211e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5211e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5211e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5211e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5211e-117">Request headers</span></span>
| <span data-ttu-id="5211e-118">名前</span><span class="sxs-lookup"><span data-stu-id="5211e-118">Name</span></span>       | <span data-ttu-id="5211e-119">説明</span><span class="sxs-lookup"><span data-stu-id="5211e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5211e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5211e-120">Authorization</span></span>  | <span data-ttu-id="5211e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5211e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5211e-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="5211e-122">Request body</span></span>
<span data-ttu-id="5211e-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5211e-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5211e-124">応答</span><span class="sxs-lookup"><span data-stu-id="5211e-124">Response</span></span>
<span data-ttu-id="5211e-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5211e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5211e-127">例</span><span class="sxs-lookup"><span data-stu-id="5211e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5211e-128">要求</span><span class="sxs-lookup"><span data-stu-id="5211e-128">Request</span></span>
<span data-ttu-id="5211e-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5211e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="5211e-130">応答</span><span class="sxs-lookup"><span data-stu-id="5211e-130">Response</span></span>
<span data-ttu-id="5211e-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5211e-131">The following is an example of the response.</span></span> <span data-ttu-id="5211e-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5211e-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5211e-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5211e-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
