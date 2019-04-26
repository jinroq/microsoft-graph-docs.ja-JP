---
title: 同期の進行状況リソースの種類
description: 完了までの同期ジョブの進行状況を表します。
localization_priority: Normal
ms.openlocfilehash: d05193c7c242dc3f890aba6f4fcec5a8badc087f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340015"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="d1dbb-103">同期の進行状況リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1dbb-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1dbb-104">完了までの[同期ジョブ](synchronization-synchronizationjob.md)の進行状況を表します。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="d1dbb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1dbb-105">Properties</span></span>

| <span data-ttu-id="d1dbb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1dbb-106">Property</span></span>                              | <span data-ttu-id="d1dbb-107">型</span><span class="sxs-lookup"><span data-stu-id="d1dbb-107">Type</span></span>      | <span data-ttu-id="d1dbb-108">説明</span><span class="sxs-lookup"><span data-stu-id="d1dbb-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="d1dbb-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="d1dbb-109">completedUnits</span></span>|<span data-ttu-id="d1dbb-110">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dbb-110">Int32</span></span>|<span data-ttu-id="d1dbb-111">進行状況の比率の分子。既に処理されている変更の単位数。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="d1dbb-112">進行法</span><span class="sxs-lookup"><span data-stu-id="d1dbb-112">progressObservationDateTime</span></span>|<span data-ttu-id="d1dbb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1dbb-113">DateTimeOffset</span></span>|<span data-ttu-id="d1dbb-114">進行状況の監視時間 (分単位で UTC からのオフセット)。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="d1dbb-115">totalunits</span><span class="sxs-lookup"><span data-stu-id="d1dbb-115">totalUnits</span></span>|<span data-ttu-id="d1dbb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dbb-116">Int32</span></span>|<span data-ttu-id="d1dbb-117">進行状況の比率の分母。同期を実行するために処理される変更の単位数。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="d1dbb-118">」</span><span class="sxs-lookup"><span data-stu-id="d1dbb-118">units</span></span>|<span data-ttu-id="d1dbb-119">String</span><span class="sxs-lookup"><span data-stu-id="d1dbb-119">String</span></span>|<span data-ttu-id="d1dbb-120">単位の説明 (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="d1dbb-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1dbb-121">JSON representation</span></span>

<span data-ttu-id="d1dbb-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1dbb-122">The following is a JSON representation of the resource.</span></span>

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
