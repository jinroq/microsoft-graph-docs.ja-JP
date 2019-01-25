---
title: Outlooktask を更新します。
description: Outlook のタスクの書き込み可能なプロパティを変更します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526887"
---
# <a name="update-outlooktask"></a><span data-ttu-id="9d539-103">Outlooktask を更新します。</span><span class="sxs-lookup"><span data-stu-id="9d539-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d539-104">Outlook のタスクの書き込み可能なプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="9d539-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="9d539-p101">CompletedDateTime プロパティは、Complete アクションによって、または明示的に PATCH 操作によって設定することができます。PATCH を使用して CompletedDateTime を設定する場合は、Status も  にしてください。</span><span class="sxs-lookup"><span data-stu-id="9d539-p101">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation. If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="9d539-107">既定では、この操作 (および投稿、取得、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="9d539-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="9d539-108">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="9d539-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d539-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d539-109">Permissions</span></span>

<span data-ttu-id="9d539-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d539-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d539-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d539-112">Permission type</span></span>      | <span data-ttu-id="9d539-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d539-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d539-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d539-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9d539-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d539-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9d539-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d539-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d539-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d539-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9d539-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d539-118">Application</span></span> | <span data-ttu-id="9d539-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d539-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d539-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d539-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d539-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d539-121">Request headers</span></span>

| <span data-ttu-id="9d539-122">名前</span><span class="sxs-lookup"><span data-stu-id="9d539-122">Name</span></span>       | <span data-ttu-id="9d539-123">説明</span><span class="sxs-lookup"><span data-stu-id="9d539-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d539-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d539-124">Authorization</span></span>  | <span data-ttu-id="9d539-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d539-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d539-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9d539-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="9d539-128">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d539-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="9d539-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9d539-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d539-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d539-130">Request body</span></span>

