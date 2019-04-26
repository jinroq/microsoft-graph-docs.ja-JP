---
title: '参加者: muteall'
description: 通話ですべての参加者をミュートします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ae154e0a9e211620d9761c9051e73d5b35ec020
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332765"
---
# <a name="participant-muteall"></a><span data-ttu-id="e3ae0-103">参加者: muteall</span><span class="sxs-lookup"><span data-stu-id="e3ae0-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3ae0-104">通話ですべての参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ae0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3ae0-105">Permissions</span></span>
<span data-ttu-id="e3ae0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3ae0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3ae0-108">Permission type</span></span>                        | <span data-ttu-id="e3ae0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3ae0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3ae0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3ae0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3ae0-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="e3ae0-111">Not Supported</span></span>                               |
| <span data-ttu-id="e3ae0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3ae0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ae0-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="e3ae0-113">Not Supported</span></span>                               |
| <span data-ttu-id="e3ae0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3ae0-114">Application</span></span>                            | <span data-ttu-id="e3ae0-115">なし</span><span class="sxs-lookup"><span data-stu-id="e3ae0-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e3ae0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3ae0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="e3ae0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3ae0-117">Request headers</span></span>
| <span data-ttu-id="e3ae0-118">名前</span><span class="sxs-lookup"><span data-stu-id="e3ae0-118">Name</span></span>          | <span data-ttu-id="e3ae0-119">説明</span><span class="sxs-lookup"><span data-stu-id="e3ae0-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e3ae0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3ae0-120">Authorization</span></span> | <span data-ttu-id="e3ae0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3ae0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3ae0-123">Request body</span></span>
<span data-ttu-id="e3ae0-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3ae0-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3ae0-125">Parameter</span></span>      | <span data-ttu-id="e3ae0-126">型</span><span class="sxs-lookup"><span data-stu-id="e3ae0-126">Type</span></span>    |<span data-ttu-id="e3ae0-127">説明</span><span class="sxs-lookup"><span data-stu-id="e3ae0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ae0-128">参加者</span><span class="sxs-lookup"><span data-stu-id="e3ae0-128">participants</span></span>|<span data-ttu-id="e3ae0-129">String collection</span><span class="sxs-lookup"><span data-stu-id="e3ae0-129">String collection</span></span>|<span data-ttu-id="e3ae0-130">ミュートする参加者。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-130">The participants to be muted.</span></span>|
|<span data-ttu-id="e3ae0-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="e3ae0-131">clientContext</span></span>|<span data-ttu-id="e3ae0-132">String</span><span class="sxs-lookup"><span data-stu-id="e3ae0-132">String</span></span>|<span data-ttu-id="e3ae0-133">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e3ae0-134">応答</span><span class="sxs-lookup"><span data-stu-id="e3ae0-134">Response</span></span>
<span data-ttu-id="e3ae0-135">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[commsOperation](../resources/commsoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ae0-136">例</span><span class="sxs-lookup"><span data-stu-id="e3ae0-136">Example</span></span>
<span data-ttu-id="e3ae0-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e3ae0-138">要求</span><span class="sxs-lookup"><span data-stu-id="e3ae0-138">Request</span></span>
<span data-ttu-id="e3ae0-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="e3ae0-140">応答</span><span class="sxs-lookup"><span data-stu-id="e3ae0-140">Response</span></span>

> <span data-ttu-id="e3ae0-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3ae0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
