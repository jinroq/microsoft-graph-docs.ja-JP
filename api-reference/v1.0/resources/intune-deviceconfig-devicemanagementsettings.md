---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3742262f2d17cdac1344379b39b4891b5b9919ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830591"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="ae1e5-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae1e5-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="ae1e5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae1e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae1e5-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ae1e5-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ae1e5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae1e5-106">Properties</span></span>
|<span data-ttu-id="ae1e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae1e5-107">Property</span></span>|<span data-ttu-id="ae1e5-108">種類</span><span class="sxs-lookup"><span data-stu-id="ae1e5-108">Type</span></span>|<span data-ttu-id="ae1e5-109">説明</span><span class="sxs-lookup"><span data-stu-id="ae1e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1e5-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="ae1e5-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="ae1e5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ae1e5-111">Int32</span></span>|<span data-ttu-id="ae1e5-112">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="ae1e5-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="ae1e5-113">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="ae1e5-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="ae1e5-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="ae1e5-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="ae1e5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1e5-115">Boolean</span></span>|<span data-ttu-id="ae1e5-116">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="ae1e5-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="ae1e5-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="ae1e5-117">secureByDefault</span></span>|<span data-ttu-id="ae1e5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae1e5-118">Boolean</span></span>|<span data-ttu-id="ae1e5-119">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="ae1e5-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae1e5-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae1e5-120">Relationships</span></span>
<span data-ttu-id="ae1e5-121">なし</span><span class="sxs-lookup"><span data-stu-id="ae1e5-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae1e5-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae1e5-122">JSON Representation</span></span>
<span data-ttu-id="ae1e5-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae1e5-123">Here is a JSON representation of the resource.</span></span>
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



