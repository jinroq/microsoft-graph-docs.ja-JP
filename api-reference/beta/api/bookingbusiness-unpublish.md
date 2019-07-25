---
title: 'bookingBusiness: 未発行'
description: 外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: df4f9fb74ab0cc82394a90b938f1b7478c99cd07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865519"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="7d463-103">bookingBusiness: 未発行</span><span class="sxs-lookup"><span data-stu-id="7d463-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d463-104">外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。</span><span class="sxs-lookup"><span data-stu-id="7d463-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="7d463-105">**IsPublished**プロパティを false に設定し、 **publicurl**プロパティを null に設定します。</span><span class="sxs-lookup"><span data-stu-id="7d463-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d463-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d463-106">Permissions</span></span>
<span data-ttu-id="7d463-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d463-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d463-109">Permission type</span></span>      | <span data-ttu-id="7d463-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d463-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d463-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d463-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="7d463-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="7d463-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7d463-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d463-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d463-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d463-114">Not supported.</span></span>   |
|<span data-ttu-id="7d463-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d463-115">Application</span></span> | <span data-ttu-id="7d463-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d463-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7d463-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d463-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="7d463-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d463-118">Request headers</span></span>
| <span data-ttu-id="7d463-119">名前</span><span class="sxs-lookup"><span data-stu-id="7d463-119">Name</span></span>       | <span data-ttu-id="7d463-120">説明</span><span class="sxs-lookup"><span data-stu-id="7d463-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d463-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d463-121">Authorization</span></span>  | <span data-ttu-id="7d463-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7d463-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d463-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d463-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7d463-124">応答</span><span class="sxs-lookup"><span data-stu-id="7d463-124">Response</span></span>
<span data-ttu-id="7d463-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7d463-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d463-127">例</span><span class="sxs-lookup"><span data-stu-id="7d463-127">Example</span></span>
<span data-ttu-id="7d463-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7d463-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d463-129">要求</span><span class="sxs-lookup"><span data-stu-id="7d463-129">Request</span></span>
<span data-ttu-id="7d463-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7d463-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7d463-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7d463-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d463-132">C#</span><span class="sxs-lookup"><span data-stu-id="7d463-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d463-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d463-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d463-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="7d463-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7d463-135">Java</span><span class="sxs-lookup"><span data-stu-id="7d463-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d463-136">応答</span><span class="sxs-lookup"><span data-stu-id="7d463-136">Response</span></span>
<span data-ttu-id="7d463-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7d463-137">The following is an example of the response.</span></span>
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
  "suppressions": [
  ]
}
-->
