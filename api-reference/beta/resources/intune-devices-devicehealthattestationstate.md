---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: c4aa43e274097d4b16b2ab3e933d269d2ad37717
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362357"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="ddf95-103">deviceHealthAttestationState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ddf95-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="ddf95-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ddf95-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddf95-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddf95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddf95-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddf95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddf95-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ddf95-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ddf95-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddf95-108">Properties</span></span>
|<span data-ttu-id="ddf95-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddf95-109">Property</span></span>|<span data-ttu-id="ddf95-110">種類</span><span class="sxs-lookup"><span data-stu-id="ddf95-110">Type</span></span>|<span data-ttu-id="ddf95-111">説明</span><span class="sxs-lookup"><span data-stu-id="ddf95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf95-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ddf95-112">lastUpdateDateTime</span></span>|<span data-ttu-id="ddf95-113">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-113">String</span></span>|<span data-ttu-id="ddf95-114">最終更新のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="ddf95-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="ddf95-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="ddf95-115">contentNamespaceUrl</span></span>|<span data-ttu-id="ddf95-116">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-116">String</span></span>|<span data-ttu-id="ddf95-117">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ddf95-117">The DHA report version.</span></span> <span data-ttu-id="ddf95-118">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="ddf95-118">(Namespace version)</span></span>|
|<span data-ttu-id="ddf95-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="ddf95-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="ddf95-120">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-120">String</span></span>|<span data-ttu-id="ddf95-121">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ddf95-121">The DHA report version.</span></span> <span data-ttu-id="ddf95-122">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="ddf95-122">(Namespace version)</span></span>|
|<span data-ttu-id="ddf95-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-123">contentVersion</span></span>|<span data-ttu-id="ddf95-124">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-124">String</span></span>|<span data-ttu-id="ddf95-125">HealthAttestation 状態のスキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="ddf95-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="ddf95-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddf95-126">issuedDateTime</span></span>|<span data-ttu-id="ddf95-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddf95-127">DateTimeOffset</span></span>|<span data-ttu-id="ddf95-128">デバイスの評価または MDM への発行が行われた DateTime</span><span class="sxs-lookup"><span data-stu-id="ddf95-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="ddf95-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="ddf95-129">attestationIdentityKey</span></span>|<span data-ttu-id="ddf95-130">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-130">String</span></span>|<span data-ttu-id="ddf95-131">構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。</span><span class="sxs-lookup"><span data-stu-id="ddf95-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="ddf95-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="ddf95-132">resetCount</span></span>|<span data-ttu-id="ddf95-133">Int64</span><span class="sxs-lookup"><span data-stu-id="ddf95-133">Int64</span></span>|<span data-ttu-id="ddf95-134">PC デバイスが休止または再開した回数</span><span class="sxs-lookup"><span data-stu-id="ddf95-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="ddf95-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="ddf95-135">restartCount</span></span>|<span data-ttu-id="ddf95-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ddf95-136">Int64</span></span>|<span data-ttu-id="ddf95-137">PC デバイスが再起動した回数</span><span class="sxs-lookup"><span data-stu-id="ddf95-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="ddf95-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="ddf95-138">dataExcutionPolicy</span></span>|<span data-ttu-id="ddf95-139">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-139">String</span></span>|<span data-ttu-id="ddf95-140">DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します</span><span class="sxs-lookup"><span data-stu-id="ddf95-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="ddf95-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="ddf95-141">bitLockerStatus</span></span>|<span data-ttu-id="ddf95-142">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-142">String</span></span>|<span data-ttu-id="ddf95-143">BitLocker ドライブ暗号化のオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="ddf95-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="ddf95-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-144">bootManagerVersion</span></span>|<span data-ttu-id="ddf95-145">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-145">String</span></span>|<span data-ttu-id="ddf95-146">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="ddf95-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="ddf95-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="ddf95-148">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-148">String</span></span>|<span data-ttu-id="ddf95-149">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="ddf95-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="ddf95-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="ddf95-150">secureBoot</span></span>|<span data-ttu-id="ddf95-151">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-151">String</span></span>|<span data-ttu-id="ddf95-152">セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です</span><span class="sxs-lookup"><span data-stu-id="ddf95-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="ddf95-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="ddf95-153">bootDebugging</span></span>|<span data-ttu-id="ddf95-154">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-154">String</span></span>|<span data-ttu-id="ddf95-155">bootDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="ddf95-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="ddf95-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="ddf95-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="ddf95-157">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-157">String</span></span>|<span data-ttu-id="ddf95-158">operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="ddf95-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="ddf95-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="ddf95-159">codeIntegrity</span></span>|<span data-ttu-id="ddf95-160">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-160">String</span></span>| <span data-ttu-id="ddf95-161">コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます</span><span class="sxs-lookup"><span data-stu-id="ddf95-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="ddf95-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="ddf95-162">testSigning</span></span>|<span data-ttu-id="ddf95-163">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-163">String</span></span>|<span data-ttu-id="ddf95-164">テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません</span><span class="sxs-lookup"><span data-stu-id="ddf95-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="ddf95-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="ddf95-165">safeMode</span></span>|<span data-ttu-id="ddf95-166">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-166">String</span></span>|<span data-ttu-id="ddf95-167">セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです</span><span class="sxs-lookup"><span data-stu-id="ddf95-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="ddf95-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="ddf95-168">windowsPE</span></span>|<span data-ttu-id="ddf95-169">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-169">String</span></span>|<span data-ttu-id="ddf95-170">Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="ddf95-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="ddf95-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="ddf95-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="ddf95-172">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-172">String</span></span>|<span data-ttu-id="ddf95-173">ELAM は、起動時にネットワーク内のコンピューターを保護します</span><span class="sxs-lookup"><span data-stu-id="ddf95-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="ddf95-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="ddf95-174">virtualSecureMode</span></span>|<span data-ttu-id="ddf95-175">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-175">String</span></span>|<span data-ttu-id="ddf95-176">VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです</span><span class="sxs-lookup"><span data-stu-id="ddf95-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="ddf95-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ddf95-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="ddf95-178">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-178">String</span></span>|<span data-ttu-id="ddf95-179">TPM で使用されていた HASH アルゴリズムを識別する情報の属性</span><span class="sxs-lookup"><span data-stu-id="ddf95-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="ddf95-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="ddf95-181">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-181">String</span></span>|<span data-ttu-id="ddf95-182">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="ddf95-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ddf95-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="ddf95-184">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-184">String</span></span>|<span data-ttu-id="ddf95-185">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="ddf95-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ddf95-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="ddf95-186">tpmVersion</span></span>|<span data-ttu-id="ddf95-187">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-187">String</span></span>|<span data-ttu-id="ddf95-188">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="ddf95-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="ddf95-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="ddf95-189">pcr0</span></span>|<span data-ttu-id="ddf95-190">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-190">String</span></span>|<span data-ttu-id="ddf95-191">PCR\[0\] でキャプチャされた測定値</span><span class="sxs-lookup"><span data-stu-id="ddf95-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="ddf95-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="ddf95-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="ddf95-193">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-193">String</span></span>|<span data-ttu-id="ddf95-194">カスタム セキュア ブート構成ポリシーの指紋</span><span class="sxs-lookup"><span data-stu-id="ddf95-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="ddf95-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="ddf95-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="ddf95-196">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-196">String</span></span>|<span data-ttu-id="ddf95-197">ブート環境のセキュリティを制御するコードの整合性ポリシー</span><span class="sxs-lookup"><span data-stu-id="ddf95-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="ddf95-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="ddf95-198">bootRevisionListInfo</span></span>|<span data-ttu-id="ddf95-199">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-199">String</span></span>|<span data-ttu-id="ddf95-200">構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="ddf95-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="ddf95-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="ddf95-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="ddf95-202">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-202">String</span></span>|<span data-ttu-id="ddf95-203">構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="ddf95-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="ddf95-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="ddf95-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="ddf95-205">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-205">String</span></span>|<span data-ttu-id="ddf95-206">この属性は、DHA サービスが整合性の問題を検出した場合に表示されます</span><span class="sxs-lookup"><span data-stu-id="ddf95-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="ddf95-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="ddf95-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="ddf95-208">String</span><span class="sxs-lookup"><span data-stu-id="ddf95-208">String</span></span>|<span data-ttu-id="ddf95-209">この属性は、DHA がデバイス向けにサポートされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ddf95-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddf95-210">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddf95-210">Relationships</span></span>
<span data-ttu-id="ddf95-211">なし</span><span class="sxs-lookup"><span data-stu-id="ddf95-211">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddf95-212">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddf95-212">JSON Representation</span></span>
<span data-ttu-id="ddf95-213">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddf95-213">Here is a JSON representation of the resource.</span></span>
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





