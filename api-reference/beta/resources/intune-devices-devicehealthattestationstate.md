---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
ms.openlocfilehash: ad0928ba64fbba8fab14d32ca6ad82209a158f28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069681"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="6b16b-103">deviceHealthAttestationState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="6b16b-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="6b16b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b16b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b16b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b16b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b16b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b16b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b16b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6b16b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6b16b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b16b-108">Properties</span></span>
|<span data-ttu-id="6b16b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b16b-109">Property</span></span>|<span data-ttu-id="6b16b-110">型</span><span class="sxs-lookup"><span data-stu-id="6b16b-110">Type</span></span>|<span data-ttu-id="6b16b-111">説明</span><span class="sxs-lookup"><span data-stu-id="6b16b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b16b-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6b16b-112">lastUpdateDateTime</span></span>|<span data-ttu-id="6b16b-113">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-113">String</span></span>|<span data-ttu-id="6b16b-114">最終更新のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="6b16b-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="6b16b-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="6b16b-115">contentNamespaceUrl</span></span>|<span data-ttu-id="6b16b-116">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-116">String</span></span>|<span data-ttu-id="6b16b-117">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6b16b-117">The DHA report version.</span></span> <span data-ttu-id="6b16b-118">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="6b16b-118">(Namespace version)</span></span>|
|<span data-ttu-id="6b16b-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="6b16b-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="6b16b-120">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-120">String</span></span>|<span data-ttu-id="6b16b-121">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6b16b-121">The DHA report version.</span></span> <span data-ttu-id="6b16b-122">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="6b16b-122">(Namespace version)</span></span>|
|<span data-ttu-id="6b16b-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-123">contentVersion</span></span>|<span data-ttu-id="6b16b-124">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-124">String</span></span>|<span data-ttu-id="6b16b-125">HealthAttestation 状態のスキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="6b16b-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="6b16b-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b16b-126">issuedDateTime</span></span>|<span data-ttu-id="6b16b-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b16b-127">DateTimeOffset</span></span>|<span data-ttu-id="6b16b-128">デバイスの評価または MDM への発行が行われた DateTime</span><span class="sxs-lookup"><span data-stu-id="6b16b-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="6b16b-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="6b16b-129">attestationIdentityKey</span></span>|<span data-ttu-id="6b16b-130">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-130">String</span></span>|<span data-ttu-id="6b16b-131">構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。</span><span class="sxs-lookup"><span data-stu-id="6b16b-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="6b16b-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="6b16b-132">resetCount</span></span>|<span data-ttu-id="6b16b-133">Int64</span><span class="sxs-lookup"><span data-stu-id="6b16b-133">Int64</span></span>|<span data-ttu-id="6b16b-134">PC デバイスが休止または再開した回数</span><span class="sxs-lookup"><span data-stu-id="6b16b-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="6b16b-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="6b16b-135">restartCount</span></span>|<span data-ttu-id="6b16b-136">Int64</span><span class="sxs-lookup"><span data-stu-id="6b16b-136">Int64</span></span>|<span data-ttu-id="6b16b-137">PC デバイスが再起動した回数</span><span class="sxs-lookup"><span data-stu-id="6b16b-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="6b16b-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="6b16b-138">dataExcutionPolicy</span></span>|<span data-ttu-id="6b16b-139">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-139">String</span></span>|<span data-ttu-id="6b16b-140">DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します</span><span class="sxs-lookup"><span data-stu-id="6b16b-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="6b16b-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="6b16b-141">bitLockerStatus</span></span>|<span data-ttu-id="6b16b-142">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-142">String</span></span>|<span data-ttu-id="6b16b-143">BitLocker ドライブ暗号化のオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="6b16b-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="6b16b-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-144">bootManagerVersion</span></span>|<span data-ttu-id="6b16b-145">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-145">String</span></span>|<span data-ttu-id="6b16b-146">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="6b16b-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="6b16b-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="6b16b-148">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-148">String</span></span>|<span data-ttu-id="6b16b-149">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="6b16b-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="6b16b-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="6b16b-150">secureBoot</span></span>|<span data-ttu-id="6b16b-151">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-151">String</span></span>|<span data-ttu-id="6b16b-152">セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です</span><span class="sxs-lookup"><span data-stu-id="6b16b-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="6b16b-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="6b16b-153">bootDebugging</span></span>|<span data-ttu-id="6b16b-154">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-154">String</span></span>|<span data-ttu-id="6b16b-155">bootDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="6b16b-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="6b16b-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="6b16b-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="6b16b-157">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-157">String</span></span>|<span data-ttu-id="6b16b-158">operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="6b16b-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="6b16b-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="6b16b-159">codeIntegrity</span></span>|<span data-ttu-id="6b16b-160">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-160">String</span></span>| <span data-ttu-id="6b16b-161">コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます</span><span class="sxs-lookup"><span data-stu-id="6b16b-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="6b16b-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="6b16b-162">testSigning</span></span>|<span data-ttu-id="6b16b-163">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-163">String</span></span>|<span data-ttu-id="6b16b-164">テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません</span><span class="sxs-lookup"><span data-stu-id="6b16b-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="6b16b-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="6b16b-165">safeMode</span></span>|<span data-ttu-id="6b16b-166">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-166">String</span></span>|<span data-ttu-id="6b16b-167">セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです</span><span class="sxs-lookup"><span data-stu-id="6b16b-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="6b16b-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="6b16b-168">windowsPE</span></span>|<span data-ttu-id="6b16b-169">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-169">String</span></span>|<span data-ttu-id="6b16b-170">Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="6b16b-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="6b16b-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="6b16b-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="6b16b-172">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-172">String</span></span>|<span data-ttu-id="6b16b-173">ELAM は、起動時にネットワーク内のコンピューターを保護します</span><span class="sxs-lookup"><span data-stu-id="6b16b-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="6b16b-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="6b16b-174">virtualSecureMode</span></span>|<span data-ttu-id="6b16b-175">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-175">String</span></span>|<span data-ttu-id="6b16b-176">VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです</span><span class="sxs-lookup"><span data-stu-id="6b16b-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="6b16b-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6b16b-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="6b16b-178">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-178">String</span></span>|<span data-ttu-id="6b16b-179">TPM で使用されていた HASH アルゴリズムを識別する情報の属性</span><span class="sxs-lookup"><span data-stu-id="6b16b-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="6b16b-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="6b16b-181">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-181">String</span></span>|<span data-ttu-id="6b16b-182">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="6b16b-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="6b16b-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="6b16b-184">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-184">String</span></span>|<span data-ttu-id="6b16b-185">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="6b16b-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="6b16b-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="6b16b-186">tpmVersion</span></span>|<span data-ttu-id="6b16b-187">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-187">String</span></span>|<span data-ttu-id="6b16b-188">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="6b16b-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="6b16b-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="6b16b-189">pcr0</span></span>|<span data-ttu-id="6b16b-190">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-190">String</span></span>|<span data-ttu-id="6b16b-191">PCR\[0\] でキャプチャされた測定値</span><span class="sxs-lookup"><span data-stu-id="6b16b-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="6b16b-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="6b16b-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="6b16b-193">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-193">String</span></span>|<span data-ttu-id="6b16b-194">カスタム セキュア ブート構成ポリシーの指紋</span><span class="sxs-lookup"><span data-stu-id="6b16b-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="6b16b-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="6b16b-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="6b16b-196">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-196">String</span></span>|<span data-ttu-id="6b16b-197">ブート環境のセキュリティを制御するコードの整合性ポリシー</span><span class="sxs-lookup"><span data-stu-id="6b16b-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="6b16b-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="6b16b-198">bootRevisionListInfo</span></span>|<span data-ttu-id="6b16b-199">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-199">String</span></span>|<span data-ttu-id="6b16b-200">構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="6b16b-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="6b16b-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="6b16b-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="6b16b-202">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-202">String</span></span>|<span data-ttu-id="6b16b-203">構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="6b16b-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="6b16b-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="6b16b-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="6b16b-205">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-205">String</span></span>|<span data-ttu-id="6b16b-206">この属性は、DHA サービスが整合性の問題を検出した場合に表示されます</span><span class="sxs-lookup"><span data-stu-id="6b16b-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="6b16b-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="6b16b-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="6b16b-208">String</span><span class="sxs-lookup"><span data-stu-id="6b16b-208">String</span></span>|<span data-ttu-id="6b16b-209">この属性は、DHA がデバイス向けにサポートされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="6b16b-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b16b-210">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b16b-210">Relationships</span></span>
<span data-ttu-id="6b16b-211">なし</span><span class="sxs-lookup"><span data-stu-id="6b16b-211">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b16b-212">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b16b-212">JSON Representation</span></span>
<span data-ttu-id="6b16b-213">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b16b-213">Here is a JSON representation of the resource.</span></span>
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





