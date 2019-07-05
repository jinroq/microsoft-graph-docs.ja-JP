---
title: outlookTask リソースの種類
description: '作業アイテムを追跡することができる Outlook アイテム。 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 231cb227c33e9f58e0dbe87dbf832b86bf2f017f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459602"
---
# <a name="outlooktask-resource-type"></a><span data-ttu-id="228ca-103">outlookTask リソースの種類</span><span class="sxs-lookup"><span data-stu-id="228ca-103">outlookTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="228ca-104">作業アイテムを追跡することができる Outlook アイテム。</span><span class="sxs-lookup"><span data-stu-id="228ca-104">An Outlook item that can track a work item.</span></span>

<span data-ttu-id="228ca-105">タスクを使用すると、開始日時、期限日時、実際の完了日時、進行状況や状態、定期的かどうか、通知が必要かどうかを追跡できます。</span><span class="sxs-lookup"><span data-stu-id="228ca-105">You can use a task to track the start, due and actual completion dates and times, its progress or status, whether it's recurring, and requires reminding.</span></span>

<span data-ttu-id="228ca-106">**outlookTask** リソースの日付関連プロパティには次が含まれます。</span><span class="sxs-lookup"><span data-stu-id="228ca-106">Date-related properties in the **outlookTask** resource include the following:</span></span>

- <span data-ttu-id="228ca-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-107">completedDateTime</span></span>
- <span data-ttu-id="228ca-108">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-108">createdDateTime</span></span>
- <span data-ttu-id="228ca-109">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-109">dueDateTime</span></span>
- <span data-ttu-id="228ca-110">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-110">lastModifiedDateTime</span></span>
- <span data-ttu-id="228ca-111">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-111">reminderDateTime</span></span>
- <span data-ttu-id="228ca-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-112">startDateTime</span></span>

<span data-ttu-id="228ca-113">既定では、POST、GET、PATCH、および [complete](../api/outlooktask-complete.md) 操作は、REST 応答の日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="228ca-113">By default, the POST, GET, PATCH, and [complete](../api/outlooktask-complete.md) operations return date-related properties in their REST responses in UTC.</span></span>
<span data-ttu-id="228ca-114">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="228ca-114">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="228ca-115">次の例では、対応する応答の日付関連プロパティが EST で返されています。</span><span class="sxs-lookup"><span data-stu-id="228ca-115">The following example returns date-related properties in EST in the corresponding response:</span></span>

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a><span data-ttu-id="228ca-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="228ca-116">Methods</span></span>

