---
title: educationClass を educationSchool に追加する
description: 学校にクラスを追加します。
author: mmast-msft
ms.openlocfilehash: 2ac40545dadb083751192ae516fb131d43cccb64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308849"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="ed9b7-103">educationClass を educationSchool に追加する</span><span class="sxs-lookup"><span data-stu-id="ed9b7-103">Add educationClass to educationSchool</span></span>

> <span data-ttu-id="ed9b7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed9b7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed9b7-106">学校にクラスを追加します。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-106">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed9b7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed9b7-107">Permissions</span></span>
<span data-ttu-id="ed9b7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed9b7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed9b7-110">Permission type</span></span>      | <span data-ttu-id="ed9b7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed9b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed9b7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9b7-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed9b7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-113">Not supported.</span></span>  |
|<span data-ttu-id="ed9b7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9b7-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ed9b7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-115">Not supported.</span></span>  |
|<span data-ttu-id="ed9b7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed9b7-116">Application</span></span> | <span data-ttu-id="ed9b7-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed9b7-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ed9b7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed9b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ed9b7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed9b7-119">Request headers</span></span>
| <span data-ttu-id="ed9b7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed9b7-120">Header</span></span>       | <span data-ttu-id="ed9b7-121">値</span><span class="sxs-lookup"><span data-stu-id="ed9b7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed9b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed9b7-122">Authorization</span></span>  | <span data-ttu-id="ed9b7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed9b7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed9b7-125">Content-Type</span></span>  | <span data-ttu-id="ed9b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed9b7-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed9b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed9b7-127">Request body</span></span>
<span data-ttu-id="ed9b7-128">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-128">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ed9b7-129">応答</span><span class="sxs-lookup"><span data-stu-id="ed9b7-129">Response</span></span>
<span data-ttu-id="ed9b7-130">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed9b7-131">例</span><span class="sxs-lookup"><span data-stu-id="ed9b7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed9b7-132">要求</span><span class="sxs-lookup"><span data-stu-id="ed9b7-132">Request</span></span>
<span data-ttu-id="ed9b7-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="ed9b7-134">応答</span><span class="sxs-lookup"><span data-stu-id="ed9b7-134">Response</span></span> 
<span data-ttu-id="ed9b7-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ed9b7-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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