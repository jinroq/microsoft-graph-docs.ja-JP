---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャーのクライアントの正常性の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9356a4aac345137ba93dc85914ddc1a12e44233f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968555"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="59f14-103">configurationManagerClientHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59f14-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="59f14-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59f14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59f14-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59f14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59f14-106">構成マネージャーのクライアントの正常性の状態</span><span class="sxs-lookup"><span data-stu-id="59f14-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="59f14-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59f14-107">Properties</span></span>
|<span data-ttu-id="59f14-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59f14-108">Property</span></span>|<span data-ttu-id="59f14-109">型</span><span class="sxs-lookup"><span data-stu-id="59f14-109">Type</span></span>|<span data-ttu-id="59f14-110">説明</span><span class="sxs-lookup"><span data-stu-id="59f14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59f14-111">state</span><span class="sxs-lookup"><span data-stu-id="59f14-111">state</span></span>|[<span data-ttu-id="59f14-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="59f14-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="59f14-113">現在の構成マネージャークライアントの状態。</span><span class="sxs-lookup"><span data-stu-id="59f14-113">Current configuration manager client state.</span></span> <span data-ttu-id="59f14-114">可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。</span><span class="sxs-lookup"><span data-stu-id="59f14-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="59f14-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="59f14-115">errorCode</span></span>|<span data-ttu-id="59f14-116">Int32</span><span class="sxs-lookup"><span data-stu-id="59f14-116">Int32</span></span>|<span data-ttu-id="59f14-117">失敗状態のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="59f14-117">Error code for failed state.</span></span>|
|<span data-ttu-id="59f14-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="59f14-118">lastSyncDateTime</span></span>|<span data-ttu-id="59f14-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59f14-119">DateTimeOffset</span></span>|<span data-ttu-id="59f14-120">Configuration manager 管理ポイントとの前回の同期を示す Datetime。</span><span class="sxs-lookup"><span data-stu-id="59f14-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59f14-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59f14-121">Relationships</span></span>
<span data-ttu-id="59f14-122">なし</span><span class="sxs-lookup"><span data-stu-id="59f14-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59f14-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59f14-123">JSON Representation</span></span>
<span data-ttu-id="59f14-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59f14-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





