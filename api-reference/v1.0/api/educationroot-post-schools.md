---
title: educationSchool を作成する
description: 学校を作成します。
ms.openlocfilehash: c6be0d1b22b15e92c324b6a3c5c43c4c49894fc3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023740"
---
# <a name="create-educationschool"></a><span data-ttu-id="f3583-103">educationSchool を作成する</span><span class="sxs-lookup"><span data-stu-id="f3583-103">Create educationSchool</span></span>

<span data-ttu-id="f3583-104">学校を作成します。</span><span class="sxs-lookup"><span data-stu-id="f3583-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3583-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3583-105">Permissions</span></span>
<span data-ttu-id="f3583-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3583-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3583-108">Permission type</span></span>      | <span data-ttu-id="f3583-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3583-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3583-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3583-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f3583-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3583-111">Not supported.</span></span>  |
|<span data-ttu-id="f3583-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3583-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f3583-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3583-113">Not supported.</span></span>  |
|<span data-ttu-id="f3583-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3583-114">Application</span></span> | <span data-ttu-id="f3583-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3583-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3583-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3583-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="f3583-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3583-117">Request headers</span></span>
| <span data-ttu-id="f3583-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3583-118">Header</span></span>       | <span data-ttu-id="f3583-119">値</span><span class="sxs-lookup"><span data-stu-id="f3583-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3583-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3583-120">Authorization</span></span>  | <span data-ttu-id="f3583-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3583-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f3583-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3583-123">Content-Type</span></span>  | <span data-ttu-id="f3583-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3583-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3583-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3583-125">Request body</span></span>
<span data-ttu-id="f3583-126">要求本文で、[educationSchool](../resources/educationschool.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3583-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f3583-127">応答</span><span class="sxs-lookup"><span data-stu-id="f3583-127">Response</span></span>
<span data-ttu-id="f3583-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3583-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3583-129">例</span><span class="sxs-lookup"><span data-stu-id="f3583-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3583-130">要求</span><span class="sxs-lookup"><span data-stu-id="f3583-130">Request</span></span>
<span data-ttu-id="f3583-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3583-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="f3583-132">応答</span><span class="sxs-lookup"><span data-stu-id="f3583-132">Response</span></span>
<span data-ttu-id="f3583-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3583-133">The following is an example of the response.</span></span> 

><span data-ttu-id="f3583-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f3583-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->