<span data-ttu-id="9d539-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9d539-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d539-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d539-134">Property</span></span> | <span data-ttu-id="9d539-135">型</span><span class="sxs-lookup"><span data-stu-id="9d539-135">Type</span></span> | <span data-ttu-id="9d539-136">説明</span><span class="sxs-lookup"><span data-stu-id="9d539-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9d539-137">AssignedTo</span><span class="sxs-lookup"><span data-stu-id="9d539-137">assignedTo</span></span>|<span data-ttu-id="9d539-138">String</span><span class="sxs-lookup"><span data-stu-id="9d539-138">String</span></span>|<span data-ttu-id="9d539-139">タスクが割り当てられているユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="9d539-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="9d539-140">body</span><span class="sxs-lookup"><span data-stu-id="9d539-140">body</span></span>|[<span data-ttu-id="9d539-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="9d539-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="9d539-p107">通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="9d539-p107">The task body that typically contains information about the task. Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="9d539-144">categories</span><span class="sxs-lookup"><span data-stu-id="9d539-144">categories</span></span>|<span data-ttu-id="9d539-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9d539-145">String collection</span></span>|<span data-ttu-id="9d539-146">タスクに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="9d539-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="9d539-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="9d539-147">changeKey</span></span>|<span data-ttu-id="9d539-148">String</span><span class="sxs-lookup"><span data-stu-id="9d539-148">String</span></span>|<span data-ttu-id="9d539-149">タスクのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9d539-149">The version of the task.</span></span>|
|<span data-ttu-id="9d539-150">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-150">completedDateTime</span></span>|[<span data-ttu-id="9d539-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d539-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d539-152">タスクが終了した日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="9d539-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="9d539-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-153">createdDateTime</span></span>|<span data-ttu-id="9d539-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d539-154">DateTimeOffset</span></span>|<span data-ttu-id="9d539-155">日付と時刻、タスクが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="9d539-155">The date and time when the task was created.</span></span> <span data-ttu-id="9d539-156">既定では、UTC であります。</span><span class="sxs-lookup"><span data-stu-id="9d539-156">By default, it is in UTC.</span></span> <span data-ttu-id="9d539-157">要求ヘッダーにカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9d539-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="9d539-158">プロパティの値は、ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="9d539-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="9d539-159">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="9d539-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9d539-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-160">dueDateTime</span></span>|[<span data-ttu-id="9d539-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d539-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d539-162">タスクが終了する予定の日時 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="9d539-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="9d539-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="9d539-163">hasAttachments</span></span>|<span data-ttu-id="9d539-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="9d539-164">Boolean</span></span>|<span data-ttu-id="9d539-165">タスクに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="9d539-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="9d539-166">importance</span><span class="sxs-lookup"><span data-stu-id="9d539-166">importance</span></span>|<span data-ttu-id="9d539-167">string</span><span class="sxs-lookup"><span data-stu-id="9d539-167">string</span></span>|<span data-ttu-id="9d539-168">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="9d539-168">The importance of the event.</span></span> <span data-ttu-id="9d539-169">可能な値は `low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="9d539-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="9d539-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="9d539-170">isReminderOn</span></span>|<span data-ttu-id="9d539-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d539-171">Boolean</span></span>|<span data-ttu-id="9d539-172">ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="9d539-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="9d539-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-173">lastModifiedDateTime</span></span>|<span data-ttu-id="9d539-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d539-174">DateTimeOffset</span></span>|<span data-ttu-id="9d539-175">日付と、タスクが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="9d539-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="9d539-176">既定では、UTC であります。</span><span class="sxs-lookup"><span data-stu-id="9d539-176">By default, it is in UTC.</span></span> <span data-ttu-id="9d539-177">要求ヘッダーにカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9d539-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="9d539-178">プロパティの値は、ISO 8601 形式を使用し、UTC 時刻が常に。</span><span class="sxs-lookup"><span data-stu-id="9d539-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d539-179">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="9d539-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9d539-180">owner</span><span class="sxs-lookup"><span data-stu-id="9d539-180">owner</span></span>|<span data-ttu-id="9d539-181">String</span><span class="sxs-lookup"><span data-stu-id="9d539-181">String</span></span>|<span data-ttu-id="9d539-182">タスクを作成したユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="9d539-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="9d539-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9d539-183">parentFolderId</span></span>|<span data-ttu-id="9d539-184">String</span><span class="sxs-lookup"><span data-stu-id="9d539-184">String</span></span>|<span data-ttu-id="9d539-185">タスクの親フォルダーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="9d539-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="9d539-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="9d539-186">recurrence</span></span>|[<span data-ttu-id="9d539-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d539-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="9d539-188">タスクの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="9d539-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="9d539-189">ReminderDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-189">reminderDateTime</span></span>|[<span data-ttu-id="9d539-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d539-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d539-191">タスクのアラーム通知を行う日時。</span><span class="sxs-lookup"><span data-stu-id="9d539-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="9d539-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="9d539-192">sensitivity</span></span>|<span data-ttu-id="9d539-193">string</span><span class="sxs-lookup"><span data-stu-id="9d539-193">string</span></span>|<span data-ttu-id="9d539-194">タスクのプライバシーのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="9d539-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="9d539-195">可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="9d539-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="9d539-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d539-196">startDateTime</span></span>|[<span data-ttu-id="9d539-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d539-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d539-198">タスクを開始する日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="9d539-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="9d539-199">status</span><span class="sxs-lookup"><span data-stu-id="9d539-199">status</span></span>|<span data-ttu-id="9d539-200">string</span><span class="sxs-lookup"><span data-stu-id="9d539-200">string</span></span>|<span data-ttu-id="9d539-201">状態またはタスクの進行状況を示します。</span><span class="sxs-lookup"><span data-stu-id="9d539-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="9d539-202">可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。</span><span class="sxs-lookup"><span data-stu-id="9d539-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="9d539-203">subject</span><span class="sxs-lookup"><span data-stu-id="9d539-203">subject</span></span>|<span data-ttu-id="9d539-204">String</span><span class="sxs-lookup"><span data-stu-id="9d539-204">String</span></span>|<span data-ttu-id="9d539-205">タスクのタイトルまたは簡単な説明。</span><span class="sxs-lookup"><span data-stu-id="9d539-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="9d539-206">応答</span><span class="sxs-lookup"><span data-stu-id="9d539-206">Response</span></span>

<span data-ttu-id="9d539-207">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[outlookTask](../resources/outlooktask.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9d539-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d539-208">例</span><span class="sxs-lookup"><span data-stu-id="9d539-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d539-209">要求</span><span class="sxs-lookup"><span data-stu-id="9d539-209">Request</span></span>

<span data-ttu-id="9d539-210">次の使用例は、 **dueDateTime**プロパティを変更してを使用して、`Prefer: outlook.timezone`の東部標準時 (EST) の応答での日付に関連するプロパティを表現することを指定するヘッダー。</span><span class="sxs-lookup"><span data-stu-id="9d539-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a><span data-ttu-id="9d539-211">応答</span><span class="sxs-lookup"><span data-stu-id="9d539-211">Response</span></span>

<span data-ttu-id="9d539-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d539-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
