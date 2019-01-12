---
title: List tasks
description: 指定したフォルダーに Outlook のすべてのタスクを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec814616447db842f4eaaa230cd6634e98859198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924518"
---
# <a name="list-tasks"></a><span data-ttu-id="dc6c5-103">List tasks</span><span class="sxs-lookup"><span data-stu-id="dc6c5-103">List tasks</span></span>

> <span data-ttu-id="dc6c5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc6c5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc6c5-106">指定したフォルダーに Outlook のすべてのタスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-106">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="dc6c5-107">既定では、この操作 (および投稿、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="dc6c5-108">使用することができます、 `Prefer: outlook.timezone` UTC 以外のタイム ゾーンで表される応答ですべての日付に関連するプロパティを持つヘッダーを要求します。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-108">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="dc6c5-109">1 つのタスクを取得する[例](outlooktask-get.md#example-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="dc6c5-110">複数のタスクを取得するには、同様にヘッダーを適用することができます。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-110">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="dc6c5-111">タスク グループが複数のグループでは特定のタスク、[タスク グループ内のすべての作業フォルダーを取得する](outlooktaskgroup-list-taskfolders.md)最初に、すべてのタスクを取得し、これらのタスク フォルダーにタスクを取得する場合。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-111">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dc6c5-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc6c5-112">Permissions</span></span>
<span data-ttu-id="dc6c5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc6c5-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc6c5-115">Permission type</span></span>      | <span data-ttu-id="dc6c5-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc6c5-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dc6c5-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dc6c5-118">Tasks.Read</span></span>    |
|<span data-ttu-id="dc6c5-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc6c5-120">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dc6c5-120">Tasks.Read</span></span>    |
|<span data-ttu-id="dc6c5-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc6c5-121">Application</span></span> | <span data-ttu-id="dc6c5-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc6c5-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc6c5-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc6c5-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dc6c5-124">Optional query parameters</span></span>
<span data-ttu-id="dc6c5-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc6c5-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc6c5-126">Request headers</span></span>
| <span data-ttu-id="dc6c5-127">名前</span><span class="sxs-lookup"><span data-stu-id="dc6c5-127">Name</span></span>      |<span data-ttu-id="dc6c5-128">説明</span><span class="sxs-lookup"><span data-stu-id="dc6c5-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc6c5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc6c5-129">Authorization</span></span>  | <span data-ttu-id="dc6c5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc6c5-132">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="dc6c5-132">Prefer: outlook.timezone</span></span> | <span data-ttu-id="dc6c5-133">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-133">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="dc6c5-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-134">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc6c5-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc6c5-135">Request body</span></span>
<span data-ttu-id="dc6c5-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc6c5-137">応答</span><span class="sxs-lookup"><span data-stu-id="dc6c5-137">Response</span></span>

<span data-ttu-id="dc6c5-138">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[outlookTask](../resources/outlooktask.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-138">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc6c5-139">例</span><span class="sxs-lookup"><span data-stu-id="dc6c5-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc6c5-140">要求</span><span class="sxs-lookup"><span data-stu-id="dc6c5-140">Request</span></span>
<span data-ttu-id="dc6c5-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="dc6c5-142">応答</span><span class="sxs-lookup"><span data-stu-id="dc6c5-142">Response</span></span>
<span data-ttu-id="dc6c5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-27T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-26T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
