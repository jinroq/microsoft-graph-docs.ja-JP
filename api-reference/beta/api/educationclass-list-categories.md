---
title: リスト educationCategories
description: Category オブジェクトのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6757f64942ee87d4e13b577964645f9a35839477
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955426"
---
# <a name="list-educationcategories"></a><span data-ttu-id="b1904-103">リスト educationCategories</span><span class="sxs-lookup"><span data-stu-id="b1904-103">List educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1904-104">[EducationCategory](../resources/educationcategory.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b1904-104">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1904-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1904-105">Permissions</span></span>

<span data-ttu-id="b1904-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1904-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1904-108">Permission type</span></span>                        | <span data-ttu-id="b1904-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1904-109">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b1904-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1904-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1904-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="b1904-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b1904-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1904-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1904-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1904-113">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="b1904-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1904-114">Application</span></span>                            | <span data-ttu-id="b1904-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1904-115">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="b1904-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1904-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1904-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b1904-117">Optional query parameters</span></span>

<span data-ttu-id="b1904-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b1904-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1904-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1904-119">Request headers</span></span>

| <span data-ttu-id="b1904-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1904-120">Header</span></span>        | <span data-ttu-id="b1904-121">値</span><span class="sxs-lookup"><span data-stu-id="b1904-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b1904-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1904-122">Authorization</span></span> | <span data-ttu-id="b1904-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1904-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1904-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1904-125">Request body</span></span>

<span data-ttu-id="b1904-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1904-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1904-127">応答</span><span class="sxs-lookup"><span data-stu-id="b1904-127">Response</span></span>

<span data-ttu-id="b1904-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationCategory](../resources/educationcategory.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b1904-128">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1904-129">例</span><span class="sxs-lookup"><span data-stu-id="b1904-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1904-130">要求</span><span class="sxs-lookup"><span data-stu-id="b1904-130">Request</span></span>

<span data-ttu-id="b1904-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1904-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="b1904-132">応答</span><span class="sxs-lookup"><span data-stu-id="b1904-132">Response</span></span>

<span data-ttu-id="b1904-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1904-133">The following is an example of the response.</span></span> 

><span data-ttu-id="b1904-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b1904-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
