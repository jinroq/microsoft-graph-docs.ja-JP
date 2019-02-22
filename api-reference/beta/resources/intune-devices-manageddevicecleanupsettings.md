---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76abaf4cb06156881a530d50e3322e649eedde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148483"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="83354-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83354-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="83354-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83354-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83354-106">管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="83354-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="83354-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83354-107">Properties</span></span>
|<span data-ttu-id="83354-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83354-108">Property</span></span>|<span data-ttu-id="83354-109">型</span><span class="sxs-lookup"><span data-stu-id="83354-109">Type</span></span>|<span data-ttu-id="83354-110">説明</span><span class="sxs-lookup"><span data-stu-id="83354-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83354-111">deviceinactivitybeforeretirementindays</span><span class="sxs-lookup"><span data-stu-id="83354-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="83354-112">String</span><span class="sxs-lookup"><span data-stu-id="83354-112">String</span></span>|<span data-ttu-id="83354-113">デバイスが Intune に接続していない場合の日数。</span><span class="sxs-lookup"><span data-stu-id="83354-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83354-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83354-114">Relationships</span></span>
<span data-ttu-id="83354-115">なし</span><span class="sxs-lookup"><span data-stu-id="83354-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83354-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83354-116">JSON Representation</span></span>
<span data-ttu-id="83354-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83354-117">Here is a JSON representation of the resource.</span></span>
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




