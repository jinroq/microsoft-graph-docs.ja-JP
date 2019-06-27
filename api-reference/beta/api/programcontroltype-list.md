---
title: ProgramControlTypes のリスト
description: Azure AD access レビュー機能で、すべての programControlType オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 2a2767a0dc55e5d2d046e897ec0ac6cde10af945
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264079"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="d9715-103">ProgramControlTypes のリスト</span><span class="sxs-lookup"><span data-stu-id="d9715-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9715-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[programcontroltype](../resources/programcontroltype.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9715-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9715-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9715-105">Permissions</span></span>
<span data-ttu-id="d9715-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9715-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9715-108">Permission type</span></span>                        | <span data-ttu-id="d9715-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9715-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9715-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9715-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9715-111">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="d9715-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="d9715-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9715-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9715-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9715-113">Not supported.</span></span> |
|<span data-ttu-id="d9715-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9715-114">Application</span></span>                            | <span data-ttu-id="d9715-115">ProgramControl. All ', ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="d9715-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="d9715-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d9715-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9715-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9715-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="d9715-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9715-118">Request headers</span></span>
| <span data-ttu-id="d9715-119">名前</span><span class="sxs-lookup"><span data-stu-id="d9715-119">Name</span></span>         | <span data-ttu-id="d9715-120">型</span><span class="sxs-lookup"><span data-stu-id="d9715-120">Type</span></span>        | <span data-ttu-id="d9715-121">説明</span><span class="sxs-lookup"><span data-stu-id="d9715-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d9715-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9715-122">Authorization</span></span> | <span data-ttu-id="d9715-123">string</span><span class="sxs-lookup"><span data-stu-id="d9715-123">string</span></span> | <span data-ttu-id="d9715-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9715-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9715-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9715-126">Request body</span></span>
<span data-ttu-id="d9715-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="d9715-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d9715-128">応答</span><span class="sxs-lookup"><span data-stu-id="d9715-128">Response</span></span>
<span data-ttu-id="d9715-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[programcontroltype](../resources/programcontroltype.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="d9715-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9715-130">例</span><span class="sxs-lookup"><span data-stu-id="d9715-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9715-131">要求</span><span class="sxs-lookup"><span data-stu-id="d9715-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="d9715-132">応答</span><span class="sxs-lookup"><span data-stu-id="d9715-132">Response</span></span>
><span data-ttu-id="d9715-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d9715-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d9715-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d9715-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d9715-136">C#</span><span class="sxs-lookup"><span data-stu-id="d9715-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9715-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9715-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d9715-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="d9715-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="d9715-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9715-139">See also</span></span>

| <span data-ttu-id="d9715-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9715-140">Method</span></span>           | <span data-ttu-id="d9715-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d9715-141">Return Type</span></span>    |<span data-ttu-id="d9715-142">説明</span><span class="sxs-lookup"><span data-stu-id="d9715-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9715-143">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d9715-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="d9715-144">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d9715-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="d9715-145">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d9715-145">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
