---
title: call://///////の役割
description: 通話中に画面共有を開始および停止します。 この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 582cd19a341e75211a457bf5ab678fb63261cace
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328044"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="f501a-104">call://///////の役割</span><span class="sxs-lookup"><span data-stu-id="f501a-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f501a-105">通話中に画面共有を開始および停止します。</span><span class="sxs-lookup"><span data-stu-id="f501a-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="f501a-106">この API は、アプリケーションが、通話または会議の参加者と画面の内容を共有できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f501a-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f501a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f501a-107">Permissions</span></span>
<span data-ttu-id="f501a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f501a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f501a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f501a-110">Permission type</span></span>                        | <span data-ttu-id="f501a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f501a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f501a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f501a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f501a-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f501a-113">Not Supported</span></span>                               |
| <span data-ttu-id="f501a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f501a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f501a-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f501a-115">Not Supported</span></span>                               |
| <span data-ttu-id="f501a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f501a-116">Application</span></span>                            | <span data-ttu-id="f501a-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f501a-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f501a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f501a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="f501a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f501a-119">Request headers</span></span>
| <span data-ttu-id="f501a-120">名前</span><span class="sxs-lookup"><span data-stu-id="f501a-120">Name</span></span>          | <span data-ttu-id="f501a-121">説明</span><span class="sxs-lookup"><span data-stu-id="f501a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f501a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f501a-122">Authorization</span></span> | <span data-ttu-id="f501a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f501a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f501a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f501a-125">Request body</span></span>
<span data-ttu-id="f501a-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f501a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f501a-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f501a-127">Parameter</span></span>      | <span data-ttu-id="f501a-128">型</span><span class="sxs-lookup"><span data-stu-id="f501a-128">Type</span></span>    |<span data-ttu-id="f501a-129">説明</span><span class="sxs-lookup"><span data-stu-id="f501a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f501a-130">role</span><span class="sxs-lookup"><span data-stu-id="f501a-130">role</span></span>|<span data-ttu-id="f501a-131">String</span><span class="sxs-lookup"><span data-stu-id="f501a-131">String</span></span>|<span data-ttu-id="f501a-132">使用可能な値は次のとおりです。 ' Viewer '、' 共有 '</span><span class="sxs-lookup"><span data-stu-id="f501a-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="f501a-133">応答</span><span class="sxs-lookup"><span data-stu-id="f501a-133">Response</span></span>
<span data-ttu-id="f501a-134">応答`202 Accepted`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f501a-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f501a-135">例</span><span class="sxs-lookup"><span data-stu-id="f501a-135">Example</span></span>
<span data-ttu-id="f501a-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f501a-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f501a-137">要求</span><span class="sxs-lookup"><span data-stu-id="f501a-137">Request</span></span>
<span data-ttu-id="f501a-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f501a-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f501a-139">応答</span><span class="sxs-lookup"><span data-stu-id="f501a-139">Response</span></span>
<span data-ttu-id="f501a-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f501a-140">Here is an example of the response.</span></span> 

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
  "suppressions": []
}
-->
