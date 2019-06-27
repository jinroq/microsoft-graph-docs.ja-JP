---
title: ProgramControls のリスト
description: Azure AD access レビュー機能で、すべての programControl オブジェクトを、テナント内のすべてのプログラムで一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 9d1b583399e8006a77f8869a44e35833e123e559
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268041"
---
# <a name="list-programcontrols"></a><span data-ttu-id="78f3d-103">ProgramControls のリスト</span><span class="sxs-lookup"><span data-stu-id="78f3d-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f3d-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[programcontrol](../resources/programcontrol.md)オブジェクトを、テナント内のすべてのプログラムで一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="78f3d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="78f3d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78f3d-105">Permissions</span></span>
<span data-ttu-id="78f3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78f3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78f3d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78f3d-108">Permission type</span></span>                        | <span data-ttu-id="78f3d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78f3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="78f3d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78f3d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="78f3d-111">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="78f3d-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="78f3d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78f3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f3d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78f3d-113">Not supported.</span></span> |
|<span data-ttu-id="78f3d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78f3d-114">Application</span></span>                            | <span data-ttu-id="78f3d-115">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="78f3d-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="78f3d-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="78f3d-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="78f3d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78f3d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="78f3d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78f3d-118">Request headers</span></span>
| <span data-ttu-id="78f3d-119">名前</span><span class="sxs-lookup"><span data-stu-id="78f3d-119">Name</span></span>         | <span data-ttu-id="78f3d-120">型</span><span class="sxs-lookup"><span data-stu-id="78f3d-120">Type</span></span>        | <span data-ttu-id="78f3d-121">説明</span><span class="sxs-lookup"><span data-stu-id="78f3d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="78f3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f3d-122">Authorization</span></span> | <span data-ttu-id="78f3d-123">string</span><span class="sxs-lookup"><span data-stu-id="78f3d-123">string</span></span> | <span data-ttu-id="78f3d-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="78f3d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78f3d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="78f3d-126">Request body</span></span>
<span data-ttu-id="78f3d-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="78f3d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="78f3d-128">応答</span><span class="sxs-lookup"><span data-stu-id="78f3d-128">Response</span></span>
<span data-ttu-id="78f3d-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="78f3d-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f3d-130">例</span><span class="sxs-lookup"><span data-stu-id="78f3d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78f3d-131">要求</span><span class="sxs-lookup"><span data-stu-id="78f3d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="78f3d-132">応答</span><span class="sxs-lookup"><span data-stu-id="78f3d-132">Response</span></span>
><span data-ttu-id="78f3d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="78f3d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="78f3d-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="78f3d-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="78f3d-136">C#</span><span class="sxs-lookup"><span data-stu-id="78f3d-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78f3d-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="78f3d-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programControl-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="78f3d-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="78f3d-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_programControl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="78f3d-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="78f3d-139">See also</span></span>

| <span data-ttu-id="78f3d-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="78f3d-140">Method</span></span>           | <span data-ttu-id="78f3d-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78f3d-141">Return Type</span></span>    |<span data-ttu-id="78f3d-142">説明</span><span class="sxs-lookup"><span data-stu-id="78f3d-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78f3d-143">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="78f3d-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="78f3d-144">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78f3d-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="78f3d-145">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="78f3d-145">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
