---
title: 'outlookTask: 完全な'
description: '現在の日付に**completedDateTime**プロパティを設定する Outlook のタスクを完了します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: de3d47d59b89f8bbef42b8b17a9099ecf9e80c98
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513558"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="b5e93-103">outlookTask: 完全な</span><span class="sxs-lookup"><span data-stu-id="b5e93-103">outlookTask: complete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e93-104">現在の日付に**completedDateTime**プロパティと**状態**プロパティを設定する Outlook のタスクを完了`completed`。</span><span class="sxs-lookup"><span data-stu-id="b5e93-104">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="b5e93-105">応答では、定期的にタスクを実行している場合、シリーズでは、完了したタスクとデータ系列の次のタスクは、タスクのコレクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b5e93-105">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="b5e93-106">**CompletedDateTime**プロパティは、タスクが完了すると、日付を表します。</span><span class="sxs-lookup"><span data-stu-id="b5e93-106">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="b5e93-107">**CompletedDateTime**の時刻部分は、UTC の午前 0 時に既定で設定されています。</span><span class="sxs-lookup"><span data-stu-id="b5e93-107">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="b5e93-108">既定では、この操作 (および投稿、取得、および更新プログラムのタスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="b5e93-108">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="b5e93-109">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="b5e93-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e93-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5e93-110">Permissions</span></span>

<span data-ttu-id="b5e93-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5e93-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e93-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5e93-113">Permission type</span></span>      | <span data-ttu-id="b5e93-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5e93-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e93-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e93-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e93-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e93-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b5e93-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e93-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e93-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e93-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b5e93-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5e93-119">Application</span></span> | <span data-ttu-id="b5e93-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5e93-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e93-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5e93-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="b5e93-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5e93-122">Request headers</span></span>

| <span data-ttu-id="b5e93-123">名前</span><span class="sxs-lookup"><span data-stu-id="b5e93-123">Name</span></span>       | <span data-ttu-id="b5e93-124">説明</span><span class="sxs-lookup"><span data-stu-id="b5e93-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5e93-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e93-125">Authorization</span></span>  | <span data-ttu-id="b5e93-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5e93-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5e93-128">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b5e93-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="b5e93-129">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5e93-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="b5e93-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b5e93-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5e93-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5e93-131">Request body</span></span>

<span data-ttu-id="b5e93-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b5e93-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e93-133">応答</span><span class="sxs-lookup"><span data-stu-id="b5e93-133">Response</span></span>

<span data-ttu-id="b5e93-134">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[outlookTask](../resources/outlooktask.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b5e93-134">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e93-135">例</span><span class="sxs-lookup"><span data-stu-id="b5e93-135">Example</span></span>

<span data-ttu-id="b5e93-136">次の例では、指定したタスクを終了に設定します。</span><span class="sxs-lookup"><span data-stu-id="b5e93-136">The following example marks the specified task as complete.</span></span> <span data-ttu-id="b5e93-137">太平洋標準時 (PST) で指定します`Prefer: outlook.timezone`ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="b5e93-137">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="b5e93-138">要求</span><span class="sxs-lookup"><span data-stu-id="b5e93-138">Request</span></span>

<span data-ttu-id="b5e93-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b5e93-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="b5e93-140">応答</span><span class="sxs-lookup"><span data-stu-id="b5e93-140">Response</span></span>

<span data-ttu-id="b5e93-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b5e93-141">Here is an example of the response.</span></span> <span data-ttu-id="b5e93-142">PST では、 **completedDateTime**と他の日付に関連するプロパティに、応答が表されます。</span><span class="sxs-lookup"><span data-stu-id="b5e93-142">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="b5e93-p108">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5e93-p108">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-complete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
