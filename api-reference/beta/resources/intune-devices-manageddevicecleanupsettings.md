---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者は、削除するデバイスを希望する場合は、ルールを定義します。
author: tfitzmac
ms.openlocfilehash: 84650c4d2d182fe0da30ced56786a2c0216a6358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304089"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="06151-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06151-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="06151-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06151-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06151-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06151-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06151-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06151-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06151-107">管理者は、削除するデバイスを希望する場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="06151-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="06151-108">Properties</span><span class="sxs-lookup"><span data-stu-id="06151-108">Properties</span></span>
|<span data-ttu-id="06151-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06151-109">Property</span></span>|<span data-ttu-id="06151-110">種類</span><span class="sxs-lookup"><span data-stu-id="06151-110">Type</span></span>|<span data-ttu-id="06151-111">説明</span><span class="sxs-lookup"><span data-stu-id="06151-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06151-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="06151-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="06151-113">String</span><span class="sxs-lookup"><span data-stu-id="06151-113">String</span></span>|<span data-ttu-id="06151-114">デバイスがない連絡した Intune 日数です。</span><span class="sxs-lookup"><span data-stu-id="06151-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06151-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06151-115">Relationships</span></span>
<span data-ttu-id="06151-116">なし</span><span class="sxs-lookup"><span data-stu-id="06151-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06151-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06151-117">JSON Representation</span></span>
<span data-ttu-id="06151-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06151-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





