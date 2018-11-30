---
title: OutlookTask を取得します。
description: ユーザーのメールボックスのプロパティと、Outlook のタスクの関係を取得します。
ms.openlocfilehash: d7d985614a37f0a4a70a074f63f4182130948495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067015"
---
# <a name="get-outlooktask"></a><span data-ttu-id="dccc0-103">OutlookTask を取得します。</span><span class="sxs-lookup"><span data-stu-id="dccc0-103">Get outlookTask</span></span>

> <span data-ttu-id="dccc0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dccc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dccc0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dccc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dccc0-106">ユーザーのメールボックスのプロパティと、Outlook のタスクの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="dccc0-106">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="dccc0-107">既定では、この操作 (および投稿、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dccc0-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="dccc0-108">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="dccc0-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="dccc0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dccc0-109">Permissions</span></span>
<span data-ttu-id="dccc0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dccc0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccc0-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dccc0-112">Permission type</span></span>      | <span data-ttu-id="dccc0-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dccc0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dccc0-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dccc0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dccc0-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dccc0-115">Tasks.Read</span></span>    |
|<span data-ttu-id="dccc0-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dccc0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dccc0-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dccc0-117">Tasks.Read</span></span>    |
|<span data-ttu-id="dccc0-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dccc0-118">Application</span></span> | <span data-ttu-id="dccc0-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dccc0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dccc0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dccc0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dccc0-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dccc0-121">Optional query parameters</span></span>
<span data-ttu-id="dccc0-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dccc0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dccc0-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dccc0-123">Request headers</span></span>
| <span data-ttu-id="dccc0-124">名前</span><span class="sxs-lookup"><span data-stu-id="dccc0-124">Name</span></span>      |<span data-ttu-id="dccc0-125">説明</span><span class="sxs-lookup"><span data-stu-id="dccc0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dccc0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dccc0-126">Authorization</span></span>  | <span data-ttu-id="dccc0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dccc0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dccc0-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="dccc0-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="dccc0-130">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="dccc0-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="dccc0-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="dccc0-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dccc0-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="dccc0-132">Request body</span></span>
<span data-ttu-id="dccc0-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dccc0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dccc0-134">応答</span><span class="sxs-lookup"><span data-stu-id="dccc0-134">Response</span></span>

<span data-ttu-id="dccc0-135">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dccc0-135">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>
## <a name="example-1"></a><span data-ttu-id="dccc0-136">例 1</span><span class="sxs-lookup"><span data-stu-id="dccc0-136">Example 1</span></span>
##### <a name="request"></a><span data-ttu-id="dccc0-137">要求</span><span class="sxs-lookup"><span data-stu-id="dccc0-137">Request</span></span>
<span data-ttu-id="dccc0-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dccc0-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```
##### <a name="response"></a><span data-ttu-id="dccc0-139">応答</span><span class="sxs-lookup"><span data-stu-id="dccc0-139">Response</span></span>
<span data-ttu-id="dccc0-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dccc0-140">Here is an example of the response.</span></span> <span data-ttu-id="dccc0-141">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="dccc0-141">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="dccc0-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dccc0-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

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
```


## <a name="example-2"></a><span data-ttu-id="dccc0-144">例 2</span><span class="sxs-lookup"><span data-stu-id="dccc0-144">Example 2</span></span>
##### <a name="request"></a><span data-ttu-id="dccc0-145">要求</span><span class="sxs-lookup"><span data-stu-id="dccc0-145">Request</span></span>
<span data-ttu-id="dccc0-146">この例では、`Prefer: outlook.timezone`ヘッダーの応答で日付と時刻のプロパティを表示するかを指定するには</span><span class="sxs-lookup"><span data-stu-id="dccc0-146">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response</span></span>  
<span data-ttu-id="dccc0-147">太平洋標準時です。</span><span class="sxs-lookup"><span data-stu-id="dccc0-147">in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="dccc0-148">応答</span><span class="sxs-lookup"><span data-stu-id="dccc0-148">Response</span></span>
<span data-ttu-id="dccc0-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dccc0-149">Here is an example of the response.</span></span> <span data-ttu-id="dccc0-150">指定の太平洋標準時では、応答内の日付と時刻のプロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="dccc0-150">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span> 

<span data-ttu-id="dccc0-p109">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dccc0-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->