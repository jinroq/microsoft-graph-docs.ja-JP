---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリの Windows 10 強制更新スケジュール
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e5d7cf1b4e32543b9937603e1b7b782e39410cc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944447"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="23dcd-103">windows10AppsForceUpdateSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23dcd-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="23dcd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23dcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23dcd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23dcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23dcd-106">アプリの Windows 10 強制更新スケジュール</span><span class="sxs-lookup"><span data-stu-id="23dcd-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="23dcd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23dcd-107">Properties</span></span>
|<span data-ttu-id="23dcd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23dcd-108">Property</span></span>|<span data-ttu-id="23dcd-109">型</span><span class="sxs-lookup"><span data-stu-id="23dcd-109">Type</span></span>|<span data-ttu-id="23dcd-110">説明</span><span class="sxs-lookup"><span data-stu-id="23dcd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23dcd-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="23dcd-111">startDateTime</span></span>|<span data-ttu-id="23dcd-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23dcd-112">DateTimeOffset</span></span>|<span data-ttu-id="23dcd-113">強制再起動の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="23dcd-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="23dcd-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="23dcd-114">recurrence</span></span>|[<span data-ttu-id="23dcd-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="23dcd-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="23dcd-116">定期的なスケジュール。</span><span class="sxs-lookup"><span data-stu-id="23dcd-116">Recurrence schedule.</span></span> <span data-ttu-id="23dcd-117">使用可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="23dcd-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="23dcd-118">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="23dcd-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="23dcd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="23dcd-119">Boolean</span></span>|<span data-ttu-id="23dcd-120">True の場合は、StartDateTime が過去の場合はすぐにタスクを実行します。それ以外の場合は、次の定期的なパターンが実行されます。</span><span class="sxs-lookup"><span data-stu-id="23dcd-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23dcd-121">関係</span><span class="sxs-lookup"><span data-stu-id="23dcd-121">Relationships</span></span>
<span data-ttu-id="23dcd-122">なし</span><span class="sxs-lookup"><span data-stu-id="23dcd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23dcd-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23dcd-123">JSON Representation</span></span>
<span data-ttu-id="23dcd-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23dcd-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




