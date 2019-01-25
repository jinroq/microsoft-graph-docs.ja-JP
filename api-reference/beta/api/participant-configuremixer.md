---
title: '参加者: configureMixer'
description: 通話の参加者に別のオーディオを混合する方法を構成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0be23ec4c9e7835c919328655e89880003546472
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530042"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="85118-103">参加者: configureMixer</span><span class="sxs-lookup"><span data-stu-id="85118-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85118-104">通話の参加者に別のオーディオを混合する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="85118-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="85118-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85118-105">Permissions</span></span>
<span data-ttu-id="85118-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85118-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85118-108">Permission type</span></span> | <span data-ttu-id="85118-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85118-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="85118-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85118-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85118-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="85118-111">Not Supported</span></span>        |
| <span data-ttu-id="85118-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85118-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85118-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="85118-113">Not Supported</span></span>        |
| <span data-ttu-id="85118-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85118-114">Application</span></span>     | <span data-ttu-id="85118-115">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="85118-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85118-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85118-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="85118-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85118-117">Request headers</span></span>
| <span data-ttu-id="85118-118">名前</span><span class="sxs-lookup"><span data-stu-id="85118-118">Name</span></span>          | <span data-ttu-id="85118-119">説明</span><span class="sxs-lookup"><span data-stu-id="85118-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="85118-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="85118-120">Authorization</span></span> | <span data-ttu-id="85118-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85118-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85118-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="85118-123">Request body</span></span>
<span data-ttu-id="85118-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="85118-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85118-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="85118-125">Parameter</span></span>      | <span data-ttu-id="85118-126">型</span><span class="sxs-lookup"><span data-stu-id="85118-126">Type</span></span>    |<span data-ttu-id="85118-127">説明</span><span class="sxs-lookup"><span data-stu-id="85118-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85118-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="85118-128">participantMixerLevels</span></span>|<span data-ttu-id="85118-129">[participantMixerLevel](../resources/participantmixerlevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85118-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="85118-130">ミキサーの設定は、オーディオの参加者が指定されているのをレベルです。</span><span class="sxs-lookup"><span data-stu-id="85118-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="85118-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="85118-131">clientContext</span></span>|<span data-ttu-id="85118-132">String</span><span class="sxs-lookup"><span data-stu-id="85118-132">String</span></span>|<span data-ttu-id="85118-133">クライアントのコンテキスト。</span><span class="sxs-lookup"><span data-stu-id="85118-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="85118-134">応答</span><span class="sxs-lookup"><span data-stu-id="85118-134">Response</span></span>
<span data-ttu-id="85118-135">返します。`202 Accepted`応答コードと、Location ヘッダーをこの要求用に作成された[commsOperation](../resources/commsoperation.md)の uri を持つ。</span><span class="sxs-lookup"><span data-stu-id="85118-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="85118-136">例</span><span class="sxs-lookup"><span data-stu-id="85118-136">Example</span></span>
<span data-ttu-id="85118-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="85118-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="85118-138">要求</span><span class="sxs-lookup"><span data-stu-id="85118-138">Request</span></span>
<span data-ttu-id="85118-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="85118-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="85118-140">応答</span><span class="sxs-lookup"><span data-stu-id="85118-140">Response</span></span>

> <span data-ttu-id="85118-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="85118-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="85118-143">通知の操作が完了しました</span><span class="sxs-lookup"><span data-stu-id="85118-143">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
