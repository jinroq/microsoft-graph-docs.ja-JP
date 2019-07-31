---
title: カテゴリを一覧表示する
description: この割り当てに関連付けられているすべてのカテゴリを一覧表示します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e74e1bfd808e3bc7a5dcd7b5e3bc18aebf248b11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955667"
---
# <a name="list-categories"></a><span data-ttu-id="758df-103">カテゴリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="758df-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758df-104">この割り当てに関連付けられているすべてのカテゴリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="758df-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="758df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="758df-105">Permissions</span></span>
<span data-ttu-id="758df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="758df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="758df-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="758df-108">Permission type</span></span>      | <span data-ttu-id="758df-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="758df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="758df-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="758df-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="758df-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="758df-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="758df-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="758df-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="758df-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="758df-113">Not supported.</span></span>  |
|<span data-ttu-id="758df-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="758df-114">Application</span></span> | <span data-ttu-id="758df-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="758df-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="758df-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="758df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="758df-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="758df-117">Optional query parameters</span></span>
<span data-ttu-id="758df-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="758df-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="758df-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="758df-119">Request headers</span></span>
| <span data-ttu-id="758df-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="758df-120">Header</span></span>       | <span data-ttu-id="758df-121">値</span><span class="sxs-lookup"><span data-stu-id="758df-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="758df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="758df-122">Authorization</span></span>  | <span data-ttu-id="758df-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="758df-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="758df-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="758df-125">Request body</span></span>
<span data-ttu-id="758df-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="758df-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="758df-127">応答</span><span class="sxs-lookup"><span data-stu-id="758df-127">Response</span></span>
<span data-ttu-id="758df-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationCategory](../resources/educationcategory.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="758df-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="758df-129">例</span><span class="sxs-lookup"><span data-stu-id="758df-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="758df-130">要求</span><span class="sxs-lookup"><span data-stu-id="758df-130">Request</span></span>
<span data-ttu-id="758df-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="758df-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="758df-132">応答</span><span class="sxs-lookup"><span data-stu-id="758df-132">Response</span></span>
<span data-ttu-id="758df-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="758df-133">The following is an example of the response.</span></span> 

><span data-ttu-id="758df-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="758df-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="758df-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="758df-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
