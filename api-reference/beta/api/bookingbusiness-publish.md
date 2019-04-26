---
title: 'bookingbusiness: 発行'
description: この業務の [スケジュール] ページを外部のお客様が利用できるようにします。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d6fae2c6d39f3abe2b460fe71863c7b570fa340b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322545"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="e38ce-103">bookingbusiness: 発行</span><span class="sxs-lookup"><span data-stu-id="e38ce-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e38ce-104">この業務の [スケジュール] ページを外部のお客様が利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="e38ce-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="e38ce-105">**isPublished**プロパティを true に、 **publicurl**プロパティを [スケジュール] ページの URL に設定します。</span><span class="sxs-lookup"><span data-stu-id="e38ce-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="e38ce-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e38ce-106">Permissions</span></span>
<span data-ttu-id="e38ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e38ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e38ce-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e38ce-109">Permission type</span></span>      | <span data-ttu-id="e38ce-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e38ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e38ce-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e38ce-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e38ce-112">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="e38ce-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e38ce-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e38ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e38ce-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38ce-114">Not supported.</span></span>   |
|<span data-ttu-id="e38ce-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e38ce-115">Application</span></span> | <span data-ttu-id="e38ce-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38ce-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e38ce-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e38ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="e38ce-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38ce-118">Request headers</span></span>
| <span data-ttu-id="e38ce-119">名前</span><span class="sxs-lookup"><span data-stu-id="e38ce-119">Name</span></span>       | <span data-ttu-id="e38ce-120">説明</span><span class="sxs-lookup"><span data-stu-id="e38ce-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e38ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e38ce-121">Authorization</span></span>  | <span data-ttu-id="e38ce-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e38ce-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e38ce-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e38ce-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e38ce-124">応答</span><span class="sxs-lookup"><span data-stu-id="e38ce-124">Response</span></span>
<span data-ttu-id="e38ce-p102">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e38ce-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e38ce-127">例</span><span class="sxs-lookup"><span data-stu-id="e38ce-127">Example</span></span>
<span data-ttu-id="e38ce-128">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e38ce-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e38ce-129">要求</span><span class="sxs-lookup"><span data-stu-id="e38ce-129">Request</span></span>
<span data-ttu-id="e38ce-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e38ce-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="e38ce-131">応答</span><span class="sxs-lookup"><span data-stu-id="e38ce-131">Response</span></span>
<span data-ttu-id="e38ce-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e38ce-132">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
