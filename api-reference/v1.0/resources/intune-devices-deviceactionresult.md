---
title: deviceActionResult リソースの種類
description: デバイス アクションの結果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b802d1b09fbe65e9e1e72e4c34a387462e12113
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861125"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="1d279-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d279-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="1d279-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d279-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d279-105">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="1d279-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="1d279-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d279-106">Properties</span></span>
|<span data-ttu-id="1d279-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d279-107">Property</span></span>|<span data-ttu-id="1d279-108">種類</span><span class="sxs-lookup"><span data-stu-id="1d279-108">Type</span></span>|<span data-ttu-id="1d279-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d279-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d279-110">actionName</span><span class="sxs-lookup"><span data-stu-id="1d279-110">actionName</span></span>|<span data-ttu-id="1d279-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1d279-111">String</span></span>|<span data-ttu-id="1d279-112">アクション名</span><span class="sxs-lookup"><span data-stu-id="1d279-112">Action name</span></span>|
|<span data-ttu-id="1d279-113">actionState</span><span class="sxs-lookup"><span data-stu-id="1d279-113">actionState</span></span>|[<span data-ttu-id="1d279-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1d279-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="1d279-115">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="1d279-115">State of the action.</span></span> <span data-ttu-id="1d279-116">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1d279-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1d279-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1d279-117">startDateTime</span></span>|<span data-ttu-id="1d279-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d279-118">DateTimeOffset</span></span>|<span data-ttu-id="1d279-119">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="1d279-119">Time the action was initiated</span></span>|
|<span data-ttu-id="1d279-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d279-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="1d279-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d279-121">DateTimeOffset</span></span>|<span data-ttu-id="1d279-122">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="1d279-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d279-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d279-123">Relationships</span></span>
<span data-ttu-id="1d279-124">なし</span><span class="sxs-lookup"><span data-stu-id="1d279-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d279-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d279-125">JSON Representation</span></span>
<span data-ttu-id="1d279-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d279-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



