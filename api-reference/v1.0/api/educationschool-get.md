---
title: educationSchool を取得する
description: 学校オブジェクトのプロパティと関係を取得します。
author: mmast-msft
ms.openlocfilehash: 4b4d68c2c71725f2ed3be1adb9067eea6d7d87bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336779"
---
# <a name="get-educationschool"></a><span data-ttu-id="9cbc0-103">educationSchool を取得する</span><span class="sxs-lookup"><span data-stu-id="9cbc0-103">Get educationSchool</span></span>

<span data-ttu-id="9cbc0-104">学校オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cbc0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9cbc0-105">Permissions</span></span>
<span data-ttu-id="9cbc0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cbc0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9cbc0-108">Permission type</span></span>      | <span data-ttu-id="9cbc0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9cbc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cbc0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9cbc0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9cbc0-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9cbc0-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="9cbc0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9cbc0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9cbc0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-113">Not supported.</span></span>  |
|<span data-ttu-id="9cbc0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9cbc0-114">Application</span></span> | <span data-ttu-id="9cbc0-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cbc0-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9cbc0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9cbc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9cbc0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9cbc0-117">Optional query parameters</span></span>
<span data-ttu-id="9cbc0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cbc0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cbc0-119">Request headers</span></span>
| <span data-ttu-id="9cbc0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cbc0-120">Header</span></span>       | <span data-ttu-id="9cbc0-121">値</span><span class="sxs-lookup"><span data-stu-id="9cbc0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9cbc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cbc0-122">Authorization</span></span>  | <span data-ttu-id="9cbc0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cbc0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9cbc0-125">Request body</span></span>
<span data-ttu-id="9cbc0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9cbc0-127">応答</span><span class="sxs-lookup"><span data-stu-id="9cbc0-127">Response</span></span>
<span data-ttu-id="9cbc0-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cbc0-129">例</span><span class="sxs-lookup"><span data-stu-id="9cbc0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cbc0-130">要求</span><span class="sxs-lookup"><span data-stu-id="9cbc0-130">Request</span></span>
<span data-ttu-id="9cbc0-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="9cbc0-132">応答</span><span class="sxs-lookup"><span data-stu-id="9cbc0-132">Response</span></span>
<span data-ttu-id="9cbc0-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-133">The following is an example of the response.</span></span> 

><span data-ttu-id="9cbc0-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9cbc0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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