---
title: 'bookingBusiness: 未発行'
description: 外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dc0d94094273579321a614c9ff2192f331550421
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636192"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="1ef17-103">bookingBusiness: 未発行</span><span class="sxs-lookup"><span data-stu-id="1ef17-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef17-104">外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。</span><span class="sxs-lookup"><span data-stu-id="1ef17-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="1ef17-105">**IsPublished**プロパティを False に設定し、 **publicurl**プロパティを null に設定します。</span><span class="sxs-lookup"><span data-stu-id="1ef17-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef17-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ef17-106">Permissions</span></span>
<span data-ttu-id="1ef17-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ef17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef17-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ef17-109">Permission type</span></span>      | <span data-ttu-id="1ef17-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ef17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ef17-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef17-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ef17-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="1ef17-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1ef17-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef17-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef17-114">Not supported.</span></span>   |
|<span data-ttu-id="1ef17-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ef17-115">Application</span></span> | <span data-ttu-id="1ef17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef17-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1ef17-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ef17-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="1ef17-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ef17-118">Request headers</span></span>
| <span data-ttu-id="1ef17-119">名前</span><span class="sxs-lookup"><span data-stu-id="1ef17-119">Name</span></span>       | <span data-ttu-id="1ef17-120">説明</span><span class="sxs-lookup"><span data-stu-id="1ef17-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ef17-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef17-121">Authorization</span></span>  | <span data-ttu-id="1ef17-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ef17-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef17-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ef17-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1ef17-124">応答</span><span class="sxs-lookup"><span data-stu-id="1ef17-124">Response</span></span>
<span data-ttu-id="1ef17-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1ef17-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef17-127">例</span><span class="sxs-lookup"><span data-stu-id="1ef17-127">Example</span></span>
<span data-ttu-id="1ef17-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ef17-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1ef17-129">要求</span><span class="sxs-lookup"><span data-stu-id="1ef17-129">Request</span></span>
<span data-ttu-id="1ef17-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ef17-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="1ef17-131">応答</span><span class="sxs-lookup"><span data-stu-id="1ef17-131">Response</span></span>
<span data-ttu-id="1ef17-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ef17-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ef17-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1ef17-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ef17-134">Visual</span><span class="sxs-lookup"><span data-stu-id="1ef17-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ef17-135">Java</span><span class="sxs-lookup"><span data-stu-id="1ef17-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
