---
title: 同期の進行状況リソースの種類
description: 完了までの同期ジョブの進行状況を表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd1292d34abdc745075e030609d3f28a17b2431a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964642"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="a9594-103">同期の進行状況リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9594-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9594-104">完了までの[同期ジョブ](synchronization-synchronizationjob.md)の進行状況を表します。</span><span class="sxs-lookup"><span data-stu-id="a9594-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="a9594-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9594-105">Properties</span></span>

| <span data-ttu-id="a9594-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9594-106">Property</span></span>                              | <span data-ttu-id="a9594-107">型</span><span class="sxs-lookup"><span data-stu-id="a9594-107">Type</span></span>      | <span data-ttu-id="a9594-108">説明</span><span class="sxs-lookup"><span data-stu-id="a9594-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="a9594-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="a9594-109">completedUnits</span></span>|<span data-ttu-id="a9594-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a9594-110">Int32</span></span>|<span data-ttu-id="a9594-111">進行状況の比率の分子。既に処理されている変更の単位数。</span><span class="sxs-lookup"><span data-stu-id="a9594-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="a9594-112">進行法</span><span class="sxs-lookup"><span data-stu-id="a9594-112">progressObservationDateTime</span></span>|<span data-ttu-id="a9594-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9594-113">DateTimeOffset</span></span>|<span data-ttu-id="a9594-114">進行状況の監視時間 (分単位で UTC からのオフセット)。</span><span class="sxs-lookup"><span data-stu-id="a9594-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="a9594-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="a9594-115">totalUnits</span></span>|<span data-ttu-id="a9594-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a9594-116">Int32</span></span>|<span data-ttu-id="a9594-117">進行状況の比率の分母。同期を実行するために処理される変更の単位数。</span><span class="sxs-lookup"><span data-stu-id="a9594-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="a9594-118">」</span><span class="sxs-lookup"><span data-stu-id="a9594-118">units</span></span>|<span data-ttu-id="a9594-119">String</span><span class="sxs-lookup"><span data-stu-id="a9594-119">String</span></span>|<span data-ttu-id="a9594-120">単位の説明 (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="a9594-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="a9594-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9594-121">JSON representation</span></span>

<span data-ttu-id="a9594-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9594-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
