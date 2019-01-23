---
title: windows10CompliancePolicy の更新
description: windows10CompliancePolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 776cd0a059b985667aa31e5ed08ad298aa111849
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396232"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="4760f-103">windows10CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="4760f-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="4760f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4760f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4760f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4760f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4760f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4760f-107">[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4760f-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4760f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4760f-108">Prerequisites</span></span>
<span data-ttu-id="4760f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4760f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4760f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4760f-111">Permission type</span></span>|<span data-ttu-id="4760f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4760f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4760f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4760f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4760f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4760f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4760f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4760f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4760f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4760f-116">Not supported.</span></span>|
|<span data-ttu-id="4760f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4760f-117">Application</span></span>|<span data-ttu-id="4760f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4760f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4760f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4760f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4760f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4760f-120">Request headers</span></span>
|<span data-ttu-id="4760f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4760f-121">Header</span></span>|<span data-ttu-id="4760f-122">値</span><span class="sxs-lookup"><span data-stu-id="4760f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4760f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4760f-123">Authorization</span></span>|<span data-ttu-id="4760f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4760f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4760f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4760f-125">Accept</span></span>|<span data-ttu-id="4760f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4760f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4760f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4760f-127">Request body</span></span>
<span data-ttu-id="4760f-128">要求本文で、[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4760f-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="4760f-129">次の表に、[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4760f-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="4760f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4760f-130">Property</span></span>|<span data-ttu-id="4760f-131">型</span><span class="sxs-lookup"><span data-stu-id="4760f-131">Type</span></span>|<span data-ttu-id="4760f-132">説明</span><span class="sxs-lookup"><span data-stu-id="4760f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4760f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4760f-133">roleScopeTagIds</span></span>|<span data-ttu-id="4760f-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4760f-134">String collection</span></span>|<span data-ttu-id="4760f-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4760f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4760f-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-137">id</span><span class="sxs-lookup"><span data-stu-id="4760f-137">id</span></span>|<span data-ttu-id="4760f-138">String</span><span class="sxs-lookup"><span data-stu-id="4760f-138">String</span></span>|<span data-ttu-id="4760f-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4760f-139">Key of the entity.</span></span> <span data-ttu-id="4760f-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4760f-141">createdDateTime</span></span>|<span data-ttu-id="4760f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4760f-142">DateTimeOffset</span></span>|<span data-ttu-id="4760f-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4760f-143">DateTime the object was created.</span></span> <span data-ttu-id="4760f-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-145">説明</span><span class="sxs-lookup"><span data-stu-id="4760f-145">description</span></span>|<span data-ttu-id="4760f-146">String</span><span class="sxs-lookup"><span data-stu-id="4760f-146">String</span></span>|<span data-ttu-id="4760f-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4760f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4760f-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4760f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4760f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4760f-150">DateTimeOffset</span></span>|<span data-ttu-id="4760f-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4760f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="4760f-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4760f-153">displayName</span></span>|<span data-ttu-id="4760f-154">String</span><span class="sxs-lookup"><span data-stu-id="4760f-154">String</span></span>|<span data-ttu-id="4760f-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4760f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4760f-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-157">version</span><span class="sxs-lookup"><span data-stu-id="4760f-157">version</span></span>|<span data-ttu-id="4760f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-158">Int32</span></span>|<span data-ttu-id="4760f-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4760f-159">Version of the device configuration.</span></span> <span data-ttu-id="4760f-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4760f-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4760f-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4760f-161">passwordRequired</span></span>|<span data-ttu-id="4760f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-162">Boolean</span></span>|<span data-ttu-id="4760f-163">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="4760f-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4760f-164">passwordBlockSimple</span></span>|<span data-ttu-id="4760f-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-165">Boolean</span></span>|<span data-ttu-id="4760f-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4760f-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="4760f-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="4760f-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="4760f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-168">Boolean</span></span>|<span data-ttu-id="4760f-169">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="4760f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4760f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4760f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-171">Int32</span></span>|<span data-ttu-id="4760f-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4760f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4760f-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4760f-173">passwordExpirationDays</span></span>|<span data-ttu-id="4760f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-174">Int32</span></span>|<span data-ttu-id="4760f-175">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="4760f-175">The password expiration in days.</span></span>|
|<span data-ttu-id="4760f-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4760f-176">passwordMinimumLength</span></span>|<span data-ttu-id="4760f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-177">Int32</span></span>|<span data-ttu-id="4760f-178">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="4760f-178">The minimum password length.</span></span>|
|<span data-ttu-id="4760f-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4760f-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4760f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-180">Int32</span></span>|<span data-ttu-id="4760f-181">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="4760f-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4760f-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4760f-182">passwordRequiredType</span></span>|[<span data-ttu-id="4760f-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4760f-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4760f-184">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4760f-184">The required password type.</span></span> <span data-ttu-id="4760f-185">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="4760f-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4760f-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4760f-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4760f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="4760f-187">Int32</span></span>|<span data-ttu-id="4760f-188">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="4760f-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="4760f-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="4760f-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="4760f-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-190">Boolean</span></span>|<span data-ttu-id="4760f-191">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4760f-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4760f-192">osMinimumVersion</span></span>|<span data-ttu-id="4760f-193">String</span><span class="sxs-lookup"><span data-stu-id="4760f-193">String</span></span>|<span data-ttu-id="4760f-194">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="4760f-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="4760f-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4760f-195">osMaximumVersion</span></span>|<span data-ttu-id="4760f-196">String</span><span class="sxs-lookup"><span data-stu-id="4760f-196">String</span></span>|<span data-ttu-id="4760f-197">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="4760f-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="4760f-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4760f-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="4760f-199">String</span><span class="sxs-lookup"><span data-stu-id="4760f-199">String</span></span>|<span data-ttu-id="4760f-200">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="4760f-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="4760f-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4760f-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="4760f-202">String</span><span class="sxs-lookup"><span data-stu-id="4760f-202">String</span></span>|<span data-ttu-id="4760f-203">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="4760f-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="4760f-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="4760f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-205">Boolean</span></span>|<span data-ttu-id="4760f-206">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="4760f-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-207">bitLockerEnabled</span></span>|<span data-ttu-id="4760f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-208">Boolean</span></span>|<span data-ttu-id="4760f-209">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="4760f-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-210">secureBootEnabled</span></span>|<span data-ttu-id="4760f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-211">Boolean</span></span>|<span data-ttu-id="4760f-212">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="4760f-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="4760f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-214">Boolean</span></span>|<span data-ttu-id="4760f-215">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4760f-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4760f-216">storageRequireEncryption</span></span>|<span data-ttu-id="4760f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-217">Boolean</span></span>|<span data-ttu-id="4760f-218">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="4760f-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="4760f-219">activeFirewallRequired</span></span>|<span data-ttu-id="4760f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-220">Boolean</span></span>|<span data-ttu-id="4760f-221">Windows デバイス上のアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="4760f-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-222">defenderEnabled</span></span>|<span data-ttu-id="4760f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-223">Boolean</span></span>|<span data-ttu-id="4760f-224">Windows デバイスで Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="4760f-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="4760f-225">defenderVersion</span></span>|<span data-ttu-id="4760f-226">String</span><span class="sxs-lookup"><span data-stu-id="4760f-226">String</span></span>|<span data-ttu-id="4760f-227">Windows デバイスの最小バージョンの Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="4760f-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="4760f-228">signatureOutOfDate</span></span>|<span data-ttu-id="4760f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-229">Boolean</span></span>|<span data-ttu-id="4760f-230">Windows デバイスで最新のものに、Windows Defender のウイルス対策署名が必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="4760f-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-231">rtpEnabled</span></span>|<span data-ttu-id="4760f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-232">Boolean</span></span>|<span data-ttu-id="4760f-233">Windows デバイスでは、Windows Defender のウイルス対策のリアルタイム保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="4760f-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="4760f-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="4760f-234">antivirusRequired</span></span>|<span data-ttu-id="4760f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-235">Boolean</span></span>|<span data-ttu-id="4760f-236">上にある Windows セキュリティ センターに登録され、(例: シマンテック、Windows Defender) を監視するウイルス対策ソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="4760f-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="4760f-237">antiSpywareRequired</span></span>|<span data-ttu-id="4760f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-238">Boolean</span></span>|<span data-ttu-id="4760f-239">任意のウイルス対策ソリューションに Windows セキュリティ センターに登録され、監視 (シマンテック、Windows Defender など) が必要です。</span><span class="sxs-lookup"><span data-stu-id="4760f-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="4760f-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="4760f-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="4760f-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4760f-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="4760f-242">有効なオペレーティング システムは、Windows デバイス上の範囲を作成します。</span><span class="sxs-lookup"><span data-stu-id="4760f-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="4760f-243">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4760f-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4760f-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4760f-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4760f-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-245">Boolean</span></span>|<span data-ttu-id="4760f-246">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="4760f-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4760f-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4760f-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4760f-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4760f-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4760f-249">法令遵守の不履行を報告する最小のリスク レベルの脅威のデバイスの保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="4760f-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4760f-250">使用可能な値: `unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="4760f-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4760f-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="4760f-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="4760f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="4760f-252">Boolean</span></span>|<span data-ttu-id="4760f-253">Intune 準拠状態の考慮事項に SCCM の準拠状態を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4760f-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="4760f-254">応答</span><span class="sxs-lookup"><span data-stu-id="4760f-254">Response</span></span>
<span data-ttu-id="4760f-255">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4760f-255">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4760f-256">例</span><span class="sxs-lookup"><span data-stu-id="4760f-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="4760f-257">要求</span><span class="sxs-lookup"><span data-stu-id="4760f-257">Request</span></span>
<span data-ttu-id="4760f-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4760f-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="4760f-259">応答</span><span class="sxs-lookup"><span data-stu-id="4760f-259">Response</span></span>
<span data-ttu-id="4760f-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4760f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```




