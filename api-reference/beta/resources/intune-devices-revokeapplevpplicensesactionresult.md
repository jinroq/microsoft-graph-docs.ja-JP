---
title: revokeAppleVppLicensesActionResult リソースの種類
description: Apple Vpp ライセンスの取り消しの操作結果
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3646aa2cf790b599abdef38eb62df1118e67d9f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941809"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="edfec-103">revokeAppleVppLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="edfec-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="edfec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edfec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edfec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="edfec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfec-106">Apple Vpp ライセンスの取り消しの操作結果</span><span class="sxs-lookup"><span data-stu-id="edfec-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="edfec-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="edfec-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="edfec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edfec-108">Properties</span></span>
|<span data-ttu-id="edfec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edfec-109">Property</span></span>|<span data-ttu-id="edfec-110">型</span><span class="sxs-lookup"><span data-stu-id="edfec-110">Type</span></span>|<span data-ttu-id="edfec-111">説明</span><span class="sxs-lookup"><span data-stu-id="edfec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfec-112">actionName</span><span class="sxs-lookup"><span data-stu-id="edfec-112">actionName</span></span>|<span data-ttu-id="edfec-113">String</span><span class="sxs-lookup"><span data-stu-id="edfec-113">String</span></span>|<span data-ttu-id="edfec-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="edfec-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="edfec-115">actionState</span><span class="sxs-lookup"><span data-stu-id="edfec-115">actionState</span></span>|[<span data-ttu-id="edfec-116">actionState</span><span class="sxs-lookup"><span data-stu-id="edfec-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="edfec-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="edfec-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="edfec-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="edfec-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="edfec-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="edfec-119">startDateTime</span></span>|<span data-ttu-id="edfec-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfec-120">DateTimeOffset</span></span>|<span data-ttu-id="edfec-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="edfec-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="edfec-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="edfec-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="edfec-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfec-123">DateTimeOffset</span></span>|<span data-ttu-id="edfec-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="edfec-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="edfec-125">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="edfec-125">totalLicensesCount</span></span>|<span data-ttu-id="edfec-126">Int32</span><span class="sxs-lookup"><span data-stu-id="edfec-126">Int32</span></span>|<span data-ttu-id="edfec-127">関連付けられている Apple Vpp ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="edfec-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="edfec-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="edfec-128">failedLicensesCount</span></span>|<span data-ttu-id="edfec-129">Int32</span><span class="sxs-lookup"><span data-stu-id="edfec-129">Int32</span></span>|<span data-ttu-id="edfec-130">失効に失敗した Apple Vpp ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="edfec-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="edfec-131">関係</span><span class="sxs-lookup"><span data-stu-id="edfec-131">Relationships</span></span>
<span data-ttu-id="edfec-132">なし</span><span class="sxs-lookup"><span data-stu-id="edfec-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edfec-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="edfec-133">JSON Representation</span></span>
<span data-ttu-id="edfec-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="edfec-134">Here is a JSON representation of the resource.</span></span>
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




