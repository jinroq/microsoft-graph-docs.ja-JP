---
title: educationSchool を削除する
description: 学校を削除します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 50d9d39da05fc85447b7a7e8ab47a14093b292b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861846"
---
# <a name="delete-educationschool"></a><span data-ttu-id="883e3-103">educationSchool を削除する</span><span class="sxs-lookup"><span data-stu-id="883e3-103">Delete educationSchool</span></span>

<span data-ttu-id="883e3-104">学校を削除します。</span><span class="sxs-lookup"><span data-stu-id="883e3-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="883e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="883e3-105">Permissions</span></span>
<span data-ttu-id="883e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="883e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="883e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="883e3-108">Permission type</span></span>      | <span data-ttu-id="883e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="883e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="883e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="883e3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="883e3-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883e3-111">Not supported.</span></span>  |
|<span data-ttu-id="883e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="883e3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="883e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883e3-113">Not supported.</span></span>  |
|<span data-ttu-id="883e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="883e3-114">Application</span></span> | <span data-ttu-id="883e3-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="883e3-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="883e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="883e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="883e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="883e3-117">Request headers</span></span>
| <span data-ttu-id="883e3-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="883e3-118">Header</span></span>       | <span data-ttu-id="883e3-119">値</span><span class="sxs-lookup"><span data-stu-id="883e3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="883e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="883e3-120">Authorization</span></span>  | <span data-ttu-id="883e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="883e3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="883e3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="883e3-123">Request body</span></span>
<span data-ttu-id="883e3-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="883e3-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="883e3-125">応答</span><span class="sxs-lookup"><span data-stu-id="883e3-125">Response</span></span>
<span data-ttu-id="883e3-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="883e3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="883e3-128">例</span><span class="sxs-lookup"><span data-stu-id="883e3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="883e3-129">要求</span><span class="sxs-lookup"><span data-stu-id="883e3-129">Request</span></span>
<span data-ttu-id="883e3-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="883e3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="883e3-131">応答</span><span class="sxs-lookup"><span data-stu-id="883e3-131">Response</span></span>
<span data-ttu-id="883e3-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="883e3-132">The following is an example of the response.</span></span> 

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
