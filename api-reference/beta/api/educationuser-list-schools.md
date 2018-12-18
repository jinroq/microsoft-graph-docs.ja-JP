---
title: 学校をリストする
description: ユーザーの学校のリストを取得します。
author: mmast-msft
ms.openlocfilehash: 35810f4b1928249576ac1216356701489f68feca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303270"
---
# <a name="list-schools"></a><span data-ttu-id="2e407-103">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="2e407-103">List schools</span></span>

> <span data-ttu-id="2e407-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e407-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e407-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e407-106">ユーザーの学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2e407-106">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="2e407-107">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="2e407-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="2e407-108">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="2e407-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e407-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e407-109">Permissions</span></span>
<span data-ttu-id="2e407-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e407-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e407-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e407-112">Permission type</span></span>      | <span data-ttu-id="2e407-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e407-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e407-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e407-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e407-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2e407-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2e407-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e407-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2e407-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e407-117">Not supported.</span></span>  |
|<span data-ttu-id="2e407-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e407-118">Application</span></span> | <span data-ttu-id="2e407-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e407-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e407-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e407-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e407-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2e407-121">Optional query parameters</span></span>
<span data-ttu-id="2e407-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2e407-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e407-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e407-123">Request headers</span></span>
| <span data-ttu-id="2e407-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e407-124">Header</span></span>       | <span data-ttu-id="2e407-125">値</span><span class="sxs-lookup"><span data-stu-id="2e407-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e407-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e407-126">Authorization</span></span>  | <span data-ttu-id="2e407-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e407-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e407-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e407-129">Request body</span></span>
<span data-ttu-id="2e407-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2e407-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e407-131">応答</span><span class="sxs-lookup"><span data-stu-id="2e407-131">Response</span></span>
<span data-ttu-id="2e407-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2e407-132">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e407-133">例</span><span class="sxs-lookup"><span data-stu-id="2e407-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e407-134">要求</span><span class="sxs-lookup"><span data-stu-id="2e407-134">Request</span></span>
<span data-ttu-id="2e407-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e407-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="2e407-136">応答</span><span class="sxs-lookup"><span data-stu-id="2e407-136">Response</span></span>
<span data-ttu-id="2e407-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e407-137">The following is an example of the response.</span></span> 

><span data-ttu-id="2e407-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2e407-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->