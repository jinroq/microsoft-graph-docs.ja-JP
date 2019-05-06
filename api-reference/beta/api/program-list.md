---
title: プログラムの一覧表示
description: Azure AD access レビュー機能で、すべてのプログラムオブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: b71b75119dfeba79df2b326979f87db695427fd4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611277"
---
# <a name="list-programs"></a><span data-ttu-id="3452c-103">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="3452c-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3452c-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[プログラム](../resources/program.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3452c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3452c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3452c-105">Permissions</span></span>
<span data-ttu-id="3452c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3452c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3452c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3452c-108">Permission type</span></span>                        | <span data-ttu-id="3452c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3452c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3452c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3452c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3452c-111">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="3452c-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="3452c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3452c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3452c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3452c-113">Not supported.</span></span> |
|<span data-ttu-id="3452c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3452c-114">Application</span></span>                            | <span data-ttu-id="3452c-115">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="3452c-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="3452c-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3452c-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="3452c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3452c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="3452c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3452c-118">Request headers</span></span>
| <span data-ttu-id="3452c-119">名前</span><span class="sxs-lookup"><span data-stu-id="3452c-119">Name</span></span>         | <span data-ttu-id="3452c-120">型</span><span class="sxs-lookup"><span data-stu-id="3452c-120">Type</span></span>        | <span data-ttu-id="3452c-121">説明</span><span class="sxs-lookup"><span data-stu-id="3452c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3452c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3452c-122">Authorization</span></span> | <span data-ttu-id="3452c-123">string</span><span class="sxs-lookup"><span data-stu-id="3452c-123">string</span></span> | <span data-ttu-id="3452c-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="3452c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3452c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3452c-126">Request body</span></span>
<span data-ttu-id="3452c-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="3452c-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3452c-128">応答</span><span class="sxs-lookup"><span data-stu-id="3452c-128">Response</span></span>
<span data-ttu-id="3452c-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="3452c-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3452c-130">例</span><span class="sxs-lookup"><span data-stu-id="3452c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3452c-131">要求</span><span class="sxs-lookup"><span data-stu-id="3452c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="3452c-132">応答</span><span class="sxs-lookup"><span data-stu-id="3452c-132">Response</span></span>
><span data-ttu-id="3452c-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3452c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3452c-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3452c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3452c-136">Visual</span><span class="sxs-lookup"><span data-stu-id="3452c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3452c-137">Java</span><span class="sxs-lookup"><span data-stu-id="3452c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="3452c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="3452c-138">See also</span></span>

| <span data-ttu-id="3452c-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="3452c-139">Method</span></span>           | <span data-ttu-id="3452c-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3452c-140">Return Type</span></span>    |<span data-ttu-id="3452c-141">説明</span><span class="sxs-lookup"><span data-stu-id="3452c-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3452c-142">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3452c-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="3452c-143">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3452c-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="3452c-144">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3452c-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
