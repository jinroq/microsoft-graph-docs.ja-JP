---
title: windowsProtectionState リソースの種類
description: デバイス保護状態エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 793cd54995fdac06f53e78c0ffdd4d16dd1c51d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999333"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="7df7f-103">windowsProtectionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7df7f-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="7df7f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7df7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7df7f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7df7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df7f-106">デバイス保護状態エンティティ。</span><span class="sxs-lookup"><span data-stu-id="7df7f-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="7df7f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7df7f-107">Methods</span></span>
|<span data-ttu-id="7df7f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7df7f-108">Method</span></span>|<span data-ttu-id="7df7f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7df7f-109">Return Type</span></span>|<span data-ttu-id="7df7f-110">説明</span><span class="sxs-lookup"><span data-stu-id="7df7f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7df7f-111">WindowsProtectionState の取得</span><span class="sxs-lookup"><span data-stu-id="7df7f-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="7df7f-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="7df7f-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="7df7f-113">[Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7df7f-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="7df7f-114">WindowsProtectionState の更新</span><span class="sxs-lookup"><span data-stu-id="7df7f-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="7df7f-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="7df7f-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="7df7f-116">[Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7df7f-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7df7f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7df7f-117">Properties</span></span>
|<span data-ttu-id="7df7f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7df7f-118">Property</span></span>|<span data-ttu-id="7df7f-119">型</span><span class="sxs-lookup"><span data-stu-id="7df7f-119">Type</span></span>|<span data-ttu-id="7df7f-120">説明</span><span class="sxs-lookup"><span data-stu-id="7df7f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df7f-121">id</span><span class="sxs-lookup"><span data-stu-id="7df7f-121">id</span></span>|<span data-ttu-id="7df7f-122">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-122">String</span></span>|<span data-ttu-id="7df7f-123">デバイス保護状態オブジェクトの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="7df7f-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="7df7f-124">これはデバイスのデバイス id です</span><span class="sxs-lookup"><span data-stu-id="7df7f-124">This is device id of the device</span></span>|
|<span data-ttu-id="7df7f-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7df7f-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="7df7f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-126">Boolean</span></span>|<span data-ttu-id="7df7f-127">マルウェア対策が有効になっているか、または使用できない</span><span class="sxs-lookup"><span data-stu-id="7df7f-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="7df7f-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="7df7f-128">deviceState</span></span>|[<span data-ttu-id="7df7f-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="7df7f-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="7df7f-130">コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。</span><span class="sxs-lookup"><span data-stu-id="7df7f-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="7df7f-131">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="7df7f-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="7df7f-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7df7f-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="7df7f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-133">Boolean</span></span>|<span data-ttu-id="7df7f-134">リアルタイム保護が有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="7df7f-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="7df7f-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="7df7f-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="7df7f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-136">Boolean</span></span>|<span data-ttu-id="7df7f-137">ネットワーク検査システムが有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="7df7f-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="7df7f-138">quickScanOverdue 超過</span><span class="sxs-lookup"><span data-stu-id="7df7f-138">quickScanOverdue</span></span>|<span data-ttu-id="7df7f-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-139">Boolean</span></span>|<span data-ttu-id="7df7f-140">クイックスキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="7df7f-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="7df7f-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="7df7f-141">fullScanOverdue</span></span>|<span data-ttu-id="7df7f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-142">Boolean</span></span>|<span data-ttu-id="7df7f-143">完全スキャンの期限が過ぎたかどうか。</span><span class="sxs-lookup"><span data-stu-id="7df7f-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="7df7f-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="7df7f-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="7df7f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-145">Boolean</span></span>|<span data-ttu-id="7df7f-146">署名が古くなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="7df7f-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="7df7f-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="7df7f-147">rebootRequired</span></span>|<span data-ttu-id="7df7f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-148">Boolean</span></span>|<span data-ttu-id="7df7f-149">再起動が必要かどうか</span><span class="sxs-lookup"><span data-stu-id="7df7f-149">Reboot required or not?</span></span>|
|<span data-ttu-id="7df7f-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="7df7f-150">fullScanRequired</span></span>|<span data-ttu-id="7df7f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df7f-151">Boolean</span></span>|<span data-ttu-id="7df7f-152">フルスキャンが必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="7df7f-152">Full scan required or not?</span></span>|
|<span data-ttu-id="7df7f-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="7df7f-153">engineVersion</span></span>|<span data-ttu-id="7df7f-154">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-154">String</span></span>|<span data-ttu-id="7df7f-155">現在のエンドポイント保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="7df7f-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="7df7f-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="7df7f-156">signatureVersion</span></span>|<span data-ttu-id="7df7f-157">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-157">String</span></span>|<span data-ttu-id="7df7f-158">現在のマルウェア定義バージョン</span><span class="sxs-lookup"><span data-stu-id="7df7f-158">Current malware definitions version</span></span>|
|<span data-ttu-id="7df7f-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="7df7f-159">antiMalwareVersion</span></span>|<span data-ttu-id="7df7f-160">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-160">String</span></span>|<span data-ttu-id="7df7f-161">現在のマルウェア対策バージョン</span><span class="sxs-lookup"><span data-stu-id="7df7f-161">Current anti malware version</span></span>|
|<span data-ttu-id="7df7f-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="7df7f-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="7df7f-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df7f-163">DateTimeOffset</span></span>|<span data-ttu-id="7df7f-164">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="7df7f-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="7df7f-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="7df7f-165">lastFullScanDateTime</span></span>|<span data-ttu-id="7df7f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df7f-166">DateTimeOffset</span></span>|<span data-ttu-id="7df7f-167">最後のクイックスキャンの日時</span><span class="sxs-lookup"><span data-stu-id="7df7f-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="7df7f-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="7df7f-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="7df7f-169">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-169">String</span></span>|<span data-ttu-id="7df7f-170">最終クイックスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="7df7f-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="7df7f-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="7df7f-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="7df7f-172">String</span><span class="sxs-lookup"><span data-stu-id="7df7f-172">String</span></span>|<span data-ttu-id="7df7f-173">前回のフルスキャン署名バージョン</span><span class="sxs-lookup"><span data-stu-id="7df7f-173">Last full scan signature version</span></span>|
|<span data-ttu-id="7df7f-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7df7f-174">lastReportedDateTime</span></span>|<span data-ttu-id="7df7f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df7f-175">DateTimeOffset</span></span>|<span data-ttu-id="7df7f-176">前回のデバイス正常性の状態が報告された時刻</span><span class="sxs-lookup"><span data-stu-id="7df7f-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df7f-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7df7f-177">Relationships</span></span>
|<span data-ttu-id="7df7f-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7df7f-178">Relationship</span></span>|<span data-ttu-id="7df7f-179">型</span><span class="sxs-lookup"><span data-stu-id="7df7f-179">Type</span></span>|<span data-ttu-id="7df7f-180">説明</span><span class="sxs-lookup"><span data-stu-id="7df7f-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df7f-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="7df7f-181">detectedMalwareState</span></span>|<span data-ttu-id="7df7f-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7df7f-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="7df7f-183">デバイスマルウェアの一覧</span><span class="sxs-lookup"><span data-stu-id="7df7f-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7df7f-184">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7df7f-184">JSON Representation</span></span>
<span data-ttu-id="7df7f-185">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7df7f-185">Here is a JSON representation of the resource.</span></span>
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





