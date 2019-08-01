---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d990271b611fdb088975e155637834dc9261580
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028419"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="f0a90-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0a90-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="f0a90-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0a90-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a90-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f0a90-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f0a90-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0a90-106">Properties</span></span>
|<span data-ttu-id="f0a90-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0a90-107">Property</span></span>|<span data-ttu-id="f0a90-108">型</span><span class="sxs-lookup"><span data-stu-id="f0a90-108">Type</span></span>|<span data-ttu-id="f0a90-109">説明</span><span class="sxs-lookup"><span data-stu-id="f0a90-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a90-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="f0a90-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="f0a90-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a90-111">Int32</span></span>|<span data-ttu-id="f0a90-112">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="f0a90-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="f0a90-113">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="f0a90-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="f0a90-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="f0a90-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="f0a90-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0a90-115">Boolean</span></span>|<span data-ttu-id="f0a90-116">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="f0a90-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="f0a90-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="f0a90-117">secureByDefault</span></span>|<span data-ttu-id="f0a90-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0a90-118">Boolean</span></span>|<span data-ttu-id="f0a90-119">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="f0a90-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0a90-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0a90-120">Relationships</span></span>
<span data-ttu-id="f0a90-121">なし</span><span class="sxs-lookup"><span data-stu-id="f0a90-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0a90-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0a90-122">JSON Representation</span></span>
<span data-ttu-id="f0a90-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0a90-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



