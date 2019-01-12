---
title: 教師をリストする
description: クラスの教師のリストを取得します。 教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 871090596ec83e9af90a37e8afc6f4b8f67faed5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960512"
---
# <a name="list-teachers"></a><span data-ttu-id="8134a-104">教師をリストする</span><span class="sxs-lookup"><span data-stu-id="8134a-104">List teachers</span></span>

> <span data-ttu-id="8134a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8134a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8134a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8134a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8134a-107">クラスの教師のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="8134a-107">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="8134a-108">教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="8134a-108">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8134a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8134a-109">Permissions</span></span>
<span data-ttu-id="8134a-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8134a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8134a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8134a-112">Permission type</span></span>      | <span data-ttu-id="8134a-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8134a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8134a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8134a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8134a-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8134a-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="8134a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8134a-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="8134a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8134a-117">Not supported.</span></span>  |
|<span data-ttu-id="8134a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8134a-118">Application</span></span> | <span data-ttu-id="8134a-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8134a-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8134a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8134a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8134a-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8134a-121">Optional query parameters</span></span>
<span data-ttu-id="8134a-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8134a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8134a-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8134a-123">Request headers</span></span>
| <span data-ttu-id="8134a-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8134a-124">Header</span></span>       | <span data-ttu-id="8134a-125">値</span><span class="sxs-lookup"><span data-stu-id="8134a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8134a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8134a-126">Authorization</span></span>  | <span data-ttu-id="8134a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8134a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8134a-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8134a-129">Request body</span></span>
<span data-ttu-id="8134a-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8134a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8134a-131">応答</span><span class="sxs-lookup"><span data-stu-id="8134a-131">Response</span></span>
<span data-ttu-id="8134a-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8134a-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8134a-133">例</span><span class="sxs-lookup"><span data-stu-id="8134a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8134a-134">要求</span><span class="sxs-lookup"><span data-stu-id="8134a-134">Request</span></span>
<span data-ttu-id="8134a-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8134a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="8134a-136">応答</span><span class="sxs-lookup"><span data-stu-id="8134a-136">Response</span></span>
<span data-ttu-id="8134a-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8134a-137">The following is an example of the response.</span></span> 

><span data-ttu-id="8134a-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8134a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
