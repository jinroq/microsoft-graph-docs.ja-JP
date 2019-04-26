---
title: 'bookingbusiness: 未発行'
description: 外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11ef80e416c1c8ffb85170c6e3171fc003bf937b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322575"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="cff71-103">bookingbusiness: 未発行</span><span class="sxs-lookup"><span data-stu-id="cff71-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff71-104">外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。</span><span class="sxs-lookup"><span data-stu-id="cff71-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="cff71-105">**isPublished**プロパティを false に設定し、 **publicurl**プロパティを null に設定します。</span><span class="sxs-lookup"><span data-stu-id="cff71-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="cff71-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cff71-106">Permissions</span></span>
<span data-ttu-id="cff71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cff71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff71-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cff71-109">Permission type</span></span>      | <span data-ttu-id="cff71-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cff71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cff71-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cff71-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="cff71-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="cff71-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cff71-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cff71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cff71-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cff71-114">Not supported.</span></span>   |
|<span data-ttu-id="cff71-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cff71-115">Application</span></span> | <span data-ttu-id="cff71-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cff71-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cff71-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cff71-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="cff71-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cff71-118">Request headers</span></span>
| <span data-ttu-id="cff71-119">名前</span><span class="sxs-lookup"><span data-stu-id="cff71-119">Name</span></span>       | <span data-ttu-id="cff71-120">説明</span><span class="sxs-lookup"><span data-stu-id="cff71-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cff71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff71-121">Authorization</span></span>  | <span data-ttu-id="cff71-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cff71-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff71-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cff71-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cff71-124">応答</span><span class="sxs-lookup"><span data-stu-id="cff71-124">Response</span></span>
<span data-ttu-id="cff71-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cff71-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff71-127">例</span><span class="sxs-lookup"><span data-stu-id="cff71-127">Example</span></span>
<span data-ttu-id="cff71-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cff71-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cff71-129">要求</span><span class="sxs-lookup"><span data-stu-id="cff71-129">Request</span></span>
<span data-ttu-id="cff71-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cff71-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="cff71-131">応答</span><span class="sxs-lookup"><span data-stu-id="cff71-131">Response</span></span>
<span data-ttu-id="cff71-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cff71-132">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
