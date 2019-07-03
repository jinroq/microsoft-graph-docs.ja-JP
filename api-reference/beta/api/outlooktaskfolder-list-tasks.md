---
title: List tasks
description: 指定したフォルダー内のすべての Outlook タスクを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2e417489f41619843c5fc107fd13acd3eb38a469
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447244"
---
# <a name="list-tasks"></a><span data-ttu-id="73123-103">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="73123-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73123-104">指定したフォルダー内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="73123-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="73123-105">既定では、この操作 (および POST、PATCH、および[完了](../api/outlooktask-complete.md)タスク操作) は、日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="73123-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="73123-106">`Prefer: outlook.timezone`要求ヘッダーを使用すると、応答内のすべての日付関連プロパティを UTC 以外のタイムゾーンで表されたものにすることができます。</span><span class="sxs-lookup"><span data-stu-id="73123-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="73123-107">1つのタスクを取得する[例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73123-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="73123-108">同じようにヘッダーを適用して、複数のタスクを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="73123-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="73123-109">複数のタスクグループがあり、特定のタスクグループ内のすべてのタスクを取得する場合は、最初に[そのタスクグループ内のすべてのタスクフォルダーを取得](outlooktaskgroup-list-taskfolders.md)し、次に各タスクフォルダー内のタスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="73123-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="73123-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73123-110">Permissions</span></span>
<span data-ttu-id="73123-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73123-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73123-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73123-113">Permission type</span></span>      | <span data-ttu-id="73123-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73123-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73123-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73123-115">Delegated (work or school account)</span></span> | <span data-ttu-id="73123-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="73123-116">Tasks.Read</span></span>    |
|<span data-ttu-id="73123-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73123-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73123-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="73123-118">Tasks.Read</span></span>    |
|<span data-ttu-id="73123-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73123-119">Application</span></span> | <span data-ttu-id="73123-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73123-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73123-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73123-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73123-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73123-122">Optional query parameters</span></span>
<span data-ttu-id="73123-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73123-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73123-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73123-124">Request headers</span></span>
| <span data-ttu-id="73123-125">名前</span><span class="sxs-lookup"><span data-stu-id="73123-125">Name</span></span>      |<span data-ttu-id="73123-126">説明</span><span class="sxs-lookup"><span data-stu-id="73123-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73123-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="73123-127">Authorization</span></span>  | <span data-ttu-id="73123-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73123-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73123-130">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="73123-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="73123-131">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="73123-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="73123-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="73123-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73123-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="73123-133">Request body</span></span>
<span data-ttu-id="73123-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73123-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73123-135">応答</span><span class="sxs-lookup"><span data-stu-id="73123-135">Response</span></span>

<span data-ttu-id="73123-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="73123-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73123-137">例</span><span class="sxs-lookup"><span data-stu-id="73123-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73123-138">要求</span><span class="sxs-lookup"><span data-stu-id="73123-138">Request</span></span>
<span data-ttu-id="73123-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73123-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73123-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="73123-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73123-141">C#</span><span class="sxs-lookup"><span data-stu-id="73123-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73123-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="73123-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73123-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="73123-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73123-144">応答</span><span class="sxs-lookup"><span data-stu-id="73123-144">Response</span></span>
<span data-ttu-id="73123-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73123-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
