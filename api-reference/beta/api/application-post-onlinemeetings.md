---
title: オンライン会議を作成する
description: 要求本文で指定されたユーザーのためにオンライン会議を作成します。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 00965b2509a37be6809e89e14043943c315bd0ae
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636479"
---
# <a name="create-online-meeting"></a><span data-ttu-id="5db5f-103">オンライン会議を作成する</span><span class="sxs-lookup"><span data-stu-id="5db5f-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db5f-104">要求本文で指定されたユーザーのためにオンライン会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="5db5f-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="5db5f-105">**注**: ユーザーの予定表に、会議が表示されません。</span><span class="sxs-lookup"><span data-stu-id="5db5f-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="5db5f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5db5f-106">Permissions</span></span>
<span data-ttu-id="5db5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5db5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5db5f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5db5f-109">Permission type</span></span>                        | <span data-ttu-id="5db5f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5db5f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5db5f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5db5f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5db5f-112">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5db5f-112">Not Supported</span></span>                               |
| <span data-ttu-id="5db5f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5db5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5db5f-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="5db5f-114">Not Supported</span></span>                               |
| <span data-ttu-id="5db5f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5db5f-115">Application</span></span>                            | <span data-ttu-id="5db5f-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db5f-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="5db5f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5db5f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="5db5f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5db5f-118">Request headers</span></span>
| <span data-ttu-id="5db5f-119">名前</span><span class="sxs-lookup"><span data-stu-id="5db5f-119">Name</span></span>          | <span data-ttu-id="5db5f-120">説明</span><span class="sxs-lookup"><span data-stu-id="5db5f-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5db5f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5db5f-121">Authorization</span></span> | <span data-ttu-id="5db5f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5db5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5db5f-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="5db5f-124">Request body</span></span>
<span data-ttu-id="5db5f-125">要求本文で、[onlineMeeting](../resources/onlinemeeting.md) オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="5db5f-125">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5db5f-126">応答</span><span class="sxs-lookup"><span data-stu-id="5db5f-126">Response</span></span>
<span data-ttu-id="5db5f-127">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [onlineMeeting](../resources/onlinemeeting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5db5f-127">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db5f-128">例</span><span class="sxs-lookup"><span data-stu-id="5db5f-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5db5f-129">要求</span><span class="sxs-lookup"><span data-stu-id="5db5f-129">Request</span></span>
<span data-ttu-id="5db5f-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5db5f-130">The following example shows the request.</span></span>

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

<span data-ttu-id="5db5f-131">要求本文で、[onlineMeeting](../resources/onlinemeeting.md) オブジェクトの JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="5db5f-131">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5db5f-132">応答</span><span class="sxs-lookup"><span data-stu-id="5db5f-132">Response</span></span>

><span data-ttu-id="5db5f-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5db5f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5db5f-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5db5f-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5db5f-136">C#</span><span class="sxs-lookup"><span data-stu-id="5db5f-136">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5db5f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="5db5f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
