---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリケーションの Windows 10 強制更新のスケジュール
ms.openlocfilehash: 89bbee05c3a76df6999c0d3d16caa591f903c45a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070384"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="e7de1-103">windows10AppsForceUpdateSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7de1-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="e7de1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7de1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7de1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7de1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7de1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7de1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7de1-107">アプリケーションの Windows 10 強制更新のスケジュール</span><span class="sxs-lookup"><span data-stu-id="e7de1-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="e7de1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7de1-108">Properties</span></span>
|<span data-ttu-id="e7de1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7de1-109">Property</span></span>|<span data-ttu-id="e7de1-110">型</span><span class="sxs-lookup"><span data-stu-id="e7de1-110">Type</span></span>|<span data-ttu-id="e7de1-111">説明</span><span class="sxs-lookup"><span data-stu-id="e7de1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7de1-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e7de1-112">startDateTime</span></span>|<span data-ttu-id="e7de1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7de1-113">DateTimeOffset</span></span>|<span data-ttu-id="e7de1-114">力の開始時刻を再起動します。</span><span class="sxs-lookup"><span data-stu-id="e7de1-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="e7de1-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="e7de1-115">recurrence</span></span>|[<span data-ttu-id="e7de1-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="e7de1-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="e7de1-117">定期的なスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="e7de1-117">Recurrence schedule.</span></span> <span data-ttu-id="e7de1-118">可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="e7de1-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="e7de1-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="e7de1-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="e7de1-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="e7de1-120">Boolean</span></span>|<span data-ttu-id="e7de1-121">True の場合、タスクはすぐに実行させるまでは、他の次の反復の実行の場合です。</span><span class="sxs-lookup"><span data-stu-id="e7de1-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7de1-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7de1-122">Relationships</span></span>
<span data-ttu-id="e7de1-123">なし</span><span class="sxs-lookup"><span data-stu-id="e7de1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7de1-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7de1-124">JSON Representation</span></span>
<span data-ttu-id="e7de1-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7de1-125">Here is a JSON representation of the resource.</span></span>
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





