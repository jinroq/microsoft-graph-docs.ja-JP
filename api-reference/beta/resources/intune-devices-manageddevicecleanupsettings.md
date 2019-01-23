---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者は、削除するデバイスを希望する場合は、ルールを定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bf756072dcc3cd13bda2fda59b8688b63f3cd43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424568"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="c7eca-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7eca-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="c7eca-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7eca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7eca-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7eca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7eca-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7eca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7eca-107">管理者は、削除するデバイスを希望する場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="c7eca-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="c7eca-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7eca-108">Properties</span></span>
|<span data-ttu-id="c7eca-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7eca-109">Property</span></span>|<span data-ttu-id="c7eca-110">型</span><span class="sxs-lookup"><span data-stu-id="c7eca-110">Type</span></span>|<span data-ttu-id="c7eca-111">説明</span><span class="sxs-lookup"><span data-stu-id="c7eca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7eca-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="c7eca-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="c7eca-113">String</span><span class="sxs-lookup"><span data-stu-id="c7eca-113">String</span></span>|<span data-ttu-id="c7eca-114">デバイスがない連絡した Intune 日数です。</span><span class="sxs-lookup"><span data-stu-id="c7eca-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7eca-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7eca-115">Relationships</span></span>
<span data-ttu-id="c7eca-116">なし</span><span class="sxs-lookup"><span data-stu-id="c7eca-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7eca-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7eca-117">JSON Representation</span></span>
<span data-ttu-id="c7eca-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7eca-118">Here is a JSON representation of the resource.</span></span>
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




