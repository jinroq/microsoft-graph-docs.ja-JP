---
title: Get オンライン会議
description: プロパティと**onlineMeeting**オブジェクトの関係を取得します。
author: VinodRavichandran
ms.openlocfilehash: bfae4273aba0583e6c10a7e10f9c67865326bacf
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380381"
---
# <a name="get-online-meeting"></a><span data-ttu-id="a6aab-103">Get オンライン会議</span><span class="sxs-lookup"><span data-stu-id="a6aab-103">Get Online Meeting</span></span>

> <span data-ttu-id="a6aab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6aab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6aab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6aab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6aab-106">プロパティと**onlineMeeting**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6aab-106">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="a6aab-107">**注:**`GET`メソッドは、 [VTC 会議 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)に制限します。雲-ビデオの相互運用機能のライセンス取得ユーザーと、このメソッドを使用して、ミーティングに参加する詳細を取得するには、これらの Id が生成されます。</span><span class="sxs-lookup"><span data-stu-id="a6aab-107">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="a6aab-108">通常のフローでは、bot を使用できます、`joinURL`参照がないと、会議に参加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6aab-108">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6aab-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6aab-109">Permissions</span></span>

<span data-ttu-id="a6aab-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6aab-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6aab-112">Permission type</span></span>                        | <span data-ttu-id="a6aab-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6aab-113">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="a6aab-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6aab-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6aab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6aab-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="a6aab-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6aab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6aab-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6aab-117">Not Supported.</span></span>                                        |
| <span data-ttu-id="a6aab-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6aab-118">Application</span></span>                            | <span data-ttu-id="a6aab-119">OnlineMeetings.Read.All、OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6aab-119">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6aab-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6aab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6aab-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6aab-121">Optional query parameters</span></span>
<span data-ttu-id="a6aab-122">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a6aab-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6aab-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6aab-123">Request headers</span></span>
| <span data-ttu-id="a6aab-124">名前</span><span class="sxs-lookup"><span data-stu-id="a6aab-124">Name</span></span>          | <span data-ttu-id="a6aab-125">説明</span><span class="sxs-lookup"><span data-stu-id="a6aab-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a6aab-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6aab-126">Authorization</span></span> | <span data-ttu-id="a6aab-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6aab-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6aab-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6aab-129">Request body</span></span>
<span data-ttu-id="a6aab-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a6aab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6aab-131">応答</span><span class="sxs-lookup"><span data-stu-id="a6aab-131">Response</span></span>
<span data-ttu-id="a6aab-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[onlineMeeting](../resources/onlinemeeting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6aab-132">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6aab-133">例</span><span class="sxs-lookup"><span data-stu-id="a6aab-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6aab-134">要求</span><span class="sxs-lookup"><span data-stu-id="a6aab-134">Request</span></span>
<span data-ttu-id="a6aab-135">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6aab-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="a6aab-136">応答</span><span class="sxs-lookup"><span data-stu-id="a6aab-136">Response</span></span>

> <span data-ttu-id="a6aab-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6aab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
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
  "meetingType": "scheduled",
  "participants": {
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "upn": "upn-value"
      }
    ],
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
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
