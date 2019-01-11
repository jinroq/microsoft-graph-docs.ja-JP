---
title: synchronizationProgress リソースの種類
description: 完了するまで、synchronizationJob の進行状況を表します。
localization_priority: Normal
ms.openlocfilehash: 3c1168cdac6a073842cb5e08d165572591d2d8e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885387"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="64a5c-103">synchronizationProgress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64a5c-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="64a5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64a5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64a5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64a5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64a5c-106">完了するまでの[synchronizationJob](synchronization-synchronizationjob.md)の進行状況を表します。</span><span class="sxs-lookup"><span data-stu-id="64a5c-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="64a5c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64a5c-107">Properties</span></span>

| <span data-ttu-id="64a5c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64a5c-108">Property</span></span>                              | <span data-ttu-id="64a5c-109">種類</span><span class="sxs-lookup"><span data-stu-id="64a5c-109">Type</span></span>      | <span data-ttu-id="64a5c-110">説明</span><span class="sxs-lookup"><span data-stu-id="64a5c-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="64a5c-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="64a5c-111">completedUnits</span></span>|<span data-ttu-id="64a5c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="64a5c-112">Int32</span></span>|<span data-ttu-id="64a5c-113">分子の進行状況の比率です。既に処理された変更単位の数です。</span><span class="sxs-lookup"><span data-stu-id="64a5c-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="64a5c-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="64a5c-114">progressObservationDateTime</span></span>|<span data-ttu-id="64a5c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64a5c-115">DateTimeOffset</span></span>|<span data-ttu-id="64a5c-116">分 UTC からのオフセットとしての進行状況の監視の時間です。</span><span class="sxs-lookup"><span data-stu-id="64a5c-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="64a5c-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="64a5c-117">totalUnits</span></span>|<span data-ttu-id="64a5c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="64a5c-118">Int32</span></span>|<span data-ttu-id="64a5c-119">分母の進行状況の比率です。変更の同期を実行する処理の単位数を示します。</span><span class="sxs-lookup"><span data-stu-id="64a5c-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="64a5c-120">単位</span><span class="sxs-lookup"><span data-stu-id="64a5c-120">units</span></span>|<span data-ttu-id="64a5c-121">String</span><span class="sxs-lookup"><span data-stu-id="64a5c-121">String</span></span>|<span data-ttu-id="64a5c-122">単位のオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="64a5c-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="64a5c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64a5c-123">JSON representation</span></span>

<span data-ttu-id="64a5c-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64a5c-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
