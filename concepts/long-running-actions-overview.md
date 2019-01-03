---
title: 長時間実行アクションの処理 (ベータ版)
description: この記事では、長時間実行アクションの処理について説明します。
ms.openlocfilehash: 73e00efd88b2656cc842c3c46f8a2241315ba184
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354530"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="dc5d0-103">長時間実行アクションの処理 (ベータ版)</span><span class="sxs-lookup"><span data-stu-id="dc5d0-103">Working with long running actions (beta)</span></span>

> <span data-ttu-id="dc5d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc5d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc5d0-106">一部の API 応答では、完了までに要する時間が不明です。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-106">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="dc5d0-107">アクションが完了するまで待機してから応答を返す代わりに、Microsoft Graph では長時間実行アクションのパターンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-107">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="dc5d0-108">このパターンでは、要求がアクションの完了を待機せずに、長時間実行アクションに関する状態の最新情報のポーリングに対しての待機をアプリに提供します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-108">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="dc5d0-109">一般的なパターンでは、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-109">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="dc5d0-110">アプリが API 経由で長時間実行アクションを要求します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-110">Your app requests a long running action via the API.</span></span> <span data-ttu-id="dc5d0-111">API はアクションを承諾し、API URL の Location ヘッダーと共に `202 Accepted` 応答を返して、アクションの状態レポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-111">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="dc5d0-112">アプリは、アクションの状態レポート URL を要求して、長時間実行アクションの進行状況を含む [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-112">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="dc5d0-113">長時間実行アクションが完了します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-113">The long running action completes.</span></span> 
4. <span data-ttu-id="dc5d0-114">アプリはアクションの状態レポート URL を再度要求して、アクションの完了を示す [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-114">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="dc5d0-115">最初のアクション要求</span><span class="sxs-lookup"><span data-stu-id="dc5d0-115">Initial action request</span></span>

<span data-ttu-id="dc5d0-116">[DriveItem コピー](/graph/api/driveitem-copy?view=graph-rest-beta) シナリオの例を順を追って説明します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-116">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="dc5d0-117">このシナリオでは、アプリは大量のデータが格納されているフォルダーのコピーを要求します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-117">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="dc5d0-118">この要求は、データが大量であるため完了までに数秒間かかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-118">This request will likely take several seconds to complete since the amount of data is large.</span></span>

<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```

<span data-ttu-id="dc5d0-119">API は、アクションが承諾されたことと、長時間実行アクションの状態を取得するための URL を応答で返します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-119">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="dc5d0-120">**注:** 場所の URL が返されても、Microsoft Graph API エンドポイントにあるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-120">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="dc5d0-121">多くの場合、コピー アクションはアプリが追加の作業をすることなく完了するため、これが要求の最後になります。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-121">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="dc5d0-122">ただし、アプリでコピー アクションの状態を表示することが必要な場合や、そのアクションがエラーなしで完了したことを確認する場合は、モニター URL を使用できます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-122">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="dc5d0-123">モニター URL から状態レポートを取得する</span><span class="sxs-lookup"><span data-stu-id="dc5d0-123">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="dc5d0-124">コピー アクションの状態を確認するために、アプリは前の応答で提供された URL に要求を行います。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-124">To check on the status of the copy action, the app makes a request to the URL provided in the previous response.</span></span>
<span data-ttu-id="dc5d0-125">*注:* この要求には、認証は必要ありません。この URL の有効期間は短く、最初の呼び出し元に一意であるためです。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-125">*Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="dc5d0-126">サービスは、長時間実行のアクションがまだ進行中であるという情報を含む応答を返します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-126">The service responses with information that the long running action is still in progress:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

<span data-ttu-id="dc5d0-127">この情報は、コピー アクションの進行状況に関する最新情報をユーザーに提供するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-127">This information can be used to provide an update to the user about the progress of the copy action.</span></span>
<span data-ttu-id="dc5d0-128">アプリは、状態の最新情報を要求してアクションの進行状況を追跡するために、継続してモニター URL をポーリングできます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-128">The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="dc5d0-129">モニター URL から完了状態レポートを取得する</span><span class="sxs-lookup"><span data-stu-id="dc5d0-129">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="dc5d0-130">コピー操作が完了してから数秒経過しています。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-130">After a few seconds the copy operation has completed.</span></span>
<span data-ttu-id="dc5d0-131">このときにアプリがモニター URL に要求を送信すると、完了したアクションの結果にリダイレクトする応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-131">This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="dc5d0-132">アクションが完了すると、モニター サービスからの応答で、結果の resourceId が返されます。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-132">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="dc5d0-133">完了した操作の結果を取得する</span><span class="sxs-lookup"><span data-stu-id="dc5d0-133">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="dc5d0-134">ジョブが完了すると、モニター URL が結果の resourceId を返します。ここでは、元のアイテムの新しいコピーを返します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-134">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="dc5d0-135">resourceId を使用してこの新しいアイテムに対処することができます。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-135">You can address this new item using the resourceId, for example:</span></span>

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a><span data-ttu-id="dc5d0-136">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="dc5d0-136">Supported resources</span></span>

<span data-ttu-id="dc5d0-137">長時間実行アクションは、次の API メソッドでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-137">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="dc5d0-138">**リソース**</span><span class="sxs-lookup"><span data-stu-id="dc5d0-138">**Resource**</span></span> | <span data-ttu-id="dc5d0-139">**API**</span><span class="sxs-lookup"><span data-stu-id="dc5d0-139">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="dc5d0-140">DriveItem</span><span class="sxs-lookup"><span data-stu-id="dc5d0-140">DriveItem</span></span> | [<span data-ttu-id="dc5d0-141">コピー</span><span class="sxs-lookup"><span data-stu-id="dc5d0-141">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="dc5d0-142">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc5d0-142">Prerequisites</span></span>

<span data-ttu-id="dc5d0-143">長時間実行アクションの実行に必要な[アクセス許可](./permissions-reference.md)と同じアクセス許可は、長時間実行アクションの状態をクエリするときにも必要です。</span><span class="sxs-lookup"><span data-stu-id="dc5d0-143">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->