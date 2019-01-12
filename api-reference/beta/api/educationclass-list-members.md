---
title: メンバーを一覧表示する
description: クラスの教師と学生を取得します。 委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 09c02d13a6c8c74b8e9cca690f605fa4ee128e67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915292"
---
# <a name="list-members"></a><span data-ttu-id="e24a4-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e24a4-104">List members</span></span>

> <span data-ttu-id="e24a4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e24a4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e24a4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e24a4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e24a4-107">クラスの教師と学生を取得します。</span><span class="sxs-lookup"><span data-stu-id="e24a4-107">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="e24a4-108">委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。</span><span class="sxs-lookup"><span data-stu-id="e24a4-108">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="e24a4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e24a4-109">Permissions</span></span>
<span data-ttu-id="e24a4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e24a4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e24a4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e24a4-112">Permission type</span></span>      | <span data-ttu-id="e24a4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e24a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e24a4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e24a4-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e24a4-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e24a4-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e24a4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e24a4-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e24a4-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e24a4-117">Not supported</span></span>  |
|<span data-ttu-id="e24a4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e24a4-118">Application</span></span> | <span data-ttu-id="e24a4-119">EduRoster.Read.All、EduRoster.ReadWrite.All と Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="e24a4-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e24a4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e24a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e24a4-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e24a4-121">Optional query parameters</span></span>
<span data-ttu-id="e24a4-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e24a4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e24a4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e24a4-123">Request headers</span></span>
| <span data-ttu-id="e24a4-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e24a4-124">Header</span></span>       | <span data-ttu-id="e24a4-125">値</span><span class="sxs-lookup"><span data-stu-id="e24a4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e24a4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e24a4-126">Authorization</span></span>  | <span data-ttu-id="e24a4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e24a4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e24a4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e24a4-129">Request body</span></span>
<span data-ttu-id="e24a4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e24a4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e24a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="e24a4-131">Response</span></span>
<span data-ttu-id="e24a4-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e24a4-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e24a4-133">例</span><span class="sxs-lookup"><span data-stu-id="e24a4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e24a4-134">要求</span><span class="sxs-lookup"><span data-stu-id="e24a4-134">Request</span></span>
<span data-ttu-id="e24a4-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e24a4-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="e24a4-136">応答</span><span class="sxs-lookup"><span data-stu-id="e24a4-136">Response</span></span>
<span data-ttu-id="e24a4-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e24a4-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e24a4-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e24a4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
