---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482232"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="dd4a2-102">AsyncJobStatus リソース</span><span class="sxs-lookup"><span data-stu-id="dd4a2-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd4a2-103">このリソースは、非同期ジョブの進行状況に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="dd4a2-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="dd4a2-104">次の API 呼び出しは、**AsyncJobStatus** リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="dd4a2-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="dd4a2-105">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="dd4a2-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="dd4a2-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd4a2-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="dd4a2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd4a2-107">Properties</span></span>

| <span data-ttu-id="dd4a2-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="dd4a2-108">Property name</span></span>          | <span data-ttu-id="dd4a2-109">種類</span><span class="sxs-lookup"><span data-stu-id="dd4a2-109">Type</span></span>   | <span data-ttu-id="dd4a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="dd4a2-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="dd4a2-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="dd4a2-111">**percentageComplete**</span></span> | <span data-ttu-id="dd4a2-112">Double</span><span class="sxs-lookup"><span data-stu-id="dd4a2-112">Double</span></span> | <span data-ttu-id="dd4a2-113">達成率を示す 0 〜 100 の値。</span><span class="sxs-lookup"><span data-stu-id="dd4a2-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="dd4a2-114">**status**</span><span class="sxs-lookup"><span data-stu-id="dd4a2-114">**status**</span></span>             | <span data-ttu-id="dd4a2-115">String</span><span class="sxs-lookup"><span data-stu-id="dd4a2-115">String</span></span> | <span data-ttu-id="dd4a2-116">ジョブの状態に関する有効な値の列挙にマップされる文字列値。</span><span class="sxs-lookup"><span data-stu-id="dd4a2-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
