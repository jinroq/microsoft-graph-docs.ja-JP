---
title: advancedThreatProtectionOnboardingStateSummary リソースの種類
description: アカウント全体での Windows defender advanced threat protection のオンボード状態の概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ecda609a38d3dc9fe44376a0df9fc49bc06f63c3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334935"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a><span data-ttu-id="2ab87-103">advancedThreatProtectionOnboardingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ab87-103">advancedThreatProtectionOnboardingStateSummary resource type</span></span>

> <span data-ttu-id="2ab87-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab87-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ab87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab87-106">アカウント全体での Windows defender advanced threat protection のオンボード状態の概要。</span><span class="sxs-lookup"><span data-stu-id="2ab87-106">Windows defender advanced threat protection onboarding state summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="2ab87-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ab87-107">Methods</span></span>
|<span data-ttu-id="2ab87-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ab87-108">Method</span></span>|<span data-ttu-id="2ab87-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ab87-109">Return Type</span></span>|<span data-ttu-id="2ab87-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ab87-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ab87-111">AdvancedThreatProtectionOnboardingStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="2ab87-111">Get advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[<span data-ttu-id="2ab87-112">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2ab87-112">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="2ab87-113">[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ab87-113">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="2ab87-114">AdvancedThreatProtectionOnboardingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="2ab87-114">Update advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[<span data-ttu-id="2ab87-115">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2ab87-115">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="2ab87-116">[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ab87-116">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ab87-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab87-117">Properties</span></span>
|<span data-ttu-id="2ab87-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab87-118">Property</span></span>|<span data-ttu-id="2ab87-119">型</span><span class="sxs-lookup"><span data-stu-id="2ab87-119">Type</span></span>|<span data-ttu-id="2ab87-120">説明</span><span class="sxs-lookup"><span data-stu-id="2ab87-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab87-121">id</span><span class="sxs-lookup"><span data-stu-id="2ab87-121">id</span></span>|<span data-ttu-id="2ab87-122">String</span><span class="sxs-lookup"><span data-stu-id="2ab87-122">String</span></span>|<span data-ttu-id="2ab87-123">一意識別子</span><span class="sxs-lookup"><span data-stu-id="2ab87-123">Unique Identifier</span></span>|
|<span data-ttu-id="2ab87-124">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-124">unknownDeviceCount</span></span>|<span data-ttu-id="2ab87-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-125">Int32</span></span>|<span data-ttu-id="2ab87-126">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-126">Number of unknown devices</span></span>|
|<span data-ttu-id="2ab87-127">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-127">notApplicableDeviceCount</span></span>|<span data-ttu-id="2ab87-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-128">Int32</span></span>|<span data-ttu-id="2ab87-129">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="2ab87-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-130">compliantDeviceCount</span></span>|<span data-ttu-id="2ab87-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-131">Int32</span></span>|<span data-ttu-id="2ab87-132">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-132">Number of compliant devices</span></span>|
|<span data-ttu-id="2ab87-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-133">remediatedDeviceCount</span></span>|<span data-ttu-id="2ab87-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-134">Int32</span></span>|<span data-ttu-id="2ab87-135">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-135">Number of remediated devices</span></span>|
|<span data-ttu-id="2ab87-136">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-136">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2ab87-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-137">Int32</span></span>|<span data-ttu-id="2ab87-138">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-138">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="2ab87-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-139">errorDeviceCount</span></span>|<span data-ttu-id="2ab87-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-140">Int32</span></span>|<span data-ttu-id="2ab87-141">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-141">Number of error devices</span></span>|
|<span data-ttu-id="2ab87-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-142">conflictDeviceCount</span></span>|<span data-ttu-id="2ab87-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-143">Int32</span></span>|<span data-ttu-id="2ab87-144">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-144">Number of conflict devices</span></span>|
|<span data-ttu-id="2ab87-145">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ab87-145">notAssignedDeviceCount</span></span>|<span data-ttu-id="2ab87-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab87-146">Int32</span></span>|<span data-ttu-id="2ab87-147">割り当てられていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2ab87-147">Number of not assigned devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab87-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ab87-148">Relationships</span></span>
|<span data-ttu-id="2ab87-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ab87-149">Relationship</span></span>|<span data-ttu-id="2ab87-150">型</span><span class="sxs-lookup"><span data-stu-id="2ab87-150">Type</span></span>|<span data-ttu-id="2ab87-151">説明</span><span class="sxs-lookup"><span data-stu-id="2ab87-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab87-152">advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="2ab87-152">advancedThreatProtectionOnboardingDeviceSettingStates</span></span>|<span data-ttu-id="2ab87-153">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2ab87-153">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) collection</span></span>|<span data-ttu-id="2ab87-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2ab87-154">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ab87-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ab87-155">JSON Representation</span></span>
<span data-ttu-id="2ab87-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ab87-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```



