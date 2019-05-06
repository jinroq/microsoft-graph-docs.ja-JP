---
title: OutlookTask の作成
description: ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f508aa05ad70246584ebc33bfaabc9317205011d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596097"
---
# <a name="create-outlooktask"></a><span data-ttu-id="2e551-103">OutlookTask の作成</span><span class="sxs-lookup"><span data-stu-id="2e551-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e551-104">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="2e551-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="2e551-105">POST メソッドは、要求本文の**startDateTime**および**dueDateTime**の時間部分を常に無視し、指定されたタイムゾーンで常に深夜になる時刻を想定します。</span><span class="sxs-lookup"><span data-stu-id="2e551-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="2e551-106">既定では、この操作 (およびタスクの取得、パッチ、[完了](../api/outlooktask-complete.md)) は、日付関連プロパティを UTC で返します。</span><span class="sxs-lookup"><span data-stu-id="2e551-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="2e551-107">`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。</span><span class="sxs-lookup"><span data-stu-id="2e551-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e551-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e551-108">Permissions</span></span>
<span data-ttu-id="2e551-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e551-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e551-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e551-111">Permission type</span></span>      | <span data-ttu-id="2e551-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e551-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e551-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e551-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2e551-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e551-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2e551-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e551-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e551-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e551-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2e551-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e551-117">Application</span></span> | <span data-ttu-id="2e551-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e551-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e551-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e551-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="2e551-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e551-120">Request headers</span></span>
| <span data-ttu-id="2e551-121">名前</span><span class="sxs-lookup"><span data-stu-id="2e551-121">Name</span></span>       | <span data-ttu-id="2e551-122">説明</span><span class="sxs-lookup"><span data-stu-id="2e551-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e551-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e551-123">Authorization</span></span>  | <span data-ttu-id="2e551-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e551-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e551-126">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2e551-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="2e551-127">応答の時間プロパティのタイムゾーンを指定します。このヘッダーが指定されていない場合は、UTC になります。</span><span class="sxs-lookup"><span data-stu-id="2e551-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="2e551-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2e551-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e551-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e551-129">Request body</span></span>
<span data-ttu-id="2e551-130">要求本文で、 [Outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e551-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2e551-131">応答</span><span class="sxs-lookup"><span data-stu-id="2e551-131">Response</span></span>

<span data-ttu-id="2e551-132">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktask](../resources/outlooktask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2e551-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e551-133">例</span><span class="sxs-lookup"><span data-stu-id="2e551-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e551-134">要求</span><span class="sxs-lookup"><span data-stu-id="2e551-134">Request</span></span>
<span data-ttu-id="2e551-135">次の例は、 `Prefer: outlook.timezone`ヘッダーの使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e551-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="2e551-136">この例では、タスクを作成し、 **startDateTime**と**dueDateTime**を東部標準時 (EST) で表し`Prefer` 、太平洋標準時 (PST) のヘッダーを含みます。</span><span class="sxs-lookup"><span data-stu-id="2e551-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="2e551-137">要求本文で、 [Outlooktask](../resources/outlooktask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e551-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2e551-138">応答</span><span class="sxs-lookup"><span data-stu-id="2e551-138">Response</span></span>
<span data-ttu-id="2e551-139">POST メソッドは、要求本文の**startDateTime**および**dueDateTime**の時間部分を無視し、指定されたタイムゾーン (EST) で常に午前0時になる時間を想定します。</span><span class="sxs-lookup"><span data-stu-id="2e551-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="2e551-140">`Prefer` ヘッダーでは PST が指定されているため、POST メソッドは応答内のすべての日付関連プロパティを PST で表記します。</span><span class="sxs-lookup"><span data-stu-id="2e551-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="2e551-141">特に、 **startDateTime**プロパティと**dueDateTime**プロパティの場合、POST メソッドは EST の午前0時を pst に変換し、それらを応答で pst で返します。</span><span class="sxs-lookup"><span data-stu-id="2e551-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="2e551-142">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2e551-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2e551-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2e551-143">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2e551-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="2e551-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2e551-145">Visual</span><span class="sxs-lookup"><span data-stu-id="2e551-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e551-146">Java</span><span class="sxs-lookup"><span data-stu-id="2e551-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
