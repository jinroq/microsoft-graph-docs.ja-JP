---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャー クライアントの正常性状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425828"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="1eb1a-103">configurationManagerClientHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1eb1a-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="1eb1a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1eb1a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1eb1a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eb1a-107">構成マネージャー クライアントの正常性状態</span><span class="sxs-lookup"><span data-stu-id="1eb1a-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="1eb1a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1eb1a-108">Properties</span></span>
|<span data-ttu-id="1eb1a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1eb1a-109">Property</span></span>|<span data-ttu-id="1eb1a-110">型</span><span class="sxs-lookup"><span data-stu-id="1eb1a-110">Type</span></span>|<span data-ttu-id="1eb1a-111">説明</span><span class="sxs-lookup"><span data-stu-id="1eb1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eb1a-112">state</span><span class="sxs-lookup"><span data-stu-id="1eb1a-112">state</span></span>|[<span data-ttu-id="1eb1a-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="1eb1a-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="1eb1a-114">現在の構成マネージャー クライアントの状態です。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-114">Current configuration manager client state.</span></span> <span data-ttu-id="1eb1a-115">可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="1eb1a-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="1eb1a-116">errorCode</span></span>|<span data-ttu-id="1eb1a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="1eb1a-117">Int32</span></span>|<span data-ttu-id="1eb1a-118">障害状態のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-118">Error code for failed state.</span></span>|
|<span data-ttu-id="1eb1a-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1eb1a-119">lastSyncDateTime</span></span>|<span data-ttu-id="1eb1a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1eb1a-120">DateTimeOffset</span></span>|<span data-ttu-id="1eb1a-121">Datetime/fo オプション最後の同期の構成マネージャーの管理をポイントします。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eb1a-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1eb1a-122">Relationships</span></span>
<span data-ttu-id="1eb1a-123">なし</span><span class="sxs-lookup"><span data-stu-id="1eb1a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eb1a-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1eb1a-124">JSON Representation</span></span>
<span data-ttu-id="1eb1a-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1eb1a-125">Here is a JSON representation of the resource.</span></span>
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




