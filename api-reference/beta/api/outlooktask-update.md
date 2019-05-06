---
title: Outlooktask) を更新する
description: Outlook タスクの書き込み可能なプロパティを変更します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fcd0c73e48cf98f52d0c87e3e48acb403d6558b2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596524"
---
# <a name="update-outlooktask"></a><span data-ttu-id="4c446-103">Outlooktask) を更新する</span><span class="sxs-lookup"><span data-stu-id="4c446-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c446-104">Outlook タスクの書き込み可能なプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="4c446-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="4c446-105">**CompletedDateTime**プロパティは、**完全な**アクションによって、または明示的に PATCH 操作によって設定できます。</span><span class="sxs-lookup"><span data-stu-id="4c446-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="4c446-106">PATCH を使用して**completedDateTime**を設定する場合は、**状態**も`completed`同様にに設定してください。</span><span class="sxs-lookup"><span data-stu-id="4c446-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="4c446-107">既定では、この操作 (および POST、GET、および[完了](../api/outlooktask-complete.md)タスク操作) は、日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="4c446-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="4c446-108">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="4c446-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c446-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c446-109">Permissions</span></span>

<span data-ttu-id="4c446-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c446-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c446-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c446-112">Permission type</span></span>      | <span data-ttu-id="4c446-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c446-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c446-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c446-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4c446-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c446-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4c446-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c446-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c446-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c446-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4c446-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c446-118">Application</span></span> | <span data-ttu-id="4c446-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c446-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c446-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c446-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c446-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c446-121">Request headers</span></span>

| <span data-ttu-id="4c446-122">名前</span><span class="sxs-lookup"><span data-stu-id="4c446-122">Name</span></span>       | <span data-ttu-id="4c446-123">説明</span><span class="sxs-lookup"><span data-stu-id="4c446-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4c446-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c446-124">Authorization</span></span>  | <span data-ttu-id="4c446-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c446-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c446-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="4c446-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="4c446-128">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="4c446-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="4c446-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4c446-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c446-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c446-130">Request body</span></span>

