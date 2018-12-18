---
title: Outlooktask を更新します。
description: Outlook のタスクの書き込み可能なプロパティを変更します。
author: angelgolfer-ms
ms.openlocfilehash: 0a162c81ef32cb35e930b000678234ede20e4874
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325705"
---
# <a name="update-outlooktask"></a><span data-ttu-id="7a8f1-103">Outlooktask を更新します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-103">Update outlooktask</span></span>

> <span data-ttu-id="7a8f1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a8f1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a8f1-106">Outlook のタスクの書き込み可能なプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="7a8f1-107">**完全な**アクション、または明示的に修正プログラムの操作では、 **completedDateTime**プロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="7a8f1-108">**状態**を設定するに**completedDateTime**の設定を確認して修正プログラムを使用する場合は、`completed`も同様です。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="7a8f1-109">既定では、この操作 (および投稿、取得、および[完了](../api/outlooktask-complete.md)タスクの操作) は UTC の日付に関連するプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="7a8f1-110">ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone`</span><span class="sxs-lookup"><span data-stu-id="7a8f1-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a8f1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7a8f1-111">Permissions</span></span>
<span data-ttu-id="7a8f1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a8f1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a8f1-114">Permission type</span></span>      | <span data-ttu-id="7a8f1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a8f1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a8f1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a8f1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7a8f1-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a8f1-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a8f1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a8f1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a8f1-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a8f1-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a8f1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a8f1-120">Application</span></span> | <span data-ttu-id="7a8f1-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a8f1-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a8f1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7a8f1-123">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a8f1-123">Optional request headers</span></span>
| <span data-ttu-id="7a8f1-124">名前</span><span class="sxs-lookup"><span data-stu-id="7a8f1-124">Name</span></span>       | <span data-ttu-id="7a8f1-125">説明</span><span class="sxs-lookup"><span data-stu-id="7a8f1-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7a8f1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a8f1-126">Authorization</span></span>  | <span data-ttu-id="7a8f1-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a8f1-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7a8f1-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7a8f1-130">このヘッダーが指定されていない場合は、UTC である応答でタイム ゾーンの時刻のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="7a8f1-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a8f1-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a8f1-132">Request body</span></span>
<span data-ttu-id="7a8f1-p107">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7a8f1-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a8f1-136">Property</span></span>     | <span data-ttu-id="7a8f1-137">種類</span><span class="sxs-lookup"><span data-stu-id="7a8f1-137">Type</span></span>   |<span data-ttu-id="7a8f1-138">説明</span><span class="sxs-lookup"><span data-stu-id="7a8f1-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a8f1-139">担当者</span><span class="sxs-lookup"><span data-stu-id="7a8f1-139">assignedTo</span></span>|<span data-ttu-id="7a8f1-140">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-140">String</span></span>|<span data-ttu-id="7a8f1-141">タスクが割り当てられているユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="7a8f1-142">body</span><span class="sxs-lookup"><span data-stu-id="7a8f1-142">body</span></span>|[<span data-ttu-id="7a8f1-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="7a8f1-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="7a8f1-p108">通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-p108">The task body that typically contains information about the task. Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="7a8f1-146">categories</span><span class="sxs-lookup"><span data-stu-id="7a8f1-146">categories</span></span>|<span data-ttu-id="7a8f1-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7a8f1-147">String collection</span></span>|<span data-ttu-id="7a8f1-148">タスクに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="7a8f1-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="7a8f1-149">changeKey</span></span>|<span data-ttu-id="7a8f1-150">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-150">String</span></span>|<span data-ttu-id="7a8f1-151">タスクのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-151">The version of the task.</span></span>|
|<span data-ttu-id="7a8f1-152">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-152">completedDateTime</span></span>|[<span data-ttu-id="7a8f1-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a8f1-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7a8f1-154">タスクが終了した日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="7a8f1-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-155">createdDateTime</span></span>|<span data-ttu-id="7a8f1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a8f1-156">DateTimeOffset</span></span>|<span data-ttu-id="7a8f1-157">日付と時刻、タスクが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-157">The date and time when the task was created.</span></span> <span data-ttu-id="7a8f1-158">既定では、UTC であります。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-158">By default, it is in UTC.</span></span> <span data-ttu-id="7a8f1-159">要求ヘッダーにカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="7a8f1-160">プロパティの値は、ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="7a8f1-161">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7a8f1-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7a8f1-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-162">dueDateTime</span></span>|[<span data-ttu-id="7a8f1-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a8f1-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7a8f1-164">タスクが終了する予定の日時 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="7a8f1-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="7a8f1-165">hasAttachments</span></span>|<span data-ttu-id="7a8f1-166">ブール型</span><span class="sxs-lookup"><span data-stu-id="7a8f1-166">Boolean</span></span>|<span data-ttu-id="7a8f1-167">タスクに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="7a8f1-168">importance</span><span class="sxs-lookup"><span data-stu-id="7a8f1-168">importance</span></span>|<span data-ttu-id="7a8f1-169">string</span><span class="sxs-lookup"><span data-stu-id="7a8f1-169">string</span></span>|<span data-ttu-id="7a8f1-170">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-170">The importance of the event.</span></span> <span data-ttu-id="7a8f1-171">可能な値は `low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="7a8f1-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="7a8f1-172">isReminderOn</span></span>|<span data-ttu-id="7a8f1-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a8f1-173">Boolean</span></span>|<span data-ttu-id="7a8f1-174">ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="7a8f1-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-175">lastModifiedDateTime</span></span>|<span data-ttu-id="7a8f1-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a8f1-176">DateTimeOffset</span></span>|<span data-ttu-id="7a8f1-177">日付と、タスクが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="7a8f1-178">既定では、UTC であります。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-178">By default, it is in UTC.</span></span> <span data-ttu-id="7a8f1-179">要求ヘッダーにカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="7a8f1-180">プロパティの値は、ISO 8601 形式を使用し、UTC 時刻が常に。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a8f1-181">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7a8f1-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7a8f1-182">owner</span><span class="sxs-lookup"><span data-stu-id="7a8f1-182">owner</span></span>|<span data-ttu-id="7a8f1-183">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-183">String</span></span>|<span data-ttu-id="7a8f1-184">タスクを作成したユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="7a8f1-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="7a8f1-185">parentFolderId</span></span>|<span data-ttu-id="7a8f1-186">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-186">String</span></span>|<span data-ttu-id="7a8f1-187">タスクの親フォルダーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="7a8f1-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="7a8f1-188">recurrence</span></span>|[<span data-ttu-id="7a8f1-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="7a8f1-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="7a8f1-190">タスクの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="7a8f1-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-191">reminderDateTime</span></span>|[<span data-ttu-id="7a8f1-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a8f1-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7a8f1-193">タスクのアラーム通知を行う日時。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="7a8f1-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="7a8f1-194">sensitivity</span></span>|<span data-ttu-id="7a8f1-195">string</span><span class="sxs-lookup"><span data-stu-id="7a8f1-195">string</span></span>|<span data-ttu-id="7a8f1-196">タスクのプライバシーのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="7a8f1-197">可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="7a8f1-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7a8f1-198">startDateTime</span></span>|[<span data-ttu-id="7a8f1-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a8f1-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="7a8f1-200">タスクを開始する日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="7a8f1-201">status</span><span class="sxs-lookup"><span data-stu-id="7a8f1-201">status</span></span>|<span data-ttu-id="7a8f1-202">string</span><span class="sxs-lookup"><span data-stu-id="7a8f1-202">string</span></span>|<span data-ttu-id="7a8f1-203">状態またはタスクの進行状況を示します。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="7a8f1-204">可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="7a8f1-205">subject</span><span class="sxs-lookup"><span data-stu-id="7a8f1-205">subject</span></span>|<span data-ttu-id="7a8f1-206">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-206">String</span></span>|<span data-ttu-id="7a8f1-207">タスクのタイトルまたは簡単な説明。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="7a8f1-208">応答</span><span class="sxs-lookup"><span data-stu-id="7a8f1-208">Response</span></span>

<span data-ttu-id="7a8f1-209">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[outlookTask](../resources/outlooktask.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a8f1-210">例</span><span class="sxs-lookup"><span data-stu-id="7a8f1-210">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a8f1-211">要求</span><span class="sxs-lookup"><span data-stu-id="7a8f1-211">Request</span></span>
<span data-ttu-id="7a8f1-212">次の使用例は、 **dueDateTime**プロパティを変更してを使用して、`Prefer: outlook.timezone`の東部標準時 (EST) の応答での日付に関連するプロパティを表現することを指定するヘッダー。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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
##### <a name="response"></a><span data-ttu-id="7a8f1-213">応答</span><span class="sxs-lookup"><span data-stu-id="7a8f1-213">Response</span></span>
<span data-ttu-id="7a8f1-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a8f1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->