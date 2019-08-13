---
title: BusinessFlowTemplates を一覧表示する
description: Azure AD access レビュー機能で、すべての businessFlowTemplate オブジェクトを一覧表示します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5a7fe7b7212a4e26dd8f0562f4a854f812cecea1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317985"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="e7a7f-103">BusinessFlowTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e7a7f-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7a7f-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7a7f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7a7f-105">Permissions</span></span>
<span data-ttu-id="e7a7f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7a7f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7a7f-108">Permission type</span></span>                        | <span data-ttu-id="e7a7f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7a7f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7a7f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7a7f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7a7f-111">Accessreview を参照してください。この後、accessreview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="e7a7f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7a7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7a7f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-113">Not supported.</span></span> |
|<span data-ttu-id="e7a7f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7a7f-114">Application</span></span>                            | <span data-ttu-id="e7a7f-115">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="e7a7f-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7a7f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7a7f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="e7a7f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7a7f-118">Request headers</span></span>
| <span data-ttu-id="e7a7f-119">名前</span><span class="sxs-lookup"><span data-stu-id="e7a7f-119">Name</span></span>         | <span data-ttu-id="e7a7f-120">型</span><span class="sxs-lookup"><span data-stu-id="e7a7f-120">Type</span></span>        | <span data-ttu-id="e7a7f-121">説明</span><span class="sxs-lookup"><span data-stu-id="e7a7f-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e7a7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7a7f-122">Authorization</span></span> | <span data-ttu-id="e7a7f-123">string</span><span class="sxs-lookup"><span data-stu-id="e7a7f-123">string</span></span> | <span data-ttu-id="e7a7f-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7a7f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7a7f-126">Request body</span></span>
<span data-ttu-id="e7a7f-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e7a7f-128">応答</span><span class="sxs-lookup"><span data-stu-id="e7a7f-128">Response</span></span>
<span data-ttu-id="e7a7f-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7a7f-130">例</span><span class="sxs-lookup"><span data-stu-id="e7a7f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7a7f-131">要求</span><span class="sxs-lookup"><span data-stu-id="e7a7f-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7a7f-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7a7f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7a7f-133">C#</span><span class="sxs-lookup"><span data-stu-id="e7a7f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7a7f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7a7f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7a7f-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7a7f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7a7f-136">Java</span><span class="sxs-lookup"><span data-stu-id="e7a7f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7a7f-137">応答</span><span class="sxs-lookup"><span data-stu-id="e7a7f-137">Response</span></span>
><span data-ttu-id="e7a7f-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e7a7f-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7a7f-140">See also</span></span>

| <span data-ttu-id="e7a7f-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7a7f-141">Method</span></span>           | <span data-ttu-id="e7a7f-142">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7a7f-142">Return Type</span></span>    |<span data-ttu-id="e7a7f-143">説明</span><span class="sxs-lookup"><span data-stu-id="e7a7f-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7a7f-144">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="e7a7f-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="e7a7f-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="e7a7f-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e7a7f-146">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="e7a7f-146">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
