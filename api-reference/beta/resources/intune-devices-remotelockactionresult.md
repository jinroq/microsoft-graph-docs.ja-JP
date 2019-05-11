---
title: remoteLockActionResult リソースの種類
description: ロック解除するためのピンが含まれるアクション結果のロック。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a8da7d99425e35c937250eee8a36ba005a133af
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941745"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="1bda3-103">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bda3-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="1bda3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bda3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bda3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1bda3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bda3-106">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="1bda3-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="1bda3-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1bda3-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1bda3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bda3-108">Properties</span></span>
|<span data-ttu-id="1bda3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bda3-109">Property</span></span>|<span data-ttu-id="1bda3-110">型</span><span class="sxs-lookup"><span data-stu-id="1bda3-110">Type</span></span>|<span data-ttu-id="1bda3-111">説明</span><span class="sxs-lookup"><span data-stu-id="1bda3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bda3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="1bda3-112">actionName</span></span>|<span data-ttu-id="1bda3-113">String</span><span class="sxs-lookup"><span data-stu-id="1bda3-113">String</span></span>|<span data-ttu-id="1bda3-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="1bda3-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1bda3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1bda3-115">actionState</span></span>|[<span data-ttu-id="1bda3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1bda3-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1bda3-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="1bda3-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1bda3-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1bda3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1bda3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1bda3-119">startDateTime</span></span>|<span data-ttu-id="1bda3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bda3-120">DateTimeOffset</span></span>|<span data-ttu-id="1bda3-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="1bda3-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1bda3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bda3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="1bda3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bda3-123">DateTimeOffset</span></span>|<span data-ttu-id="1bda3-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="1bda3-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1bda3-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="1bda3-125">unlockPin</span></span>|<span data-ttu-id="1bda3-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1bda3-126">String</span></span>|<span data-ttu-id="1bda3-127">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="1bda3-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bda3-128">関係</span><span class="sxs-lookup"><span data-stu-id="1bda3-128">Relationships</span></span>
<span data-ttu-id="1bda3-129">なし</span><span class="sxs-lookup"><span data-stu-id="1bda3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bda3-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1bda3-130">JSON Representation</span></span>
<span data-ttu-id="1bda3-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1bda3-131">Here is a JSON representation of the resource.</span></span>
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




