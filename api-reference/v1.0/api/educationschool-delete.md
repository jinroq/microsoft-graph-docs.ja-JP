---
title: educationSchool を削除する
description: 学校を削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bb865ef12d0ad8eb0f18b5f9c7c9631346921e17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923846"
---
# <a name="delete-educationschool"></a><span data-ttu-id="3374f-103">educationSchool を削除する</span><span class="sxs-lookup"><span data-stu-id="3374f-103">Delete educationSchool</span></span>

<span data-ttu-id="3374f-104">学校を削除します。</span><span class="sxs-lookup"><span data-stu-id="3374f-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="3374f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3374f-105">Permissions</span></span>
<span data-ttu-id="3374f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3374f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3374f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3374f-108">Permission type</span></span>      | <span data-ttu-id="3374f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3374f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3374f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3374f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3374f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3374f-111">Not supported.</span></span>  |
|<span data-ttu-id="3374f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3374f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3374f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3374f-113">Not supported.</span></span>  |
|<span data-ttu-id="3374f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3374f-114">Application</span></span> | <span data-ttu-id="3374f-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3374f-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3374f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3374f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3374f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3374f-117">Request headers</span></span>
| <span data-ttu-id="3374f-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3374f-118">Header</span></span>       | <span data-ttu-id="3374f-119">値</span><span class="sxs-lookup"><span data-stu-id="3374f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3374f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3374f-120">Authorization</span></span>  | <span data-ttu-id="3374f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3374f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3374f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3374f-123">Request body</span></span>
<span data-ttu-id="3374f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3374f-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3374f-125">応答</span><span class="sxs-lookup"><span data-stu-id="3374f-125">Response</span></span>
<span data-ttu-id="3374f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3374f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3374f-128">例</span><span class="sxs-lookup"><span data-stu-id="3374f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3374f-129">要求</span><span class="sxs-lookup"><span data-stu-id="3374f-129">Request</span></span>
<span data-ttu-id="3374f-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3374f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="3374f-131">応答</span><span class="sxs-lookup"><span data-stu-id="3374f-131">Response</span></span>
<span data-ttu-id="3374f-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3374f-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
