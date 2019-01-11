---
title: リスト programControls
description: Azure AD アクセスのレビュー機能では、テナント内のすべてのプログラム間でデバッギング オブジェクトがすべてを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: bc56fd5013bcf0013007b9d4264ab89eca02d43b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843954"
---
# <a name="list-programcontrols"></a><span data-ttu-id="07a9f-103">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="07a9f-103">List programControls</span></span>

> <span data-ttu-id="07a9f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07a9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07a9f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07a9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07a9f-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)テナント内のすべてのプログラム間ですべての[デバッギング](../resources/programcontrol.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="07a9f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="07a9f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07a9f-107">Permissions</span></span>
<span data-ttu-id="07a9f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07a9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a9f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07a9f-110">Permission type</span></span>                        | <span data-ttu-id="07a9f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07a9f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a9f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07a9f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="07a9f-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="07a9f-113"></span></span>  <span data-ttu-id="07a9f-114">サインインしているユーザーは、プログラムを読むことを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="07a9f-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="07a9f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07a9f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a9f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07a9f-116">Not supported.</span></span> |
|<span data-ttu-id="07a9f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07a9f-117">Application</span></span>                            | <span data-ttu-id="07a9f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07a9f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07a9f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07a9f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="07a9f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07a9f-120">Request headers</span></span>
| <span data-ttu-id="07a9f-121">名前</span><span class="sxs-lookup"><span data-stu-id="07a9f-121">Name</span></span>         | <span data-ttu-id="07a9f-122">種類</span><span class="sxs-lookup"><span data-stu-id="07a9f-122">Type</span></span>        | <span data-ttu-id="07a9f-123">説明</span><span class="sxs-lookup"><span data-stu-id="07a9f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="07a9f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="07a9f-124">Authorization</span></span> | <span data-ttu-id="07a9f-125">string</span><span class="sxs-lookup"><span data-stu-id="07a9f-125">string</span></span> | <span data-ttu-id="07a9f-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="07a9f-126">Bearer \{token\}.</span></span> <span data-ttu-id="07a9f-127">必須。</span><span class="sxs-lookup"><span data-stu-id="07a9f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07a9f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="07a9f-128">Request body</span></span>
<span data-ttu-id="07a9f-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="07a9f-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="07a9f-130">応答</span><span class="sxs-lookup"><span data-stu-id="07a9f-130">Response</span></span>
<span data-ttu-id="07a9f-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="07a9f-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a9f-132">例</span><span class="sxs-lookup"><span data-stu-id="07a9f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07a9f-133">要求</span><span class="sxs-lookup"><span data-stu-id="07a9f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="07a9f-134">応答</span><span class="sxs-lookup"><span data-stu-id="07a9f-134">Response</span></span>
><span data-ttu-id="07a9f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="07a9f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="07a9f-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="07a9f-137">See also</span></span>

| <span data-ttu-id="07a9f-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="07a9f-138">Method</span></span>           | <span data-ttu-id="07a9f-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="07a9f-139">Return Type</span></span>    |<span data-ttu-id="07a9f-140">説明</span><span class="sxs-lookup"><span data-stu-id="07a9f-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07a9f-141">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="07a9f-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="07a9f-142">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07a9f-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="07a9f-143">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="07a9f-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
