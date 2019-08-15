---
title: call://///////の役割
description: 通話中に画面共有を開始および停止します。 この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc5d6822ef42bbbb37d423ba8d7824a85d164bf6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418993"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="84774-104">call://///////の役割</span><span class="sxs-lookup"><span data-stu-id="84774-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84774-105">通話中に画面共有を開始および停止します。</span><span class="sxs-lookup"><span data-stu-id="84774-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="84774-106">この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="84774-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="84774-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84774-107">Permissions</span></span>
<span data-ttu-id="84774-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84774-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84774-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84774-110">Permission type</span></span>                        | <span data-ttu-id="84774-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84774-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84774-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84774-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="84774-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="84774-113">Not Supported</span></span>                               |
| <span data-ttu-id="84774-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84774-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84774-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="84774-115">Not Supported</span></span>                               |
| <span data-ttu-id="84774-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84774-116">Application</span></span>                            | <span data-ttu-id="84774-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="84774-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="84774-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84774-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="84774-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84774-119">Request headers</span></span>
| <span data-ttu-id="84774-120">名前</span><span class="sxs-lookup"><span data-stu-id="84774-120">Name</span></span>          | <span data-ttu-id="84774-121">説明</span><span class="sxs-lookup"><span data-stu-id="84774-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="84774-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84774-122">Authorization</span></span> | <span data-ttu-id="84774-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84774-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84774-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="84774-125">Request body</span></span>
<span data-ttu-id="84774-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="84774-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="84774-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="84774-127">Parameter</span></span>      | <span data-ttu-id="84774-128">型</span><span class="sxs-lookup"><span data-stu-id="84774-128">Type</span></span>    |<span data-ttu-id="84774-129">説明</span><span class="sxs-lookup"><span data-stu-id="84774-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84774-130">role</span><span class="sxs-lookup"><span data-stu-id="84774-130">role</span></span>|<span data-ttu-id="84774-131">String</span><span class="sxs-lookup"><span data-stu-id="84774-131">String</span></span>|<span data-ttu-id="84774-132">使用可能な値は次のとおりです。 ' Viewer '、' 共有 '</span><span class="sxs-lookup"><span data-stu-id="84774-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="84774-133">応答</span><span class="sxs-lookup"><span data-stu-id="84774-133">Response</span></span>
<span data-ttu-id="84774-134">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="84774-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84774-135">例</span><span class="sxs-lookup"><span data-stu-id="84774-135">Example</span></span>
<span data-ttu-id="84774-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="84774-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="84774-137">要求</span><span class="sxs-lookup"><span data-stu-id="84774-137">Request</span></span>
<span data-ttu-id="84774-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="84774-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="84774-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="84774-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84774-140">C#</span><span class="sxs-lookup"><span data-stu-id="84774-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84774-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84774-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84774-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="84774-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="84774-143">応答</span><span class="sxs-lookup"><span data-stu-id="84774-143">Response</span></span>
<span data-ttu-id="84774-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="84774-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
