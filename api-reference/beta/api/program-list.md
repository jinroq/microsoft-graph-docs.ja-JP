---
title: プログラムを一覧表示
description: Azure AD のレビュー機能にアクセス、プログラムのすべてのオブジェクトを一覧表示します。
ms.openlocfilehash: fd934ec4dcfe4feb6167a6cf397be3669099c123
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067767"
---
# <a name="list-programs"></a><span data-ttu-id="a3734-103">プログラムを一覧表示</span><span class="sxs-lookup"><span data-stu-id="a3734-103">List programs</span></span>

> <span data-ttu-id="a3734-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3734-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3734-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3734-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3734-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、[プログラム](../resources/program.md)のすべてのオブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a3734-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3734-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3734-107">Permissions</span></span>
<span data-ttu-id="a3734-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3734-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3734-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3734-110">Permission type</span></span>                        | <span data-ttu-id="a3734-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3734-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3734-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3734-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3734-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a3734-113"></span></span>  <span data-ttu-id="a3734-114">サインインしているユーザーは、プログラムを読むことを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="a3734-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="a3734-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3734-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3734-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3734-116">Not supported.</span></span> |
|<span data-ttu-id="a3734-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3734-117">Application</span></span>                            | <span data-ttu-id="a3734-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3734-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3734-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3734-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="a3734-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3734-120">Request headers</span></span>
| <span data-ttu-id="a3734-121">名前</span><span class="sxs-lookup"><span data-stu-id="a3734-121">Name</span></span>         | <span data-ttu-id="a3734-122">型</span><span class="sxs-lookup"><span data-stu-id="a3734-122">Type</span></span>        | <span data-ttu-id="a3734-123">説明</span><span class="sxs-lookup"><span data-stu-id="a3734-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a3734-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3734-124">Authorization</span></span> | <span data-ttu-id="a3734-125">string</span><span class="sxs-lookup"><span data-stu-id="a3734-125">string</span></span> | <span data-ttu-id="a3734-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="a3734-126">Bearer \{token\}.</span></span> <span data-ttu-id="a3734-127">必須。</span><span class="sxs-lookup"><span data-stu-id="a3734-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3734-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3734-128">Request body</span></span>
<span data-ttu-id="a3734-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="a3734-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a3734-130">応答</span><span class="sxs-lookup"><span data-stu-id="a3734-130">Response</span></span>
<span data-ttu-id="a3734-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本体の[プログラム](../resources/program.md)のオブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="a3734-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3734-132">例</span><span class="sxs-lookup"><span data-stu-id="a3734-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3734-133">要求</span><span class="sxs-lookup"><span data-stu-id="a3734-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="a3734-134">応答</span><span class="sxs-lookup"><span data-stu-id="a3734-134">Response</span></span>
><span data-ttu-id="a3734-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3734-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a3734-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3734-137">See also</span></span>

| <span data-ttu-id="a3734-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3734-138">Method</span></span>           | <span data-ttu-id="a3734-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3734-139">Return Type</span></span>    |<span data-ttu-id="a3734-140">説明</span><span class="sxs-lookup"><span data-stu-id="a3734-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3734-141">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="a3734-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="a3734-142">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a3734-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="a3734-143">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a3734-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
