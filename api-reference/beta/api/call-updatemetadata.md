---
title: '電話: updateMetadata'
description: 呼び出しに関連付けられているアプリケーションのメタデータを更新します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 19e56c3ac00aa0b61efef6be3a25020166e364d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976479"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="8569c-103">電話: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="8569c-103">call: updateMetadata</span></span>

> <span data-ttu-id="8569c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8569c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8569c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8569c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8569c-106">呼び出しに関連付けられているアプリケーションのメタデータを更新します。</span><span class="sxs-lookup"><span data-stu-id="8569c-106">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8569c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8569c-107">Permissions</span></span>
<span data-ttu-id="8569c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8569c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8569c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8569c-110">Permission type</span></span>                        | <span data-ttu-id="8569c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8569c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8569c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8569c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8569c-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="8569c-113">Not Supported</span></span>                               |
| <span data-ttu-id="8569c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8569c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8569c-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="8569c-115">Not Supported</span></span>                               |
| <span data-ttu-id="8569c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8569c-116">Application</span></span>     | <span data-ttu-id="8569c-117">Calls.JoinGroupCallsasGuest.All、Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="8569c-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8569c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8569c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="8569c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8569c-119">Request headers</span></span>
| <span data-ttu-id="8569c-120">名前</span><span class="sxs-lookup"><span data-stu-id="8569c-120">Name</span></span>          | <span data-ttu-id="8569c-121">説明</span><span class="sxs-lookup"><span data-stu-id="8569c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8569c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8569c-122">Authorization</span></span> | <span data-ttu-id="8569c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8569c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8569c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8569c-125">Request body</span></span>
<span data-ttu-id="8569c-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8569c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8569c-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8569c-127">Parameter</span></span>      | <span data-ttu-id="8569c-128">型</span><span class="sxs-lookup"><span data-stu-id="8569c-128">Type</span></span>    |<span data-ttu-id="8569c-129">説明</span><span class="sxs-lookup"><span data-stu-id="8569c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8569c-130">metadata</span><span class="sxs-lookup"><span data-stu-id="8569c-130">metadata</span></span>|<span data-ttu-id="8569c-131">String</span><span class="sxs-lookup"><span data-stu-id="8569c-131">String</span></span>|<span data-ttu-id="8569c-132">名簿にある参加者が提供するデータの blob です。</span><span class="sxs-lookup"><span data-stu-id="8569c-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="8569c-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="8569c-133">clientContext</span></span>|<span data-ttu-id="8569c-134">String</span><span class="sxs-lookup"><span data-stu-id="8569c-134">String</span></span>|<span data-ttu-id="8569c-135">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="8569c-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8569c-136">応答</span><span class="sxs-lookup"><span data-stu-id="8569c-136">Response</span></span>
<span data-ttu-id="8569c-137">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="8569c-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8569c-138">例</span><span class="sxs-lookup"><span data-stu-id="8569c-138">Example</span></span>
<span data-ttu-id="8569c-139">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8569c-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8569c-140">要求</span><span class="sxs-lookup"><span data-stu-id="8569c-140">Request</span></span>
<span data-ttu-id="8569c-141">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8569c-141">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8569c-142">応答</span><span class="sxs-lookup"><span data-stu-id="8569c-142">Response</span></span>

> <span data-ttu-id="8569c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8569c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
