---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者は、削除するデバイスを希望する場合は、ルールを定義します。
ms.openlocfilehash: f7782ac9d6571b58c8ed1e7964637736fcb5f3d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070505"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="beca3-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="beca3-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="beca3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="beca3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beca3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beca3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beca3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="beca3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beca3-107">管理者は、削除するデバイスを希望する場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="beca3-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="beca3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="beca3-108">Properties</span></span>
|<span data-ttu-id="beca3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="beca3-109">Property</span></span>|<span data-ttu-id="beca3-110">型</span><span class="sxs-lookup"><span data-stu-id="beca3-110">Type</span></span>|<span data-ttu-id="beca3-111">説明</span><span class="sxs-lookup"><span data-stu-id="beca3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beca3-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="beca3-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="beca3-113">String</span><span class="sxs-lookup"><span data-stu-id="beca3-113">String</span></span>|<span data-ttu-id="beca3-114">デバイスがない連絡した Intune 日数です。</span><span class="sxs-lookup"><span data-stu-id="beca3-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="beca3-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="beca3-115">Relationships</span></span>
<span data-ttu-id="beca3-116">なし</span><span class="sxs-lookup"><span data-stu-id="beca3-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="beca3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="beca3-117">JSON Representation</span></span>
<span data-ttu-id="beca3-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="beca3-118">Here is a JSON representation of the resource.</span></span>
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





