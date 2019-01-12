---
title: windowsProtectionState リソースの種類
description: デバイス保護の状態のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f15044f597fb04e98571de7aec8796e9a9ddf74
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954527"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="8a98f-103">windowsProtectionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a98f-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="8a98f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a98f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a98f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a98f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a98f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a98f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a98f-107">デバイス保護の状態のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="8a98f-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="8a98f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a98f-108">Methods</span></span>
|<span data-ttu-id="8a98f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a98f-109">Method</span></span>|<span data-ttu-id="8a98f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a98f-110">Return Type</span></span>|<span data-ttu-id="8a98f-111">説明</span><span class="sxs-lookup"><span data-stu-id="8a98f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a98f-112">WindowsProtectionState を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a98f-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="8a98f-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8a98f-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="8a98f-114">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a98f-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="8a98f-115">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="8a98f-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="8a98f-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8a98f-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="8a98f-117">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a98f-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a98f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a98f-118">Properties</span></span>
|<span data-ttu-id="8a98f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a98f-119">Property</span></span>|<span data-ttu-id="8a98f-120">型</span><span class="sxs-lookup"><span data-stu-id="8a98f-120">Type</span></span>|<span data-ttu-id="8a98f-121">説明</span><span class="sxs-lookup"><span data-stu-id="8a98f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a98f-122">ID</span><span class="sxs-lookup"><span data-stu-id="8a98f-122">id</span></span>|<span data-ttu-id="8a98f-123">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-123">String</span></span>|<span data-ttu-id="8a98f-124">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="8a98f-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="8a98f-125">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="8a98f-125">This is device id of the device</span></span>|
|<span data-ttu-id="8a98f-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8a98f-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="8a98f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-127">Boolean</span></span>|<span data-ttu-id="8a98f-128">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="8a98f-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="8a98f-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="8a98f-129">deviceState</span></span>|[<span data-ttu-id="8a98f-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="8a98f-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="8a98f-131">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="8a98f-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="8a98f-132">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="8a98f-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="8a98f-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8a98f-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="8a98f-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-134">Boolean</span></span>|<span data-ttu-id="8a98f-135">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="8a98f-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="8a98f-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="8a98f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-137">Boolean</span></span>|<span data-ttu-id="8a98f-138">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="8a98f-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="8a98f-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8a98f-139">quickScanOverdue</span></span>|<span data-ttu-id="8a98f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-140">Boolean</span></span>|<span data-ttu-id="8a98f-141">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="8a98f-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8a98f-142">fullScanOverdue</span></span>|<span data-ttu-id="8a98f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-143">Boolean</span></span>|<span data-ttu-id="8a98f-144">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="8a98f-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="8a98f-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="8a98f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-146">Boolean</span></span>|<span data-ttu-id="8a98f-147">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="8a98f-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="8a98f-148">rebootRequired</span></span>|<span data-ttu-id="8a98f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-149">Boolean</span></span>|<span data-ttu-id="8a98f-150">しましたか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-150">Reboot required or not?</span></span>|
|<span data-ttu-id="8a98f-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="8a98f-151">fullScanRequired</span></span>|<span data-ttu-id="8a98f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98f-152">Boolean</span></span>|<span data-ttu-id="8a98f-153">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="8a98f-153">Full scan required or not?</span></span>|
|<span data-ttu-id="8a98f-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="8a98f-154">engineVersion</span></span>|<span data-ttu-id="8a98f-155">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-155">String</span></span>|<span data-ttu-id="8a98f-156">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="8a98f-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="8a98f-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="8a98f-157">signatureVersion</span></span>|<span data-ttu-id="8a98f-158">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-158">String</span></span>|<span data-ttu-id="8a98f-159">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="8a98f-159">Current malware definitions version</span></span>|
|<span data-ttu-id="8a98f-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="8a98f-160">antiMalwareVersion</span></span>|<span data-ttu-id="8a98f-161">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-161">String</span></span>|<span data-ttu-id="8a98f-162">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="8a98f-162">Current anti malware version</span></span>|
|<span data-ttu-id="8a98f-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8a98f-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="8a98f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a98f-164">DateTimeOffset</span></span>|<span data-ttu-id="8a98f-165">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="8a98f-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="8a98f-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8a98f-166">lastFullScanDateTime</span></span>|<span data-ttu-id="8a98f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a98f-167">DateTimeOffset</span></span>|<span data-ttu-id="8a98f-168">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="8a98f-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="8a98f-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8a98f-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="8a98f-170">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-170">String</span></span>|<span data-ttu-id="8a98f-171">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="8a98f-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="8a98f-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8a98f-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="8a98f-173">String</span><span class="sxs-lookup"><span data-stu-id="8a98f-173">String</span></span>|<span data-ttu-id="8a98f-174">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="8a98f-174">Last full scan signature version</span></span>|
|<span data-ttu-id="8a98f-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a98f-175">lastReportedDateTime</span></span>|<span data-ttu-id="8a98f-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a98f-176">DateTimeOffset</span></span>|<span data-ttu-id="8a98f-177">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="8a98f-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a98f-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a98f-178">Relationships</span></span>
|<span data-ttu-id="8a98f-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a98f-179">Relationship</span></span>|<span data-ttu-id="8a98f-180">型</span><span class="sxs-lookup"><span data-stu-id="8a98f-180">Type</span></span>|<span data-ttu-id="8a98f-181">説明</span><span class="sxs-lookup"><span data-stu-id="8a98f-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a98f-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="8a98f-182">detectedMalwareState</span></span>|<span data-ttu-id="8a98f-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a98f-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="8a98f-184">マルウェアのデバイス ・ リスト</span><span class="sxs-lookup"><span data-stu-id="8a98f-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a98f-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a98f-185">JSON Representation</span></span>
<span data-ttu-id="8a98f-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a98f-186">Here is a JSON representation of the resource.</span></span>
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





