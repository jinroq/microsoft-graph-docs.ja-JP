---
title: educationSchool を取得する
description: 学校オブジェクトのプロパティと関係を取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6b43360dd6582cb0f9c0f84166eb27e362dd0e0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976948"
---
# <a name="get-educationschool"></a><span data-ttu-id="8a5ef-103">educationSchool を取得する</span><span class="sxs-lookup"><span data-stu-id="8a5ef-103">Get educationSchool</span></span>

<span data-ttu-id="8a5ef-104">学校オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a5ef-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a5ef-105">Permissions</span></span>
<span data-ttu-id="8a5ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a5ef-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a5ef-108">Permission type</span></span>      | <span data-ttu-id="8a5ef-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a5ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a5ef-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5ef-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a5ef-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8a5ef-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="8a5ef-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5ef-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a5ef-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-113">Not supported.</span></span>  |
|<span data-ttu-id="8a5ef-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a5ef-114">Application</span></span> | <span data-ttu-id="8a5ef-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5ef-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a5ef-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a5ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a5ef-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a5ef-117">Optional query parameters</span></span>
<span data-ttu-id="8a5ef-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a5ef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5ef-119">Request headers</span></span>
| <span data-ttu-id="8a5ef-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5ef-120">Header</span></span>       | <span data-ttu-id="8a5ef-121">値</span><span class="sxs-lookup"><span data-stu-id="8a5ef-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a5ef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a5ef-122">Authorization</span></span>  | <span data-ttu-id="8a5ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a5ef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a5ef-125">Request body</span></span>
<span data-ttu-id="8a5ef-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8a5ef-127">応答</span><span class="sxs-lookup"><span data-stu-id="8a5ef-127">Response</span></span>
<span data-ttu-id="8a5ef-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a5ef-129">例</span><span class="sxs-lookup"><span data-stu-id="8a5ef-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a5ef-130">要求</span><span class="sxs-lookup"><span data-stu-id="8a5ef-130">Request</span></span>
<span data-ttu-id="8a5ef-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="8a5ef-132">応答</span><span class="sxs-lookup"><span data-stu-id="8a5ef-132">Response</span></span>
<span data-ttu-id="8a5ef-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-133">The following is an example of the response.</span></span> 

><span data-ttu-id="8a5ef-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a5ef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
