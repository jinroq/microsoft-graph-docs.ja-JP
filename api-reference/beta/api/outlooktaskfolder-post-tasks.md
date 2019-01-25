---
title: OutlookTask を作成します。
description: 指定されたタスクのフォルダーに Outlook のタスクを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8ba293d83e2a202a45cfebf4c318ee73d808e1e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510597"
---
# <a name="create-outlooktask"></a><span data-ttu-id="8e07c-103">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e07c-104">指定されたタスクのフォルダーに Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-104">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="8e07c-105">POST メソッドは常に**させる**と、要求の本文では、 **dueDateTime**の時刻部分を無視し、指定されたタイム ゾーンで午前 0 時を常に時間を想定しています。</span><span class="sxs-lookup"><span data-stu-id="8e07c-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e07c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e07c-106">Permissions</span></span>
<span data-ttu-id="8e07c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e07c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e07c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e07c-109">Permission type</span></span>      | <span data-ttu-id="8e07c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e07c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e07c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e07c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e07c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e07c-112">Not supported.</span></span>    |
|<span data-ttu-id="8e07c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e07c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e07c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e07c-114">Not supported.</span></span>    |
|<span data-ttu-id="8e07c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e07c-115">Application</span></span> | <span data-ttu-id="8e07c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e07c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e07c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e07c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="8e07c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e07c-118">Request headers</span></span>
| <span data-ttu-id="8e07c-119">名前</span><span class="sxs-lookup"><span data-stu-id="8e07c-119">Name</span></span>       | <span data-ttu-id="8e07c-120">説明</span><span class="sxs-lookup"><span data-stu-id="8e07c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e07c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e07c-121">Authorization</span></span>  | <span data-ttu-id="8e07c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e07c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e07c-124">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8e07c-124">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8e07c-125">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-125">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8e07c-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8e07c-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e07c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e07c-127">Request body</span></span>
<span data-ttu-id="8e07c-128">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-128">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e07c-129">応答</span><span class="sxs-lookup"><span data-stu-id="8e07c-129">Response</span></span>

<span data-ttu-id="8e07c-130">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTask](../resources/outlooktask.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e07c-130">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e07c-131">例</span><span class="sxs-lookup"><span data-stu-id="8e07c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e07c-132">要求</span><span class="sxs-lookup"><span data-stu-id="8e07c-132">Request</span></span>
<span data-ttu-id="8e07c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8e07c-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="8e07c-134">要求の本文には、 [outlookTask](../resources/outlooktask.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-134">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8e07c-135">応答</span><span class="sxs-lookup"><span data-stu-id="8e07c-135">Response</span></span>
<span data-ttu-id="8e07c-p104">POST メソッドは、要求本文の時間部分を無視し、時間が常に、指定されたタイム ゾーン (PST) の午前 0 時であると想定します。既定では、POST メソッドはすべての日付関連プロパティを変換し、応答ではそれらを UTC で表示します。</span><span class="sxs-lookup"><span data-stu-id="8e07c-p104">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST). Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="8e07c-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e07c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
