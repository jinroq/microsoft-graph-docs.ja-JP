---
title: educationSchool を削除する
description: 学校を削除します。
author: mmast-msft
ms.openlocfilehash: e104265f718ad69a84b9e2362962d72763e8fc54
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323066"
---
# <a name="delete-educationschool"></a><span data-ttu-id="15051-103">educationSchool を削除する</span><span class="sxs-lookup"><span data-stu-id="15051-103">Delete educationSchool</span></span>

> <span data-ttu-id="15051-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15051-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15051-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15051-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15051-106">学校を削除します。</span><span class="sxs-lookup"><span data-stu-id="15051-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="15051-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15051-107">Permissions</span></span>
<span data-ttu-id="15051-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15051-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15051-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15051-110">Permission type</span></span>      | <span data-ttu-id="15051-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15051-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15051-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15051-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="15051-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15051-113">Not supported.</span></span>  |
|<span data-ttu-id="15051-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15051-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="15051-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15051-115">Not supported.</span></span>  |
|<span data-ttu-id="15051-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15051-116">Application</span></span> | <span data-ttu-id="15051-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15051-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="15051-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15051-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="15051-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15051-119">Request headers</span></span>
| <span data-ttu-id="15051-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15051-120">Header</span></span>       | <span data-ttu-id="15051-121">値</span><span class="sxs-lookup"><span data-stu-id="15051-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15051-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15051-122">Authorization</span></span>  | <span data-ttu-id="15051-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15051-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15051-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="15051-125">Request body</span></span>
<span data-ttu-id="15051-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15051-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="15051-127">応答</span><span class="sxs-lookup"><span data-stu-id="15051-127">Response</span></span>
<span data-ttu-id="15051-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="15051-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15051-130">例</span><span class="sxs-lookup"><span data-stu-id="15051-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15051-131">要求</span><span class="sxs-lookup"><span data-stu-id="15051-131">Request</span></span>
<span data-ttu-id="15051-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15051-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="15051-133">応答</span><span class="sxs-lookup"><span data-stu-id="15051-133">Response</span></span>
<span data-ttu-id="15051-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15051-134">The following is an example of the response.</span></span> 

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