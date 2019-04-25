---
title: 教師をリストする
description: クラスの教師のリストを取得します。 教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9e07ea3deb1cf8ec683a331ac3d76abb576be181
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550533"
---
# <a name="list-teachers"></a><span data-ttu-id="2f702-104">教師をリストする</span><span class="sxs-lookup"><span data-stu-id="2f702-104">List teachers</span></span>

<span data-ttu-id="2f702-105">クラスの教師のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2f702-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="2f702-106">教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2f702-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f702-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f702-107">Permissions</span></span>
<span data-ttu-id="2f702-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f702-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f702-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f702-110">Permission type</span></span>      | <span data-ttu-id="2f702-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f702-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f702-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f702-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f702-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2f702-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2f702-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f702-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="2f702-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f702-115">Not supported.</span></span>  |
|<span data-ttu-id="2f702-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f702-116">Application</span></span> | <span data-ttu-id="2f702-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f702-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f702-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f702-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f702-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f702-119">Optional query parameters</span></span>
<span data-ttu-id="2f702-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f702-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f702-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f702-121">Request headers</span></span>
| <span data-ttu-id="2f702-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f702-122">Header</span></span>       | <span data-ttu-id="2f702-123">値</span><span class="sxs-lookup"><span data-stu-id="2f702-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f702-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f702-124">Authorization</span></span>  | <span data-ttu-id="2f702-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f702-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f702-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f702-127">Request body</span></span>
<span data-ttu-id="2f702-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f702-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f702-129">応答</span><span class="sxs-lookup"><span data-stu-id="2f702-129">Response</span></span>
<span data-ttu-id="2f702-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2f702-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f702-131">例</span><span class="sxs-lookup"><span data-stu-id="2f702-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f702-132">要求</span><span class="sxs-lookup"><span data-stu-id="2f702-132">Request</span></span>
<span data-ttu-id="2f702-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f702-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
##### <a name="response"></a><span data-ttu-id="2f702-134">応答</span><span class="sxs-lookup"><span data-stu-id="2f702-134">Response</span></span>
<span data-ttu-id="2f702-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f702-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2f702-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2f702-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
