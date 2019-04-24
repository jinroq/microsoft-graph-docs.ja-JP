---
title: カテゴリを一覧表示する
description: この割り当てに関連付けられているすべてのカテゴリを一覧表示します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 925b2f558b98e50cfcebd7b68c3af52452f2e3df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458237"
---
# <a name="list-categories"></a><span data-ttu-id="be5e3-103">カテゴリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="be5e3-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5e3-104">この割り当てに関連付けられているすべてのカテゴリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="be5e3-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="be5e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be5e3-105">Permissions</span></span>
<span data-ttu-id="be5e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be5e3-108">Permission type</span></span>      | <span data-ttu-id="be5e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be5e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be5e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be5e3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="be5e3-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="be5e3-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="be5e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be5e3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="be5e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be5e3-113">Not supported.</span></span>  |
|<span data-ttu-id="be5e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be5e3-114">Application</span></span> | <span data-ttu-id="be5e3-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="be5e3-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="be5e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be5e3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5e3-117">Optional query parameters</span></span>
<span data-ttu-id="be5e3-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be5e3-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be5e3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be5e3-119">Request headers</span></span>
| <span data-ttu-id="be5e3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be5e3-120">Header</span></span>       | <span data-ttu-id="be5e3-121">値</span><span class="sxs-lookup"><span data-stu-id="be5e3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be5e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be5e3-122">Authorization</span></span>  | <span data-ttu-id="be5e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be5e3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be5e3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="be5e3-125">Request body</span></span>
<span data-ttu-id="be5e3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be5e3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be5e3-127">応答</span><span class="sxs-lookup"><span data-stu-id="be5e3-127">Response</span></span>
<span data-ttu-id="be5e3-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationCategory](../resources/educationcategory.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="be5e3-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be5e3-129">例</span><span class="sxs-lookup"><span data-stu-id="be5e3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be5e3-130">要求</span><span class="sxs-lookup"><span data-stu-id="be5e3-130">Request</span></span>
<span data-ttu-id="be5e3-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be5e3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="be5e3-132">応答</span><span class="sxs-lookup"><span data-stu-id="be5e3-132">Response</span></span>
<span data-ttu-id="be5e3-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be5e3-133">The following is an example of the response.</span></span> 

><span data-ttu-id="be5e3-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="be5e3-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be5e3-135">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be5e3-135">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-categories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
