---
title: リスト businessFlowTemplates
description: Azure AD のレビュー機能にアクセス、すべての businessFlowTemplate オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 5b1d96330f808600c7f306ca85009bc5948a22f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525564"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="f1339-103">リスト businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="f1339-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1339-104">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [businessFlowTemplate](../resources/businessflowtemplate.md)のすべてのオブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f1339-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1339-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1339-105">Permissions</span></span>
<span data-ttu-id="f1339-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1339-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1339-108">Permission type</span></span>                        | <span data-ttu-id="f1339-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1339-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1339-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1339-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1339-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f1339-111"></span></span>  <span data-ttu-id="f1339-112">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1339-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="f1339-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1339-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1339-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1339-114">Not supported.</span></span> |
|<span data-ttu-id="f1339-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1339-115">Application</span></span>                            | <span data-ttu-id="f1339-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1339-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1339-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1339-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="f1339-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1339-118">Request headers</span></span>
| <span data-ttu-id="f1339-119">名前</span><span class="sxs-lookup"><span data-stu-id="f1339-119">Name</span></span>         | <span data-ttu-id="f1339-120">型</span><span class="sxs-lookup"><span data-stu-id="f1339-120">Type</span></span>        | <span data-ttu-id="f1339-121">説明</span><span class="sxs-lookup"><span data-stu-id="f1339-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f1339-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1339-122">Authorization</span></span> | <span data-ttu-id="f1339-123">string</span><span class="sxs-lookup"><span data-stu-id="f1339-123">string</span></span> | <span data-ttu-id="f1339-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="f1339-124">Bearer \{token\}.</span></span> <span data-ttu-id="f1339-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="f1339-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1339-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1339-126">Request body</span></span>
<span data-ttu-id="f1339-127">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="f1339-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f1339-128">応答</span><span class="sxs-lookup"><span data-stu-id="f1339-128">Response</span></span>
<span data-ttu-id="f1339-129">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[businessFlowTemplate](../resources/businessflowtemplate.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="f1339-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1339-130">例</span><span class="sxs-lookup"><span data-stu-id="f1339-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1339-131">要求</span><span class="sxs-lookup"><span data-stu-id="f1339-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="f1339-132">応答</span><span class="sxs-lookup"><span data-stu-id="f1339-132">Response</span></span>
><span data-ttu-id="f1339-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1339-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f1339-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="f1339-135">See also</span></span>

| <span data-ttu-id="f1339-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="f1339-136">Method</span></span>           | <span data-ttu-id="f1339-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f1339-137">Return Type</span></span>    |<span data-ttu-id="f1339-138">説明</span><span class="sxs-lookup"><span data-stu-id="f1339-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1339-139">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f1339-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="f1339-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="f1339-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f1339-141">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f1339-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
