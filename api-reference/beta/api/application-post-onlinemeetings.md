---
title: オンライン会議を作成します。
description: 要求の本文で指定されたユーザーの代わりにオンライン会議を作成します。
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: bd16b6979eed2c7d9386313f2ca07cb9ea2c5c6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838949"
---
# <a name="create-online-meeting"></a><span data-ttu-id="57372-103">オンライン会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="57372-103">Create online meeting</span></span>

> <span data-ttu-id="57372-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57372-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57372-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57372-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57372-106">要求の本文で指定されたユーザーの代わりにオンライン会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="57372-106">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="57372-107">**注**: ユーザーの予定表に会議が表示されません。</span><span class="sxs-lookup"><span data-stu-id="57372-107">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="57372-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57372-108">Permissions</span></span>
<span data-ttu-id="57372-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57372-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57372-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57372-111">Permission type</span></span>                        | <span data-ttu-id="57372-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="57372-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57372-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57372-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="57372-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="57372-114">Not Supported</span></span>                               |
| <span data-ttu-id="57372-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57372-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57372-116">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="57372-116">Not Supported</span></span>                               |
| <span data-ttu-id="57372-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57372-117">Application</span></span>                            | <span data-ttu-id="57372-118">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57372-118">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="57372-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57372-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="57372-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57372-120">Request headers</span></span>
| <span data-ttu-id="57372-121">名前</span><span class="sxs-lookup"><span data-stu-id="57372-121">Name</span></span>          | <span data-ttu-id="57372-122">説明</span><span class="sxs-lookup"><span data-stu-id="57372-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="57372-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57372-123">Authorization</span></span> | <span data-ttu-id="57372-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="57372-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57372-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="57372-126">Request body</span></span>
<span data-ttu-id="57372-127">要求の本文には、 [onlineMeeting](../resources/onlinemeeting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="57372-127">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57372-128">応答</span><span class="sxs-lookup"><span data-stu-id="57372-128">Response</span></span>
<span data-ttu-id="57372-129">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文内の[onlineMeeting](../resources/onlinemeeting.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="57372-129">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57372-130">例</span><span class="sxs-lookup"><span data-stu-id="57372-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57372-131">要求</span><span class="sxs-lookup"><span data-stu-id="57372-131">Request</span></span>
<span data-ttu-id="57372-132">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="57372-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

<span data-ttu-id="57372-133">要求の本文には、 [onlineMeeting](../resources/onlinemeeting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="57372-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="57372-134">応答</span><span class="sxs-lookup"><span data-stu-id="57372-134">Response</span></span>

><span data-ttu-id="57372-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="57372-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1574

{
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
