---
title: イベントの作成
description: この API を使用して、新しいイベントを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 978f156302380edc05df79ec3a53c1ab0f853f41
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889955"
---
# <a name="create-event"></a><span data-ttu-id="f0645-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="f0645-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0645-104">この API を使用して、新しい[イベント](../resources/event.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="f0645-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0645-105">権限</span><span class="sxs-lookup"><span data-stu-id="f0645-105">Permissions</span></span>
<span data-ttu-id="f0645-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0645-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0645-108">Permission type</span></span>      | <span data-ttu-id="f0645-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0645-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0645-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0645-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0645-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0645-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0645-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0645-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0645-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0645-113">Not supported.</span></span>    |
|<span data-ttu-id="f0645-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0645-114">Application</span></span> | <span data-ttu-id="f0645-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0645-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0645-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0645-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="f0645-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0645-117">Request headers</span></span>
| <span data-ttu-id="f0645-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0645-118">Header</span></span>       | <span data-ttu-id="f0645-119">値</span><span class="sxs-lookup"><span data-stu-id="f0645-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0645-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0645-120">Authorization</span></span>  | <span data-ttu-id="f0645-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0645-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0645-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0645-123">Request body</span></span>
<span data-ttu-id="f0645-124">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0645-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0645-125">応答</span><span class="sxs-lookup"><span data-stu-id="f0645-125">Response</span></span>
<span data-ttu-id="f0645-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0645-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0645-127">例</span><span class="sxs-lookup"><span data-stu-id="f0645-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f0645-128">要求</span><span class="sxs-lookup"><span data-stu-id="f0645-128">Request</span></span>
<span data-ttu-id="f0645-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0645-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="f0645-130">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0645-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="f0645-131">応答</span><span class="sxs-lookup"><span data-stu-id="f0645-131">Response</span></span>
<span data-ttu-id="f0645-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0645-132">The following is an example of the response.</span></span>
><span data-ttu-id="f0645-133">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f0645-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f0645-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f0645-134">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
