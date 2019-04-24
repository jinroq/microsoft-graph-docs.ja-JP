---
title: macOSCompliancePolicy の作成
description: 新しい macOSCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3505738d9d499655652cf72782337e11c1b50610
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518955"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="85552-103">macOSCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="85552-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="85552-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85552-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85552-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85552-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85552-106">新しい [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="85552-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85552-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="85552-107">Prerequisites</span></span>
<span data-ttu-id="85552-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85552-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85552-110">Permission type</span></span>|<span data-ttu-id="85552-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85552-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85552-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85552-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85552-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85552-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85552-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85552-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85552-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85552-115">Not supported.</span></span>|
|<span data-ttu-id="85552-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85552-116">Application</span></span>|<span data-ttu-id="85552-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85552-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85552-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85552-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="85552-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85552-119">Request headers</span></span>
|<span data-ttu-id="85552-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85552-120">Header</span></span>|<span data-ttu-id="85552-121">値</span><span class="sxs-lookup"><span data-stu-id="85552-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85552-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85552-122">Authorization</span></span>|<span data-ttu-id="85552-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="85552-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85552-124">承諾</span><span class="sxs-lookup"><span data-stu-id="85552-124">Accept</span></span>|<span data-ttu-id="85552-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85552-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85552-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="85552-126">Request body</span></span>
<span data-ttu-id="85552-127">要求本文で、macOSCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="85552-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="85552-128">次の表に、macOSCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="85552-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="85552-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85552-129">Property</span></span>|<span data-ttu-id="85552-130">型</span><span class="sxs-lookup"><span data-stu-id="85552-130">Type</span></span>|<span data-ttu-id="85552-131">説明</span><span class="sxs-lookup"><span data-stu-id="85552-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85552-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85552-132">roleScopeTagIds</span></span>|<span data-ttu-id="85552-133">String collection</span><span class="sxs-lookup"><span data-stu-id="85552-133">String collection</span></span>|<span data-ttu-id="85552-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="85552-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85552-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-136">id</span><span class="sxs-lookup"><span data-stu-id="85552-136">id</span></span>|<span data-ttu-id="85552-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="85552-137">String</span></span>|<span data-ttu-id="85552-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="85552-138">Key of the entity.</span></span> <span data-ttu-id="85552-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85552-140">createdDateTime</span></span>|<span data-ttu-id="85552-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85552-141">DateTimeOffset</span></span>|<span data-ttu-id="85552-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="85552-142">DateTime the object was created.</span></span> <span data-ttu-id="85552-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-144">説明</span><span class="sxs-lookup"><span data-stu-id="85552-144">description</span></span>|<span data-ttu-id="85552-145">String</span><span class="sxs-lookup"><span data-stu-id="85552-145">String</span></span>|<span data-ttu-id="85552-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="85552-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85552-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85552-148">lastModifiedDateTime</span></span>|<span data-ttu-id="85552-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85552-149">DateTimeOffset</span></span>|<span data-ttu-id="85552-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="85552-150">DateTime the object was last modified.</span></span> <span data-ttu-id="85552-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-152">displayName</span><span class="sxs-lookup"><span data-stu-id="85552-152">displayName</span></span>|<span data-ttu-id="85552-153">String</span><span class="sxs-lookup"><span data-stu-id="85552-153">String</span></span>|<span data-ttu-id="85552-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="85552-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85552-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-156">version</span><span class="sxs-lookup"><span data-stu-id="85552-156">version</span></span>|<span data-ttu-id="85552-157">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-157">Int32</span></span>|<span data-ttu-id="85552-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="85552-158">Version of the device configuration.</span></span> <span data-ttu-id="85552-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85552-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="85552-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="85552-160">passwordRequired</span></span>|<span data-ttu-id="85552-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-161">Boolean</span></span>|<span data-ttu-id="85552-162">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="85552-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="85552-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="85552-163">passwordBlockSimple</span></span>|<span data-ttu-id="85552-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-164">Boolean</span></span>|<span data-ttu-id="85552-165">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="85552-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="85552-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="85552-166">passwordExpirationDays</span></span>|<span data-ttu-id="85552-167">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-167">Int32</span></span>|<span data-ttu-id="85552-168">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="85552-168">Number of days before the password expires.</span></span> <span data-ttu-id="85552-169">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="85552-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="85552-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="85552-170">passwordMinimumLength</span></span>|<span data-ttu-id="85552-171">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-171">Int32</span></span>|<span data-ttu-id="85552-172">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="85552-172">Minimum length of password.</span></span> <span data-ttu-id="85552-173">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="85552-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="85552-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="85552-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="85552-175">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-175">Int32</span></span>|<span data-ttu-id="85552-176">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="85552-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="85552-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="85552-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="85552-178">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-178">Int32</span></span>|<span data-ttu-id="85552-179">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="85552-179">Number of previous passwords to block.</span></span> <span data-ttu-id="85552-180">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="85552-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="85552-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="85552-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="85552-182">Int32</span><span class="sxs-lookup"><span data-stu-id="85552-182">Int32</span></span>|<span data-ttu-id="85552-183">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="85552-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="85552-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="85552-184">passwordRequiredType</span></span>|[<span data-ttu-id="85552-185">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="85552-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="85552-186">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="85552-186">The required password type.</span></span> <span data-ttu-id="85552-187">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="85552-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="85552-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="85552-188">osMinimumVersion</span></span>|<span data-ttu-id="85552-189">String</span><span class="sxs-lookup"><span data-stu-id="85552-189">String</span></span>|<span data-ttu-id="85552-190">最小 os バージョン。</span><span class="sxs-lookup"><span data-stu-id="85552-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="85552-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="85552-191">osMaximumVersion</span></span>|<span data-ttu-id="85552-192">String</span><span class="sxs-lookup"><span data-stu-id="85552-192">String</span></span>|<span data-ttu-id="85552-193">最大 os バージョン。</span><span class="sxs-lookup"><span data-stu-id="85552-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="85552-194">osminimumbuildversion</span><span class="sxs-lookup"><span data-stu-id="85552-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="85552-195">String</span><span class="sxs-lookup"><span data-stu-id="85552-195">String</span></span>|<span data-ttu-id="85552-196">最小 os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="85552-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="85552-197">osmaximumbuildversion</span><span class="sxs-lookup"><span data-stu-id="85552-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="85552-198">String</span><span class="sxs-lookup"><span data-stu-id="85552-198">String</span></span>|<span data-ttu-id="85552-199">最大 os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="85552-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="85552-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="85552-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="85552-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-201">Boolean</span></span>|<span data-ttu-id="85552-202">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="85552-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="85552-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="85552-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="85552-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-204">Boolean</span></span>|<span data-ttu-id="85552-205">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="85552-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="85552-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85552-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="85552-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="85552-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="85552-208">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="85552-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="85552-209">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="85552-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="85552-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="85552-210">storageRequireEncryption</span></span>|<span data-ttu-id="85552-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-211">Boolean</span></span>|<span data-ttu-id="85552-212">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="85552-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="85552-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="85552-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="85552-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="85552-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="85552-215">macOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="85552-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="85552-216">可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="85552-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="85552-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="85552-217">firewallEnabled</span></span>|<span data-ttu-id="85552-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-218">Boolean</span></span>|<span data-ttu-id="85552-219">ファイアウォールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="85552-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="85552-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="85552-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="85552-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-221">Boolean</span></span>|<span data-ttu-id="85552-222">[着信接続をすべてブロックする] オプションに対応しています。</span><span class="sxs-lookup"><span data-stu-id="85552-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="85552-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="85552-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="85552-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="85552-224">Boolean</span></span>|<span data-ttu-id="85552-225">[ステルスモードを有効にする] に相当します。</span><span class="sxs-lookup"><span data-stu-id="85552-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="85552-226">応答</span><span class="sxs-lookup"><span data-stu-id="85552-226">Response</span></span>
<span data-ttu-id="85552-227">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="85552-227">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85552-228">例</span><span class="sxs-lookup"><span data-stu-id="85552-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="85552-229">要求</span><span class="sxs-lookup"><span data-stu-id="85552-229">Request</span></span>
<span data-ttu-id="85552-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85552-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="85552-231">応答</span><span class="sxs-lookup"><span data-stu-id="85552-231">Response</span></span>
<span data-ttu-id="85552-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85552-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```





