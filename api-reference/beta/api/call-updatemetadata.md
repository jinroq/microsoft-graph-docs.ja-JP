---
title: '通話: updateMetadata'
description: 呼び出しに関連付けられているメタデータを更新します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fa2b92118b6a1e0862044427dd73a2a0d2bf3a35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864681"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="98ce7-103">通話: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="98ce7-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ce7-104">呼び出しに関連付けられているメタデータを更新します。</span><span class="sxs-lookup"><span data-stu-id="98ce7-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="98ce7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98ce7-105">Permissions</span></span>
<span data-ttu-id="98ce7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98ce7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98ce7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98ce7-108">Permission type</span></span>                        | <span data-ttu-id="98ce7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98ce7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98ce7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98ce7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98ce7-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="98ce7-111">Not Supported</span></span>                               |
| <span data-ttu-id="98ce7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98ce7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98ce7-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="98ce7-113">Not Supported</span></span>                               |
| <span data-ttu-id="98ce7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98ce7-114">Application</span></span>     | <span data-ttu-id="98ce7-115">JoinGroupCallsasGuest が呼び出されます。すべての呼び出し、InitiateGroupCalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="98ce7-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98ce7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98ce7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="98ce7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98ce7-117">Request headers</span></span>
| <span data-ttu-id="98ce7-118">名前</span><span class="sxs-lookup"><span data-stu-id="98ce7-118">Name</span></span>          | <span data-ttu-id="98ce7-119">説明</span><span class="sxs-lookup"><span data-stu-id="98ce7-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="98ce7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98ce7-120">Authorization</span></span> | <span data-ttu-id="98ce7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98ce7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98ce7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="98ce7-123">Request body</span></span>
<span data-ttu-id="98ce7-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="98ce7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98ce7-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="98ce7-125">Parameter</span></span>      | <span data-ttu-id="98ce7-126">型</span><span class="sxs-lookup"><span data-stu-id="98ce7-126">Type</span></span>    |<span data-ttu-id="98ce7-127">説明</span><span class="sxs-lookup"><span data-stu-id="98ce7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98ce7-128">metadata</span><span class="sxs-lookup"><span data-stu-id="98ce7-128">metadata</span></span>|<span data-ttu-id="98ce7-129">String</span><span class="sxs-lookup"><span data-stu-id="98ce7-129">String</span></span>|<span data-ttu-id="98ce7-130">参加者が名簿に提供するデータの blob。</span><span class="sxs-lookup"><span data-stu-id="98ce7-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="98ce7-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="98ce7-131">clientContext</span></span>|<span data-ttu-id="98ce7-132">String</span><span class="sxs-lookup"><span data-stu-id="98ce7-132">String</span></span>|<span data-ttu-id="98ce7-133">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="98ce7-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="98ce7-134">応答</span><span class="sxs-lookup"><span data-stu-id="98ce7-134">Response</span></span>
<span data-ttu-id="98ce7-135">この`202 Accepted`要求に対して作成された[commsOperation](../resources/commsoperation.md)への uri を持つ応答コードと位置ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="98ce7-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="98ce7-136">例</span><span class="sxs-lookup"><span data-stu-id="98ce7-136">Example</span></span>
<span data-ttu-id="98ce7-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98ce7-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="98ce7-138">要求</span><span class="sxs-lookup"><span data-stu-id="98ce7-138">Request</span></span>
<span data-ttu-id="98ce7-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="98ce7-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="98ce7-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="98ce7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98ce7-141">C#</span><span class="sxs-lookup"><span data-stu-id="98ce7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98ce7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="98ce7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98ce7-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="98ce7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98ce7-144">Java</span><span class="sxs-lookup"><span data-stu-id="98ce7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updatemetadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98ce7-145">応答</span><span class="sxs-lookup"><span data-stu-id="98ce7-145">Response</span></span>

> <span data-ttu-id="98ce7-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98ce7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
