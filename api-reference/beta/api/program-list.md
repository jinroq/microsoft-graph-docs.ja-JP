---
title: プログラムの一覧表示
description: Azure AD access レビュー機能で、すべてのプログラムオブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 6200cfe9a2f9879b5589c52cd9f48b4cfa2253ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337263"
---
# <a name="list-programs"></a><span data-ttu-id="237ab-103">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="237ab-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="237ab-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[プログラム](../resources/program.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="237ab-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="237ab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="237ab-105">Permissions</span></span>
<span data-ttu-id="237ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="237ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="237ab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="237ab-108">Permission type</span></span>                        | <span data-ttu-id="237ab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="237ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="237ab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="237ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="237ab-111">programcontrol. all、programcontrol.</span><span class="sxs-lookup"><span data-stu-id="237ab-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="237ab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="237ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="237ab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="237ab-113">Not supported.</span></span> |
|<span data-ttu-id="237ab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="237ab-114">Application</span></span>                            | <span data-ttu-id="237ab-115">programcontrol. all、programcontrol.</span><span class="sxs-lookup"><span data-stu-id="237ab-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="237ab-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="237ab-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="237ab-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="237ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="237ab-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="237ab-118">Request headers</span></span>
| <span data-ttu-id="237ab-119">名前</span><span class="sxs-lookup"><span data-stu-id="237ab-119">Name</span></span>         | <span data-ttu-id="237ab-120">型</span><span class="sxs-lookup"><span data-stu-id="237ab-120">Type</span></span>        | <span data-ttu-id="237ab-121">説明</span><span class="sxs-lookup"><span data-stu-id="237ab-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="237ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="237ab-122">Authorization</span></span> | <span data-ttu-id="237ab-123">string</span><span class="sxs-lookup"><span data-stu-id="237ab-123">string</span></span> | <span data-ttu-id="237ab-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="237ab-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="237ab-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="237ab-126">Request body</span></span>
<span data-ttu-id="237ab-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="237ab-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="237ab-128">応答</span><span class="sxs-lookup"><span data-stu-id="237ab-128">Response</span></span>
<span data-ttu-id="237ab-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="237ab-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="237ab-130">例</span><span class="sxs-lookup"><span data-stu-id="237ab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="237ab-131">要求</span><span class="sxs-lookup"><span data-stu-id="237ab-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="237ab-132">応答</span><span class="sxs-lookup"><span data-stu-id="237ab-132">Response</span></span>
><span data-ttu-id="237ab-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="237ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="237ab-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="237ab-135">See also</span></span>

| <span data-ttu-id="237ab-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="237ab-136">Method</span></span>           | <span data-ttu-id="237ab-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="237ab-137">Return Type</span></span>    |<span data-ttu-id="237ab-138">説明</span><span class="sxs-lookup"><span data-stu-id="237ab-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="237ab-139">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="237ab-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="237ab-140">[programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="237ab-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="237ab-141">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="237ab-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
