---
title: educationUsers をリストする
description: 学校のユーザーのリストを取得します。
author: mmast-msft
ms.openlocfilehash: 6e642792b8cb3d7463b13288b0ed95838590ec52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336415"
---
# <a name="list-educationusers"></a><span data-ttu-id="58e22-103">educationUsers をリストする</span><span class="sxs-lookup"><span data-stu-id="58e22-103">List educationUsers</span></span>

> <span data-ttu-id="58e22-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58e22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58e22-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58e22-106">学校のユーザーのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="58e22-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="58e22-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58e22-107">Permissions</span></span>
<span data-ttu-id="58e22-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58e22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e22-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58e22-110">Permission type</span></span>      | <span data-ttu-id="58e22-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58e22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e22-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58e22-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="58e22-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e22-113">Not supported.</span></span>  |
|<span data-ttu-id="58e22-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58e22-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="58e22-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58e22-115">Not supported.</span></span>  |
|<span data-ttu-id="58e22-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58e22-116">Application</span></span> | <span data-ttu-id="58e22-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e22-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="58e22-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58e22-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58e22-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="58e22-119">Optional query parameters</span></span>
<span data-ttu-id="58e22-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="58e22-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e22-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58e22-121">Request headers</span></span>
| <span data-ttu-id="58e22-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58e22-122">Header</span></span>       | <span data-ttu-id="58e22-123">値</span><span class="sxs-lookup"><span data-stu-id="58e22-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58e22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e22-124">Authorization</span></span>  | <span data-ttu-id="58e22-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58e22-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58e22-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="58e22-127">Request body</span></span>
<span data-ttu-id="58e22-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="58e22-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="58e22-129">応答</span><span class="sxs-lookup"><span data-stu-id="58e22-129">Response</span></span>
<span data-ttu-id="58e22-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="58e22-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58e22-131">例</span><span class="sxs-lookup"><span data-stu-id="58e22-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58e22-132">要求</span><span class="sxs-lookup"><span data-stu-id="58e22-132">Request</span></span>
<span data-ttu-id="58e22-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58e22-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="58e22-134">応答</span><span class="sxs-lookup"><span data-stu-id="58e22-134">Response</span></span>
<span data-ttu-id="58e22-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58e22-135">The following is an example of the response.</span></span> 

><span data-ttu-id="58e22-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="58e22-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->