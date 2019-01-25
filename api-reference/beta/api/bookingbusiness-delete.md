---
title: BookingBusiness を削除します。
description: BookingBusiness オブジェクトを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 88f07b46231a942098a157f00097393d60253982
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511899"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="5568c-103">BookingBusiness を削除します。</span><span class="sxs-lookup"><span data-stu-id="5568c-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5568c-104">[BookingBusiness](../resources/bookingbusiness.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="5568c-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5568c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5568c-105">Permissions</span></span>
<span data-ttu-id="5568c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5568c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5568c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5568c-108">Permission type</span></span>      | <span data-ttu-id="5568c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5568c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5568c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5568c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5568c-111">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5568c-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5568c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5568c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5568c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5568c-113">Not supported.</span></span>   |
|<span data-ttu-id="5568c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5568c-114">Application</span></span> | <span data-ttu-id="5568c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5568c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5568c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5568c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="5568c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5568c-117">Request headers</span></span>
| <span data-ttu-id="5568c-118">名前</span><span class="sxs-lookup"><span data-stu-id="5568c-118">Name</span></span>       | <span data-ttu-id="5568c-119">説明</span><span class="sxs-lookup"><span data-stu-id="5568c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5568c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5568c-120">Authorization</span></span>  | <span data-ttu-id="5568c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5568c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5568c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="5568c-122">Request body</span></span>
<span data-ttu-id="5568c-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5568c-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5568c-124">応答</span><span class="sxs-lookup"><span data-stu-id="5568c-124">Response</span></span>
<span data-ttu-id="5568c-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5568c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5568c-127">例</span><span class="sxs-lookup"><span data-stu-id="5568c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5568c-128">要求</span><span class="sxs-lookup"><span data-stu-id="5568c-128">Request</span></span>
<span data-ttu-id="5568c-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5568c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="5568c-130">応答</span><span class="sxs-lookup"><span data-stu-id="5568c-130">Response</span></span>
<span data-ttu-id="5568c-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5568c-131">The following is an example of the response.</span></span>
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
