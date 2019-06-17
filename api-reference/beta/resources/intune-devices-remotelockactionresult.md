---
title: remoteLockActionResult リソースの種類
description: ロック解除するためのピンが含まれるアクション結果のロック。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31af22f66b87d8102eeaf81d68d211640326f3fd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963857"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="13af2-103">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13af2-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="13af2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13af2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13af2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13af2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13af2-106">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="13af2-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="13af2-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="13af2-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13af2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13af2-108">Properties</span></span>
|<span data-ttu-id="13af2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13af2-109">Property</span></span>|<span data-ttu-id="13af2-110">型</span><span class="sxs-lookup"><span data-stu-id="13af2-110">Type</span></span>|<span data-ttu-id="13af2-111">説明</span><span class="sxs-lookup"><span data-stu-id="13af2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13af2-112">actionName</span><span class="sxs-lookup"><span data-stu-id="13af2-112">actionName</span></span>|<span data-ttu-id="13af2-113">String</span><span class="sxs-lookup"><span data-stu-id="13af2-113">String</span></span>|<span data-ttu-id="13af2-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="13af2-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="13af2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="13af2-115">actionState</span></span>|[<span data-ttu-id="13af2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="13af2-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="13af2-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="13af2-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="13af2-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="13af2-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="13af2-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="13af2-119">startDateTime</span></span>|<span data-ttu-id="13af2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13af2-120">DateTimeOffset</span></span>|<span data-ttu-id="13af2-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="13af2-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="13af2-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="13af2-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="13af2-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13af2-123">DateTimeOffset</span></span>|<span data-ttu-id="13af2-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="13af2-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="13af2-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="13af2-125">unlockPin</span></span>|<span data-ttu-id="13af2-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="13af2-126">String</span></span>|<span data-ttu-id="13af2-127">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="13af2-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="13af2-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13af2-128">Relationships</span></span>
<span data-ttu-id="13af2-129">なし</span><span class="sxs-lookup"><span data-stu-id="13af2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13af2-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13af2-130">JSON Representation</span></span>
<span data-ttu-id="13af2-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13af2-131">Here is a JSON representation of the resource.</span></span>
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





