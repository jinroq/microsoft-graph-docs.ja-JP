---
title: オンライン会議を作成する
description: 要求本文で指定されたユーザーのためにオンライン会議を作成します。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3387654ea1964418994d2850c48ca1cbcd50712a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322972"
---
# <a name="create-online-meeting"></a><span data-ttu-id="b0c6d-103">オンライン会議を作成する</span><span class="sxs-lookup"><span data-stu-id="b0c6d-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c6d-104">要求本文で指定されたユーザーのためにオンライン会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="b0c6d-105">**注**: ユーザーの予定表に、会議が表示されません。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c6d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0c6d-106">Permissions</span></span>
<span data-ttu-id="b0c6d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0c6d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0c6d-109">Permission type</span></span>                        | <span data-ttu-id="b0c6d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0c6d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0c6d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0c6d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0c6d-112">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b0c6d-112">Not Supported</span></span>                               |
| <span data-ttu-id="b0c6d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0c6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c6d-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b0c6d-114">Not Supported</span></span>                               |
| <span data-ttu-id="b0c6d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0c6d-115">Application</span></span>                            | <span data-ttu-id="b0c6d-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c6d-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="b0c6d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0c6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="b0c6d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0c6d-118">Request headers</span></span>
| <span data-ttu-id="b0c6d-119">名前</span><span class="sxs-lookup"><span data-stu-id="b0c6d-119">Name</span></span>          | <span data-ttu-id="b0c6d-120">説明</span><span class="sxs-lookup"><span data-stu-id="b0c6d-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b0c6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c6d-121">Authorization</span></span> | <span data-ttu-id="b0c6d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0c6d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0c6d-124">Request body</span></span>
<span data-ttu-id="b0c6d-125">要求本文で、[onlineMeeting](../resources/onlinemeeting.md) オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-125">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0c6d-126">応答</span><span class="sxs-lookup"><span data-stu-id="b0c6d-126">Response</span></span>
<span data-ttu-id="b0c6d-127">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [onlineMeeting](../resources/onlinemeeting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-127">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c6d-128">例</span><span class="sxs-lookup"><span data-stu-id="b0c6d-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0c6d-129">要求</span><span class="sxs-lookup"><span data-stu-id="b0c6d-129">Request</span></span>
<span data-ttu-id="b0c6d-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-130">The following example shows the request.</span></span>

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

<span data-ttu-id="b0c6d-131">要求本文で、[onlineMeeting](../resources/onlinemeeting.md) オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-131">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b0c6d-132">応答</span><span class="sxs-lookup"><span data-stu-id="b0c6d-132">Response</span></span>

><span data-ttu-id="b0c6d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b0c6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
