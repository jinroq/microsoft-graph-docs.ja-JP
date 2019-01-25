---
title: 'bookingBusiness: 発行'
description: このビジネスのスケジュール ページを外部の顧客が使用できるようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11d8bea864772c0bcc4365c056973fac782add5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508658"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="50b78-103">bookingBusiness: 発行</span><span class="sxs-lookup"><span data-stu-id="50b78-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50b78-104">このビジネスのスケジュール ページを外部の顧客が使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="50b78-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="50b78-105">True の場合、およびスケジュールのページの URL を**publicUrl**プロパティに**isPublished**プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="50b78-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="50b78-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50b78-106">Permissions</span></span>
<span data-ttu-id="50b78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b78-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50b78-109">Permission type</span></span>      | <span data-ttu-id="50b78-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50b78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50b78-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50b78-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="50b78-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="50b78-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="50b78-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50b78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50b78-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50b78-114">Not supported.</span></span>   |
|<span data-ttu-id="50b78-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50b78-115">Application</span></span> | <span data-ttu-id="50b78-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50b78-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="50b78-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50b78-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="50b78-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50b78-118">Request headers</span></span>
| <span data-ttu-id="50b78-119">名前</span><span class="sxs-lookup"><span data-stu-id="50b78-119">Name</span></span>       | <span data-ttu-id="50b78-120">説明</span><span class="sxs-lookup"><span data-stu-id="50b78-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50b78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b78-121">Authorization</span></span>  | <span data-ttu-id="50b78-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="50b78-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b78-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="50b78-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="50b78-124">応答</span><span class="sxs-lookup"><span data-stu-id="50b78-124">Response</span></span>
<span data-ttu-id="50b78-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="50b78-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b78-127">例</span><span class="sxs-lookup"><span data-stu-id="50b78-127">Example</span></span>
<span data-ttu-id="50b78-128">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="50b78-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50b78-129">要求</span><span class="sxs-lookup"><span data-stu-id="50b78-129">Request</span></span>
<span data-ttu-id="50b78-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50b78-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="50b78-131">応答</span><span class="sxs-lookup"><span data-stu-id="50b78-131">Response</span></span>
<span data-ttu-id="50b78-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50b78-132">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
