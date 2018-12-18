---
title: windowsProtectionState リソースの種類
description: デバイス保護の状態のエンティティです。
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328078"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="4fb67-103">windowsProtectionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fb67-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="4fb67-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fb67-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fb67-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fb67-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fb67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fb67-107">デバイス保護の状態のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="4fb67-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="4fb67-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb67-108">Methods</span></span>
|<span data-ttu-id="4fb67-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb67-109">Method</span></span>|<span data-ttu-id="4fb67-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fb67-110">Return Type</span></span>|<span data-ttu-id="4fb67-111">説明</span><span class="sxs-lookup"><span data-stu-id="4fb67-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fb67-112">WindowsProtectionState を取得します。</span><span class="sxs-lookup"><span data-stu-id="4fb67-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="4fb67-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="4fb67-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="4fb67-114">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fb67-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="4fb67-115">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="4fb67-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="4fb67-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="4fb67-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="4fb67-117">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4fb67-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fb67-118">Properties</span><span class="sxs-lookup"><span data-stu-id="4fb67-118">Properties</span></span>
|<span data-ttu-id="4fb67-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb67-119">Property</span></span>|<span data-ttu-id="4fb67-120">種類</span><span class="sxs-lookup"><span data-stu-id="4fb67-120">Type</span></span>|<span data-ttu-id="4fb67-121">説明</span><span class="sxs-lookup"><span data-stu-id="4fb67-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb67-122">ID</span><span class="sxs-lookup"><span data-stu-id="4fb67-122">id</span></span>|<span data-ttu-id="4fb67-123">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-123">String</span></span>|<span data-ttu-id="4fb67-124">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="4fb67-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="4fb67-125">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="4fb67-125">This is device id of the device</span></span>|
|<span data-ttu-id="4fb67-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4fb67-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="4fb67-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-127">Boolean</span></span>|<span data-ttu-id="4fb67-128">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="4fb67-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="4fb67-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="4fb67-129">deviceState</span></span>|[<span data-ttu-id="4fb67-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="4fb67-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="4fb67-131">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="4fb67-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="4fb67-132">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="4fb67-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="4fb67-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4fb67-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="4fb67-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-134">Boolean</span></span>|<span data-ttu-id="4fb67-135">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="4fb67-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="4fb67-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="4fb67-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-137">Boolean</span></span>|<span data-ttu-id="4fb67-138">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="4fb67-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="4fb67-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4fb67-139">quickScanOverdue</span></span>|<span data-ttu-id="4fb67-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-140">Boolean</span></span>|<span data-ttu-id="4fb67-141">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="4fb67-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4fb67-142">fullScanOverdue</span></span>|<span data-ttu-id="4fb67-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-143">Boolean</span></span>|<span data-ttu-id="4fb67-144">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="4fb67-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="4fb67-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="4fb67-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-146">Boolean</span></span>|<span data-ttu-id="4fb67-147">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="4fb67-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="4fb67-148">rebootRequired</span></span>|<span data-ttu-id="4fb67-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-149">Boolean</span></span>|<span data-ttu-id="4fb67-150">しましたか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-150">Reboot required or not?</span></span>|
|<span data-ttu-id="4fb67-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="4fb67-151">fullScanRequired</span></span>|<span data-ttu-id="4fb67-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="4fb67-152">Boolean</span></span>|<span data-ttu-id="4fb67-153">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="4fb67-153">Full scan required or not?</span></span>|
|<span data-ttu-id="4fb67-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="4fb67-154">engineVersion</span></span>|<span data-ttu-id="4fb67-155">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-155">String</span></span>|<span data-ttu-id="4fb67-156">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="4fb67-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="4fb67-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="4fb67-157">signatureVersion</span></span>|<span data-ttu-id="4fb67-158">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-158">String</span></span>|<span data-ttu-id="4fb67-159">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="4fb67-159">Current malware definitions version</span></span>|
|<span data-ttu-id="4fb67-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="4fb67-160">antiMalwareVersion</span></span>|<span data-ttu-id="4fb67-161">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-161">String</span></span>|<span data-ttu-id="4fb67-162">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="4fb67-162">Current anti malware version</span></span>|
|<span data-ttu-id="4fb67-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb67-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="4fb67-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb67-164">DateTimeOffset</span></span>|<span data-ttu-id="4fb67-165">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="4fb67-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="4fb67-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb67-166">lastFullScanDateTime</span></span>|<span data-ttu-id="4fb67-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb67-167">DateTimeOffset</span></span>|<span data-ttu-id="4fb67-168">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="4fb67-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="4fb67-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4fb67-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="4fb67-170">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-170">String</span></span>|<span data-ttu-id="4fb67-171">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="4fb67-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="4fb67-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4fb67-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="4fb67-173">String</span><span class="sxs-lookup"><span data-stu-id="4fb67-173">String</span></span>|<span data-ttu-id="4fb67-174">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="4fb67-174">Last full scan signature version</span></span>|
|<span data-ttu-id="4fb67-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb67-175">lastReportedDateTime</span></span>|<span data-ttu-id="4fb67-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb67-176">DateTimeOffset</span></span>|<span data-ttu-id="4fb67-177">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="4fb67-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fb67-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fb67-178">Relationships</span></span>
|<span data-ttu-id="4fb67-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fb67-179">Relationship</span></span>|<span data-ttu-id="4fb67-180">型</span><span class="sxs-lookup"><span data-stu-id="4fb67-180">Type</span></span>|<span data-ttu-id="4fb67-181">説明</span><span class="sxs-lookup"><span data-stu-id="4fb67-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb67-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="4fb67-182">detectedMalwareState</span></span>|<span data-ttu-id="4fb67-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb67-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="4fb67-184">マルウェアのデバイス ・ リスト</span><span class="sxs-lookup"><span data-stu-id="4fb67-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fb67-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb67-185">JSON Representation</span></span>
<span data-ttu-id="4fb67-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fb67-186">Here is a JSON representation of the resource.</span></span>
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





