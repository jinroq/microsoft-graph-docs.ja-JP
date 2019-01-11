---
title: educationClass を削除する
description: 学校からクラスを削除します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 69e5bab04ac9c9c4d595eb40f76d379082806717
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815436"
---
# <a name="remove-educationclass"></a><span data-ttu-id="7ef09-103">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="7ef09-103">Remove educationClass</span></span>

<span data-ttu-id="7ef09-104">学校からクラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="7ef09-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef09-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ef09-105">Permissions</span></span>
<span data-ttu-id="7ef09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ef09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef09-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ef09-108">Permission type</span></span>      | <span data-ttu-id="7ef09-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ef09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ef09-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ef09-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7ef09-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ef09-111">Not supported.</span></span>  |
|<span data-ttu-id="7ef09-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ef09-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7ef09-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ef09-113">Not supported.</span></span>  |
|<span data-ttu-id="7ef09-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ef09-114">Application</span></span> | <span data-ttu-id="7ef09-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef09-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7ef09-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ef09-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7ef09-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ef09-117">Request headers</span></span>
| <span data-ttu-id="7ef09-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ef09-118">Header</span></span>       | <span data-ttu-id="7ef09-119">値</span><span class="sxs-lookup"><span data-stu-id="7ef09-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ef09-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ef09-120">Authorization</span></span>  | <span data-ttu-id="7ef09-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7ef09-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ef09-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ef09-123">Request body</span></span>
<span data-ttu-id="7ef09-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ef09-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7ef09-125">応答</span><span class="sxs-lookup"><span data-stu-id="7ef09-125">Response</span></span>
<span data-ttu-id="7ef09-126">成功した場合、このメソッドは `204 No Content` 応答コードと応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="7ef09-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ef09-127">例</span><span class="sxs-lookup"><span data-stu-id="7ef09-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ef09-128">要求</span><span class="sxs-lookup"><span data-stu-id="7ef09-128">Request</span></span>
<span data-ttu-id="7ef09-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ef09-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="7ef09-130">応答</span><span class="sxs-lookup"><span data-stu-id="7ef09-130">Response</span></span>
<span data-ttu-id="7ef09-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ef09-131">The following is an example of the response.</span></span> 

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
