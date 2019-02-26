---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256148"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="20ff9-103">deviceHealthAttestationState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="20ff9-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="20ff9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20ff9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20ff9-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="20ff9-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20ff9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20ff9-106">Properties</span></span>
|<span data-ttu-id="20ff9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20ff9-107">Property</span></span>|<span data-ttu-id="20ff9-108">型</span><span class="sxs-lookup"><span data-stu-id="20ff9-108">Type</span></span>|<span data-ttu-id="20ff9-109">説明</span><span class="sxs-lookup"><span data-stu-id="20ff9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20ff9-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="20ff9-110">lastUpdateDateTime</span></span>|<span data-ttu-id="20ff9-111">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-111">String</span></span>|<span data-ttu-id="20ff9-112">最終更新のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="20ff9-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="20ff9-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="20ff9-113">contentNamespaceUrl</span></span>|<span data-ttu-id="20ff9-114">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-114">String</span></span>|<span data-ttu-id="20ff9-115">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="20ff9-115">The DHA report version.</span></span> <span data-ttu-id="20ff9-116">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="20ff9-116">(Namespace version)</span></span>|
|<span data-ttu-id="20ff9-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="20ff9-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="20ff9-118">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-118">String</span></span>|<span data-ttu-id="20ff9-119">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="20ff9-119">The DHA report version.</span></span> <span data-ttu-id="20ff9-120">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="20ff9-120">(Namespace version)</span></span>|
|<span data-ttu-id="20ff9-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-121">contentVersion</span></span>|<span data-ttu-id="20ff9-122">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-122">String</span></span>|<span data-ttu-id="20ff9-123">HealthAttestation 状態のスキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="20ff9-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="20ff9-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="20ff9-124">issuedDateTime</span></span>|<span data-ttu-id="20ff9-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20ff9-125">DateTimeOffset</span></span>|<span data-ttu-id="20ff9-126">デバイスの評価または MDM への発行が行われた DateTime</span><span class="sxs-lookup"><span data-stu-id="20ff9-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="20ff9-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="20ff9-127">attestationIdentityKey</span></span>|<span data-ttu-id="20ff9-128">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-128">String</span></span>|<span data-ttu-id="20ff9-129">構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。</span><span class="sxs-lookup"><span data-stu-id="20ff9-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="20ff9-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="20ff9-130">resetCount</span></span>|<span data-ttu-id="20ff9-131">Int64</span><span class="sxs-lookup"><span data-stu-id="20ff9-131">Int64</span></span>|<span data-ttu-id="20ff9-132">PC デバイスが休止または再開した回数</span><span class="sxs-lookup"><span data-stu-id="20ff9-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="20ff9-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="20ff9-133">restartCount</span></span>|<span data-ttu-id="20ff9-134">Int64</span><span class="sxs-lookup"><span data-stu-id="20ff9-134">Int64</span></span>|<span data-ttu-id="20ff9-135">PC デバイスが再起動した回数</span><span class="sxs-lookup"><span data-stu-id="20ff9-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="20ff9-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="20ff9-136">dataExcutionPolicy</span></span>|<span data-ttu-id="20ff9-137">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-137">String</span></span>|<span data-ttu-id="20ff9-138">DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します</span><span class="sxs-lookup"><span data-stu-id="20ff9-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="20ff9-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="20ff9-139">bitLockerStatus</span></span>|<span data-ttu-id="20ff9-140">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-140">String</span></span>|<span data-ttu-id="20ff9-141">BitLocker ドライブ暗号化のオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="20ff9-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="20ff9-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-142">bootManagerVersion</span></span>|<span data-ttu-id="20ff9-143">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-143">String</span></span>|<span data-ttu-id="20ff9-144">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="20ff9-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="20ff9-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="20ff9-146">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-146">String</span></span>|<span data-ttu-id="20ff9-147">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="20ff9-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="20ff9-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="20ff9-148">secureBoot</span></span>|<span data-ttu-id="20ff9-149">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-149">String</span></span>|<span data-ttu-id="20ff9-150">セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です</span><span class="sxs-lookup"><span data-stu-id="20ff9-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="20ff9-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="20ff9-151">bootDebugging</span></span>|<span data-ttu-id="20ff9-152">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-152">String</span></span>|<span data-ttu-id="20ff9-153">bootDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="20ff9-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="20ff9-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="20ff9-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="20ff9-155">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-155">String</span></span>|<span data-ttu-id="20ff9-156">operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="20ff9-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="20ff9-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="20ff9-157">codeIntegrity</span></span>|<span data-ttu-id="20ff9-158">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-158">String</span></span>| <span data-ttu-id="20ff9-159">コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます</span><span class="sxs-lookup"><span data-stu-id="20ff9-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="20ff9-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="20ff9-160">testSigning</span></span>|<span data-ttu-id="20ff9-161">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-161">String</span></span>|<span data-ttu-id="20ff9-162">テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません</span><span class="sxs-lookup"><span data-stu-id="20ff9-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="20ff9-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="20ff9-163">safeMode</span></span>|<span data-ttu-id="20ff9-164">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-164">String</span></span>|<span data-ttu-id="20ff9-165">セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです</span><span class="sxs-lookup"><span data-stu-id="20ff9-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="20ff9-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="20ff9-166">windowsPE</span></span>|<span data-ttu-id="20ff9-167">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-167">String</span></span>|<span data-ttu-id="20ff9-168">Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="20ff9-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="20ff9-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="20ff9-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="20ff9-170">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-170">String</span></span>|<span data-ttu-id="20ff9-171">ELAM は、起動時にネットワーク内のコンピューターを保護します</span><span class="sxs-lookup"><span data-stu-id="20ff9-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="20ff9-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="20ff9-172">virtualSecureMode</span></span>|<span data-ttu-id="20ff9-173">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-173">String</span></span>|<span data-ttu-id="20ff9-174">VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです</span><span class="sxs-lookup"><span data-stu-id="20ff9-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="20ff9-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="20ff9-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="20ff9-176">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-176">String</span></span>|<span data-ttu-id="20ff9-177">TPM で使用されていた HASH アルゴリズムを識別する情報の属性</span><span class="sxs-lookup"><span data-stu-id="20ff9-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="20ff9-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="20ff9-179">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-179">String</span></span>|<span data-ttu-id="20ff9-180">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="20ff9-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20ff9-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="20ff9-182">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-182">String</span></span>|<span data-ttu-id="20ff9-183">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="20ff9-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20ff9-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="20ff9-184">tpmVersion</span></span>|<span data-ttu-id="20ff9-185">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-185">String</span></span>|<span data-ttu-id="20ff9-186">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="20ff9-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20ff9-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="20ff9-187">pcr0</span></span>|<span data-ttu-id="20ff9-188">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-188">String</span></span>|<span data-ttu-id="20ff9-189">PCR\[0\] でキャプチャされた測定値</span><span class="sxs-lookup"><span data-stu-id="20ff9-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="20ff9-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="20ff9-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="20ff9-191">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-191">String</span></span>|<span data-ttu-id="20ff9-192">カスタム セキュア ブート構成ポリシーの指紋</span><span class="sxs-lookup"><span data-stu-id="20ff9-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="20ff9-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="20ff9-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="20ff9-194">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-194">String</span></span>|<span data-ttu-id="20ff9-195">ブート環境のセキュリティを制御するコードの整合性ポリシー</span><span class="sxs-lookup"><span data-stu-id="20ff9-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="20ff9-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="20ff9-196">bootRevisionListInfo</span></span>|<span data-ttu-id="20ff9-197">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-197">String</span></span>|<span data-ttu-id="20ff9-198">構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="20ff9-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="20ff9-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="20ff9-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="20ff9-200">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-200">String</span></span>|<span data-ttu-id="20ff9-201">構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="20ff9-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="20ff9-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="20ff9-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="20ff9-203">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-203">String</span></span>|<span data-ttu-id="20ff9-204">この属性は、DHA サービスが整合性の問題を検出した場合に表示されます</span><span class="sxs-lookup"><span data-stu-id="20ff9-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="20ff9-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="20ff9-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="20ff9-206">String</span><span class="sxs-lookup"><span data-stu-id="20ff9-206">String</span></span>|<span data-ttu-id="20ff9-207">この属性は、DHA がデバイス向けにサポートされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="20ff9-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="20ff9-208">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20ff9-208">Relationships</span></span>
<span data-ttu-id="20ff9-209">なし</span><span class="sxs-lookup"><span data-stu-id="20ff9-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20ff9-210">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20ff9-210">JSON Representation</span></span>
<span data-ttu-id="20ff9-211">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20ff9-211">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```



