---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
ms.openlocfilehash: 4b394a6113c0b695092ba7f53d68db937ababfbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023068"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="8b90a-103">deviceHealthAttestationState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8b90a-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="8b90a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b90a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b90a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8b90a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8b90a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b90a-106">Properties</span></span>
|<span data-ttu-id="8b90a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b90a-107">Property</span></span>|<span data-ttu-id="8b90a-108">型</span><span class="sxs-lookup"><span data-stu-id="8b90a-108">Type</span></span>|<span data-ttu-id="8b90a-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b90a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b90a-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8b90a-110">lastUpdateDateTime</span></span>|<span data-ttu-id="8b90a-111">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-111">String</span></span>|<span data-ttu-id="8b90a-112">最終更新のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="8b90a-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="8b90a-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="8b90a-113">contentNamespaceUrl</span></span>|<span data-ttu-id="8b90a-114">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-114">String</span></span>|<span data-ttu-id="8b90a-115">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8b90a-115">The DHA report version.</span></span> <span data-ttu-id="8b90a-116">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="8b90a-116">(Namespace version)</span></span>|
|<span data-ttu-id="8b90a-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="8b90a-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="8b90a-118">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-118">String</span></span>|<span data-ttu-id="8b90a-119">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8b90a-119">The DHA report version.</span></span> <span data-ttu-id="8b90a-120">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="8b90a-120">(Namespace version)</span></span>|
|<span data-ttu-id="8b90a-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-121">contentVersion</span></span>|<span data-ttu-id="8b90a-122">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-122">String</span></span>|<span data-ttu-id="8b90a-123">HealthAttestation 状態のスキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="8b90a-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="8b90a-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b90a-124">issuedDateTime</span></span>|<span data-ttu-id="8b90a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b90a-125">DateTimeOffset</span></span>|<span data-ttu-id="8b90a-126">デバイスの評価または MDM への発行が行われた DateTime</span><span class="sxs-lookup"><span data-stu-id="8b90a-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="8b90a-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="8b90a-127">attestationIdentityKey</span></span>|<span data-ttu-id="8b90a-128">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-128">String</span></span>|<span data-ttu-id="8b90a-129">構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。</span><span class="sxs-lookup"><span data-stu-id="8b90a-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="8b90a-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="8b90a-130">resetCount</span></span>|<span data-ttu-id="8b90a-131">Int64</span><span class="sxs-lookup"><span data-stu-id="8b90a-131">Int64</span></span>|<span data-ttu-id="8b90a-132">PC デバイスが休止または再開した回数</span><span class="sxs-lookup"><span data-stu-id="8b90a-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="8b90a-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="8b90a-133">restartCount</span></span>|<span data-ttu-id="8b90a-134">Int64</span><span class="sxs-lookup"><span data-stu-id="8b90a-134">Int64</span></span>|<span data-ttu-id="8b90a-135">PC デバイスが再起動した回数</span><span class="sxs-lookup"><span data-stu-id="8b90a-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="8b90a-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b90a-136">dataExcutionPolicy</span></span>|<span data-ttu-id="8b90a-137">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-137">String</span></span>|<span data-ttu-id="8b90a-138">DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します</span><span class="sxs-lookup"><span data-stu-id="8b90a-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="8b90a-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="8b90a-139">bitLockerStatus</span></span>|<span data-ttu-id="8b90a-140">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-140">String</span></span>|<span data-ttu-id="8b90a-141">BitLocker ドライブ暗号化のオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="8b90a-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="8b90a-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-142">bootManagerVersion</span></span>|<span data-ttu-id="8b90a-143">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-143">String</span></span>|<span data-ttu-id="8b90a-144">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="8b90a-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="8b90a-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="8b90a-146">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-146">String</span></span>|<span data-ttu-id="8b90a-147">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="8b90a-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="8b90a-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="8b90a-148">secureBoot</span></span>|<span data-ttu-id="8b90a-149">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-149">String</span></span>|<span data-ttu-id="8b90a-150">セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です</span><span class="sxs-lookup"><span data-stu-id="8b90a-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="8b90a-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="8b90a-151">bootDebugging</span></span>|<span data-ttu-id="8b90a-152">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-152">String</span></span>|<span data-ttu-id="8b90a-153">bootDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="8b90a-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="8b90a-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="8b90a-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="8b90a-155">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-155">String</span></span>|<span data-ttu-id="8b90a-156">operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="8b90a-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="8b90a-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="8b90a-157">codeIntegrity</span></span>|<span data-ttu-id="8b90a-158">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-158">String</span></span>| <span data-ttu-id="8b90a-159">コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます</span><span class="sxs-lookup"><span data-stu-id="8b90a-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="8b90a-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="8b90a-160">testSigning</span></span>|<span data-ttu-id="8b90a-161">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-161">String</span></span>|<span data-ttu-id="8b90a-162">テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません</span><span class="sxs-lookup"><span data-stu-id="8b90a-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="8b90a-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="8b90a-163">safeMode</span></span>|<span data-ttu-id="8b90a-164">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-164">String</span></span>|<span data-ttu-id="8b90a-165">セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです</span><span class="sxs-lookup"><span data-stu-id="8b90a-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="8b90a-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="8b90a-166">windowsPE</span></span>|<span data-ttu-id="8b90a-167">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-167">String</span></span>|<span data-ttu-id="8b90a-168">Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="8b90a-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="8b90a-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="8b90a-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="8b90a-170">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-170">String</span></span>|<span data-ttu-id="8b90a-171">ELAM は、起動時にネットワーク内のコンピューターを保護します</span><span class="sxs-lookup"><span data-stu-id="8b90a-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="8b90a-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="8b90a-172">virtualSecureMode</span></span>|<span data-ttu-id="8b90a-173">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-173">String</span></span>|<span data-ttu-id="8b90a-174">VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです</span><span class="sxs-lookup"><span data-stu-id="8b90a-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="8b90a-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8b90a-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="8b90a-176">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-176">String</span></span>|<span data-ttu-id="8b90a-177">TPM で使用されていた HASH アルゴリズムを識別する情報の属性</span><span class="sxs-lookup"><span data-stu-id="8b90a-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="8b90a-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="8b90a-179">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-179">String</span></span>|<span data-ttu-id="8b90a-180">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="8b90a-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="8b90a-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="8b90a-182">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-182">String</span></span>|<span data-ttu-id="8b90a-183">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="8b90a-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="8b90a-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="8b90a-184">tpmVersion</span></span>|<span data-ttu-id="8b90a-185">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-185">String</span></span>|<span data-ttu-id="8b90a-186">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="8b90a-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="8b90a-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="8b90a-187">pcr0</span></span>|<span data-ttu-id="8b90a-188">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-188">String</span></span>|<span data-ttu-id="8b90a-189">PCR\[0\] でキャプチャされた測定値</span><span class="sxs-lookup"><span data-stu-id="8b90a-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="8b90a-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="8b90a-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="8b90a-191">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-191">String</span></span>|<span data-ttu-id="8b90a-192">カスタム セキュア ブート構成ポリシーの指紋</span><span class="sxs-lookup"><span data-stu-id="8b90a-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="8b90a-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="8b90a-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="8b90a-194">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-194">String</span></span>|<span data-ttu-id="8b90a-195">ブート環境のセキュリティを制御するコードの整合性ポリシー</span><span class="sxs-lookup"><span data-stu-id="8b90a-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="8b90a-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="8b90a-196">bootRevisionListInfo</span></span>|<span data-ttu-id="8b90a-197">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-197">String</span></span>|<span data-ttu-id="8b90a-198">構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="8b90a-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="8b90a-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="8b90a-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="8b90a-200">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-200">String</span></span>|<span data-ttu-id="8b90a-201">構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="8b90a-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="8b90a-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="8b90a-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="8b90a-203">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-203">String</span></span>|<span data-ttu-id="8b90a-204">この属性は、DHA サービスが整合性の問題を検出した場合に表示されます</span><span class="sxs-lookup"><span data-stu-id="8b90a-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="8b90a-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="8b90a-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="8b90a-206">String</span><span class="sxs-lookup"><span data-stu-id="8b90a-206">String</span></span>|<span data-ttu-id="8b90a-207">この属性は、DHA がデバイス向けにサポートされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="8b90a-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b90a-208">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b90a-208">Relationships</span></span>
<span data-ttu-id="8b90a-209">なし</span><span class="sxs-lookup"><span data-stu-id="8b90a-209">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b90a-210">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b90a-210">JSON Representation</span></span>
<span data-ttu-id="8b90a-211">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b90a-211">Here is a JSON representation of the resource.</span></span>
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



