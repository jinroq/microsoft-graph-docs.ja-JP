---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャーのクライアントの正常性の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 618282f2a061ec8327ff93d1af441e088523260b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983240"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="e5d5b-103">configurationManagerClientHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5d5b-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="e5d5b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5d5b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d5b-106">構成マネージャーのクライアントの正常性の状態</span><span class="sxs-lookup"><span data-stu-id="e5d5b-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="e5d5b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5d5b-107">Properties</span></span>
|<span data-ttu-id="e5d5b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5d5b-108">Property</span></span>|<span data-ttu-id="e5d5b-109">型</span><span class="sxs-lookup"><span data-stu-id="e5d5b-109">Type</span></span>|<span data-ttu-id="e5d5b-110">説明</span><span class="sxs-lookup"><span data-stu-id="e5d5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d5b-111">state</span><span class="sxs-lookup"><span data-stu-id="e5d5b-111">state</span></span>|[<span data-ttu-id="e5d5b-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="e5d5b-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="e5d5b-113">現在の構成マネージャークライアントの状態。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-113">Current configuration manager client state.</span></span> <span data-ttu-id="e5d5b-114">可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="e5d5b-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="e5d5b-115">errorCode</span></span>|<span data-ttu-id="e5d5b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d5b-116">Int32</span></span>|<span data-ttu-id="e5d5b-117">失敗状態のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-117">Error code for failed state.</span></span>|
|<span data-ttu-id="e5d5b-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d5b-118">lastSyncDateTime</span></span>|<span data-ttu-id="e5d5b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d5b-119">DateTimeOffset</span></span>|<span data-ttu-id="e5d5b-120">Configuration manager 管理ポイントとの前回の同期を示す Datetime。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5d5b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5d5b-121">Relationships</span></span>
<span data-ttu-id="e5d5b-122">なし</span><span class="sxs-lookup"><span data-stu-id="e5d5b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d5b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5d5b-123">JSON Representation</span></span>
<span data-ttu-id="e5d5b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5d5b-124">Here is a JSON representation of the resource.</span></span>
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





