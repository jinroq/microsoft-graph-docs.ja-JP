---
title: synchronizationProgress リソースの種類
description: 完了するまで、synchronizationJob の進行状況を表します。
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640071"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="1fbfd-103">synchronizationProgress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1fbfd-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fbfd-104">完了するまでの[synchronizationJob](synchronization-synchronizationjob.md)の進行状況を表します。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="1fbfd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fbfd-105">Properties</span></span>

| <span data-ttu-id="1fbfd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fbfd-106">Property</span></span>                              | <span data-ttu-id="1fbfd-107">型</span><span class="sxs-lookup"><span data-stu-id="1fbfd-107">Type</span></span>      | <span data-ttu-id="1fbfd-108">説明</span><span class="sxs-lookup"><span data-stu-id="1fbfd-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="1fbfd-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="1fbfd-109">completedUnits</span></span>|<span data-ttu-id="1fbfd-110">Int32</span><span class="sxs-lookup"><span data-stu-id="1fbfd-110">Int32</span></span>|<span data-ttu-id="1fbfd-111">分子の進行状況の比率です。既に処理された変更単位の数です。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="1fbfd-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="1fbfd-112">progressObservationDateTime</span></span>|<span data-ttu-id="1fbfd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fbfd-113">DateTimeOffset</span></span>|<span data-ttu-id="1fbfd-114">分 UTC からのオフセットとしての進行状況の監視の時間です。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="1fbfd-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="1fbfd-115">totalUnits</span></span>|<span data-ttu-id="1fbfd-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1fbfd-116">Int32</span></span>|<span data-ttu-id="1fbfd-117">分母の進行状況の比率です。変更の同期を実行する処理の単位数を示します。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="1fbfd-118">単位</span><span class="sxs-lookup"><span data-stu-id="1fbfd-118">units</span></span>|<span data-ttu-id="1fbfd-119">String</span><span class="sxs-lookup"><span data-stu-id="1fbfd-119">String</span></span>|<span data-ttu-id="1fbfd-120">単位のオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="1fbfd-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1fbfd-121">JSON representation</span></span>

<span data-ttu-id="1fbfd-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1fbfd-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
