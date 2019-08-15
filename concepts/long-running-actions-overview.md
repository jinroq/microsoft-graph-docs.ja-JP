---
title: 長時間実行アクションの処理 (ベータ版)
description: この記事では、長時間実行アクションの処理について説明します。
localization_priority: Normal
author: daspek
ms.openlocfilehash: 3d1dae399147cb1aed40a045e4365faf15d753f5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422311"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="0b553-103">長時間実行アクションの処理 (ベータ版)</span><span class="sxs-lookup"><span data-stu-id="0b553-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="0b553-104">一部の API 応答では、完了までに要する時間が不明です。</span><span class="sxs-lookup"><span data-stu-id="0b553-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="0b553-105">アクションが完了するまで待機してから応答を返す代わりに、Microsoft Graph では長時間実行アクションのパターンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0b553-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="0b553-106">このパターンでは、要求がアクションの完了を待機せずに、長時間実行アクションに関する状態の最新情報のポーリングに対しての待機をアプリに提供します。</span><span class="sxs-lookup"><span data-stu-id="0b553-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="0b553-107">一般的なパターンでは、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="0b553-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="0b553-108">アプリが API 経由で長時間実行アクションを要求します。</span><span class="sxs-lookup"><span data-stu-id="0b553-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="0b553-109">API はアクションを承諾し、API URL の Location ヘッダーと共に `202 Accepted` 応答を返して、アクションの状態レポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="0b553-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="0b553-110">アプリは、アクションの状態レポート URL を要求して、長時間実行アクションの進行状況を含む [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="0b553-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="0b553-111">長時間実行アクションが完了します。</span><span class="sxs-lookup"><span data-stu-id="0b553-111">The long running action completes.</span></span> 
4. <span data-ttu-id="0b553-112">アプリはアクションの状態レポート URL を再度要求して、アクションの完了を示す [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="0b553-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="0b553-113">最初のアクション要求</span><span class="sxs-lookup"><span data-stu-id="0b553-113">Initial action request</span></span>

<span data-ttu-id="0b553-114">[DriveItem コピー](/graph/api/driveitem-copy?view=graph-rest-beta) シナリオの例を順を追って説明します。</span><span class="sxs-lookup"><span data-stu-id="0b553-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="0b553-115">このシナリオでは、アプリは大量のデータが格納されているフォルダーのコピーを要求します。</span><span class="sxs-lookup"><span data-stu-id="0b553-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="0b553-116">この要求は、データが大量であるため完了までに数秒間かかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0b553-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b553-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0b553-117">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b553-118">C#</span><span class="sxs-lookup"><span data-stu-id="0b553-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b553-119">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b553-119">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b553-120">目的-C</span><span class="sxs-lookup"><span data-stu-id="0b553-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0b553-121">API は、アクションが承諾されたことと、長時間実行アクションの状態を取得するための URL を応答で返します。</span><span class="sxs-lookup"><span data-stu-id="0b553-121">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0b553-122">**注:** 場所の URL が返されても、Microsoft Graph API エンドポイントにあるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="0b553-122">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="0b553-123">多くの場合、コピー アクションはアプリが追加の作業をすることなく完了するため、これが要求の最後になります。</span><span class="sxs-lookup"><span data-stu-id="0b553-123">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="0b553-124">ただし、アプリでコピー アクションの状態を表示することが必要な場合や、そのアクションがエラーなしで完了したことを確認する場合は、モニター URL を使用できます。</span><span class="sxs-lookup"><span data-stu-id="0b553-124">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="0b553-125">モニター URL から状態レポートを取得する</span><span class="sxs-lookup"><span data-stu-id="0b553-125">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="0b553-p105">コピー アクションのステータスを確認するために、アプリは前の応答で提供された URL に要求を送信します。 *注:* この要求には、認証は必要ありません。この URL の有効期間は短く、最初の呼び出し元に一意であるためです。</span><span class="sxs-lookup"><span data-stu-id="0b553-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0b553-128">サービスは、長時間実行のアクションがまだ進行中であるという情報を含む応答を返します。</span><span class="sxs-lookup"><span data-stu-id="0b553-128">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="0b553-p106">この情報は、コピー アクションの進行状況に関する最新情報をユーザーに提供するために使用できます。 アプリは、ステータスの最新情報を要求してアクションの進行状況を追跡するために、モニター URL へのポーリングを継続できます。</span><span class="sxs-lookup"><span data-stu-id="0b553-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="0b553-131">モニター URL から完了状態レポートを取得する</span><span class="sxs-lookup"><span data-stu-id="0b553-131">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="0b553-p107">コピー操作が完了してから数秒経過しています。 このときにアプリがモニター URL に要求を送信すると、完了したアクションの結果にリダイレクトする応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0b553-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0b553-134">アクションが完了すると、モニター サービスからの応答で、結果の resourceId が返されます。</span><span class="sxs-lookup"><span data-stu-id="0b553-134">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="0b553-135">完了した操作の結果を取得する</span><span class="sxs-lookup"><span data-stu-id="0b553-135">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="0b553-136">ジョブが完了すると、モニター URL が結果の resourceId を返します。ここでは、元のアイテムの新しいコピーを返します。</span><span class="sxs-lookup"><span data-stu-id="0b553-136">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="0b553-137">resourceId を使用してこの新しいアイテムに対処することができます。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="0b553-137">You can address this new item using the resourceId, for example:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b553-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0b553-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b553-139">C#</span><span class="sxs-lookup"><span data-stu-id="0b553-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b553-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b553-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b553-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="0b553-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

## <a name="supported-resources"></a><span data-ttu-id="0b553-142">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="0b553-142">Supported resources</span></span>

<span data-ttu-id="0b553-143">長時間実行アクションは、次の API メソッドでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0b553-143">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="0b553-144">**リソース**</span><span class="sxs-lookup"><span data-stu-id="0b553-144">**Resource**</span></span> | <span data-ttu-id="0b553-145">**API**</span><span class="sxs-lookup"><span data-stu-id="0b553-145">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="0b553-146">DriveItem</span><span class="sxs-lookup"><span data-stu-id="0b553-146">DriveItem</span></span> | [<span data-ttu-id="0b553-147">コピー</span><span class="sxs-lookup"><span data-stu-id="0b553-147">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="0b553-148">前提条件</span><span class="sxs-lookup"><span data-stu-id="0b553-148">Prerequisites</span></span>

<span data-ttu-id="0b553-149">長時間実行アクションの実行に必要な[アクセス許可](./permissions-reference.md)と同じアクセス許可は、長時間実行アクションの状態をクエリするときにも必要です。</span><span class="sxs-lookup"><span data-stu-id="0b553-149">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




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
