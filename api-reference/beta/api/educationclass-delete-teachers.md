---
title: 教師を削除する
description: クラスから教師を削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39a9df74ea6f816b179844f6c26218a0caa17210
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965118"
---
# <a name="remove-teacher"></a><span data-ttu-id="89938-103">教師を削除する</span><span class="sxs-lookup"><span data-stu-id="89938-103">Remove teacher</span></span>

> <span data-ttu-id="89938-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89938-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89938-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89938-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89938-106">クラスから教師を削除します。</span><span class="sxs-lookup"><span data-stu-id="89938-106">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="89938-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89938-107">Permissions</span></span>
<span data-ttu-id="89938-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89938-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89938-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89938-110">Permission type</span></span>      | <span data-ttu-id="89938-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89938-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89938-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89938-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="89938-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89938-113">Not supported.</span></span>  |
|<span data-ttu-id="89938-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89938-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="89938-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89938-115">Not supported.</span></span>  |
|<span data-ttu-id="89938-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89938-116">Application</span></span> | <span data-ttu-id="89938-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89938-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="89938-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89938-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="89938-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89938-119">Request headers</span></span>
| <span data-ttu-id="89938-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89938-120">Header</span></span>       | <span data-ttu-id="89938-121">値</span><span class="sxs-lookup"><span data-stu-id="89938-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89938-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89938-122">Authorization</span></span>  | <span data-ttu-id="89938-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="89938-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89938-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="89938-125">Request body</span></span>
<span data-ttu-id="89938-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89938-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="89938-127">応答</span><span class="sxs-lookup"><span data-stu-id="89938-127">Response</span></span>
<span data-ttu-id="89938-128">成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="89938-128">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="89938-129">例</span><span class="sxs-lookup"><span data-stu-id="89938-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89938-130">要求</span><span class="sxs-lookup"><span data-stu-id="89938-130">Request</span></span>
<span data-ttu-id="89938-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89938-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/<id>/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="89938-132">応答</span><span class="sxs-lookup"><span data-stu-id="89938-132">Response</span></span>
<span data-ttu-id="89938-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89938-133">The following is an example of the response.</span></span> 
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
