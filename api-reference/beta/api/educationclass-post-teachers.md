---
title: 教師を追加する
description: クラスに教師を追加します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 959b873dba3f88665b170f52da4e4063adb200ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457729"
---
# <a name="add-teacher"></a><span data-ttu-id="f1b5b-103">教師を追加する</span><span class="sxs-lookup"><span data-stu-id="f1b5b-103">Add teacher</span></span>

<span data-ttu-id="f1b5b-104">クラスに教師を追加します。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1b5b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1b5b-105">Permissions</span></span>
<span data-ttu-id="f1b5b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b5b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1b5b-108">Permission type</span></span>      | <span data-ttu-id="f1b5b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1b5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1b5b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1b5b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1b5b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-111">Not supported.</span></span>  |
|<span data-ttu-id="f1b5b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1b5b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1b5b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-113">Not supported.</span></span>  |
|<span data-ttu-id="f1b5b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1b5b-114">Application</span></span> | <span data-ttu-id="f1b5b-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b5b-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f1b5b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1b5b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f1b5b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1b5b-117">Request headers</span></span>
| <span data-ttu-id="f1b5b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1b5b-118">Header</span></span>       | <span data-ttu-id="f1b5b-119">値</span><span class="sxs-lookup"><span data-stu-id="f1b5b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1b5b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b5b-120">Authorization</span></span>  | <span data-ttu-id="f1b5b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1b5b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1b5b-123">Content-Type</span></span>  | <span data-ttu-id="f1b5b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b5b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1b5b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1b5b-125">Request body</span></span>
<span data-ttu-id="f1b5b-126">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f1b5b-127">応答</span><span class="sxs-lookup"><span data-stu-id="f1b5b-127">Response</span></span>
<span data-ttu-id="f1b5b-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b5b-129">例</span><span class="sxs-lookup"><span data-stu-id="f1b5b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1b5b-130">要求</span><span class="sxs-lookup"><span data-stu-id="f1b5b-130">Request</span></span>
<span data-ttu-id="f1b5b-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="f1b5b-132">応答</span><span class="sxs-lookup"><span data-stu-id="f1b5b-132">Response</span></span>
<span data-ttu-id="f1b5b-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="f1b5b-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1b5b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
