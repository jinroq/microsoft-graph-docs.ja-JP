---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャー クライアントの正常性状態
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302787"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="847a0-103">configurationManagerClientHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="847a0-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="847a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="847a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="847a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="847a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="847a0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="847a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="847a0-107">構成マネージャー クライアントの正常性状態</span><span class="sxs-lookup"><span data-stu-id="847a0-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="847a0-108">Properties</span><span class="sxs-lookup"><span data-stu-id="847a0-108">Properties</span></span>
|<span data-ttu-id="847a0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="847a0-109">Property</span></span>|<span data-ttu-id="847a0-110">種類</span><span class="sxs-lookup"><span data-stu-id="847a0-110">Type</span></span>|<span data-ttu-id="847a0-111">説明</span><span class="sxs-lookup"><span data-stu-id="847a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="847a0-112">state</span><span class="sxs-lookup"><span data-stu-id="847a0-112">state</span></span>|[<span data-ttu-id="847a0-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="847a0-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="847a0-114">現在の構成マネージャー クライアントの状態です。</span><span class="sxs-lookup"><span data-stu-id="847a0-114">Current configuration manager client state.</span></span> <span data-ttu-id="847a0-115">可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。</span><span class="sxs-lookup"><span data-stu-id="847a0-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="847a0-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="847a0-116">errorCode</span></span>|<span data-ttu-id="847a0-117">Int32</span><span class="sxs-lookup"><span data-stu-id="847a0-117">Int32</span></span>|<span data-ttu-id="847a0-118">障害状態のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="847a0-118">Error code for failed state.</span></span>|
|<span data-ttu-id="847a0-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="847a0-119">lastSyncDateTime</span></span>|<span data-ttu-id="847a0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="847a0-120">DateTimeOffset</span></span>|<span data-ttu-id="847a0-121">Datetime/fo オプション最後の同期の構成マネージャーの管理をポイントします。</span><span class="sxs-lookup"><span data-stu-id="847a0-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="847a0-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="847a0-122">Relationships</span></span>
<span data-ttu-id="847a0-123">なし</span><span class="sxs-lookup"><span data-stu-id="847a0-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="847a0-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="847a0-124">JSON Representation</span></span>
<span data-ttu-id="847a0-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="847a0-125">Here is a JSON representation of the resource.</span></span>
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





