---
title: windows10CompliancePolicy の作成
description: 新しい windows10CompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c03c8a3b8ce4ac43da35eba89b18bc57c5db867a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982505"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="b11f6-103">windows10CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="b11f6-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="b11f6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b11f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b11f6-105">新しい [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-105">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b11f6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b11f6-106">Prerequisites</span></span>
<span data-ttu-id="b11f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b11f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b11f6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b11f6-109">Permission type</span></span>|<span data-ttu-id="b11f6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b11f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b11f6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b11f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b11f6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b11f6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b11f6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b11f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b11f6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b11f6-114">Not supported.</span></span>|
|<span data-ttu-id="b11f6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b11f6-115">Application</span></span>|<span data-ttu-id="b11f6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b11f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b11f6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b11f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b11f6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b11f6-118">Request headers</span></span>
|<span data-ttu-id="b11f6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b11f6-119">Header</span></span>|<span data-ttu-id="b11f6-120">値</span><span class="sxs-lookup"><span data-stu-id="b11f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b11f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b11f6-121">Authorization</span></span>|<span data-ttu-id="b11f6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b11f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b11f6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b11f6-123">Accept</span></span>|<span data-ttu-id="b11f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b11f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b11f6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b11f6-125">Request body</span></span>
<span data-ttu-id="b11f6-126">要求本文で、windows10CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-126">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="b11f6-127">次の表に、windows10CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-127">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="b11f6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b11f6-128">Property</span></span>|<span data-ttu-id="b11f6-129">型</span><span class="sxs-lookup"><span data-stu-id="b11f6-129">Type</span></span>|<span data-ttu-id="b11f6-130">説明</span><span class="sxs-lookup"><span data-stu-id="b11f6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11f6-131">id</span><span class="sxs-lookup"><span data-stu-id="b11f6-131">id</span></span>|<span data-ttu-id="b11f6-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b11f6-132">String</span></span>|<span data-ttu-id="b11f6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b11f6-133">Key of the entity.</span></span> <span data-ttu-id="b11f6-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b11f6-135">createdDateTime</span></span>|<span data-ttu-id="b11f6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b11f6-136">DateTimeOffset</span></span>|<span data-ttu-id="b11f6-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b11f6-137">DateTime the object was created.</span></span> <span data-ttu-id="b11f6-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-139">description</span><span class="sxs-lookup"><span data-stu-id="b11f6-139">description</span></span>|<span data-ttu-id="b11f6-140">String</span><span class="sxs-lookup"><span data-stu-id="b11f6-140">String</span></span>|<span data-ttu-id="b11f6-141">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b11f6-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b11f6-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b11f6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b11f6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b11f6-144">DateTimeOffset</span></span>|<span data-ttu-id="b11f6-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b11f6-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b11f6-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b11f6-147">displayName</span></span>|<span data-ttu-id="b11f6-148">String</span><span class="sxs-lookup"><span data-stu-id="b11f6-148">String</span></span>|<span data-ttu-id="b11f6-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b11f6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b11f6-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-151">version</span><span class="sxs-lookup"><span data-stu-id="b11f6-151">version</span></span>|<span data-ttu-id="b11f6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-152">Int32</span></span>|<span data-ttu-id="b11f6-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b11f6-153">Version of the device configuration.</span></span> <span data-ttu-id="b11f6-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b11f6-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b11f6-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b11f6-155">passwordRequired</span></span>|<span data-ttu-id="b11f6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-156">Boolean</span></span>|<span data-ttu-id="b11f6-157">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b11f6-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b11f6-158">passwordBlockSimple</span></span>|<span data-ttu-id="b11f6-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-159">Boolean</span></span>|<span data-ttu-id="b11f6-160">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b11f6-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="b11f6-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="b11f6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-162">Boolean</span></span>|<span data-ttu-id="b11f6-163">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="b11f6-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b11f6-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b11f6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-165">Int32</span></span>|<span data-ttu-id="b11f6-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b11f6-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b11f6-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b11f6-167">passwordExpirationDays</span></span>|<span data-ttu-id="b11f6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-168">Int32</span></span>|<span data-ttu-id="b11f6-169">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="b11f6-169">The password expiration in days.</span></span>|
|<span data-ttu-id="b11f6-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b11f6-170">passwordMinimumLength</span></span>|<span data-ttu-id="b11f6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-171">Int32</span></span>|<span data-ttu-id="b11f6-172">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="b11f6-172">The minimum password length.</span></span>|
|<span data-ttu-id="b11f6-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b11f6-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b11f6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-174">Int32</span></span>|<span data-ttu-id="b11f6-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="b11f6-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b11f6-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b11f6-176">passwordRequiredType</span></span>|[<span data-ttu-id="b11f6-177">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="b11f6-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b11f6-178">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="b11f6-178">The required password type.</span></span> <span data-ttu-id="b11f6-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="b11f6-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b11f6-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b11f6-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b11f6-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b11f6-181">Int32</span></span>|<span data-ttu-id="b11f6-182">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="b11f6-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="b11f6-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="b11f6-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="b11f6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-184">Boolean</span></span>|<span data-ttu-id="b11f6-185">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b11f6-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b11f6-186">osMinimumVersion</span></span>|<span data-ttu-id="b11f6-187">String</span><span class="sxs-lookup"><span data-stu-id="b11f6-187">String</span></span>|<span data-ttu-id="b11f6-188">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="b11f6-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="b11f6-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b11f6-189">osMaximumVersion</span></span>|<span data-ttu-id="b11f6-190">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b11f6-190">String</span></span>|<span data-ttu-id="b11f6-191">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="b11f6-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="b11f6-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b11f6-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="b11f6-193">String</span><span class="sxs-lookup"><span data-stu-id="b11f6-193">String</span></span>|<span data-ttu-id="b11f6-194">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="b11f6-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b11f6-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b11f6-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="b11f6-196">String</span><span class="sxs-lookup"><span data-stu-id="b11f6-196">String</span></span>|<span data-ttu-id="b11f6-197">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="b11f6-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b11f6-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="b11f6-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="b11f6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-199">Boolean</span></span>|<span data-ttu-id="b11f6-200">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="b11f6-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="b11f6-201">bitLockerEnabled</span></span>|<span data-ttu-id="b11f6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-202">Boolean</span></span>|<span data-ttu-id="b11f6-203">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="b11f6-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="b11f6-204">secureBootEnabled</span></span>|<span data-ttu-id="b11f6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-205">Boolean</span></span>|<span data-ttu-id="b11f6-206">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="b11f6-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="b11f6-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="b11f6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-208">Boolean</span></span>|<span data-ttu-id="b11f6-209">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b11f6-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b11f6-210">storageRequireEncryption</span></span>|<span data-ttu-id="b11f6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b11f6-211">Boolean</span></span>|<span data-ttu-id="b11f6-212">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b11f6-213">応答</span><span class="sxs-lookup"><span data-stu-id="b11f6-213">Response</span></span>
<span data-ttu-id="b11f6-214">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b11f6-214">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b11f6-215">例</span><span class="sxs-lookup"><span data-stu-id="b11f6-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="b11f6-216">要求</span><span class="sxs-lookup"><span data-stu-id="b11f6-216">Request</span></span>
<span data-ttu-id="b11f6-217">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b11f6-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="b11f6-218">応答</span><span class="sxs-lookup"><span data-stu-id="b11f6-218">Response</span></span>
<span data-ttu-id="b11f6-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b11f6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```



