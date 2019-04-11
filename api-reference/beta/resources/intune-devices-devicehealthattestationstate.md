---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66a22d0d3cc5caa53c41607da1d1de8185f22a62
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793757"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="f3cd2-103">deviceHealthAttestationState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f3cd2-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="f3cd2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3cd2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3cd2-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3cd2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3cd2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3cd2-107">Properties</span></span>
|<span data-ttu-id="f3cd2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3cd2-108">Property</span></span>|<span data-ttu-id="f3cd2-109">型</span><span class="sxs-lookup"><span data-stu-id="f3cd2-109">Type</span></span>|<span data-ttu-id="f3cd2-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3cd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cd2-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f3cd2-111">lastUpdateDateTime</span></span>|<span data-ttu-id="f3cd2-112">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-112">String</span></span>|<span data-ttu-id="f3cd2-113">最終更新のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="f3cd2-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="f3cd2-114">contentNamespaceUrl</span></span>|<span data-ttu-id="f3cd2-115">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-115">String</span></span>|<span data-ttu-id="f3cd2-116">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-116">The DHA report version.</span></span> <span data-ttu-id="f3cd2-117">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="f3cd2-117">(Namespace version)</span></span>|
|<span data-ttu-id="f3cd2-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="f3cd2-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="f3cd2-119">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-119">String</span></span>|<span data-ttu-id="f3cd2-120">DHA レポートのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-120">The DHA report version.</span></span> <span data-ttu-id="f3cd2-121">(名前空間のバージョン)</span><span class="sxs-lookup"><span data-stu-id="f3cd2-121">(Namespace version)</span></span>|
|<span data-ttu-id="f3cd2-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-122">contentVersion</span></span>|<span data-ttu-id="f3cd2-123">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-123">String</span></span>|<span data-ttu-id="f3cd2-124">HealthAttestation 状態のスキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="f3cd2-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="f3cd2-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3cd2-125">issuedDateTime</span></span>|<span data-ttu-id="f3cd2-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3cd2-126">DateTimeOffset</span></span>|<span data-ttu-id="f3cd2-127">デバイスの評価または MDM への発行が行われた DateTime</span><span class="sxs-lookup"><span data-stu-id="f3cd2-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="f3cd2-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="f3cd2-128">attestationIdentityKey</span></span>|<span data-ttu-id="f3cd2-129">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-129">String</span></span>|<span data-ttu-id="f3cd2-130">構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="f3cd2-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="f3cd2-131">resetCount</span></span>|<span data-ttu-id="f3cd2-132">Int64</span><span class="sxs-lookup"><span data-stu-id="f3cd2-132">Int64</span></span>|<span data-ttu-id="f3cd2-133">PC デバイスが休止または再開した回数</span><span class="sxs-lookup"><span data-stu-id="f3cd2-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="f3cd2-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="f3cd2-134">restartCount</span></span>|<span data-ttu-id="f3cd2-135">Int64</span><span class="sxs-lookup"><span data-stu-id="f3cd2-135">Int64</span></span>|<span data-ttu-id="f3cd2-136">PC デバイスが再起動した回数</span><span class="sxs-lookup"><span data-stu-id="f3cd2-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="f3cd2-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="f3cd2-137">dataExcutionPolicy</span></span>|<span data-ttu-id="f3cd2-138">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-138">String</span></span>|<span data-ttu-id="f3cd2-139">DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します</span><span class="sxs-lookup"><span data-stu-id="f3cd2-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="f3cd2-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="f3cd2-140">bitLockerStatus</span></span>|<span data-ttu-id="f3cd2-141">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-141">String</span></span>|<span data-ttu-id="f3cd2-142">BitLocker ドライブ暗号化のオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="f3cd2-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="f3cd2-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-143">bootManagerVersion</span></span>|<span data-ttu-id="f3cd2-144">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-144">String</span></span>|<span data-ttu-id="f3cd2-145">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="f3cd2-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="f3cd2-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="f3cd2-147">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-147">String</span></span>|<span data-ttu-id="f3cd2-148">ブート マネージャーのバージョン</span><span class="sxs-lookup"><span data-stu-id="f3cd2-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="f3cd2-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="f3cd2-149">secureBoot</span></span>|<span data-ttu-id="f3cd2-150">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-150">String</span></span>|<span data-ttu-id="f3cd2-151">セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です</span><span class="sxs-lookup"><span data-stu-id="f3cd2-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="f3cd2-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="f3cd2-152">bootDebugging</span></span>|<span data-ttu-id="f3cd2-153">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-153">String</span></span>|<span data-ttu-id="f3cd2-154">bootDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="f3cd2-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="f3cd2-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="f3cd2-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="f3cd2-156">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-156">String</span></span>|<span data-ttu-id="f3cd2-157">operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます</span><span class="sxs-lookup"><span data-stu-id="f3cd2-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="f3cd2-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="f3cd2-158">codeIntegrity</span></span>|<span data-ttu-id="f3cd2-159">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-159">String</span></span>| <span data-ttu-id="f3cd2-160">コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます</span><span class="sxs-lookup"><span data-stu-id="f3cd2-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="f3cd2-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="f3cd2-161">testSigning</span></span>|<span data-ttu-id="f3cd2-162">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-162">String</span></span>|<span data-ttu-id="f3cd2-163">テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません</span><span class="sxs-lookup"><span data-stu-id="f3cd2-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="f3cd2-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="f3cd2-164">safeMode</span></span>|<span data-ttu-id="f3cd2-165">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-165">String</span></span>|<span data-ttu-id="f3cd2-166">セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです</span><span class="sxs-lookup"><span data-stu-id="f3cd2-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="f3cd2-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="f3cd2-167">windowsPE</span></span>|<span data-ttu-id="f3cd2-168">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-168">String</span></span>|<span data-ttu-id="f3cd2-169">Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="f3cd2-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="f3cd2-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="f3cd2-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="f3cd2-171">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-171">String</span></span>|<span data-ttu-id="f3cd2-172">ELAM は、起動時にネットワーク内のコンピューターを保護します</span><span class="sxs-lookup"><span data-stu-id="f3cd2-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="f3cd2-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="f3cd2-173">virtualSecureMode</span></span>|<span data-ttu-id="f3cd2-174">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-174">String</span></span>|<span data-ttu-id="f3cd2-175">VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです</span><span class="sxs-lookup"><span data-stu-id="f3cd2-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="f3cd2-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f3cd2-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="f3cd2-177">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-177">String</span></span>|<span data-ttu-id="f3cd2-178">TPM で使用されていた HASH アルゴリズムを識別する情報の属性</span><span class="sxs-lookup"><span data-stu-id="f3cd2-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="f3cd2-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="f3cd2-180">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-180">String</span></span>|<span data-ttu-id="f3cd2-181">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="f3cd2-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="f3cd2-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="f3cd2-183">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-183">String</span></span>|<span data-ttu-id="f3cd2-184">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="f3cd2-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="f3cd2-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="f3cd2-185">tpmVersion</span></span>|<span data-ttu-id="f3cd2-186">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-186">String</span></span>|<span data-ttu-id="f3cd2-187">ブート アプリケーションのセキュリティ バージョン番号</span><span class="sxs-lookup"><span data-stu-id="f3cd2-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="f3cd2-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="f3cd2-188">pcr0</span></span>|<span data-ttu-id="f3cd2-189">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-189">String</span></span>|<span data-ttu-id="f3cd2-190">PCR\[0\] でキャプチャされた測定値</span><span class="sxs-lookup"><span data-stu-id="f3cd2-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="f3cd2-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="f3cd2-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="f3cd2-192">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-192">String</span></span>|<span data-ttu-id="f3cd2-193">カスタム セキュア ブート構成ポリシーの指紋</span><span class="sxs-lookup"><span data-stu-id="f3cd2-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="f3cd2-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="f3cd2-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="f3cd2-195">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-195">String</span></span>|<span data-ttu-id="f3cd2-196">ブート環境のセキュリティを制御するコードの整合性ポリシー</span><span class="sxs-lookup"><span data-stu-id="f3cd2-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="f3cd2-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="f3cd2-197">bootRevisionListInfo</span></span>|<span data-ttu-id="f3cd2-198">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-198">String</span></span>|<span data-ttu-id="f3cd2-199">構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="f3cd2-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="f3cd2-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="f3cd2-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="f3cd2-201">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cd2-201">String</span></span>|<span data-ttu-id="f3cd2-202">構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト</span><span class="sxs-lookup"><span data-stu-id="f3cd2-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="f3cd2-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="f3cd2-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="f3cd2-204">String</span><span class="sxs-lookup"><span data-stu-id="f3cd2-204">String</span></span>|<span data-ttu-id="f3cd2-205">この属性は、DHA サービスが整合性の問題を検出した場合に表示されます</span><span class="sxs-lookup"><span data-stu-id="f3cd2-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="f3cd2-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="f3cd2-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="f3cd2-207">String</span><span class="sxs-lookup"><span data-stu-id="f3cd2-207">String</span></span>|<span data-ttu-id="f3cd2-208">この属性は、DHA がデバイス向けにサポートされているかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="f3cd2-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3cd2-209">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3cd2-209">Relationships</span></span>
<span data-ttu-id="f3cd2-210">なし</span><span class="sxs-lookup"><span data-stu-id="f3cd2-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3cd2-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3cd2-211">JSON Representation</span></span>
<span data-ttu-id="f3cd2-212">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-212">Here is a JSON representation of the resource.</span></span>
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





