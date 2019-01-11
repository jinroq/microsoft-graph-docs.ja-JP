---
title: 呼び出しを取得します。
description: プロパティと、呼び出しオブジェクトの関係を取得します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c209c263f2dfcffe274bf726296d7e6c427afa6d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833552"
---
# <a name="get-call"></a><span data-ttu-id="bbff0-103">呼び出しを取得します。</span><span class="sxs-lookup"><span data-stu-id="bbff0-103">Get call</span></span>

> <span data-ttu-id="bbff0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bbff0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbff0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbff0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbff0-106">プロパティと、呼び出しオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="bbff0-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbff0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bbff0-107">Permissions</span></span>
<span data-ttu-id="bbff0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbff0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbff0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbff0-110">Permission type</span></span> | <span data-ttu-id="bbff0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbff0-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="bbff0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbff0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbff0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbff0-113">Not Supported.</span></span>                         |
| <span data-ttu-id="bbff0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbff0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbff0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbff0-115">Not Supported.</span></span>                         |
| <span data-ttu-id="bbff0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbff0-116">Application</span></span>                            | <span data-ttu-id="bbff0-117">なし。</span><span class="sxs-lookup"><span data-stu-id="bbff0-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="bbff0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbff0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbff0-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bbff0-119">Optional query parameters</span></span>
<span data-ttu-id="bbff0-120">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bbff0-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbff0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbff0-121">Request headers</span></span>
| <span data-ttu-id="bbff0-122">名前</span><span class="sxs-lookup"><span data-stu-id="bbff0-122">Name</span></span>          | <span data-ttu-id="bbff0-123">説明</span><span class="sxs-lookup"><span data-stu-id="bbff0-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bbff0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbff0-124">Authorization</span></span> | <span data-ttu-id="bbff0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bbff0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbff0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbff0-127">Request body</span></span>
<span data-ttu-id="bbff0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bbff0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbff0-129">応答</span><span class="sxs-lookup"><span data-stu-id="bbff0-129">Response</span></span>
<span data-ttu-id="bbff0-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと応答の本文[を呼び出す](../resources/call.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="bbff0-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbff0-131">例</span><span class="sxs-lookup"><span data-stu-id="bbff0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbff0-132">要求</span><span class="sxs-lookup"><span data-stu-id="bbff0-132">Request</span></span>
<span data-ttu-id="bbff0-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="bbff0-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="bbff0-134">応答</span><span class="sxs-lookup"><span data-stu-id="bbff0-134">Response</span></span>

> <span data-ttu-id="bbff0-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bbff0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2821

{
  "activeModalities": [
    "unknown"
  ],
  "answeredBy": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "callRoutes": [
    {
      "final": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "original": {
        "phone": {
          "id": "+14258828080"
        }
      },
      "routingType": "forwarded"
    }
  ],
  "callbackUri": "callbackUri-value",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "direction": "incoming",
  "id": "id-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "meetingCapability": {
    "allowAnonymousUsersToDialOut": true,
    "allowAnonymousUsersToStartMeeting": true,
    "autoAdmittedUsers": "everyoneInCompany"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "myParticipantId-value",
  "requestedModalities": [
    "audio", "video"
  ],
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": [
    "none"
  ],
  "source": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "state": "incoming",
  "subject": "subject-value",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    }
  ],
  "tenantId": "tenantId-value",
  "terminationReason": "terminationReason-value",
  "toneInfo": {
    "sequenceId": 99,
    "tone": "tone0"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
