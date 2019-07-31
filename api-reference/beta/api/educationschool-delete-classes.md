---
title: educationClass を削除する
description: 学校からクラスを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15ab30facb9c8d762e05c37ea8230b3178ab86f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955223"
---
# <a name="remove-educationclass"></a><span data-ttu-id="b7b43-103">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="b7b43-103">Remove educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b43-104">学校からクラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="b7b43-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7b43-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7b43-105">Permissions</span></span>
<span data-ttu-id="b7b43-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7b43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b43-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7b43-108">Permission type</span></span>      | <span data-ttu-id="b7b43-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7b43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b43-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7b43-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b7b43-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b43-111">Not supported.</span></span>  |
|<span data-ttu-id="b7b43-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7b43-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b7b43-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b43-113">Not supported.</span></span>  |
|<span data-ttu-id="b7b43-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7b43-114">Application</span></span> | <span data-ttu-id="b7b43-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b43-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b7b43-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7b43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b7b43-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7b43-117">Request headers</span></span>
| <span data-ttu-id="b7b43-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7b43-118">Header</span></span>       | <span data-ttu-id="b7b43-119">値</span><span class="sxs-lookup"><span data-stu-id="b7b43-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7b43-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b43-120">Authorization</span></span>  | <span data-ttu-id="b7b43-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7b43-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7b43-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7b43-123">Request body</span></span>
<span data-ttu-id="b7b43-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b7b43-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b7b43-125">応答</span><span class="sxs-lookup"><span data-stu-id="b7b43-125">Response</span></span>
<span data-ttu-id="b7b43-126">成功した場合、このメソッドは `204 No Content` 応答コードと応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="b7b43-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b43-127">例</span><span class="sxs-lookup"><span data-stu-id="b7b43-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7b43-128">要求</span><span class="sxs-lookup"><span data-stu-id="b7b43-128">Request</span></span>
<span data-ttu-id="b7b43-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7b43-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="b7b43-130">応答</span><span class="sxs-lookup"><span data-stu-id="b7b43-130">Response</span></span>
<span data-ttu-id="b7b43-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7b43-131">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
