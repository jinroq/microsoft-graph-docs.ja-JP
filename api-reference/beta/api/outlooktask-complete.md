---
title: 'outlookTask: 完全な'
description: '現在の日付に**completedDateTime**プロパティを設定する Outlook のタスクを完了します。 '
localization_priority: Normal
ms.openlocfilehash: 6a033624a1fafbc30b200550acc466f7fdb432d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891918"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="8ed4d-103">outlookTask: 完全な</span><span class="sxs-lookup"><span data-stu-id="8ed4d-103">outlookTask: complete</span></span>

> <span data-ttu-id="8ed4d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ed4d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ed4d-106">現在の日付に**completedDateTime**プロパティと**状態**プロパティを設定する Outlook のタスクを完了`completed`。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="8ed4d-107">応答では、定期的にタスクを実行している場合、シリーズでは、完了したタスクとデータ系列の次のタスクは、タスクのコレクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="8ed4d-108">**CompletedDateTime**プロパティは、タスクが完了すると、日付を表します。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="8ed4d-109">**CompletedDateTime**の時刻部分は、UTC の午前 0 時に既定で設定されています。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="8ed4d-110">既定では、この操作 (および投稿、取得、および更新プログラムのタスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="8ed4d-111">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="8ed4d-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed4d-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ed4d-112">Permissions</span></span>

<span data-ttu-id="8ed4d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed4d-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ed4d-115">Permission type</span></span>      | <span data-ttu-id="8ed4d-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ed4d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ed4d-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ed4d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8ed4d-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ed4d-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8ed4d-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ed4d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ed4d-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ed4d-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8ed4d-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ed4d-121">Application</span></span> | <span data-ttu-id="8ed4d-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ed4d-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ed4d-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="8ed4d-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ed4d-124">Request headers</span></span>

| <span data-ttu-id="8ed4d-125">名前</span><span class="sxs-lookup"><span data-stu-id="8ed4d-125">Name</span></span>       | <span data-ttu-id="8ed4d-126">説明</span><span class="sxs-lookup"><span data-stu-id="8ed4d-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ed4d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ed4d-127">Authorization</span></span>  | <span data-ttu-id="8ed4d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ed4d-130">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8ed4d-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8ed4d-131">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8ed4d-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed4d-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ed4d-133">Request body</span></span>

<span data-ttu-id="8ed4d-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed4d-135">応答</span><span class="sxs-lookup"><span data-stu-id="8ed4d-135">Response</span></span>

<span data-ttu-id="8ed4d-136">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[outlookTask](../resources/outlooktask.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-136">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed4d-137">例</span><span class="sxs-lookup"><span data-stu-id="8ed4d-137">Example</span></span>

<span data-ttu-id="8ed4d-138">次の例では、指定したタスクを終了に設定します。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-138">The following example marks the specified task as complete.</span></span> <span data-ttu-id="8ed4d-139">太平洋標準時 (PST) で指定します`Prefer: outlook.timezone`ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-139">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="8ed4d-140">要求</span><span class="sxs-lookup"><span data-stu-id="8ed4d-140">Request</span></span>

<span data-ttu-id="8ed4d-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="8ed4d-142">応答</span><span class="sxs-lookup"><span data-stu-id="8ed4d-142">Response</span></span>

<span data-ttu-id="8ed4d-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-143">Here is an example of the response.</span></span> <span data-ttu-id="8ed4d-144">PST では、 **completedDateTime**と他の日付に関連するプロパティに、応答が表されます。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-144">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="8ed4d-145">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8ed4d-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8ed4d-146">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
