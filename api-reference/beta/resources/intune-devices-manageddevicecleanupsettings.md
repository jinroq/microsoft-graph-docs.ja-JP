---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者は、削除するデバイスを希望する場合は、ルールを定義します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 334b561ffa19d4161553f761ce65b7da7d9dbcfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961898"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="c0298-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0298-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="c0298-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0298-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0298-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0298-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0298-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0298-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0298-107">管理者は、削除するデバイスを希望する場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="c0298-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="c0298-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0298-108">Properties</span></span>
|<span data-ttu-id="c0298-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0298-109">Property</span></span>|<span data-ttu-id="c0298-110">種類</span><span class="sxs-lookup"><span data-stu-id="c0298-110">Type</span></span>|<span data-ttu-id="c0298-111">説明</span><span class="sxs-lookup"><span data-stu-id="c0298-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0298-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="c0298-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="c0298-113">String</span><span class="sxs-lookup"><span data-stu-id="c0298-113">String</span></span>|<span data-ttu-id="c0298-114">デバイスがない連絡した Intune 日数です。</span><span class="sxs-lookup"><span data-stu-id="c0298-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0298-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0298-115">Relationships</span></span>
<span data-ttu-id="c0298-116">なし</span><span class="sxs-lookup"><span data-stu-id="c0298-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0298-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0298-117">JSON Representation</span></span>
<span data-ttu-id="c0298-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0298-118">Here is a JSON representation of the resource.</span></span>
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