<span data-ttu-id="4c446-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4c446-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c446-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c446-134">Property</span></span> | <span data-ttu-id="4c446-135">型</span><span class="sxs-lookup"><span data-stu-id="4c446-135">Type</span></span> | <span data-ttu-id="4c446-136">説明</span><span class="sxs-lookup"><span data-stu-id="4c446-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4c446-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="4c446-137">assignedTo</span></span>|<span data-ttu-id="4c446-138">String</span><span class="sxs-lookup"><span data-stu-id="4c446-138">String</span></span>|<span data-ttu-id="4c446-139">タスクが割り当てられているユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="4c446-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="4c446-140">body</span><span class="sxs-lookup"><span data-stu-id="4c446-140">body</span></span>|[<span data-ttu-id="4c446-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="4c446-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="4c446-p107">通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4c446-p107">The task body that typically contains information about the task. Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="4c446-144">categories</span><span class="sxs-lookup"><span data-stu-id="4c446-144">categories</span></span>|<span data-ttu-id="4c446-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4c446-145">String collection</span></span>|<span data-ttu-id="4c446-146">タスクに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="4c446-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="4c446-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="4c446-147">changeKey</span></span>|<span data-ttu-id="4c446-148">String</span><span class="sxs-lookup"><span data-stu-id="4c446-148">String</span></span>|<span data-ttu-id="4c446-149">タスクのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4c446-149">The version of the task.</span></span>|
|<span data-ttu-id="4c446-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-150">completedDateTime</span></span>|[<span data-ttu-id="4c446-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c446-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c446-152">タスクが終了した日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="4c446-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="4c446-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-153">createdDateTime</span></span>|<span data-ttu-id="4c446-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c446-154">DateTimeOffset</span></span>|<span data-ttu-id="4c446-155">タスクが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4c446-155">The date and time when the task was created.</span></span> <span data-ttu-id="4c446-156">既定では、UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4c446-156">By default, it is in UTC.</span></span> <span data-ttu-id="4c446-157">要求ヘッダーでカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c446-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="4c446-158">プロパティの値は、ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="4c446-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="4c446-159">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="4c446-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4c446-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-160">dueDateTime</span></span>|[<span data-ttu-id="4c446-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c446-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c446-162">タスクが終了する予定の日時 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="4c446-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="4c446-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4c446-163">hasAttachments</span></span>|<span data-ttu-id="4c446-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="4c446-164">Boolean</span></span>|<span data-ttu-id="4c446-165">タスクに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c446-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="4c446-166">importance</span><span class="sxs-lookup"><span data-stu-id="4c446-166">importance</span></span>|<span data-ttu-id="4c446-167">string</span><span class="sxs-lookup"><span data-stu-id="4c446-167">string</span></span>|<span data-ttu-id="4c446-168">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="4c446-168">The importance of the event.</span></span> <span data-ttu-id="4c446-169">可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="4c446-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="4c446-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="4c446-170">isReminderOn</span></span>|<span data-ttu-id="4c446-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c446-171">Boolean</span></span>|<span data-ttu-id="4c446-172">ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c446-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="4c446-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-173">lastModifiedDateTime</span></span>|<span data-ttu-id="4c446-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c446-174">DateTimeOffset</span></span>|<span data-ttu-id="4c446-175">タスクが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4c446-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="4c446-176">既定では、UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4c446-176">By default, it is in UTC.</span></span> <span data-ttu-id="4c446-177">要求ヘッダーでカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c446-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="4c446-178">プロパティの値は、ISO 8601 形式を使って表され、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4c446-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c446-179">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="4c446-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4c446-180">owner</span><span class="sxs-lookup"><span data-stu-id="4c446-180">owner</span></span>|<span data-ttu-id="4c446-181">String</span><span class="sxs-lookup"><span data-stu-id="4c446-181">String</span></span>|<span data-ttu-id="4c446-182">タスクを作成したユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="4c446-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="4c446-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="4c446-183">parentFolderId</span></span>|<span data-ttu-id="4c446-184">String</span><span class="sxs-lookup"><span data-stu-id="4c446-184">String</span></span>|<span data-ttu-id="4c446-185">タスクの親フォルダーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="4c446-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="4c446-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="4c446-186">recurrence</span></span>|[<span data-ttu-id="4c446-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4c446-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="4c446-188">タスクの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="4c446-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="4c446-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-189">reminderDateTime</span></span>|[<span data-ttu-id="4c446-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c446-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c446-191">タスクのアラーム通知を行う日時。</span><span class="sxs-lookup"><span data-stu-id="4c446-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="4c446-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="4c446-192">sensitivity</span></span>|<span data-ttu-id="4c446-193">string</span><span class="sxs-lookup"><span data-stu-id="4c446-193">string</span></span>|<span data-ttu-id="4c446-194">タスクのプライバシーのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="4c446-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="4c446-195">使用可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="4c446-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="4c446-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4c446-196">startDateTime</span></span>|[<span data-ttu-id="4c446-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c446-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c446-198">タスクを開始する日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="4c446-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="4c446-199">status</span><span class="sxs-lookup"><span data-stu-id="4c446-199">status</span></span>|<span data-ttu-id="4c446-200">string</span><span class="sxs-lookup"><span data-stu-id="4c446-200">string</span></span>|<span data-ttu-id="4c446-201">タスクの状態または進行状況を示します。</span><span class="sxs-lookup"><span data-stu-id="4c446-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="4c446-202">可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。</span><span class="sxs-lookup"><span data-stu-id="4c446-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="4c446-203">subject</span><span class="sxs-lookup"><span data-stu-id="4c446-203">subject</span></span>|<span data-ttu-id="4c446-204">String</span><span class="sxs-lookup"><span data-stu-id="4c446-204">String</span></span>|<span data-ttu-id="4c446-205">タスクのタイトルまたは簡単な説明。</span><span class="sxs-lookup"><span data-stu-id="4c446-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="4c446-206">応答</span><span class="sxs-lookup"><span data-stu-id="4c446-206">Response</span></span>

<span data-ttu-id="4c446-207">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[outlooktask](../resources/outlooktask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c446-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c446-208">例</span><span class="sxs-lookup"><span data-stu-id="4c446-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c446-209">要求</span><span class="sxs-lookup"><span data-stu-id="4c446-209">Request</span></span>

<span data-ttu-id="4c446-210">次の例では、 **dueDateTime**プロパティを変更`Prefer: outlook.timezone`し、ヘッダーを使用して、応答の日付関連プロパティを東部標準時 (EST) で表現するように指定しています。</span><span class="sxs-lookup"><span data-stu-id="4c446-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
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

### <a name="response"></a><span data-ttu-id="4c446-211">応答</span><span class="sxs-lookup"><span data-stu-id="4c446-211">Response</span></span>

<span data-ttu-id="4c446-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c446-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c446-215">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="4c446-215">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c446-216">Visual</span><span class="sxs-lookup"><span data-stu-id="4c446-216">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c446-217">Java</span><span class="sxs-lookup"><span data-stu-id="4c446-217">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktask-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
