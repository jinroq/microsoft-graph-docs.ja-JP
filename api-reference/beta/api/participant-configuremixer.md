---
title: '参加者: configureMixer'
description: マルチパーティの会話で、さまざまな参加者に対して音声を混在させる方法を構成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc3bb039fa005d83738d8fd0a762a465c092048b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992466"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="98318-103">参加者: configureMixer</span><span class="sxs-lookup"><span data-stu-id="98318-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98318-104">マルチパーティの会話で、さまざまな参加者に対して音声を混在させる方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="98318-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="98318-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98318-105">Permissions</span></span>
<span data-ttu-id="98318-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98318-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98318-108">Permission type</span></span> | <span data-ttu-id="98318-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98318-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="98318-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98318-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98318-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="98318-111">Not Supported</span></span>        |
| <span data-ttu-id="98318-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98318-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98318-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="98318-113">Not Supported</span></span>        |
| <span data-ttu-id="98318-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98318-114">Application</span></span>     | <span data-ttu-id="98318-115">JoinGroupCalls を呼び出します。すべて、InitiateGroupCalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="98318-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98318-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98318-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="98318-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98318-117">Request headers</span></span>
| <span data-ttu-id="98318-118">名前</span><span class="sxs-lookup"><span data-stu-id="98318-118">Name</span></span>          | <span data-ttu-id="98318-119">説明</span><span class="sxs-lookup"><span data-stu-id="98318-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="98318-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98318-120">Authorization</span></span> | <span data-ttu-id="98318-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98318-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98318-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="98318-123">Request body</span></span>
<span data-ttu-id="98318-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="98318-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98318-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="98318-125">Parameter</span></span>      | <span data-ttu-id="98318-126">型</span><span class="sxs-lookup"><span data-stu-id="98318-126">Type</span></span>    |<span data-ttu-id="98318-127">説明</span><span class="sxs-lookup"><span data-stu-id="98318-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98318-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="98318-128">participantMixerLevels</span></span>|<span data-ttu-id="98318-129">[participantMixerLevel](../resources/participantmixerlevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98318-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="98318-130">特定の音声参加者のミキサーレベルの構成。</span><span class="sxs-lookup"><span data-stu-id="98318-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="98318-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="98318-131">clientContext</span></span>|<span data-ttu-id="98318-132">String</span><span class="sxs-lookup"><span data-stu-id="98318-132">String</span></span>|<span data-ttu-id="98318-133">クライアントコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="98318-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="98318-134">応答</span><span class="sxs-lookup"><span data-stu-id="98318-134">Response</span></span>
<span data-ttu-id="98318-135">この`202 Accepted`要求に対して作成された[commsOperation](../resources/commsoperation.md)への uri を持つ応答コードと位置ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="98318-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="98318-136">例</span><span class="sxs-lookup"><span data-stu-id="98318-136">Example</span></span>
<span data-ttu-id="98318-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98318-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="98318-138">要求</span><span class="sxs-lookup"><span data-stu-id="98318-138">Request</span></span>
<span data-ttu-id="98318-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="98318-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="98318-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="98318-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="98318-141">C#</span><span class="sxs-lookup"><span data-stu-id="98318-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98318-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="98318-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98318-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="98318-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98318-144">Java</span><span class="sxs-lookup"><span data-stu-id="98318-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-configuremixer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98318-145">応答</span><span class="sxs-lookup"><span data-stu-id="98318-145">Response</span></span>

> <span data-ttu-id="98318-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98318-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="98318-148">通知-操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="98318-148">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
