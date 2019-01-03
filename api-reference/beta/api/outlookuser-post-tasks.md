---
title: OutlookTask を作成します。
description: デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。
ms.openlocfilehash: c9019db8e36151c70c5e3d2abe1ea4fea2e94ef0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072920"
---
# <a name="create-outlooktask"></a><span data-ttu-id="a1260-103">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="a1260-103">Create outlookTask</span></span>

> <span data-ttu-id="a1260-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1260-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1260-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1260-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1260-106">デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。</span><span class="sxs-lookup"><span data-stu-id="a1260-106">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="a1260-107">POST メソッドは常に**させる**と、要求の本文では、 **dueDateTime**の時刻部分を無視し、指定されたタイム ゾーンで午前 0 時を常に時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="a1260-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="a1260-108">既定では、この操作 (と取得、パッチ、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a1260-108">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="a1260-109">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="a1260-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1260-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1260-110">Permissions</span></span>
<span data-ttu-id="a1260-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1260-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1260-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1260-113">Permission type</span></span>      | <span data-ttu-id="a1260-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1260-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1260-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1260-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1260-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1260-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a1260-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1260-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1260-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1260-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a1260-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1260-119">Application</span></span> | <span data-ttu-id="a1260-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1260-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1260-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1260-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="a1260-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1260-122">Request headers</span></span>
| <span data-ttu-id="a1260-123">名前</span><span class="sxs-lookup"><span data-stu-id="a1260-123">Name</span></span>       | <span data-ttu-id="a1260-124">説明</span><span class="sxs-lookup"><span data-stu-id="a1260-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1260-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1260-125">Authorization</span></span>  | <span data-ttu-id="a1260-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a1260-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1260-128">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a1260-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a1260-129">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="a1260-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="a1260-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a1260-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1260-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1260-131">Request body</span></span>
<span data-ttu-id="a1260-132">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1260-132">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a1260-133">応答</span><span class="sxs-lookup"><span data-stu-id="a1260-133">Response</span></span>

<span data-ttu-id="a1260-134">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a1260-134">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1260-135">例</span><span class="sxs-lookup"><span data-stu-id="a1260-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1260-136">要求</span><span class="sxs-lookup"><span data-stu-id="a1260-136">Request</span></span>
<span data-ttu-id="a1260-137">次の例を使用して、`Prefer: outlook.timezone`ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="a1260-137">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="a1260-138">タスクを作成**させる**と**dueDateTime**東部標準時 (EST) で表されますが含まれています、`Prefer`ヘッダーの太平洋標準時 (PST) です。</span><span class="sxs-lookup"><span data-stu-id="a1260-138">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
<span data-ttu-id="a1260-139">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1260-139">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a1260-140">応答</span><span class="sxs-lookup"><span data-stu-id="a1260-140">Response</span></span>
<span data-ttu-id="a1260-141">POST メソッドでは、**示す**および要求の本文では、 **dueDateTime**の時刻部分は無視され、指定されたタイム ゾーン (EST) の午前 0 時を常に時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="a1260-141">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="a1260-142">ヘッダーでは PST が指定されているため、POST メソッドは応答内のすべての日付関連プロパティを PST で表記します。`Prefer`</span><span class="sxs-lookup"><span data-stu-id="a1260-142">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="a1260-143">具体的には、**させる**と**dueDateTime**のプロパティの POST メソッドは EST の午前 0 時を PST に変換し、PST の応答で返します。</span><span class="sxs-lookup"><span data-stu-id="a1260-143">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="a1260-p108">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1260-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
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
    "contentType": "Text",
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
  "sensitivity": "Normal",
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
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->