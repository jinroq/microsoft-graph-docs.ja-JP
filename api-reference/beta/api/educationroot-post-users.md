---
title: educationUser を作成する
description: 新しいユーザーを作成します。
ms.openlocfilehash: d0edc82187d52df07d1954e8098cc4744c68ca15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069887"
---
# <a name="create-educationuser"></a><span data-ttu-id="13131-103">educationUser を作成する</span><span class="sxs-lookup"><span data-stu-id="13131-103">Create educationUser</span></span>

> <span data-ttu-id="13131-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13131-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13131-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13131-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13131-106">新しいユーザーを作成します。</span><span class="sxs-lookup"><span data-stu-id="13131-106">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="13131-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13131-107">Permissions</span></span>
<span data-ttu-id="13131-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13131-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13131-110">Permission type</span></span>      | <span data-ttu-id="13131-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13131-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13131-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13131-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="13131-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13131-113">Not supported.</span></span>  |
|<span data-ttu-id="13131-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13131-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13131-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13131-115">Not supported.</span></span>  |
|<span data-ttu-id="13131-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13131-116">Application</span></span> | <span data-ttu-id="13131-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13131-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="13131-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13131-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="13131-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13131-119">Request headers</span></span>
| <span data-ttu-id="13131-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13131-120">Header</span></span>       | <span data-ttu-id="13131-121">値</span><span class="sxs-lookup"><span data-stu-id="13131-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13131-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13131-122">Authorization</span></span>  | <span data-ttu-id="13131-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13131-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="13131-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13131-125">Content-Type</span></span>  | <span data-ttu-id="13131-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13131-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13131-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13131-127">Request body</span></span>
<span data-ttu-id="13131-128">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13131-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="13131-129">応答</span><span class="sxs-lookup"><span data-stu-id="13131-129">Response</span></span>
<span data-ttu-id="13131-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13131-130">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13131-131">例</span><span class="sxs-lookup"><span data-stu-id="13131-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13131-132">要求</span><span class="sxs-lookup"><span data-stu-id="13131-132">Request</span></span>
<span data-ttu-id="13131-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13131-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

##### <a name="response"></a><span data-ttu-id="13131-134">応答</span><span class="sxs-lookup"><span data-stu-id="13131-134">Response</span></span>
<span data-ttu-id="13131-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13131-135">The following is an example of the response.</span></span> 

><span data-ttu-id="13131-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13131-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
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