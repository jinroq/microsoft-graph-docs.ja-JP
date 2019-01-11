---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者は、削除するデバイスを希望する場合は、ルールを定義します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 755fc90b957427c4b9f8ee9007decea320141601
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808975"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="3ac05-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ac05-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="3ac05-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ac05-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ac05-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ac05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ac05-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ac05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ac05-107">管理者は、削除するデバイスを希望する場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="3ac05-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="3ac05-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ac05-108">Properties</span></span>
|<span data-ttu-id="3ac05-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ac05-109">Property</span></span>|<span data-ttu-id="3ac05-110">種類</span><span class="sxs-lookup"><span data-stu-id="3ac05-110">Type</span></span>|<span data-ttu-id="3ac05-111">説明</span><span class="sxs-lookup"><span data-stu-id="3ac05-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ac05-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="3ac05-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="3ac05-113">String</span><span class="sxs-lookup"><span data-stu-id="3ac05-113">String</span></span>|<span data-ttu-id="3ac05-114">デバイスがない連絡した Intune 日数です。</span><span class="sxs-lookup"><span data-stu-id="3ac05-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ac05-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ac05-115">Relationships</span></span>
<span data-ttu-id="3ac05-116">なし</span><span class="sxs-lookup"><span data-stu-id="3ac05-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ac05-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ac05-117">JSON Representation</span></span>
<span data-ttu-id="3ac05-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ac05-118">Here is a JSON representation of the resource.</span></span>
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





