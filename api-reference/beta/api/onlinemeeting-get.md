---
title: オンライン会議を取得する
description: '**onlineMeeting**オブジェクトのプロパティとリレーションシップを取得します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 556482073374d0c8a9381b10128ce6d4d0ae9dec
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332989"
---
# <a name="get-online-meeting"></a><span data-ttu-id="7c988-103">オンライン会議を取得する</span><span class="sxs-lookup"><span data-stu-id="7c988-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c988-104">**onlineMeeting**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="7c988-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="7c988-105">**注:** この`GET`メソッドは、 [vtc 会議 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)に制限されています。これらの id は、クラウドビデオ相互運用ライセンスユーザーを対象として生成され、このメソッドを使用して会議に参加するための詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7c988-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="7c988-106">通常のフローでは、 `joinURL` bot はを使用して会議に参加でき、参照は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="7c988-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c988-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c988-107">Permissions</span></span>

<span data-ttu-id="7c988-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c988-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c988-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c988-110">Permission type</span></span>                        | <span data-ttu-id="7c988-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c988-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="7c988-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c988-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c988-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="7c988-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="7c988-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c988-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c988-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="7c988-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="7c988-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c988-116">Application</span></span>                            | <span data-ttu-id="7c988-117">OnlineMeetings、OnlineMeetings のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="7c988-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c988-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c988-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c988-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c988-119">Optional query parameters</span></span>
<span data-ttu-id="7c988-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7c988-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c988-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c988-121">Request headers</span></span>
| <span data-ttu-id="7c988-122">名前</span><span class="sxs-lookup"><span data-stu-id="7c988-122">Name</span></span>          | <span data-ttu-id="7c988-123">説明</span><span class="sxs-lookup"><span data-stu-id="7c988-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7c988-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c988-124">Authorization</span></span> | <span data-ttu-id="7c988-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c988-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c988-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c988-127">Request body</span></span>
<span data-ttu-id="7c988-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c988-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c988-129">応答</span><span class="sxs-lookup"><span data-stu-id="7c988-129">Response</span></span>
<span data-ttu-id="7c988-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onlineMeeting](../resources/onlinemeeting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c988-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c988-131">例</span><span class="sxs-lookup"><span data-stu-id="7c988-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c988-132">要求</span><span class="sxs-lookup"><span data-stu-id="7c988-132">Request</span></span>
<span data-ttu-id="7c988-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7c988-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="7c988-134">応答</span><span class="sxs-lookup"><span data-stu-id="7c988-134">Response</span></span>

> <span data-ttu-id="7c988-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c988-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
