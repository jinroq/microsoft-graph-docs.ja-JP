---
title: 教師を追加する
description: クラスに教師を追加します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 284c84cc140f0f9c15831396ed5adddaff73fdc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882987"
---
# <a name="add-teacher"></a><span data-ttu-id="51385-103">教師を追加する</span><span class="sxs-lookup"><span data-stu-id="51385-103">Add teacher</span></span>

> <span data-ttu-id="51385-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51385-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51385-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51385-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51385-106">クラスに教師を追加します。</span><span class="sxs-lookup"><span data-stu-id="51385-106">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="51385-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51385-107">Permissions</span></span>
<span data-ttu-id="51385-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51385-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51385-110">Permission type</span></span>      | <span data-ttu-id="51385-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51385-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51385-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51385-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="51385-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51385-113">Not supported.</span></span>  |
|<span data-ttu-id="51385-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51385-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="51385-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51385-115">Not supported.</span></span>  |
|<span data-ttu-id="51385-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51385-116">Application</span></span> | <span data-ttu-id="51385-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51385-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51385-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51385-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="51385-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51385-119">Request headers</span></span>
| <span data-ttu-id="51385-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51385-120">Header</span></span>       | <span data-ttu-id="51385-121">値</span><span class="sxs-lookup"><span data-stu-id="51385-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51385-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51385-122">Authorization</span></span>  | <span data-ttu-id="51385-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="51385-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51385-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51385-125">Content-Type</span></span>  | <span data-ttu-id="51385-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51385-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51385-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51385-127">Request body</span></span>
<span data-ttu-id="51385-128">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51385-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="51385-129">応答</span><span class="sxs-lookup"><span data-stu-id="51385-129">Response</span></span>
<span data-ttu-id="51385-130">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51385-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51385-131">例</span><span class="sxs-lookup"><span data-stu-id="51385-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51385-132">要求</span><span class="sxs-lookup"><span data-stu-id="51385-132">Request</span></span>
<span data-ttu-id="51385-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51385-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="51385-134">応答</span><span class="sxs-lookup"><span data-stu-id="51385-134">Response</span></span>
<span data-ttu-id="51385-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51385-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="51385-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="51385-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
