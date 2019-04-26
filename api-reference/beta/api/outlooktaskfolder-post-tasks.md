---
title: outlooktask の作成
description: 指定したタスクフォルダーに Outlook のタスクを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 050d45319f822531c951a665788f1c1669406532
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337913"
---
# <a name="create-outlooktask"></a><span data-ttu-id="94c3f-103">outlooktask の作成</span><span class="sxs-lookup"><span data-stu-id="94c3f-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c3f-104">指定したタスクフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-104">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="94c3f-105">POST メソッドは、要求本文の**startDateTime**および**dueDateTime**の時間部分を常に無視し、指定されたタイムゾーンで常に深夜になる時刻を想定します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="94c3f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94c3f-106">Permissions</span></span>
<span data-ttu-id="94c3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c3f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94c3f-109">Permission type</span></span>      | <span data-ttu-id="94c3f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94c3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94c3f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94c3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94c3f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94c3f-112">Not supported.</span></span>    |
|<span data-ttu-id="94c3f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94c3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94c3f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94c3f-114">Not supported.</span></span>    |
|<span data-ttu-id="94c3f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94c3f-115">Application</span></span> | <span data-ttu-id="94c3f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94c3f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94c3f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94c3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="94c3f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94c3f-118">Request headers</span></span>
| <span data-ttu-id="94c3f-119">名前</span><span class="sxs-lookup"><span data-stu-id="94c3f-119">Name</span></span>       | <span data-ttu-id="94c3f-120">説明</span><span class="sxs-lookup"><span data-stu-id="94c3f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94c3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94c3f-121">Authorization</span></span>  | <span data-ttu-id="94c3f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94c3f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94c3f-124">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="94c3f-124">Prefer: outlook.timezone</span></span> | <span data-ttu-id="94c3f-125">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="94c3f-125">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="94c3f-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="94c3f-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94c3f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="94c3f-127">Request body</span></span>
<span data-ttu-id="94c3f-128">要求本文で、 [outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-128">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94c3f-129">応答</span><span class="sxs-lookup"><span data-stu-id="94c3f-129">Response</span></span>

<span data-ttu-id="94c3f-130">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-130">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94c3f-131">例</span><span class="sxs-lookup"><span data-stu-id="94c3f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94c3f-132">要求</span><span class="sxs-lookup"><span data-stu-id="94c3f-132">Request</span></span>
<span data-ttu-id="94c3f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94c3f-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="94c3f-134">要求本文で、 [outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-134">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="94c3f-135">応答</span><span class="sxs-lookup"><span data-stu-id="94c3f-135">Response</span></span>
<span data-ttu-id="94c3f-p104">POST メソッドは、要求本文の時間部分を無視し、時間が常に、指定されたタイム ゾーン (PST) の午前 0 時であると想定します。既定では、POST メソッドはすべての日付関連プロパティを変換し、応答ではそれらを UTC で表示します。</span><span class="sxs-lookup"><span data-stu-id="94c3f-p104">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST). Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="94c3f-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="94c3f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
