---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
ms.openlocfilehash: 9e0f95802f9f75930384ab1534bf4c519fd9cfeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066808"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="abf9e-102">AsyncJobStatus リソース</span><span class="sxs-lookup"><span data-stu-id="abf9e-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="abf9e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abf9e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abf9e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abf9e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abf9e-105">このリソースは、非同期ジョブの進行状況に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="abf9e-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="abf9e-106">次の API 呼び出しは、**AsyncJobStatus** リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="abf9e-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="abf9e-107">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="abf9e-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="abf9e-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abf9e-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="abf9e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abf9e-109">Properties</span></span>

| <span data-ttu-id="abf9e-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="abf9e-110">Property name</span></span>          | <span data-ttu-id="abf9e-111">型</span><span class="sxs-lookup"><span data-stu-id="abf9e-111">Type</span></span>   | <span data-ttu-id="abf9e-112">説明</span><span class="sxs-lookup"><span data-stu-id="abf9e-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="abf9e-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="abf9e-113">**percentageComplete**</span></span> | <span data-ttu-id="abf9e-114">Double</span><span class="sxs-lookup"><span data-stu-id="abf9e-114">Double</span></span> | <span data-ttu-id="abf9e-115">達成率を示す 0 〜 100 の値。</span><span class="sxs-lookup"><span data-stu-id="abf9e-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="abf9e-116">**status**</span><span class="sxs-lookup"><span data-stu-id="abf9e-116">**status**</span></span>             | <span data-ttu-id="abf9e-117">String</span><span class="sxs-lookup"><span data-stu-id="abf9e-117">String</span></span> | <span data-ttu-id="abf9e-118">ジョブの状態に関する有効な値の列挙にマップされる文字列値。</span><span class="sxs-lookup"><span data-stu-id="abf9e-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
