---
title: macOSCompliancePolicy の更新
description: macOSCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2eb1e7835d0febcd608f8019557d6955065fab1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797397"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="b1389-103">macOSCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="b1389-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="b1389-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1389-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1389-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1389-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1389-106">[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b1389-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1389-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1389-107">Prerequisites</span></span>
<span data-ttu-id="b1389-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1389-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1389-110">Permission type</span></span>|<span data-ttu-id="b1389-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1389-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1389-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1389-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1389-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1389-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1389-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1389-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1389-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1389-115">Not supported.</span></span>|
|<span data-ttu-id="b1389-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1389-116">Application</span></span>|<span data-ttu-id="b1389-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1389-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1389-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1389-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b1389-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1389-119">Request headers</span></span>
|<span data-ttu-id="b1389-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1389-120">Header</span></span>|<span data-ttu-id="b1389-121">値</span><span class="sxs-lookup"><span data-stu-id="b1389-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1389-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1389-122">Authorization</span></span>|<span data-ttu-id="b1389-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1389-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1389-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b1389-124">Accept</span></span>|<span data-ttu-id="b1389-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1389-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1389-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1389-126">Request body</span></span>
<span data-ttu-id="b1389-127">要求本文で、[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1389-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="b1389-128">次の表に、[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b1389-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="b1389-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1389-129">Property</span></span>|<span data-ttu-id="b1389-130">型</span><span class="sxs-lookup"><span data-stu-id="b1389-130">Type</span></span>|<span data-ttu-id="b1389-131">説明</span><span class="sxs-lookup"><span data-stu-id="b1389-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1389-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1389-132">roleScopeTagIds</span></span>|<span data-ttu-id="b1389-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b1389-133">String collection</span></span>|<span data-ttu-id="b1389-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b1389-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1389-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-136">id</span><span class="sxs-lookup"><span data-stu-id="b1389-136">id</span></span>|<span data-ttu-id="b1389-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b1389-137">String</span></span>|<span data-ttu-id="b1389-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b1389-138">Key of the entity.</span></span> <span data-ttu-id="b1389-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1389-140">createdDateTime</span></span>|<span data-ttu-id="b1389-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1389-141">DateTimeOffset</span></span>|<span data-ttu-id="b1389-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b1389-142">DateTime the object was created.</span></span> <span data-ttu-id="b1389-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-144">説明</span><span class="sxs-lookup"><span data-stu-id="b1389-144">description</span></span>|<span data-ttu-id="b1389-145">String</span><span class="sxs-lookup"><span data-stu-id="b1389-145">String</span></span>|<span data-ttu-id="b1389-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b1389-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1389-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1389-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b1389-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1389-149">DateTimeOffset</span></span>|<span data-ttu-id="b1389-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b1389-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b1389-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b1389-152">displayName</span></span>|<span data-ttu-id="b1389-153">String</span><span class="sxs-lookup"><span data-stu-id="b1389-153">String</span></span>|<span data-ttu-id="b1389-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b1389-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1389-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-156">version</span><span class="sxs-lookup"><span data-stu-id="b1389-156">version</span></span>|<span data-ttu-id="b1389-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-157">Int32</span></span>|<span data-ttu-id="b1389-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b1389-158">Version of the device configuration.</span></span> <span data-ttu-id="b1389-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1389-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1389-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b1389-160">passwordRequired</span></span>|<span data-ttu-id="b1389-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-161">Boolean</span></span>|<span data-ttu-id="b1389-162">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b1389-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b1389-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b1389-163">passwordBlockSimple</span></span>|<span data-ttu-id="b1389-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-164">Boolean</span></span>|<span data-ttu-id="b1389-165">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b1389-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="b1389-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b1389-166">passwordExpirationDays</span></span>|<span data-ttu-id="b1389-167">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-167">Int32</span></span>|<span data-ttu-id="b1389-168">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="b1389-168">Number of days before the password expires.</span></span> <span data-ttu-id="b1389-169">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="b1389-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b1389-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b1389-170">passwordMinimumLength</span></span>|<span data-ttu-id="b1389-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-171">Int32</span></span>|<span data-ttu-id="b1389-172">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="b1389-172">Minimum length of password.</span></span> <span data-ttu-id="b1389-173">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="b1389-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b1389-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b1389-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b1389-175">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-175">Int32</span></span>|<span data-ttu-id="b1389-176">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b1389-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b1389-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b1389-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b1389-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-178">Int32</span></span>|<span data-ttu-id="b1389-179">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="b1389-179">Number of previous passwords to block.</span></span> <span data-ttu-id="b1389-180">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="b1389-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b1389-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b1389-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b1389-182">Int32</span><span class="sxs-lookup"><span data-stu-id="b1389-182">Int32</span></span>|<span data-ttu-id="b1389-183">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="b1389-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b1389-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b1389-184">passwordRequiredType</span></span>|[<span data-ttu-id="b1389-185">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="b1389-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b1389-186">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="b1389-186">The required password type.</span></span> <span data-ttu-id="b1389-187">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="b1389-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b1389-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1389-188">osMinimumVersion</span></span>|<span data-ttu-id="b1389-189">文字列</span><span class="sxs-lookup"><span data-stu-id="b1389-189">String</span></span>|<span data-ttu-id="b1389-190">最小 os バージョン。</span><span class="sxs-lookup"><span data-stu-id="b1389-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="b1389-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1389-191">osMaximumVersion</span></span>|<span data-ttu-id="b1389-192">String</span><span class="sxs-lookup"><span data-stu-id="b1389-192">String</span></span>|<span data-ttu-id="b1389-193">最大 os バージョン。</span><span class="sxs-lookup"><span data-stu-id="b1389-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="b1389-194">osminimumbuildversion</span><span class="sxs-lookup"><span data-stu-id="b1389-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="b1389-195">文字列</span><span class="sxs-lookup"><span data-stu-id="b1389-195">String</span></span>|<span data-ttu-id="b1389-196">最小 os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="b1389-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="b1389-197">osmaximumbuildversion</span><span class="sxs-lookup"><span data-stu-id="b1389-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="b1389-198">文字列</span><span class="sxs-lookup"><span data-stu-id="b1389-198">String</span></span>|<span data-ttu-id="b1389-199">最大 os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="b1389-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="b1389-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1389-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="b1389-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-201">Boolean</span></span>|<span data-ttu-id="b1389-202">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1389-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="b1389-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1389-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b1389-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-204">Boolean</span></span>|<span data-ttu-id="b1389-205">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="b1389-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b1389-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1389-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1389-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1389-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1389-208">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="b1389-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1389-209">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="b1389-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1389-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b1389-210">storageRequireEncryption</span></span>|<span data-ttu-id="b1389-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-211">Boolean</span></span>|<span data-ttu-id="b1389-212">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="b1389-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="b1389-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="b1389-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="b1389-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="b1389-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="b1389-215">macOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="b1389-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="b1389-216">可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="b1389-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="b1389-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="b1389-217">firewallEnabled</span></span>|<span data-ttu-id="b1389-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-218">Boolean</span></span>|<span data-ttu-id="b1389-219">ファイアウォールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b1389-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="b1389-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="b1389-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="b1389-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-221">Boolean</span></span>|<span data-ttu-id="b1389-222">[着信接続をすべてブロックする] オプションに対応しています。</span><span class="sxs-lookup"><span data-stu-id="b1389-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="b1389-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="b1389-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="b1389-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1389-224">Boolean</span></span>|<span data-ttu-id="b1389-225">[ステルスモードを有効にする] に相当します。</span><span class="sxs-lookup"><span data-stu-id="b1389-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="b1389-226">応答</span><span class="sxs-lookup"><span data-stu-id="b1389-226">Response</span></span>
<span data-ttu-id="b1389-227">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b1389-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1389-228">例</span><span class="sxs-lookup"><span data-stu-id="b1389-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1389-229">要求</span><span class="sxs-lookup"><span data-stu-id="b1389-229">Request</span></span>
<span data-ttu-id="b1389-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1389-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="b1389-231">応答</span><span class="sxs-lookup"><span data-stu-id="b1389-231">Response</span></span>
<span data-ttu-id="b1389-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1389-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





