---
title: BusinessFlowTemplates を一覧表示する
description: Azure AD access レビュー機能で、すべての businessFlowTemplate オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 3f7fc6ac155b22845c13c75fddd1af49f7b32e32
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262448"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="08253-103">BusinessFlowTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08253-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08253-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="08253-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="08253-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08253-105">Permissions</span></span>
<span data-ttu-id="08253-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08253-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08253-108">Permission type</span></span>                        | <span data-ttu-id="08253-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08253-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="08253-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08253-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="08253-111">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08253-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="08253-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08253-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08253-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08253-113">Not supported.</span></span> |
|<span data-ttu-id="08253-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08253-114">Application</span></span>                            | <span data-ttu-id="08253-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="08253-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="08253-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="08253-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="08253-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08253-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="08253-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08253-118">Request headers</span></span>
| <span data-ttu-id="08253-119">名前</span><span class="sxs-lookup"><span data-stu-id="08253-119">Name</span></span>         | <span data-ttu-id="08253-120">型</span><span class="sxs-lookup"><span data-stu-id="08253-120">Type</span></span>        | <span data-ttu-id="08253-121">説明</span><span class="sxs-lookup"><span data-stu-id="08253-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="08253-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08253-122">Authorization</span></span> | <span data-ttu-id="08253-123">string</span><span class="sxs-lookup"><span data-stu-id="08253-123">string</span></span> | <span data-ttu-id="08253-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="08253-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08253-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="08253-126">Request body</span></span>
<span data-ttu-id="08253-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="08253-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="08253-128">応答</span><span class="sxs-lookup"><span data-stu-id="08253-128">Response</span></span>
<span data-ttu-id="08253-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="08253-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08253-130">例</span><span class="sxs-lookup"><span data-stu-id="08253-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08253-131">要求</span><span class="sxs-lookup"><span data-stu-id="08253-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="08253-132">応答</span><span class="sxs-lookup"><span data-stu-id="08253-132">Response</span></span>
><span data-ttu-id="08253-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="08253-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="08253-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="08253-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="08253-136">C#</span><span class="sxs-lookup"><span data-stu-id="08253-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08253-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="08253-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="08253-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="08253-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="08253-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="08253-139">See also</span></span>

| <span data-ttu-id="08253-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="08253-140">Method</span></span>           | <span data-ttu-id="08253-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="08253-141">Return Type</span></span>    |<span data-ttu-id="08253-142">説明</span><span class="sxs-lookup"><span data-stu-id="08253-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08253-143">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="08253-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="08253-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="08253-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="08253-145">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="08253-145">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}
-->
