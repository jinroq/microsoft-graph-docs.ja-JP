---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 9e444f0a92a2e28dfa571c51f08c886537701f3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343611"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="e2ea8-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2ea8-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="e2ea8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2ea8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2ea8-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2ea8-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e2ea8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2ea8-106">Properties</span></span>
|<span data-ttu-id="e2ea8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2ea8-107">Property</span></span>|<span data-ttu-id="e2ea8-108">種類</span><span class="sxs-lookup"><span data-stu-id="e2ea8-108">Type</span></span>|<span data-ttu-id="e2ea8-109">説明</span><span class="sxs-lookup"><span data-stu-id="e2ea8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ea8-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="e2ea8-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="e2ea8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ea8-111">Int32</span></span>|<span data-ttu-id="e2ea8-112">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="e2ea8-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="e2ea8-113">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="e2ea8-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="e2ea8-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="e2ea8-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="e2ea8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2ea8-115">Boolean</span></span>|<span data-ttu-id="e2ea8-116">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="e2ea8-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="e2ea8-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="e2ea8-117">secureByDefault</span></span>|<span data-ttu-id="e2ea8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2ea8-118">Boolean</span></span>|<span data-ttu-id="e2ea8-119">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="e2ea8-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ea8-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2ea8-120">Relationships</span></span>
<span data-ttu-id="e2ea8-121">なし</span><span class="sxs-lookup"><span data-stu-id="e2ea8-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2ea8-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2ea8-122">JSON Representation</span></span>
<span data-ttu-id="e2ea8-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2ea8-123">Here is a JSON representation of the resource.</span></span>
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



