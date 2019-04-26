---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328651"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="06037-102">AsyncJobStatus リソース</span><span class="sxs-lookup"><span data-stu-id="06037-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06037-103">このリソースは、非同期ジョブの進行状況に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="06037-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="06037-104">次の API 呼び出しは、**AsyncJobStatus** リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="06037-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="06037-105">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="06037-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="06037-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06037-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="06037-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06037-107">Properties</span></span>

| <span data-ttu-id="06037-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="06037-108">Property name</span></span>          | <span data-ttu-id="06037-109">種類</span><span class="sxs-lookup"><span data-stu-id="06037-109">Type</span></span>   | <span data-ttu-id="06037-110">説明</span><span class="sxs-lookup"><span data-stu-id="06037-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="06037-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="06037-111">**percentageComplete**</span></span> | <span data-ttu-id="06037-112">Double</span><span class="sxs-lookup"><span data-stu-id="06037-112">Double</span></span> | <span data-ttu-id="06037-113">達成率を示す 0 〜 100 の値。</span><span class="sxs-lookup"><span data-stu-id="06037-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="06037-114">**status**</span><span class="sxs-lookup"><span data-stu-id="06037-114">**status**</span></span>             | <span data-ttu-id="06037-115">String</span><span class="sxs-lookup"><span data-stu-id="06037-115">String</span></span> | <span data-ttu-id="06037-116">ジョブの状態に関する有効な値の列挙にマップされる文字列値。</span><span class="sxs-lookup"><span data-stu-id="06037-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
