---
title: '参加者: configureMixer'
description: 通話の参加者に別のオーディオを混合する方法を構成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9b1cff0cee8ffd8d5bc3d13fa27aacc419754a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969619"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="90b02-103">参加者: configureMixer</span><span class="sxs-lookup"><span data-stu-id="90b02-103">participant: configureMixer</span></span>

> <span data-ttu-id="90b02-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90b02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90b02-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90b02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90b02-106">通話の参加者に別のオーディオを混合する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="90b02-106">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="90b02-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="90b02-107">Permissions</span></span>
<span data-ttu-id="90b02-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90b02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90b02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90b02-110">Permission type</span></span> | <span data-ttu-id="90b02-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="90b02-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="90b02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90b02-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90b02-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="90b02-113">Not Supported</span></span>        |
| <span data-ttu-id="90b02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90b02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b02-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="90b02-115">Not Supported</span></span>        |
| <span data-ttu-id="90b02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90b02-116">Application</span></span>     | <span data-ttu-id="90b02-117">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="90b02-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90b02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="90b02-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90b02-119">Request headers</span></span>
| <span data-ttu-id="90b02-120">名前</span><span class="sxs-lookup"><span data-stu-id="90b02-120">Name</span></span>          | <span data-ttu-id="90b02-121">説明</span><span class="sxs-lookup"><span data-stu-id="90b02-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="90b02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90b02-122">Authorization</span></span> | <span data-ttu-id="90b02-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="90b02-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90b02-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="90b02-125">Request body</span></span>
<span data-ttu-id="90b02-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="90b02-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90b02-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="90b02-127">Parameter</span></span>      | <span data-ttu-id="90b02-128">型</span><span class="sxs-lookup"><span data-stu-id="90b02-128">Type</span></span>    |<span data-ttu-id="90b02-129">説明</span><span class="sxs-lookup"><span data-stu-id="90b02-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90b02-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="90b02-130">participantMixerLevels</span></span>|<span data-ttu-id="90b02-131">[participantMixerLevel](../resources/participantmixerlevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90b02-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="90b02-132">ミキサーの設定は、オーディオの参加者が指定されているのをレベルです。</span><span class="sxs-lookup"><span data-stu-id="90b02-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="90b02-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="90b02-133">clientContext</span></span>|<span data-ttu-id="90b02-134">String</span><span class="sxs-lookup"><span data-stu-id="90b02-134">String</span></span>|<span data-ttu-id="90b02-135">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="90b02-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="90b02-136">応答</span><span class="sxs-lookup"><span data-stu-id="90b02-136">Response</span></span>
<span data-ttu-id="90b02-137">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="90b02-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="90b02-138">例</span><span class="sxs-lookup"><span data-stu-id="90b02-138">Example</span></span>
<span data-ttu-id="90b02-139">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="90b02-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="90b02-140">要求</span><span class="sxs-lookup"><span data-stu-id="90b02-140">Request</span></span>
<span data-ttu-id="90b02-141">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="90b02-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="90b02-142">応答</span><span class="sxs-lookup"><span data-stu-id="90b02-142">Response</span></span>

> <span data-ttu-id="90b02-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="90b02-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="90b02-145">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="90b02-145">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