| <span data-ttu-id="228ca-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="228ca-117">Method</span></span>           | <span data-ttu-id="228ca-118">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="228ca-118">Return Type</span></span>    |<span data-ttu-id="228ca-119">説明</span><span class="sxs-lookup"><span data-stu-id="228ca-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="228ca-120">outlookTask を取得する</span><span class="sxs-lookup"><span data-stu-id="228ca-120">Get outlookTask</span></span>](../api/outlooktask-get.md) | [<span data-ttu-id="228ca-121">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-121">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="228ca-122">ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="228ca-122">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>|
|[<span data-ttu-id="228ca-123">更新する</span><span class="sxs-lookup"><span data-stu-id="228ca-123">Update</span></span>](../api/outlooktask-update.md) | [<span data-ttu-id="228ca-124">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-124">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="228ca-125">Outlook タスクの書き込み可能なプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="228ca-125">Change writeable properties of an Outlook task.</span></span> |
|[<span data-ttu-id="228ca-126">削除する</span><span class="sxs-lookup"><span data-stu-id="228ca-126">Delete</span></span>](../api/outlooktask-delete.md) | <span data-ttu-id="228ca-127">なし</span><span class="sxs-lookup"><span data-stu-id="228ca-127">None</span></span> |<span data-ttu-id="228ca-128">ユーザーのメールボックス内の指定されたタスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="228ca-128">Delete the specified task in the user's mailbox.</span></span> |
|[<span data-ttu-id="228ca-129">完了する</span><span class="sxs-lookup"><span data-stu-id="228ca-129">Complete</span></span>](../api/outlooktask-complete.md)|<span data-ttu-id="228ca-130">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-130">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="228ca-131">**completedDateTime** プロパティを現在の日付に設定し、**status** プロパティを `completed` に設定する Outlook タスクを完了します。</span><span class="sxs-lookup"><span data-stu-id="228ca-131">Complete an Outlook task which sets the **completedDateTime** property to the current date, and **status** property to `completed`.</span></span>|
|<span data-ttu-id="228ca-132">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="228ca-132">**Attachments**</span></span>| | |
|[<span data-ttu-id="228ca-133">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="228ca-133">List attachments</span></span>](../api/outlooktask-list-attachments.md) |<span data-ttu-id="228ca-134">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-134">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="228ca-135">Outlook タスクのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="228ca-135">Get all attachments on an Outlook task.</span></span>|
|[<span data-ttu-id="228ca-136">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="228ca-136">Add attachment</span></span>](../api/outlooktask-post-attachments.md) |[<span data-ttu-id="228ca-137">attachment</span><span class="sxs-lookup"><span data-stu-id="228ca-137">attachment</span></span>](attachment.md)| <span data-ttu-id="228ca-138">タスクへの添付としてファイル、アイテム (メッセージ、イベント、連絡先)、またはファイルへのリンクを追加します。</span><span class="sxs-lookup"><span data-stu-id="228ca-138">Add a file, item (message, event or contact), or link to a file as an attachment to a task.</span></span>|
|<span data-ttu-id="228ca-139">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="228ca-139">**Extended properties**</span></span>| | |
|[<span data-ttu-id="228ca-140">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="228ca-140">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="228ca-141">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-141">outlookTask</span></span>](outlooktask.md)  |<span data-ttu-id="228ca-142">新規または既存の Outlook タスクに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="228ca-142">Create one or more single-value extended properties in a new or existing Outlook task.</span></span>   |
|[<span data-ttu-id="228ca-143">単一値の拡張プロパティを持つタスクを取得する</span><span class="sxs-lookup"><span data-stu-id="228ca-143">Get task with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="228ca-144">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-144">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="228ca-145">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="228ca-145">Get Outlook tasks that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="228ca-146">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="228ca-146">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="228ca-147">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-147">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="228ca-148">新規または既存の Outlook タスクに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="228ca-148">Create one or more multi-value extended properties in a new or existing Outlook task.</span></span>  |
|[<span data-ttu-id="228ca-149">複数値の拡張プロパティを持つタスクの取得</span><span class="sxs-lookup"><span data-stu-id="228ca-149">Get task with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="228ca-150">outlookTask</span><span class="sxs-lookup"><span data-stu-id="228ca-150">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="228ca-151">`$expand` を使用して、複数値の拡張プロパティを含む Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="228ca-151">Get an Outlook task that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="228ca-152">プロパティ</span><span class="sxs-lookup"><span data-stu-id="228ca-152">Properties</span></span>
| <span data-ttu-id="228ca-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="228ca-153">Property</span></span>     | <span data-ttu-id="228ca-154">型</span><span class="sxs-lookup"><span data-stu-id="228ca-154">Type</span></span>   |<span data-ttu-id="228ca-155">説明</span><span class="sxs-lookup"><span data-stu-id="228ca-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="228ca-156">assignedTo</span><span class="sxs-lookup"><span data-stu-id="228ca-156">assignedTo</span></span>|<span data-ttu-id="228ca-157">String</span><span class="sxs-lookup"><span data-stu-id="228ca-157">String</span></span>|<span data-ttu-id="228ca-158">Outlook でタスクが割り当てられているユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="228ca-158">The name of the person who has been assigned the task.</span></span> <span data-ttu-id="228ca-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="228ca-159">Read-only.</span></span>|
|<span data-ttu-id="228ca-160">body</span><span class="sxs-lookup"><span data-stu-id="228ca-160">body</span></span>|[<span data-ttu-id="228ca-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="228ca-161">itemBody</span></span>](itembody.md)|<span data-ttu-id="228ca-p103">通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="228ca-p103">The task body that typically contains information about the task. Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="228ca-164">categories</span><span class="sxs-lookup"><span data-stu-id="228ca-164">categories</span></span>|<span data-ttu-id="228ca-165">String コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-165">String collection</span></span>|<span data-ttu-id="228ca-166">タスクに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="228ca-166">The categories associated with the task.</span></span> <span data-ttu-id="228ca-167">各カテゴリは、ユーザーが定義した [outlookCategory](outlookcategory.md) の **displayName** プロパティに対応しています。</span><span class="sxs-lookup"><span data-stu-id="228ca-167">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that the user has defined.</span></span>|
|<span data-ttu-id="228ca-168">changeKey</span><span class="sxs-lookup"><span data-stu-id="228ca-168">changeKey</span></span>|<span data-ttu-id="228ca-169">String</span><span class="sxs-lookup"><span data-stu-id="228ca-169">String</span></span>|<span data-ttu-id="228ca-170">タスクのバージョン。</span><span class="sxs-lookup"><span data-stu-id="228ca-170">The version of the task.</span></span>|
|<span data-ttu-id="228ca-171">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-171">completedDateTime</span></span>|[<span data-ttu-id="228ca-172">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="228ca-172">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="228ca-173">タスクが終了した日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="228ca-173">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="228ca-174">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-174">createdDateTime</span></span>|<span data-ttu-id="228ca-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="228ca-175">DateTimeOffset</span></span>|<span data-ttu-id="228ca-176">タスクが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="228ca-176">The date and time when the task was created.</span></span> <span data-ttu-id="228ca-177">既定では、UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="228ca-177">By default, it is in UTC.</span></span> <span data-ttu-id="228ca-178">要求ヘッダーでカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="228ca-178">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="228ca-179">プロパティの値は、ISO 8601 形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="228ca-179">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="228ca-180">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="228ca-180">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="228ca-181">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-181">dueDateTime</span></span>|[<span data-ttu-id="228ca-182">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="228ca-182">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="228ca-183">タスクが終了する予定の日時 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="228ca-183">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="228ca-184">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="228ca-184">hasAttachments</span></span>|<span data-ttu-id="228ca-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ca-185">Boolean</span></span>|<span data-ttu-id="228ca-186">タスクに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="228ca-186">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="228ca-187">id</span><span class="sxs-lookup"><span data-stu-id="228ca-187">id</span></span>|<span data-ttu-id="228ca-188">String</span><span class="sxs-lookup"><span data-stu-id="228ca-188">String</span></span>| <span data-ttu-id="228ca-189">タスクの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="228ca-189">Unique identifier for the certificate.</span></span> <span data-ttu-id="228ca-190">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="228ca-190">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)]Read-only.</span></span> |
|<span data-ttu-id="228ca-191">importance</span><span class="sxs-lookup"><span data-stu-id="228ca-191">importance</span></span>|<span data-ttu-id="228ca-192">string</span><span class="sxs-lookup"><span data-stu-id="228ca-192">string</span></span>|<span data-ttu-id="228ca-193">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="228ca-193">The importance of the event.</span></span> <span data-ttu-id="228ca-194">可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="228ca-194">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="228ca-195">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="228ca-195">isReminderOn</span></span>|<span data-ttu-id="228ca-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ca-196">Boolean</span></span>|<span data-ttu-id="228ca-197">ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="228ca-197">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="228ca-198">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-198">lastModifiedDateTime</span></span>|<span data-ttu-id="228ca-199">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="228ca-199">DateTimeOffset</span></span>|<span data-ttu-id="228ca-200">タスクが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="228ca-200">The date and time when the task was last modified.</span></span> <span data-ttu-id="228ca-201">既定では、UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="228ca-201">By default, it is in UTC.</span></span> <span data-ttu-id="228ca-202">要求ヘッダーでカスタム タイム ゾーンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="228ca-202">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="228ca-203">プロパティの値は、ISO 8601 形式を使って表され、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="228ca-203">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="228ca-204">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="228ca-204">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="228ca-205">owner</span><span class="sxs-lookup"><span data-stu-id="228ca-205">owner</span></span>|<span data-ttu-id="228ca-206">String</span><span class="sxs-lookup"><span data-stu-id="228ca-206">String</span></span>|<span data-ttu-id="228ca-207">タスクを作成したユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="228ca-207">The name of the person who created the task.</span></span>|
|<span data-ttu-id="228ca-208">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="228ca-208">parentFolderId</span></span>|<span data-ttu-id="228ca-209">String</span><span class="sxs-lookup"><span data-stu-id="228ca-209">String</span></span>|<span data-ttu-id="228ca-210">タスクの親フォルダーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="228ca-210">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="228ca-211">recurrence</span><span class="sxs-lookup"><span data-stu-id="228ca-211">recurrence</span></span>|[<span data-ttu-id="228ca-212">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="228ca-212">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="228ca-213">タスクの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="228ca-213">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="228ca-214">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-214">reminderDateTime</span></span>|[<span data-ttu-id="228ca-215">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="228ca-215">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="228ca-216">タスクのアラーム通知を行う日時。</span><span class="sxs-lookup"><span data-stu-id="228ca-216">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="228ca-217">sensitivity</span><span class="sxs-lookup"><span data-stu-id="228ca-217">sensitivity</span></span>|<span data-ttu-id="228ca-218">string</span><span class="sxs-lookup"><span data-stu-id="228ca-218">string</span></span>|<span data-ttu-id="228ca-219">タスクのプライバシーのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="228ca-219">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="228ca-220">使用可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="228ca-220">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="228ca-221">startDateTime</span><span class="sxs-lookup"><span data-stu-id="228ca-221">startDateTime</span></span>|[<span data-ttu-id="228ca-222">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="228ca-222">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="228ca-223">タスクを開始する日付 (指定のタイム ゾーン)。</span><span class="sxs-lookup"><span data-stu-id="228ca-223">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="228ca-224">status</span><span class="sxs-lookup"><span data-stu-id="228ca-224">status</span></span>|<span data-ttu-id="228ca-225">string</span><span class="sxs-lookup"><span data-stu-id="228ca-225">string</span></span>|<span data-ttu-id="228ca-226">タスクの状態または進行状況を示します。</span><span class="sxs-lookup"><span data-stu-id="228ca-226">Indicates the state or progress of the task.</span></span> <span data-ttu-id="228ca-227">可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。</span><span class="sxs-lookup"><span data-stu-id="228ca-227">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="228ca-228">subject</span><span class="sxs-lookup"><span data-stu-id="228ca-228">subject</span></span>|<span data-ttu-id="228ca-229">String</span><span class="sxs-lookup"><span data-stu-id="228ca-229">String</span></span>|<span data-ttu-id="228ca-230">タスクのタイトルまたは簡単な説明。</span><span class="sxs-lookup"><span data-stu-id="228ca-230">A brief description or title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="228ca-231">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="228ca-231">Relationships</span></span>
| <span data-ttu-id="228ca-232">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="228ca-232">Relationship</span></span> | <span data-ttu-id="228ca-233">型</span><span class="sxs-lookup"><span data-stu-id="228ca-233">Type</span></span>   |<span data-ttu-id="228ca-234">説明</span><span class="sxs-lookup"><span data-stu-id="228ca-234">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="228ca-235">attachments</span><span class="sxs-lookup"><span data-stu-id="228ca-235">attachments</span></span>|<span data-ttu-id="228ca-236">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-236">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="228ca-237">タスクの [fileAttachment](fileattachment.md)、[itemAttachment](itemattachment.md)、[referenceAttachment](referenceattachment.md) の各添付ファイルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="228ca-237">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the task.</span></span>  <span data-ttu-id="228ca-238">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="228ca-238">Read-only.</span></span> <span data-ttu-id="228ca-239">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="228ca-239">Nullable.</span></span>|
|<span data-ttu-id="228ca-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="228ca-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="228ca-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="228ca-242">そのタスクに対して定義された、複数値拡張プロパティのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="228ca-242">The collection of multi-value extended properties defined for the task.</span></span> <span data-ttu-id="228ca-243">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="228ca-243">Read-only.</span></span> <span data-ttu-id="228ca-244">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="228ca-244">Nullable.</span></span>|
|<span data-ttu-id="228ca-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="228ca-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="228ca-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="228ca-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="228ca-247">そのタスクに対して定義された、単一値拡張プロパティのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="228ca-247">The collection of single-value extended properties defined for the task.</span></span> <span data-ttu-id="228ca-248">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="228ca-248">Read-only.</span></span> <span data-ttu-id="228ca-249">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="228ca-249">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="228ca-250">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="228ca-250">JSON representation</span></span>
<span data-ttu-id="228ca-251">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="228ca-251">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
