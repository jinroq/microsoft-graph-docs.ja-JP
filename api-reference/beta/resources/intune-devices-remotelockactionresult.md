---
title: remoteLockActionResult リソースの種類
description: ロック解除するためのピンが含まれるアクション結果のロック。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e57949e689f3d8e26c5217acec1a36662145b1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416469"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="2fc73-103">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fc73-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="2fc73-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fc73-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2fc73-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fc73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fc73-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fc73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fc73-107">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="2fc73-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="2fc73-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2fc73-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2fc73-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fc73-109">Properties</span></span>
|<span data-ttu-id="2fc73-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fc73-110">Property</span></span>|<span data-ttu-id="2fc73-111">型</span><span class="sxs-lookup"><span data-stu-id="2fc73-111">Type</span></span>|<span data-ttu-id="2fc73-112">説明</span><span class="sxs-lookup"><span data-stu-id="2fc73-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc73-113">actionName</span><span class="sxs-lookup"><span data-stu-id="2fc73-113">actionName</span></span>|<span data-ttu-id="2fc73-114">String</span><span class="sxs-lookup"><span data-stu-id="2fc73-114">String</span></span>|<span data-ttu-id="2fc73-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="2fc73-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fc73-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2fc73-116">actionState</span></span>|[<span data-ttu-id="2fc73-117">actionState</span><span class="sxs-lookup"><span data-stu-id="2fc73-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2fc73-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="2fc73-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2fc73-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="2fc73-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2fc73-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc73-120">startDateTime</span></span>|<span data-ttu-id="2fc73-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc73-121">DateTimeOffset</span></span>|<span data-ttu-id="2fc73-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2fc73-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fc73-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc73-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="2fc73-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc73-124">DateTimeOffset</span></span>|<span data-ttu-id="2fc73-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="2fc73-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fc73-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="2fc73-126">unlockPin</span></span>|<span data-ttu-id="2fc73-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fc73-127">String</span></span>|<span data-ttu-id="2fc73-128">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="2fc73-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fc73-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fc73-129">Relationships</span></span>
<span data-ttu-id="2fc73-130">なし</span><span class="sxs-lookup"><span data-stu-id="2fc73-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fc73-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fc73-131">JSON Representation</span></span>
<span data-ttu-id="2fc73-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2fc73-132">Here is a JSON representation of the resource.</span></span>
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




