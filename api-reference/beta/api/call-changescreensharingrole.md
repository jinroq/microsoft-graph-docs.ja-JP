---
title: call://///////の役割
description: 通話中に画面共有を開始および停止します。 この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 75d423e54309853d2fd6b39043a14e5bd5926daf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864854"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="bafa8-104">call://///////の役割</span><span class="sxs-lookup"><span data-stu-id="bafa8-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafa8-105">通話中に画面共有を開始および停止します。</span><span class="sxs-lookup"><span data-stu-id="bafa8-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="bafa8-106">この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bafa8-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="bafa8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bafa8-107">Permissions</span></span>
<span data-ttu-id="bafa8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bafa8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bafa8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bafa8-110">Permission type</span></span>                        | <span data-ttu-id="bafa8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bafa8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bafa8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bafa8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bafa8-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="bafa8-113">Not Supported</span></span>                               |
| <span data-ttu-id="bafa8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bafa8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bafa8-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="bafa8-115">Not Supported</span></span>                               |
| <span data-ttu-id="bafa8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bafa8-116">Application</span></span>                            | <span data-ttu-id="bafa8-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="bafa8-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="bafa8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bafa8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="bafa8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bafa8-119">Request headers</span></span>
| <span data-ttu-id="bafa8-120">名前</span><span class="sxs-lookup"><span data-stu-id="bafa8-120">Name</span></span>          | <span data-ttu-id="bafa8-121">説明</span><span class="sxs-lookup"><span data-stu-id="bafa8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bafa8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bafa8-122">Authorization</span></span> | <span data-ttu-id="bafa8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bafa8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bafa8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bafa8-125">Request body</span></span>
<span data-ttu-id="bafa8-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bafa8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bafa8-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bafa8-127">Parameter</span></span>      | <span data-ttu-id="bafa8-128">型</span><span class="sxs-lookup"><span data-stu-id="bafa8-128">Type</span></span>    |<span data-ttu-id="bafa8-129">説明</span><span class="sxs-lookup"><span data-stu-id="bafa8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bafa8-130">role</span><span class="sxs-lookup"><span data-stu-id="bafa8-130">role</span></span>|<span data-ttu-id="bafa8-131">String</span><span class="sxs-lookup"><span data-stu-id="bafa8-131">String</span></span>|<span data-ttu-id="bafa8-132">使用可能な値は次のとおりです。 ' Viewer '、' 共有 '</span><span class="sxs-lookup"><span data-stu-id="bafa8-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="bafa8-133">応答</span><span class="sxs-lookup"><span data-stu-id="bafa8-133">Response</span></span>
<span data-ttu-id="bafa8-134">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bafa8-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bafa8-135">例</span><span class="sxs-lookup"><span data-stu-id="bafa8-135">Example</span></span>
<span data-ttu-id="bafa8-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bafa8-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bafa8-137">要求</span><span class="sxs-lookup"><span data-stu-id="bafa8-137">Request</span></span>
<span data-ttu-id="bafa8-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="bafa8-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bafa8-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bafa8-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bafa8-140">C#</span><span class="sxs-lookup"><span data-stu-id="bafa8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bafa8-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="bafa8-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bafa8-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="bafa8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bafa8-143">Java</span><span class="sxs-lookup"><span data-stu-id="bafa8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bafa8-144">応答</span><span class="sxs-lookup"><span data-stu-id="bafa8-144">Response</span></span>
<span data-ttu-id="bafa8-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bafa8-145">Here is an example of the response.</span></span> 

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
