---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: ee7cc92bff47edc3a1a15b5f27cb2f5afe061d4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510212"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="afc13-102">AsyncJobStatus リソース</span><span class="sxs-lookup"><span data-stu-id="afc13-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afc13-103">このリソースは、非同期ジョブの進行状況に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="afc13-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="afc13-104">次の API 呼び出しは、**AsyncJobStatus** リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="afc13-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="afc13-105">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="afc13-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="afc13-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="afc13-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="afc13-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afc13-107">Properties</span></span>

| <span data-ttu-id="afc13-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="afc13-108">Property name</span></span>          | <span data-ttu-id="afc13-109">型</span><span class="sxs-lookup"><span data-stu-id="afc13-109">Type</span></span>   | <span data-ttu-id="afc13-110">説明</span><span class="sxs-lookup"><span data-stu-id="afc13-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="afc13-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="afc13-111">**percentageComplete**</span></span> | <span data-ttu-id="afc13-112">Double</span><span class="sxs-lookup"><span data-stu-id="afc13-112">Double</span></span> | <span data-ttu-id="afc13-113">達成率を示す 0 〜 100 の値。</span><span class="sxs-lookup"><span data-stu-id="afc13-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="afc13-114">**status**</span><span class="sxs-lookup"><span data-stu-id="afc13-114">**status**</span></span>             | <span data-ttu-id="afc13-115">String</span><span class="sxs-lookup"><span data-stu-id="afc13-115">String</span></span> | <span data-ttu-id="afc13-116">ジョブの状態に関する有効な値の列挙にマップされる文字列値。</span><span class="sxs-lookup"><span data-stu-id="afc13-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

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
