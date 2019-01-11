---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリケーションの Windows 10 強制更新のスケジュール
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef8a0583bd02a62a4461a3415aae86833e24e948
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811236"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="644fa-103">windows10AppsForceUpdateSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="644fa-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="644fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="644fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="644fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="644fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="644fa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="644fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="644fa-107">アプリケーションの Windows 10 強制更新のスケジュール</span><span class="sxs-lookup"><span data-stu-id="644fa-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="644fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644fa-108">Properties</span></span>
|<span data-ttu-id="644fa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644fa-109">Property</span></span>|<span data-ttu-id="644fa-110">種類</span><span class="sxs-lookup"><span data-stu-id="644fa-110">Type</span></span>|<span data-ttu-id="644fa-111">説明</span><span class="sxs-lookup"><span data-stu-id="644fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="644fa-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="644fa-112">startDateTime</span></span>|<span data-ttu-id="644fa-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644fa-113">DateTimeOffset</span></span>|<span data-ttu-id="644fa-114">力の開始時刻を再起動します。</span><span class="sxs-lookup"><span data-stu-id="644fa-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="644fa-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="644fa-115">recurrence</span></span>|[<span data-ttu-id="644fa-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="644fa-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="644fa-117">定期的なスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="644fa-117">Recurrence schedule.</span></span> <span data-ttu-id="644fa-118">可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="644fa-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="644fa-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="644fa-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="644fa-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="644fa-120">Boolean</span></span>|<span data-ttu-id="644fa-121">True の場合、タスクはすぐに実行させるまでは、他の次の反復の実行の場合です。</span><span class="sxs-lookup"><span data-stu-id="644fa-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="644fa-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="644fa-122">Relationships</span></span>
<span data-ttu-id="644fa-123">なし</span><span class="sxs-lookup"><span data-stu-id="644fa-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="644fa-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="644fa-124">JSON Representation</span></span>
<span data-ttu-id="644fa-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="644fa-125">Here is a JSON representation of the resource.</span></span>
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





