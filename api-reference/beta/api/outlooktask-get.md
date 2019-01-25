---
title: OutlookTask を取得します。
description: ユーザーのメールボックスのプロパティと、Outlook のタスクの関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 47c6a24ccb76eb7752736386cf6ec17330832780
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526320"
---
# <a name="get-outlooktask"></a><span data-ttu-id="bd28e-103">OutlookTask を取得します。</span><span class="sxs-lookup"><span data-stu-id="bd28e-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd28e-104">ユーザーのメールボックスのプロパティと、Outlook のタスクの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="bd28e-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="bd28e-105">既定では、この操作 (および投稿、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="bd28e-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="bd28e-106">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="bd28e-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd28e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd28e-107">Permissions</span></span>

<span data-ttu-id="bd28e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd28e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd28e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd28e-110">Permission type</span></span>      | <span data-ttu-id="bd28e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd28e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd28e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd28e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bd28e-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bd28e-113">Tasks.Read</span></span>    |
|<span data-ttu-id="bd28e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd28e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd28e-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bd28e-115">Tasks.Read</span></span>    |
|<span data-ttu-id="bd28e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd28e-116">Application</span></span> | <span data-ttu-id="bd28e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd28e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd28e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd28e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd28e-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bd28e-119">Optional query parameters</span></span>

<span data-ttu-id="bd28e-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bd28e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd28e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd28e-121">Request headers</span></span>

| <span data-ttu-id="bd28e-122">名前</span><span class="sxs-lookup"><span data-stu-id="bd28e-122">Name</span></span>      |<span data-ttu-id="bd28e-123">説明</span><span class="sxs-lookup"><span data-stu-id="bd28e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd28e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd28e-124">Authorization</span></span>  | <span data-ttu-id="bd28e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bd28e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd28e-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bd28e-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="bd28e-128">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="bd28e-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="bd28e-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bd28e-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd28e-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd28e-130">Request body</span></span>

<span data-ttu-id="bd28e-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bd28e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd28e-132">応答</span><span class="sxs-lookup"><span data-stu-id="bd28e-132">Response</span></span>

<span data-ttu-id="bd28e-133">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bd28e-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="bd28e-134">例 1</span><span class="sxs-lookup"><span data-stu-id="bd28e-134">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="bd28e-135">要求</span><span class="sxs-lookup"><span data-stu-id="bd28e-135">Request</span></span>

<span data-ttu-id="bd28e-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd28e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="bd28e-137">応答</span><span class="sxs-lookup"><span data-stu-id="bd28e-137">Response</span></span>

<span data-ttu-id="bd28e-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bd28e-138">Here is an example of the response.</span></span> <span data-ttu-id="bd28e-139">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="bd28e-139">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="bd28e-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd28e-p106">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-2"></a><span data-ttu-id="bd28e-142">例 2</span><span class="sxs-lookup"><span data-stu-id="bd28e-142">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="bd28e-143">要求</span><span class="sxs-lookup"><span data-stu-id="bd28e-143">Request</span></span>

<span data-ttu-id="bd28e-144">この例では、`Prefer: outlook.timezone`太平洋標準時の応答で日付と時刻のプロパティを表示するかを指定するヘッダー。</span><span class="sxs-lookup"><span data-stu-id="bd28e-144">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="bd28e-145">応答</span><span class="sxs-lookup"><span data-stu-id="bd28e-145">Response</span></span>

<span data-ttu-id="bd28e-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bd28e-146">Here is an example of the response.</span></span> <span data-ttu-id="bd28e-147">指定の太平洋標準時では、応答内の日付と時刻のプロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bd28e-147">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="bd28e-p108">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd28e-p108">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
