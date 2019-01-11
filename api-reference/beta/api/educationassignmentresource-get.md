---
title: EducationAssignmentResource を取得します。
description: '割り当ての特定のリソースのプロパティを取得します。  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: da96f7476e6feda2f27b0653393de8c2eaac3022
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832957"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="9a1c3-103">EducationAssignmentResource を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-103">Get educationAssignmentResource</span></span>

> <span data-ttu-id="9a1c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a1c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a1c3-106">割り当ての特定のリソースのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-106">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="9a1c3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a1c3-107">Permissions</span></span>
<span data-ttu-id="9a1c3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a1c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a1c3-110">Permission type</span></span>      | <span data-ttu-id="9a1c3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a1c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a1c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a1c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a1c3-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a1c3-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="9a1c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a1c3-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9a1c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-115">Not supported.</span></span>  |
|<span data-ttu-id="9a1c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a1c3-116">Application</span></span> |  <span data-ttu-id="9a1c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9a1c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a1c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a1c3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a1c3-119">Optional query parameters</span></span>
<span data-ttu-id="9a1c3-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a1c3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a1c3-121">Request headers</span></span>
| <span data-ttu-id="9a1c3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a1c3-122">Header</span></span>       | <span data-ttu-id="9a1c3-123">値</span><span class="sxs-lookup"><span data-stu-id="9a1c3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a1c3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a1c3-124">Authorization</span></span>  | <span data-ttu-id="9a1c3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a1c3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a1c3-127">Request body</span></span>
<span data-ttu-id="9a1c3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9a1c3-129">応答</span><span class="sxs-lookup"><span data-stu-id="9a1c3-129">Response</span></span>
<span data-ttu-id="9a1c3-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a1c3-131">例</span><span class="sxs-lookup"><span data-stu-id="9a1c3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a1c3-132">要求</span><span class="sxs-lookup"><span data-stu-id="9a1c3-132">Request</span></span>
<span data-ttu-id="9a1c3-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="9a1c3-134">応答</span><span class="sxs-lookup"><span data-stu-id="9a1c3-134">Response</span></span>
<span data-ttu-id="9a1c3-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9a1c3-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a1c3-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a1c3-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
