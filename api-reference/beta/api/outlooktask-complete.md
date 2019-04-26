---
title: 'outlooktask: 完了'
description: '**completedDateTime**プロパティを現在の日付に設定する Outlook のタスクを完了します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c1d1fb36f94c2948cd2430e07f35c682b0608962
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338061"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="494f1-103">outlooktask: 完了</span><span class="sxs-lookup"><span data-stu-id="494f1-103">outlookTask: complete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="494f1-104">**completedDateTime**プロパティを現在の日付に設定し、 **status**プロパティをに`completed`設定する Outlook のタスクを完了します。</span><span class="sxs-lookup"><span data-stu-id="494f1-104">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="494f1-105">一連のタスクを定期的に実行している場合、返信には、タスクのコレクションには、データ系列の完了したタスクと、一連の次のタスクが含まれます。</span><span class="sxs-lookup"><span data-stu-id="494f1-105">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="494f1-106">**completedDateTime**プロパティは、タスクが終了した日付を表します。</span><span class="sxs-lookup"><span data-stu-id="494f1-106">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="494f1-107">**completedDateTime**の時間部分は、既定で UTC の午前0時に設定されます。</span><span class="sxs-lookup"><span data-stu-id="494f1-107">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="494f1-108">既定では、この操作 (および POST、GET、および PATCH タスクの操作) は、日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="494f1-108">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="494f1-109">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="494f1-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="494f1-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="494f1-110">Permissions</span></span>

<span data-ttu-id="494f1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="494f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="494f1-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="494f1-113">Permission type</span></span>      | <span data-ttu-id="494f1-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="494f1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="494f1-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="494f1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="494f1-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="494f1-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="494f1-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="494f1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="494f1-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="494f1-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="494f1-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="494f1-119">Application</span></span> | <span data-ttu-id="494f1-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="494f1-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="494f1-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="494f1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="494f1-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="494f1-122">Request headers</span></span>

| <span data-ttu-id="494f1-123">名前</span><span class="sxs-lookup"><span data-stu-id="494f1-123">Name</span></span>       | <span data-ttu-id="494f1-124">説明</span><span class="sxs-lookup"><span data-stu-id="494f1-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="494f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="494f1-125">Authorization</span></span>  | <span data-ttu-id="494f1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="494f1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="494f1-128">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="494f1-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="494f1-129">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="494f1-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="494f1-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="494f1-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="494f1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="494f1-131">Request body</span></span>

<span data-ttu-id="494f1-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="494f1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="494f1-133">応答</span><span class="sxs-lookup"><span data-stu-id="494f1-133">Response</span></span>

<span data-ttu-id="494f1-134">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="494f1-134">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="494f1-135">例</span><span class="sxs-lookup"><span data-stu-id="494f1-135">Example</span></span>

<span data-ttu-id="494f1-136">次の例では、指定したタスクを終了に設定します。</span><span class="sxs-lookup"><span data-stu-id="494f1-136">The following example marks the specified task as complete.</span></span> <span data-ttu-id="494f1-137">`Prefer: outlook.timezone`ヘッダーに太平洋標準時 (PST) を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f1-137">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="494f1-138">要求</span><span class="sxs-lookup"><span data-stu-id="494f1-138">Request</span></span>

<span data-ttu-id="494f1-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="494f1-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="494f1-140">応答</span><span class="sxs-lookup"><span data-stu-id="494f1-140">Response</span></span>

<span data-ttu-id="494f1-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="494f1-141">Here is an example of the response.</span></span> <span data-ttu-id="494f1-142">応答内の**completedDateTime**およびその他の日付関連プロパティは、PST で表されます。</span><span class="sxs-lookup"><span data-stu-id="494f1-142">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="494f1-143">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="494f1-143">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="494f1-144">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="494f1-144">All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTIBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
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
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
