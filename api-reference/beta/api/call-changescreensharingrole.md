---
title: '電話: changeScreenSharingRole'
description: 起動し、画面の呼び出しでの共有を停止します。 この API を使用して、通話や会議の参加者と画面の内容を共有するアプリケーションを許可します。
ms.openlocfilehash: f0aa69b43813bd248048ad1bd965dfbc4afc012b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069881"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="f98ff-104">電話: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="f98ff-104">call: changeScreenSharingRole</span></span>

> <span data-ttu-id="f98ff-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f98ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f98ff-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f98ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f98ff-107">起動し、画面の呼び出しでの共有を停止します。</span><span class="sxs-lookup"><span data-stu-id="f98ff-107">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="f98ff-108">この API を使用して、通話や会議の参加者と画面の内容を共有するアプリケーションを許可します。</span><span class="sxs-lookup"><span data-stu-id="f98ff-108">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f98ff-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f98ff-109">Permissions</span></span>
<span data-ttu-id="f98ff-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f98ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f98ff-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f98ff-112">Permission type</span></span>                        | <span data-ttu-id="f98ff-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f98ff-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f98ff-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f98ff-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f98ff-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f98ff-115">Not Supported</span></span>                               |
| <span data-ttu-id="f98ff-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f98ff-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f98ff-117">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f98ff-117">Not Supported</span></span>                               |
| <span data-ttu-id="f98ff-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f98ff-118">Application</span></span>                            | <span data-ttu-id="f98ff-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f98ff-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f98ff-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f98ff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="f98ff-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f98ff-121">Request headers</span></span>
| <span data-ttu-id="f98ff-122">名前</span><span class="sxs-lookup"><span data-stu-id="f98ff-122">Name</span></span>          | <span data-ttu-id="f98ff-123">説明</span><span class="sxs-lookup"><span data-stu-id="f98ff-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f98ff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f98ff-124">Authorization</span></span> | <span data-ttu-id="f98ff-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f98ff-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f98ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f98ff-127">Request body</span></span>
<span data-ttu-id="f98ff-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f98ff-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f98ff-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f98ff-129">Parameter</span></span>      | <span data-ttu-id="f98ff-130">型</span><span class="sxs-lookup"><span data-stu-id="f98ff-130">Type</span></span>    |<span data-ttu-id="f98ff-131">説明</span><span class="sxs-lookup"><span data-stu-id="f98ff-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f98ff-132">role</span><span class="sxs-lookup"><span data-stu-id="f98ff-132">role</span></span>|<span data-ttu-id="f98ff-133">String</span><span class="sxs-lookup"><span data-stu-id="f98ff-133">String</span></span>|<span data-ttu-id="f98ff-134">使用可能な値: 'ビューアー'、'共有'</span><span class="sxs-lookup"><span data-stu-id="f98ff-134">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="f98ff-135">応答</span><span class="sxs-lookup"><span data-stu-id="f98ff-135">Response</span></span>
<span data-ttu-id="f98ff-136">返します。`202 Accepted`応答コード。</span><span class="sxs-lookup"><span data-stu-id="f98ff-136">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f98ff-137">例</span><span class="sxs-lookup"><span data-stu-id="f98ff-137">Example</span></span>
<span data-ttu-id="f98ff-138">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f98ff-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f98ff-139">要求</span><span class="sxs-lookup"><span data-stu-id="f98ff-139">Request</span></span>
<span data-ttu-id="f98ff-140">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f98ff-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="f98ff-141">応答</span><span class="sxs-lookup"><span data-stu-id="f98ff-141">Response</span></span>
<span data-ttu-id="f98ff-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f98ff-142">Here is an example of the response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->