---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリの Windows 10 強制更新スケジュール
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c8c76c08c434ab9c5e3506339e53cda41156e09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572263"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="a20c3-103">windows10AppsForceUpdateSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a20c3-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="a20c3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a20c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a20c3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a20c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a20c3-106">アプリの Windows 10 強制更新スケジュール</span><span class="sxs-lookup"><span data-stu-id="a20c3-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="a20c3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a20c3-107">Properties</span></span>
|<span data-ttu-id="a20c3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a20c3-108">Property</span></span>|<span data-ttu-id="a20c3-109">型</span><span class="sxs-lookup"><span data-stu-id="a20c3-109">Type</span></span>|<span data-ttu-id="a20c3-110">説明</span><span class="sxs-lookup"><span data-stu-id="a20c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20c3-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a20c3-111">startDateTime</span></span>|<span data-ttu-id="a20c3-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20c3-112">DateTimeOffset</span></span>|<span data-ttu-id="a20c3-113">強制再起動の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="a20c3-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="a20c3-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="a20c3-114">recurrence</span></span>|[<span data-ttu-id="a20c3-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a20c3-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="a20c3-116">定期的なスケジュール。</span><span class="sxs-lookup"><span data-stu-id="a20c3-116">Recurrence schedule.</span></span> <span data-ttu-id="a20c3-117">使用可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="a20c3-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="a20c3-118">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a20c3-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="a20c3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a20c3-119">Boolean</span></span>|<span data-ttu-id="a20c3-120">true の場合は、StartDateTime が過去の場合はすぐにタスクを実行します。それ以外の場合は、次の定期的なパターンが実行されます。</span><span class="sxs-lookup"><span data-stu-id="a20c3-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20c3-121">関係</span><span class="sxs-lookup"><span data-stu-id="a20c3-121">Relationships</span></span>
<span data-ttu-id="a20c3-122">なし</span><span class="sxs-lookup"><span data-stu-id="a20c3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a20c3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a20c3-123">JSON Representation</span></span>
<span data-ttu-id="a20c3-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a20c3-124">Here is a JSON representation of the resource.</span></span>
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





