---
title: revokeAppleVppLicensesActionResult リソースの種類
description: アップル Vpp ライセンスのアクションの結果を取り消す
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cd77bee330e919ab51927af0773d913099cea6e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419227"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="ee865-103">revokeAppleVppLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee865-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="ee865-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee865-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee865-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee865-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee865-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee865-107">アップル Vpp ライセンスのアクションの結果を取り消す</span><span class="sxs-lookup"><span data-stu-id="ee865-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="ee865-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee865-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee865-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee865-109">Properties</span></span>
|<span data-ttu-id="ee865-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee865-110">Property</span></span>|<span data-ttu-id="ee865-111">型</span><span class="sxs-lookup"><span data-stu-id="ee865-111">Type</span></span>|<span data-ttu-id="ee865-112">説明</span><span class="sxs-lookup"><span data-stu-id="ee865-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee865-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ee865-113">actionName</span></span>|<span data-ttu-id="ee865-114">String</span><span class="sxs-lookup"><span data-stu-id="ee865-114">String</span></span>|<span data-ttu-id="ee865-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="ee865-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee865-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ee865-116">actionState</span></span>|[<span data-ttu-id="ee865-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ee865-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ee865-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="ee865-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ee865-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="ee865-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ee865-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ee865-120">startDateTime</span></span>|<span data-ttu-id="ee865-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee865-121">DateTimeOffset</span></span>|<span data-ttu-id="ee865-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ee865-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee865-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee865-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ee865-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee865-124">DateTimeOffset</span></span>|<span data-ttu-id="ee865-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ee865-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee865-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ee865-126">totalLicensesCount</span></span>|<span data-ttu-id="ee865-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ee865-127">Int32</span></span>|<span data-ttu-id="ee865-128">関連付けられている Apple Vpp ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="ee865-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="ee865-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ee865-129">failedLicensesCount</span></span>|<span data-ttu-id="ee865-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ee865-130">Int32</span></span>|<span data-ttu-id="ee865-131">アップル Vpp ライセンスを失効に失敗した数の合計</span><span class="sxs-lookup"><span data-stu-id="ee865-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee865-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee865-132">Relationships</span></span>
<span data-ttu-id="ee865-133">なし</span><span class="sxs-lookup"><span data-stu-id="ee865-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee865-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee865-134">JSON Representation</span></span>
<span data-ttu-id="ee865-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee865-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```




