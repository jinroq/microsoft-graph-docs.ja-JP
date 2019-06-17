---
title: macOSCompliancePolicy の更新
description: macOSCompliancePolicy オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7f262efdf3d49a4543d7ac4b3188dfb0a4b5a78
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976905"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="0713e-103">macOSCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="0713e-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="0713e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0713e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0713e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0713e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0713e-106">[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0713e-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0713e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0713e-107">Prerequisites</span></span>
<span data-ttu-id="0713e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0713e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0713e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0713e-110">Permission type</span></span>|<span data-ttu-id="0713e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0713e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0713e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0713e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0713e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0713e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0713e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0713e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0713e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0713e-115">Not supported.</span></span>|
|<span data-ttu-id="0713e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0713e-116">Application</span></span>|<span data-ttu-id="0713e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0713e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0713e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0713e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0713e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0713e-119">Request headers</span></span>
|<span data-ttu-id="0713e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0713e-120">Header</span></span>|<span data-ttu-id="0713e-121">値</span><span class="sxs-lookup"><span data-stu-id="0713e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0713e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0713e-122">Authorization</span></span>|<span data-ttu-id="0713e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0713e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0713e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0713e-124">Accept</span></span>|<span data-ttu-id="0713e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0713e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0713e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0713e-126">Request body</span></span>
<span data-ttu-id="0713e-127">要求本文で、[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0713e-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="0713e-128">次の表に、[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0713e-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="0713e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0713e-129">Property</span></span>|<span data-ttu-id="0713e-130">型</span><span class="sxs-lookup"><span data-stu-id="0713e-130">Type</span></span>|<span data-ttu-id="0713e-131">説明</span><span class="sxs-lookup"><span data-stu-id="0713e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0713e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0713e-132">roleScopeTagIds</span></span>|<span data-ttu-id="0713e-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0713e-133">String collection</span></span>|<span data-ttu-id="0713e-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0713e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0713e-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-136">id</span><span class="sxs-lookup"><span data-stu-id="0713e-136">id</span></span>|<span data-ttu-id="0713e-137">文字列</span><span class="sxs-lookup"><span data-stu-id="0713e-137">String</span></span>|<span data-ttu-id="0713e-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0713e-138">Key of the entity.</span></span> <span data-ttu-id="0713e-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0713e-140">createdDateTime</span></span>|<span data-ttu-id="0713e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0713e-141">DateTimeOffset</span></span>|<span data-ttu-id="0713e-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0713e-142">DateTime the object was created.</span></span> <span data-ttu-id="0713e-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-144">description</span><span class="sxs-lookup"><span data-stu-id="0713e-144">description</span></span>|<span data-ttu-id="0713e-145">String</span><span class="sxs-lookup"><span data-stu-id="0713e-145">String</span></span>|<span data-ttu-id="0713e-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0713e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0713e-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0713e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0713e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0713e-149">DateTimeOffset</span></span>|<span data-ttu-id="0713e-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0713e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="0713e-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="0713e-152">displayName</span></span>|<span data-ttu-id="0713e-153">String</span><span class="sxs-lookup"><span data-stu-id="0713e-153">String</span></span>|<span data-ttu-id="0713e-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0713e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0713e-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-156">version</span><span class="sxs-lookup"><span data-stu-id="0713e-156">version</span></span>|<span data-ttu-id="0713e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-157">Int32</span></span>|<span data-ttu-id="0713e-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0713e-158">Version of the device configuration.</span></span> <span data-ttu-id="0713e-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0713e-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0713e-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0713e-160">passwordRequired</span></span>|<span data-ttu-id="0713e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-161">Boolean</span></span>|<span data-ttu-id="0713e-162">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0713e-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0713e-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0713e-163">passwordBlockSimple</span></span>|<span data-ttu-id="0713e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-164">Boolean</span></span>|<span data-ttu-id="0713e-165">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0713e-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="0713e-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0713e-166">passwordExpirationDays</span></span>|<span data-ttu-id="0713e-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-167">Int32</span></span>|<span data-ttu-id="0713e-168">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="0713e-168">Number of days before the password expires.</span></span> <span data-ttu-id="0713e-169">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="0713e-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0713e-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0713e-170">passwordMinimumLength</span></span>|<span data-ttu-id="0713e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-171">Int32</span></span>|<span data-ttu-id="0713e-172">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="0713e-172">Minimum length of password.</span></span> <span data-ttu-id="0713e-173">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="0713e-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0713e-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0713e-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0713e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-175">Int32</span></span>|<span data-ttu-id="0713e-176">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="0713e-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0713e-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0713e-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0713e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-178">Int32</span></span>|<span data-ttu-id="0713e-179">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="0713e-179">Number of previous passwords to block.</span></span> <span data-ttu-id="0713e-180">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="0713e-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0713e-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0713e-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0713e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0713e-182">Int32</span></span>|<span data-ttu-id="0713e-183">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="0713e-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0713e-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0713e-184">passwordRequiredType</span></span>|[<span data-ttu-id="0713e-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0713e-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0713e-186">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="0713e-186">The required password type.</span></span> <span data-ttu-id="0713e-187">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="0713e-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0713e-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0713e-188">osMinimumVersion</span></span>|<span data-ttu-id="0713e-189">String</span><span class="sxs-lookup"><span data-stu-id="0713e-189">String</span></span>|<span data-ttu-id="0713e-190">最小 Os バージョン。</span><span class="sxs-lookup"><span data-stu-id="0713e-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="0713e-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0713e-191">osMaximumVersion</span></span>|<span data-ttu-id="0713e-192">String</span><span class="sxs-lookup"><span data-stu-id="0713e-192">String</span></span>|<span data-ttu-id="0713e-193">最大 Os バージョン。</span><span class="sxs-lookup"><span data-stu-id="0713e-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="0713e-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0713e-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="0713e-195">String</span><span class="sxs-lookup"><span data-stu-id="0713e-195">String</span></span>|<span data-ttu-id="0713e-196">最小 Os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="0713e-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="0713e-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0713e-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="0713e-198">String</span><span class="sxs-lookup"><span data-stu-id="0713e-198">String</span></span>|<span data-ttu-id="0713e-199">最大 Os ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="0713e-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="0713e-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0713e-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="0713e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-201">Boolean</span></span>|<span data-ttu-id="0713e-202">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0713e-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="0713e-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0713e-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0713e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-204">Boolean</span></span>|<span data-ttu-id="0713e-205">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="0713e-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0713e-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0713e-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0713e-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0713e-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0713e-208">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="0713e-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0713e-209">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="0713e-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0713e-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0713e-210">storageRequireEncryption</span></span>|<span data-ttu-id="0713e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-211">Boolean</span></span>|<span data-ttu-id="0713e-212">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="0713e-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="0713e-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="0713e-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="0713e-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="0713e-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="0713e-215">MacOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="0713e-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="0713e-216">使用可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="0713e-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="0713e-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0713e-217">firewallEnabled</span></span>|<span data-ttu-id="0713e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-218">Boolean</span></span>|<span data-ttu-id="0713e-219">ファイアウォールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0713e-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0713e-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0713e-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0713e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-221">Boolean</span></span>|<span data-ttu-id="0713e-222">[着信接続をすべてブロックする] オプションに対応しています。</span><span class="sxs-lookup"><span data-stu-id="0713e-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0713e-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0713e-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="0713e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0713e-224">Boolean</span></span>|<span data-ttu-id="0713e-225">[ステルスモードを有効にする] に相当します。</span><span class="sxs-lookup"><span data-stu-id="0713e-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="0713e-226">応答</span><span class="sxs-lookup"><span data-stu-id="0713e-226">Response</span></span>
<span data-ttu-id="0713e-227">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="0713e-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0713e-228">例</span><span class="sxs-lookup"><span data-stu-id="0713e-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="0713e-229">要求</span><span class="sxs-lookup"><span data-stu-id="0713e-229">Request</span></span>
<span data-ttu-id="0713e-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0713e-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0713e-231">応答</span><span class="sxs-lookup"><span data-stu-id="0713e-231">Response</span></span>
<span data-ttu-id="0713e-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0713e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





