---
title: windowsprotectionstate リソースの種類
description: デバイス保護状態エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520082"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="1e16d-103">windowsprotectionstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e16d-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="1e16d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e16d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e16d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e16d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e16d-106">デバイス保護状態エンティティ。</span><span class="sxs-lookup"><span data-stu-id="1e16d-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1e16d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e16d-107">Methods</span></span>
|<span data-ttu-id="1e16d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e16d-108">Method</span></span>|<span data-ttu-id="1e16d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e16d-109">Return Type</span></span>|<span data-ttu-id="1e16d-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e16d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e16d-111">windowsprotectionstate の取得</span><span class="sxs-lookup"><span data-stu-id="1e16d-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="1e16d-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1e16d-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1e16d-113">[windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1e16d-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="1e16d-114">windowsprotectionstate の更新</span><span class="sxs-lookup"><span data-stu-id="1e16d-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="1e16d-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1e16d-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1e16d-116">[windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e16d-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e16d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e16d-117">Properties</span></span>
|<span data-ttu-id="1e16d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e16d-118">Property</span></span>|<span data-ttu-id="1e16d-119">型</span><span class="sxs-lookup"><span data-stu-id="1e16d-119">Type</span></span>|<span data-ttu-id="1e16d-120">説明</span><span class="sxs-lookup"><span data-stu-id="1e16d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e16d-121">id</span><span class="sxs-lookup"><span data-stu-id="1e16d-121">id</span></span>|<span data-ttu-id="1e16d-122">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-122">String</span></span>|<span data-ttu-id="1e16d-123">デバイス保護状態オブジェクトの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1e16d-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="1e16d-124">これはデバイスのデバイス id です</span><span class="sxs-lookup"><span data-stu-id="1e16d-124">This is device id of the device</span></span>|
|<span data-ttu-id="1e16d-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1e16d-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="1e16d-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-126">Boolean</span></span>|<span data-ttu-id="1e16d-127">マルウェア対策が有効になっているか、または使用できない</span><span class="sxs-lookup"><span data-stu-id="1e16d-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="1e16d-128">devicestate</span><span class="sxs-lookup"><span data-stu-id="1e16d-128">deviceState</span></span>|[<span data-ttu-id="1e16d-129">windowsdevicehealthstate</span><span class="sxs-lookup"><span data-stu-id="1e16d-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="1e16d-130">コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。</span><span class="sxs-lookup"><span data-stu-id="1e16d-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="1e16d-131">可能な値は `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical` です。</span><span class="sxs-lookup"><span data-stu-id="1e16d-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="1e16d-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1e16d-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="1e16d-133">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-133">Boolean</span></span>|<span data-ttu-id="1e16d-134">リアルタイム保護が有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e16d-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="1e16d-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="1e16d-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="1e16d-136">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-136">Boolean</span></span>|<span data-ttu-id="1e16d-137">ネットワーク検査システムが有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e16d-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="1e16d-138">quickscanoverdue 超過</span><span class="sxs-lookup"><span data-stu-id="1e16d-138">quickScanOverdue</span></span>|<span data-ttu-id="1e16d-139">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-139">Boolean</span></span>|<span data-ttu-id="1e16d-140">クイックスキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e16d-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="1e16d-141">fullscanoverdue</span><span class="sxs-lookup"><span data-stu-id="1e16d-141">fullScanOverdue</span></span>|<span data-ttu-id="1e16d-142">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-142">Boolean</span></span>|<span data-ttu-id="1e16d-143">完全スキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e16d-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="1e16d-144">signatureupdateoverdue</span><span class="sxs-lookup"><span data-stu-id="1e16d-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="1e16d-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-145">Boolean</span></span>|<span data-ttu-id="1e16d-146">署名が古くなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="1e16d-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="1e16d-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="1e16d-147">rebootRequired</span></span>|<span data-ttu-id="1e16d-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-148">Boolean</span></span>|<span data-ttu-id="1e16d-149">再起動が必要かどうか</span><span class="sxs-lookup"><span data-stu-id="1e16d-149">Reboot required or not?</span></span>|
|<span data-ttu-id="1e16d-150">fullscanrequired</span><span class="sxs-lookup"><span data-stu-id="1e16d-150">fullScanRequired</span></span>|<span data-ttu-id="1e16d-151">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e16d-151">Boolean</span></span>|<span data-ttu-id="1e16d-152">フルスキャンが必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="1e16d-152">Full scan required or not?</span></span>|
|<span data-ttu-id="1e16d-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="1e16d-153">engineVersion</span></span>|<span data-ttu-id="1e16d-154">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-154">String</span></span>|<span data-ttu-id="1e16d-155">現在のエンドポイント保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="1e16d-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="1e16d-156">signatureversion</span><span class="sxs-lookup"><span data-stu-id="1e16d-156">signatureVersion</span></span>|<span data-ttu-id="1e16d-157">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-157">String</span></span>|<span data-ttu-id="1e16d-158">現在のマルウェア定義バージョン</span><span class="sxs-lookup"><span data-stu-id="1e16d-158">Current malware definitions version</span></span>|
|<span data-ttu-id="1e16d-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="1e16d-159">antiMalwareVersion</span></span>|<span data-ttu-id="1e16d-160">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-160">String</span></span>|<span data-ttu-id="1e16d-161">現在のマルウェア対策バージョン</span><span class="sxs-lookup"><span data-stu-id="1e16d-161">Current anti malware version</span></span>|
|<span data-ttu-id="1e16d-162">lastquickscandatetime</span><span class="sxs-lookup"><span data-stu-id="1e16d-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="1e16d-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e16d-163">DateTimeOffset</span></span>|<span data-ttu-id="1e16d-164">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="1e16d-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="1e16d-165">lastfullscandatetime</span><span class="sxs-lookup"><span data-stu-id="1e16d-165">lastFullScanDateTime</span></span>|<span data-ttu-id="1e16d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e16d-166">DateTimeOffset</span></span>|<span data-ttu-id="1e16d-167">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="1e16d-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="1e16d-168">lastquickscansignatureversion</span><span class="sxs-lookup"><span data-stu-id="1e16d-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="1e16d-169">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-169">String</span></span>|<span data-ttu-id="1e16d-170">最終クイックスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="1e16d-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="1e16d-171">lastfullscansignatureversion</span><span class="sxs-lookup"><span data-stu-id="1e16d-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="1e16d-172">String</span><span class="sxs-lookup"><span data-stu-id="1e16d-172">String</span></span>|<span data-ttu-id="1e16d-173">前回のフルスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="1e16d-173">Last full scan signature version</span></span>|
|<span data-ttu-id="1e16d-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e16d-174">lastReportedDateTime</span></span>|<span data-ttu-id="1e16d-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e16d-175">DateTimeOffset</span></span>|<span data-ttu-id="1e16d-176">前回のデバイス正常性の状態が報告された時刻</span><span class="sxs-lookup"><span data-stu-id="1e16d-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e16d-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e16d-177">Relationships</span></span>
|<span data-ttu-id="1e16d-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e16d-178">Relationship</span></span>|<span data-ttu-id="1e16d-179">型</span><span class="sxs-lookup"><span data-stu-id="1e16d-179">Type</span></span>|<span data-ttu-id="1e16d-180">説明</span><span class="sxs-lookup"><span data-stu-id="1e16d-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e16d-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="1e16d-181">detectedMalwareState</span></span>|<span data-ttu-id="1e16d-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1e16d-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="1e16d-183">デバイスマルウェアの一覧</span><span class="sxs-lookup"><span data-stu-id="1e16d-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e16d-184">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e16d-184">JSON Representation</span></span>
<span data-ttu-id="1e16d-185">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e16d-185">Here is a JSON representation of the resource.</span></span>
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





