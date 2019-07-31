---
title: managedDeviceCleanupSettings リソースの種類
description: 管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 558c8f14f431bb10421ee77b6569f69560e8023f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968366"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="b4feb-103">managedDeviceCleanupSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4feb-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="b4feb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4feb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4feb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4feb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4feb-106">管理者がデバイスをクリーンアップする必要がある場合は、ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="b4feb-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="b4feb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4feb-107">Properties</span></span>
|<span data-ttu-id="b4feb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4feb-108">Property</span></span>|<span data-ttu-id="b4feb-109">型</span><span class="sxs-lookup"><span data-stu-id="b4feb-109">Type</span></span>|<span data-ttu-id="b4feb-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4feb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4feb-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="b4feb-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="b4feb-112">String</span><span class="sxs-lookup"><span data-stu-id="b4feb-112">String</span></span>|<span data-ttu-id="b4feb-113">デバイスが Intune に接続していない場合の日数。</span><span class="sxs-lookup"><span data-stu-id="b4feb-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4feb-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4feb-114">Relationships</span></span>
<span data-ttu-id="b4feb-115">なし</span><span class="sxs-lookup"><span data-stu-id="b4feb-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4feb-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4feb-116">JSON Representation</span></span>
<span data-ttu-id="b4feb-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4feb-117">Here is a JSON representation of the resource.</span></span>
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





