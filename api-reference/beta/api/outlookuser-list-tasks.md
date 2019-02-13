---
title: List tasks
description: ユーザーのメールボックス内のすべての Outlook タスクを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f854d5649c311531e65909c3d6b33f356cd5bac2
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967355"
---
# <a name="list-tasks"></a><span data-ttu-id="afa06-103">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="afa06-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afa06-104">ユーザーのメールボックス内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="afa06-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="afa06-105">既定では、この操作 (および投稿、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="afa06-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="afa06-106">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="afa06-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="afa06-107">1 つのタスクを取得する[例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afa06-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="afa06-108">複数のタスクを取得するには、同様にヘッダーを適用することができます。</span><span class="sxs-lookup"><span data-stu-id="afa06-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="afa06-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afa06-109">Permissions</span></span>
<span data-ttu-id="afa06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afa06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa06-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afa06-112">Permission type</span></span>      | <span data-ttu-id="afa06-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="afa06-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afa06-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afa06-114">Delegated (work or school account)</span></span> | <span data-ttu-id="afa06-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="afa06-115">Tasks.Read</span></span>    |
|<span data-ttu-id="afa06-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afa06-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afa06-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="afa06-117">Tasks.Read</span></span>    |
|<span data-ttu-id="afa06-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afa06-118">Application</span></span> | <span data-ttu-id="afa06-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa06-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afa06-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afa06-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afa06-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="afa06-121">Optional query parameters</span></span>
<span data-ttu-id="afa06-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="afa06-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afa06-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afa06-123">Request headers</span></span>
| <span data-ttu-id="afa06-124">名前</span><span class="sxs-lookup"><span data-stu-id="afa06-124">Name</span></span>      |<span data-ttu-id="afa06-125">説明</span><span class="sxs-lookup"><span data-stu-id="afa06-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afa06-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="afa06-126">Authorization</span></span>  | <span data-ttu-id="afa06-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="afa06-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afa06-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="afa06-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="afa06-130">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="afa06-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="afa06-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="afa06-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afa06-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="afa06-132">Request body</span></span>
<span data-ttu-id="afa06-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="afa06-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afa06-134">応答</span><span class="sxs-lookup"><span data-stu-id="afa06-134">Response</span></span>

<span data-ttu-id="afa06-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[outlookTask](../resources/outlooktask.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="afa06-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afa06-136">例</span><span class="sxs-lookup"><span data-stu-id="afa06-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afa06-137">要求</span><span class="sxs-lookup"><span data-stu-id="afa06-137">Request</span></span>
<span data-ttu-id="afa06-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afa06-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="afa06-139">応答</span><span class="sxs-lookup"><span data-stu-id="afa06-139">Response</span></span>
<span data-ttu-id="afa06-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="afa06-140">Here is an example of the response.</span></span> <span data-ttu-id="afa06-141">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="afa06-141">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="afa06-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afa06-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
