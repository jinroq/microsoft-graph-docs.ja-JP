---
title: リスト businessFlowTemplates
description: Azure AD のレビュー機能にアクセス、すべての businessFlowTemplate オブジェクトを一覧表示します。
ms.openlocfilehash: 9c6dc976244c60151cb2c230430ab6b4d0dc4b43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067040"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="ebecb-103">リスト businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="ebecb-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="ebecb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebecb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebecb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebecb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebecb-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [businessFlowTemplate](../resources/businessflowtemplate.md)のすべてのオブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ebecb-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebecb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebecb-107">Permissions</span></span>
<span data-ttu-id="ebecb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebecb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebecb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebecb-110">Permission type</span></span>                        | <span data-ttu-id="ebecb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebecb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebecb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebecb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebecb-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="ebecb-113"></span></span>  <span data-ttu-id="ebecb-114">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebecb-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="ebecb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebecb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebecb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebecb-116">Not supported.</span></span> |
|<span data-ttu-id="ebecb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebecb-117">Application</span></span>                            | <span data-ttu-id="ebecb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebecb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebecb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebecb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="ebecb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebecb-120">Request headers</span></span>
| <span data-ttu-id="ebecb-121">名前</span><span class="sxs-lookup"><span data-stu-id="ebecb-121">Name</span></span>         | <span data-ttu-id="ebecb-122">型</span><span class="sxs-lookup"><span data-stu-id="ebecb-122">Type</span></span>        | <span data-ttu-id="ebecb-123">説明</span><span class="sxs-lookup"><span data-stu-id="ebecb-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ebecb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebecb-124">Authorization</span></span> | <span data-ttu-id="ebecb-125">string</span><span class="sxs-lookup"><span data-stu-id="ebecb-125">string</span></span> | <span data-ttu-id="ebecb-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="ebecb-126">Bearer \{token\}.</span></span> <span data-ttu-id="ebecb-127">必須。</span><span class="sxs-lookup"><span data-stu-id="ebecb-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebecb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebecb-128">Request body</span></span>
<span data-ttu-id="ebecb-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="ebecb-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ebecb-130">応答</span><span class="sxs-lookup"><span data-stu-id="ebecb-130">Response</span></span>
<span data-ttu-id="ebecb-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[businessFlowTemplate](../resources/businessflowtemplate.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="ebecb-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebecb-132">例</span><span class="sxs-lookup"><span data-stu-id="ebecb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebecb-133">要求</span><span class="sxs-lookup"><span data-stu-id="ebecb-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="ebecb-134">応答</span><span class="sxs-lookup"><span data-stu-id="ebecb-134">Response</span></span>
><span data-ttu-id="ebecb-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ebecb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ebecb-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebecb-137">See also</span></span>

| <span data-ttu-id="ebecb-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebecb-138">Method</span></span>           | <span data-ttu-id="ebecb-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ebecb-139">Return Type</span></span>    |<span data-ttu-id="ebecb-140">説明</span><span class="sxs-lookup"><span data-stu-id="ebecb-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebecb-141">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="ebecb-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="ebecb-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="ebecb-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="ebecb-143">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="ebecb-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
