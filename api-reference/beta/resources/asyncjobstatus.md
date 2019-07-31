---
author: JeremyKelley
description: このリソースは、非同期ジョブの進行状況に関する情報を提供します。
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e8a745a6ab03728eb879767c6af45a423f151d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974305"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="6cdf9-103">AsyncJobStatus リソース</span><span class="sxs-lookup"><span data-stu-id="6cdf9-103">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cdf9-104">このリソースは、非同期ジョブの進行状況に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cdf9-104">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="6cdf9-105">次の API 呼び出しは、**AsyncJobStatus** リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="6cdf9-105">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="6cdf9-106">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="6cdf9-106">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="6cdf9-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cdf9-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="6cdf9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cdf9-108">Properties</span></span>

| <span data-ttu-id="6cdf9-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6cdf9-109">Property name</span></span>          | <span data-ttu-id="6cdf9-110">種類</span><span class="sxs-lookup"><span data-stu-id="6cdf9-110">Type</span></span>   | <span data-ttu-id="6cdf9-111">説明</span><span class="sxs-lookup"><span data-stu-id="6cdf9-111">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="6cdf9-112">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="6cdf9-112">**percentageComplete**</span></span> | <span data-ttu-id="6cdf9-113">Double</span><span class="sxs-lookup"><span data-stu-id="6cdf9-113">Double</span></span> | <span data-ttu-id="6cdf9-114">達成率を示す 0 〜 100 の値。</span><span class="sxs-lookup"><span data-stu-id="6cdf9-114">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="6cdf9-115">**status**</span><span class="sxs-lookup"><span data-stu-id="6cdf9-115">**status**</span></span>             | <span data-ttu-id="6cdf9-116">String</span><span class="sxs-lookup"><span data-stu-id="6cdf9-116">String</span></span> | <span data-ttu-id="6cdf9-117">ジョブの状態に関する有効な値の列挙にマップされる文字列値。</span><span class="sxs-lookup"><span data-stu-id="6cdf9-117">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
