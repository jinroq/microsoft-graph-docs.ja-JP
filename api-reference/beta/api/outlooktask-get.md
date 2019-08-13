---
title: outlookTask を取得する
description: ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b900b29f87fabfeedf8318446d616f5ff1b862ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349918"
---
# <a name="get-outlooktask"></a><span data-ttu-id="cd888-103">outlookTask を取得する</span><span class="sxs-lookup"><span data-stu-id="cd888-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd888-104">ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd888-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="cd888-105">既定では、この操作 (および POST、PATCH、および[完了](../api/outlooktask-complete.md)タスク操作) は、日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="cd888-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="cd888-106">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="cd888-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd888-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd888-107">Permissions</span></span>

<span data-ttu-id="cd888-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd888-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd888-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd888-110">Permission type</span></span>                        | <span data-ttu-id="cd888-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd888-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="cd888-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd888-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd888-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cd888-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="cd888-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd888-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd888-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cd888-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="cd888-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd888-116">Application</span></span>                            | <span data-ttu-id="cd888-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd888-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="cd888-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd888-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd888-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cd888-119">Optional query parameters</span></span>

<span data-ttu-id="cd888-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cd888-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd888-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd888-121">Request headers</span></span>

| <span data-ttu-id="cd888-122">名前</span><span class="sxs-lookup"><span data-stu-id="cd888-122">Name</span></span>                     | <span data-ttu-id="cd888-123">説明</span><span class="sxs-lookup"><span data-stu-id="cd888-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="cd888-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd888-124">Authorization</span></span>            | <span data-ttu-id="cd888-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cd888-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="cd888-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cd888-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="cd888-128">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="cd888-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="cd888-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cd888-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd888-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd888-130">Request body</span></span>

<span data-ttu-id="cd888-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cd888-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd888-132">応答</span><span class="sxs-lookup"><span data-stu-id="cd888-132">Response</span></span>

<span data-ttu-id="cd888-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cd888-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd888-134">例</span><span class="sxs-lookup"><span data-stu-id="cd888-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="cd888-135">例 1: Outlook のタスクを取得する</span><span class="sxs-lookup"><span data-stu-id="cd888-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="cd888-136">要求</span><span class="sxs-lookup"><span data-stu-id="cd888-136">Request</span></span>

<span data-ttu-id="cd888-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd888-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cd888-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cd888-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd888-139">C#</span><span class="sxs-lookup"><span data-stu-id="cd888-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd888-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd888-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd888-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="cd888-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cd888-142">Java</span><span class="sxs-lookup"><span data-stu-id="cd888-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="cd888-143">応答</span><span class="sxs-lookup"><span data-stu-id="cd888-143">Response</span></span>

<span data-ttu-id="cd888-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cd888-144">Here is an example of the response.</span></span> <span data-ttu-id="cd888-145">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="cd888-145">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="cd888-146">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd888-146">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cd888-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cd888-147">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
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
  "hasAttachments": false,
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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="cd888-148">例 2: 太平洋標準時で日付と時刻のプロパティを使用して Outlook タスクを取得する</span><span class="sxs-lookup"><span data-stu-id="cd888-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="cd888-149">要求</span><span class="sxs-lookup"><span data-stu-id="cd888-149">Request</span></span>

<span data-ttu-id="cd888-150">この例では`Prefer: outlook.timezone` 、ヘッダーを使用して、API が太平洋標準時に応答で日付と時刻のプロパティを返すように指定します。</span><span class="sxs-lookup"><span data-stu-id="cd888-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cd888-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cd888-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd888-152">C#</span><span class="sxs-lookup"><span data-stu-id="cd888-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd888-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd888-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd888-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="cd888-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cd888-155">Java</span><span class="sxs-lookup"><span data-stu-id="cd888-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd888-156">応答</span><span class="sxs-lookup"><span data-stu-id="cd888-156">Response</span></span>

<span data-ttu-id="cd888-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cd888-157">Here is an example of the response.</span></span> <span data-ttu-id="cd888-158">応答内の日付と時刻のプロパティは、指定された太平洋標準時に返されます。</span><span class="sxs-lookup"><span data-stu-id="cd888-158">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="cd888-159">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd888-159">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cd888-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cd888-160">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
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
  "hasAttachments": false,
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
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
