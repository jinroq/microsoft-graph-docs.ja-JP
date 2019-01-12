---
title: OutlookTask を作成します。
description: 指定されたタスクのフォルダーに Outlook のタスクを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 80e1c6dda762ae46b5463fde9cff353e1d46408f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969633"
---
# <a name="create-outlooktask"></a><span data-ttu-id="8eb20-103">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-103">Create outlookTask</span></span>

> <span data-ttu-id="8eb20-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8eb20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb20-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eb20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eb20-106">指定されたタスクのフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-106">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="8eb20-107">POST メソッドは常に**させる**と、要求の本文では、 **dueDateTime**の時刻部分を無視し、指定されたタイム ゾーンで午前 0 時を常に時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="8eb20-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eb20-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8eb20-108">Permissions</span></span>
<span data-ttu-id="8eb20-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8eb20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb20-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8eb20-111">Permission type</span></span>      | <span data-ttu-id="8eb20-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8eb20-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eb20-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8eb20-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8eb20-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eb20-114">Not supported.</span></span>    |
|<span data-ttu-id="8eb20-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8eb20-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eb20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eb20-116">Not supported.</span></span>    |
|<span data-ttu-id="8eb20-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8eb20-117">Application</span></span> | <span data-ttu-id="8eb20-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eb20-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eb20-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8eb20-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="8eb20-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8eb20-120">Request headers</span></span>
| <span data-ttu-id="8eb20-121">名前</span><span class="sxs-lookup"><span data-stu-id="8eb20-121">Name</span></span>       | <span data-ttu-id="8eb20-122">説明</span><span class="sxs-lookup"><span data-stu-id="8eb20-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8eb20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eb20-123">Authorization</span></span>  | <span data-ttu-id="8eb20-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8eb20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8eb20-126">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8eb20-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8eb20-127">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8eb20-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8eb20-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb20-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8eb20-129">Request body</span></span>
<span data-ttu-id="8eb20-130">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8eb20-131">応答</span><span class="sxs-lookup"><span data-stu-id="8eb20-131">Response</span></span>

<span data-ttu-id="8eb20-132">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8eb20-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb20-133">例</span><span class="sxs-lookup"><span data-stu-id="8eb20-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8eb20-134">要求</span><span class="sxs-lookup"><span data-stu-id="8eb20-134">Request</span></span>
<span data-ttu-id="8eb20-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8eb20-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
Content-type: application/json
Content-length: 376

{
  "subject": "Shop for dinner",
  "startDateTime": {
      "dateTime": "2016-04-23T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-04-25T13:00:00",
      "timeZone": "Pacific Standard Time"
  }
}
```
<span data-ttu-id="8eb20-136">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-136">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8eb20-137">応答</span><span class="sxs-lookup"><span data-stu-id="8eb20-137">Response</span></span>
<span data-ttu-id="8eb20-p105">POST メソッドは、要求本文の時間部分を無視し、時間が常に、指定されたタイム ゾーン (PST) の午前 0 時であると想定します。既定では、POST メソッドはすべての日付関連プロパティを変換し、応答ではそれらを UTC で表示します。</span><span class="sxs-lookup"><span data-stu-id="8eb20-p105">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST). Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="8eb20-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8eb20-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 376

{
  "createdDateTime": "2016-04-22T05:44:01.2012012Z",
  "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
  "categories": [ ],
  "assignedTo": "null",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-25T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments":false,
  "importance": "Normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTkAAAAIBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-04-23T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "NotStarted",
  "subject": "Shop for dinner"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
