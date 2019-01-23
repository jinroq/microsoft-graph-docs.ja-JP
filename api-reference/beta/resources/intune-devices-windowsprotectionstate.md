---
title: windowsProtectionState リソースの種類
description: デバイス保護の状態のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423588"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="1c48f-103">windowsProtectionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c48f-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="1c48f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1c48f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1c48f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c48f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c48f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c48f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c48f-107">デバイス保護の状態のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="1c48f-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1c48f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1c48f-108">Methods</span></span>
|<span data-ttu-id="1c48f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1c48f-109">Method</span></span>|<span data-ttu-id="1c48f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1c48f-110">Return Type</span></span>|<span data-ttu-id="1c48f-111">説明</span><span class="sxs-lookup"><span data-stu-id="1c48f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c48f-112">WindowsProtectionState を取得します。</span><span class="sxs-lookup"><span data-stu-id="1c48f-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="1c48f-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1c48f-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1c48f-114">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c48f-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="1c48f-115">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="1c48f-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="1c48f-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1c48f-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1c48f-117">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1c48f-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c48f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c48f-118">Properties</span></span>
|<span data-ttu-id="1c48f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c48f-119">Property</span></span>|<span data-ttu-id="1c48f-120">型</span><span class="sxs-lookup"><span data-stu-id="1c48f-120">Type</span></span>|<span data-ttu-id="1c48f-121">説明</span><span class="sxs-lookup"><span data-stu-id="1c48f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c48f-122">id</span><span class="sxs-lookup"><span data-stu-id="1c48f-122">id</span></span>|<span data-ttu-id="1c48f-123">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-123">String</span></span>|<span data-ttu-id="1c48f-124">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1c48f-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="1c48f-125">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="1c48f-125">This is device id of the device</span></span>|
|<span data-ttu-id="1c48f-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1c48f-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="1c48f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-127">Boolean</span></span>|<span data-ttu-id="1c48f-128">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="1c48f-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="1c48f-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="1c48f-129">deviceState</span></span>|[<span data-ttu-id="1c48f-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="1c48f-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="1c48f-131">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="1c48f-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="1c48f-132">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="1c48f-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="1c48f-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1c48f-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="1c48f-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-134">Boolean</span></span>|<span data-ttu-id="1c48f-135">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="1c48f-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="1c48f-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="1c48f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-137">Boolean</span></span>|<span data-ttu-id="1c48f-138">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="1c48f-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="1c48f-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="1c48f-139">quickScanOverdue</span></span>|<span data-ttu-id="1c48f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-140">Boolean</span></span>|<span data-ttu-id="1c48f-141">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="1c48f-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="1c48f-142">fullScanOverdue</span></span>|<span data-ttu-id="1c48f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-143">Boolean</span></span>|<span data-ttu-id="1c48f-144">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="1c48f-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="1c48f-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="1c48f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-146">Boolean</span></span>|<span data-ttu-id="1c48f-147">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="1c48f-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="1c48f-148">rebootRequired</span></span>|<span data-ttu-id="1c48f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-149">Boolean</span></span>|<span data-ttu-id="1c48f-150">しましたか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-150">Reboot required or not?</span></span>|
|<span data-ttu-id="1c48f-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="1c48f-151">fullScanRequired</span></span>|<span data-ttu-id="1c48f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c48f-152">Boolean</span></span>|<span data-ttu-id="1c48f-153">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="1c48f-153">Full scan required or not?</span></span>|
|<span data-ttu-id="1c48f-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="1c48f-154">engineVersion</span></span>|<span data-ttu-id="1c48f-155">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-155">String</span></span>|<span data-ttu-id="1c48f-156">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="1c48f-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="1c48f-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="1c48f-157">signatureVersion</span></span>|<span data-ttu-id="1c48f-158">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-158">String</span></span>|<span data-ttu-id="1c48f-159">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="1c48f-159">Current malware definitions version</span></span>|
|<span data-ttu-id="1c48f-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="1c48f-160">antiMalwareVersion</span></span>|<span data-ttu-id="1c48f-161">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-161">String</span></span>|<span data-ttu-id="1c48f-162">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="1c48f-162">Current anti malware version</span></span>|
|<span data-ttu-id="1c48f-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="1c48f-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="1c48f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c48f-164">DateTimeOffset</span></span>|<span data-ttu-id="1c48f-165">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="1c48f-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="1c48f-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="1c48f-166">lastFullScanDateTime</span></span>|<span data-ttu-id="1c48f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c48f-167">DateTimeOffset</span></span>|<span data-ttu-id="1c48f-168">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="1c48f-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="1c48f-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="1c48f-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="1c48f-170">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-170">String</span></span>|<span data-ttu-id="1c48f-171">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="1c48f-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="1c48f-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="1c48f-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="1c48f-173">String</span><span class="sxs-lookup"><span data-stu-id="1c48f-173">String</span></span>|<span data-ttu-id="1c48f-174">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="1c48f-174">Last full scan signature version</span></span>|
|<span data-ttu-id="1c48f-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c48f-175">lastReportedDateTime</span></span>|<span data-ttu-id="1c48f-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c48f-176">DateTimeOffset</span></span>|<span data-ttu-id="1c48f-177">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="1c48f-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c48f-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1c48f-178">Relationships</span></span>
|<span data-ttu-id="1c48f-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1c48f-179">Relationship</span></span>|<span data-ttu-id="1c48f-180">型</span><span class="sxs-lookup"><span data-stu-id="1c48f-180">Type</span></span>|<span data-ttu-id="1c48f-181">説明</span><span class="sxs-lookup"><span data-stu-id="1c48f-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c48f-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="1c48f-182">detectedMalwareState</span></span>|<span data-ttu-id="1c48f-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1c48f-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="1c48f-184">マルウェアのデバイス ・ リスト</span><span class="sxs-lookup"><span data-stu-id="1c48f-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c48f-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c48f-185">JSON Representation</span></span>
<span data-ttu-id="1c48f-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1c48f-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```




