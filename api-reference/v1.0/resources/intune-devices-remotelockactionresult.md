---
title: remoteLockActionResult リソースの種類
description: ロック解除するためのピンが含まれるアクション結果のロック。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550639"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="994da-103">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="994da-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="994da-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="994da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="994da-105">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="994da-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="994da-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="994da-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="994da-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="994da-107">Properties</span></span>
|<span data-ttu-id="994da-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="994da-108">Property</span></span>|<span data-ttu-id="994da-109">型</span><span class="sxs-lookup"><span data-stu-id="994da-109">Type</span></span>|<span data-ttu-id="994da-110">説明</span><span class="sxs-lookup"><span data-stu-id="994da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="994da-111">actionName</span><span class="sxs-lookup"><span data-stu-id="994da-111">actionName</span></span>|<span data-ttu-id="994da-112">String</span><span class="sxs-lookup"><span data-stu-id="994da-112">String</span></span>|<span data-ttu-id="994da-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="994da-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="994da-114">actionState</span><span class="sxs-lookup"><span data-stu-id="994da-114">actionState</span></span>|[<span data-ttu-id="994da-115">actionState</span><span class="sxs-lookup"><span data-stu-id="994da-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="994da-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="994da-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="994da-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="994da-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="994da-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="994da-118">startDateTime</span></span>|<span data-ttu-id="994da-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994da-119">DateTimeOffset</span></span>|<span data-ttu-id="994da-120">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="994da-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="994da-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="994da-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="994da-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994da-122">DateTimeOffset</span></span>|<span data-ttu-id="994da-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="994da-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="994da-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="994da-124">unlockPin</span></span>|<span data-ttu-id="994da-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="994da-125">String</span></span>|<span data-ttu-id="994da-126">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="994da-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="994da-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="994da-127">Relationships</span></span>
<span data-ttu-id="994da-128">なし</span><span class="sxs-lookup"><span data-stu-id="994da-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="994da-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="994da-129">JSON Representation</span></span>
<span data-ttu-id="994da-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="994da-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



