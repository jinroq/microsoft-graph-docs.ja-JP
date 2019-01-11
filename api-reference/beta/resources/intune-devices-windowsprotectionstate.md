---
title: windowsProtectionState リソースの種類
description: デバイス保護の状態のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884106"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="5463e-103">windowsProtectionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5463e-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="5463e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5463e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5463e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5463e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5463e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5463e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5463e-107">デバイス保護の状態のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="5463e-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="5463e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5463e-108">Methods</span></span>
|<span data-ttu-id="5463e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5463e-109">Method</span></span>|<span data-ttu-id="5463e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5463e-110">Return Type</span></span>|<span data-ttu-id="5463e-111">説明</span><span class="sxs-lookup"><span data-stu-id="5463e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5463e-112">WindowsProtectionState を取得します。</span><span class="sxs-lookup"><span data-stu-id="5463e-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="5463e-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5463e-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5463e-114">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5463e-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="5463e-115">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="5463e-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="5463e-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5463e-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5463e-117">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5463e-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5463e-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5463e-118">Properties</span></span>
|<span data-ttu-id="5463e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5463e-119">Property</span></span>|<span data-ttu-id="5463e-120">種類</span><span class="sxs-lookup"><span data-stu-id="5463e-120">Type</span></span>|<span data-ttu-id="5463e-121">説明</span><span class="sxs-lookup"><span data-stu-id="5463e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5463e-122">ID</span><span class="sxs-lookup"><span data-stu-id="5463e-122">id</span></span>|<span data-ttu-id="5463e-123">String</span><span class="sxs-lookup"><span data-stu-id="5463e-123">String</span></span>|<span data-ttu-id="5463e-124">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5463e-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5463e-125">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="5463e-125">This is device id of the device</span></span>|
|<span data-ttu-id="5463e-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5463e-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="5463e-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-127">Boolean</span></span>|<span data-ttu-id="5463e-128">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="5463e-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5463e-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="5463e-129">deviceState</span></span>|[<span data-ttu-id="5463e-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="5463e-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5463e-131">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="5463e-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5463e-132">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="5463e-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5463e-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5463e-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5463e-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-134">Boolean</span></span>|<span data-ttu-id="5463e-135">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="5463e-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5463e-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="5463e-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5463e-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-137">Boolean</span></span>|<span data-ttu-id="5463e-138">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="5463e-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5463e-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5463e-139">quickScanOverdue</span></span>|<span data-ttu-id="5463e-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-140">Boolean</span></span>|<span data-ttu-id="5463e-141">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="5463e-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5463e-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5463e-142">fullScanOverdue</span></span>|<span data-ttu-id="5463e-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-143">Boolean</span></span>|<span data-ttu-id="5463e-144">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="5463e-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5463e-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="5463e-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="5463e-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-146">Boolean</span></span>|<span data-ttu-id="5463e-147">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="5463e-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="5463e-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="5463e-148">rebootRequired</span></span>|<span data-ttu-id="5463e-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-149">Boolean</span></span>|<span data-ttu-id="5463e-150">しましたか。</span><span class="sxs-lookup"><span data-stu-id="5463e-150">Reboot required or not?</span></span>|
|<span data-ttu-id="5463e-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="5463e-151">fullScanRequired</span></span>|<span data-ttu-id="5463e-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="5463e-152">Boolean</span></span>|<span data-ttu-id="5463e-153">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="5463e-153">Full scan required or not?</span></span>|
|<span data-ttu-id="5463e-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="5463e-154">engineVersion</span></span>|<span data-ttu-id="5463e-155">String</span><span class="sxs-lookup"><span data-stu-id="5463e-155">String</span></span>|<span data-ttu-id="5463e-156">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="5463e-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5463e-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="5463e-157">signatureVersion</span></span>|<span data-ttu-id="5463e-158">String</span><span class="sxs-lookup"><span data-stu-id="5463e-158">String</span></span>|<span data-ttu-id="5463e-159">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="5463e-159">Current malware definitions version</span></span>|
|<span data-ttu-id="5463e-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="5463e-160">antiMalwareVersion</span></span>|<span data-ttu-id="5463e-161">String</span><span class="sxs-lookup"><span data-stu-id="5463e-161">String</span></span>|<span data-ttu-id="5463e-162">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="5463e-162">Current anti malware version</span></span>|
|<span data-ttu-id="5463e-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5463e-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="5463e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5463e-164">DateTimeOffset</span></span>|<span data-ttu-id="5463e-165">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="5463e-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="5463e-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5463e-166">lastFullScanDateTime</span></span>|<span data-ttu-id="5463e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5463e-167">DateTimeOffset</span></span>|<span data-ttu-id="5463e-168">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="5463e-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="5463e-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5463e-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5463e-170">String</span><span class="sxs-lookup"><span data-stu-id="5463e-170">String</span></span>|<span data-ttu-id="5463e-171">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="5463e-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="5463e-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5463e-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5463e-173">String</span><span class="sxs-lookup"><span data-stu-id="5463e-173">String</span></span>|<span data-ttu-id="5463e-174">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="5463e-174">Last full scan signature version</span></span>|
|<span data-ttu-id="5463e-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5463e-175">lastReportedDateTime</span></span>|<span data-ttu-id="5463e-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5463e-176">DateTimeOffset</span></span>|<span data-ttu-id="5463e-177">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="5463e-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="5463e-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5463e-178">Relationships</span></span>
|<span data-ttu-id="5463e-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5463e-179">Relationship</span></span>|<span data-ttu-id="5463e-180">型</span><span class="sxs-lookup"><span data-stu-id="5463e-180">Type</span></span>|<span data-ttu-id="5463e-181">説明</span><span class="sxs-lookup"><span data-stu-id="5463e-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5463e-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="5463e-182">detectedMalwareState</span></span>|<span data-ttu-id="5463e-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5463e-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="5463e-184">マルウェアのデバイス ・ リスト</span><span class="sxs-lookup"><span data-stu-id="5463e-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5463e-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5463e-185">JSON Representation</span></span>
<span data-ttu-id="5463e-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5463e-186">Here is a JSON representation of the resource.</span></span>
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





