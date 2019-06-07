---
title: BusinessFlowTemplates を一覧表示する
description: Azure AD access レビュー機能で、すべての businessFlowTemplate オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 1cb95b9c5eda1f561aaffcc936b2c95f8a21c980
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750067"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="f8e33-103">BusinessFlowTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f8e33-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8e33-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f8e33-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8e33-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8e33-105">Permissions</span></span>
<span data-ttu-id="f8e33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e33-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8e33-108">Permission type</span></span>                        | <span data-ttu-id="f8e33-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8e33-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8e33-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8e33-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8e33-111">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8e33-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f8e33-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8e33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8e33-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8e33-113">Not supported.</span></span> |
|<span data-ttu-id="f8e33-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8e33-114">Application</span></span>                            | <span data-ttu-id="f8e33-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e33-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="f8e33-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8e33-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f8e33-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8e33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="f8e33-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8e33-118">Request headers</span></span>
| <span data-ttu-id="f8e33-119">名前</span><span class="sxs-lookup"><span data-stu-id="f8e33-119">Name</span></span>         | <span data-ttu-id="f8e33-120">型</span><span class="sxs-lookup"><span data-stu-id="f8e33-120">Type</span></span>        | <span data-ttu-id="f8e33-121">説明</span><span class="sxs-lookup"><span data-stu-id="f8e33-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f8e33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8e33-122">Authorization</span></span> | <span data-ttu-id="f8e33-123">string</span><span class="sxs-lookup"><span data-stu-id="f8e33-123">string</span></span> | <span data-ttu-id="f8e33-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8e33-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8e33-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8e33-126">Request body</span></span>
<span data-ttu-id="f8e33-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="f8e33-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f8e33-128">応答</span><span class="sxs-lookup"><span data-stu-id="f8e33-128">Response</span></span>
<span data-ttu-id="f8e33-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[businessflowtemplate](../resources/businessflowtemplate.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="f8e33-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e33-130">例</span><span class="sxs-lookup"><span data-stu-id="f8e33-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8e33-131">要求</span><span class="sxs-lookup"><span data-stu-id="f8e33-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="f8e33-132">応答</span><span class="sxs-lookup"><span data-stu-id="f8e33-132">Response</span></span>
><span data-ttu-id="f8e33-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f8e33-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f8e33-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="f8e33-135">See also</span></span>

| <span data-ttu-id="f8e33-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8e33-136">Method</span></span>           | <span data-ttu-id="f8e33-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f8e33-137">Return Type</span></span>    |<span data-ttu-id="f8e33-138">説明</span><span class="sxs-lookup"><span data-stu-id="f8e33-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8e33-139">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="f8e33-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="f8e33-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="f8e33-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f8e33-141">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f8e33-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
