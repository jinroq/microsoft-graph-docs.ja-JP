---
title: deviceActionResult リソースの種類
description: デバイスのアクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ecb0028cd6e75d57f95868d16440881c4ac1bba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030857"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ad4a7-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad4a7-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="ad4a7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad4a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad4a7-105">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ad4a7-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="ad4a7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad4a7-106">Properties</span></span>
|<span data-ttu-id="ad4a7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad4a7-107">Property</span></span>|<span data-ttu-id="ad4a7-108">型</span><span class="sxs-lookup"><span data-stu-id="ad4a7-108">Type</span></span>|<span data-ttu-id="ad4a7-109">説明</span><span class="sxs-lookup"><span data-stu-id="ad4a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad4a7-110">actionName</span><span class="sxs-lookup"><span data-stu-id="ad4a7-110">actionName</span></span>|<span data-ttu-id="ad4a7-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ad4a7-111">String</span></span>|<span data-ttu-id="ad4a7-112">アクション名</span><span class="sxs-lookup"><span data-stu-id="ad4a7-112">Action name</span></span>|
|<span data-ttu-id="ad4a7-113">actionState</span><span class="sxs-lookup"><span data-stu-id="ad4a7-113">actionState</span></span>|[<span data-ttu-id="ad4a7-114">actionState</span><span class="sxs-lookup"><span data-stu-id="ad4a7-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="ad4a7-115">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="ad4a7-115">State of the action.</span></span> <span data-ttu-id="ad4a7-116">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="ad4a7-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ad4a7-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ad4a7-117">startDateTime</span></span>|<span data-ttu-id="ad4a7-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad4a7-118">DateTimeOffset</span></span>|<span data-ttu-id="ad4a7-119">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="ad4a7-119">Time the action was initiated</span></span>|
|<span data-ttu-id="ad4a7-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad4a7-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="ad4a7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad4a7-121">DateTimeOffset</span></span>|<span data-ttu-id="ad4a7-122">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="ad4a7-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad4a7-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad4a7-123">Relationships</span></span>
<span data-ttu-id="ad4a7-124">なし</span><span class="sxs-lookup"><span data-stu-id="ad4a7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad4a7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad4a7-125">JSON Representation</span></span>
<span data-ttu-id="ad4a7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad4a7-126">Here is a JSON representation of the resource.</span></span>
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



