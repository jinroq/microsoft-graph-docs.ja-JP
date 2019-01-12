---
title: educationClass を削除する
description: 学校からクラスを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1ae6e96358f0ea6c85feb8cfec50a68ba1a7ee4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934976"
---
# <a name="remove-educationclass"></a><span data-ttu-id="95875-103">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="95875-103">Remove educationClass</span></span>

> <span data-ttu-id="95875-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95875-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95875-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95875-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95875-106">学校からクラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="95875-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="95875-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95875-107">Permissions</span></span>
<span data-ttu-id="95875-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95875-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95875-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95875-110">Permission type</span></span>      | <span data-ttu-id="95875-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95875-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95875-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95875-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="95875-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95875-113">Not supported.</span></span>  |
|<span data-ttu-id="95875-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95875-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="95875-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95875-115">Not supported.</span></span>  |
|<span data-ttu-id="95875-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95875-116">Application</span></span> | <span data-ttu-id="95875-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95875-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95875-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95875-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="95875-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95875-119">Request headers</span></span>
| <span data-ttu-id="95875-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95875-120">Header</span></span>       | <span data-ttu-id="95875-121">値</span><span class="sxs-lookup"><span data-stu-id="95875-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95875-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95875-122">Authorization</span></span>  | <span data-ttu-id="95875-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95875-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95875-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="95875-125">Request body</span></span>
<span data-ttu-id="95875-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95875-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="95875-127">応答</span><span class="sxs-lookup"><span data-stu-id="95875-127">Response</span></span>
<span data-ttu-id="95875-128">成功した場合、このメソッドは `204 No Content` 応答コードと応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="95875-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="95875-129">例</span><span class="sxs-lookup"><span data-stu-id="95875-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95875-130">要求</span><span class="sxs-lookup"><span data-stu-id="95875-130">Request</span></span>
<span data-ttu-id="95875-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95875-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="95875-132">応答</span><span class="sxs-lookup"><span data-stu-id="95875-132">Response</span></span>
<span data-ttu-id="95875-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95875-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
