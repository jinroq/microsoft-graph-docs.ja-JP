---
title: windows10CompliancePolicy の更新
description: windows10CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 700789db9918d51a86d814f7154283370841f6df
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258822"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="67c32-103">windows10CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="67c32-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="67c32-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67c32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c32-105">[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67c32-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67c32-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="67c32-106">Prerequisites</span></span>
<span data-ttu-id="67c32-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67c32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67c32-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67c32-109">Permission type</span></span>|<span data-ttu-id="67c32-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67c32-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67c32-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67c32-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67c32-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c32-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67c32-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67c32-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67c32-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c32-114">Not supported.</span></span>|
|<span data-ttu-id="67c32-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67c32-115">Application</span></span>|<span data-ttu-id="67c32-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c32-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67c32-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67c32-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="67c32-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c32-118">Request headers</span></span>
|<span data-ttu-id="67c32-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c32-119">Header</span></span>|<span data-ttu-id="67c32-120">値</span><span class="sxs-lookup"><span data-stu-id="67c32-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67c32-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c32-121">Authorization</span></span>|<span data-ttu-id="67c32-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67c32-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67c32-123">承諾</span><span class="sxs-lookup"><span data-stu-id="67c32-123">Accept</span></span>|<span data-ttu-id="67c32-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67c32-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c32-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67c32-125">Request body</span></span>
<span data-ttu-id="67c32-126">要求本文で、[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67c32-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="67c32-127">次の表に、[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67c32-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="67c32-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67c32-128">Property</span></span>|<span data-ttu-id="67c32-129">型</span><span class="sxs-lookup"><span data-stu-id="67c32-129">Type</span></span>|<span data-ttu-id="67c32-130">説明</span><span class="sxs-lookup"><span data-stu-id="67c32-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c32-131">id</span><span class="sxs-lookup"><span data-stu-id="67c32-131">id</span></span>|<span data-ttu-id="67c32-132">文字列</span><span class="sxs-lookup"><span data-stu-id="67c32-132">String</span></span>|<span data-ttu-id="67c32-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67c32-133">Key of the entity.</span></span> <span data-ttu-id="67c32-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67c32-135">createdDateTime</span></span>|<span data-ttu-id="67c32-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c32-136">DateTimeOffset</span></span>|<span data-ttu-id="67c32-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="67c32-137">DateTime the object was created.</span></span> <span data-ttu-id="67c32-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-139">説明</span><span class="sxs-lookup"><span data-stu-id="67c32-139">description</span></span>|<span data-ttu-id="67c32-140">文字列</span><span class="sxs-lookup"><span data-stu-id="67c32-140">String</span></span>|<span data-ttu-id="67c32-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="67c32-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67c32-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67c32-143">lastModifiedDateTime</span></span>|<span data-ttu-id="67c32-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c32-144">DateTimeOffset</span></span>|<span data-ttu-id="67c32-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="67c32-145">DateTime the object was last modified.</span></span> <span data-ttu-id="67c32-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-147">displayName</span><span class="sxs-lookup"><span data-stu-id="67c32-147">displayName</span></span>|<span data-ttu-id="67c32-148">String</span><span class="sxs-lookup"><span data-stu-id="67c32-148">String</span></span>|<span data-ttu-id="67c32-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="67c32-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67c32-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-151">version</span><span class="sxs-lookup"><span data-stu-id="67c32-151">version</span></span>|<span data-ttu-id="67c32-152">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-152">Int32</span></span>|<span data-ttu-id="67c32-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="67c32-153">Version of the device configuration.</span></span> <span data-ttu-id="67c32-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c32-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67c32-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="67c32-155">passwordRequired</span></span>|<span data-ttu-id="67c32-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-156">Boolean</span></span>|<span data-ttu-id="67c32-157">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="67c32-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="67c32-158">passwordBlockSimple</span></span>|<span data-ttu-id="67c32-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-159">Boolean</span></span>|<span data-ttu-id="67c32-160">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="67c32-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="67c32-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="67c32-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="67c32-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-162">Boolean</span></span>|<span data-ttu-id="67c32-163">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="67c32-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="67c32-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="67c32-165">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-165">Int32</span></span>|<span data-ttu-id="67c32-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="67c32-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="67c32-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="67c32-167">passwordExpirationDays</span></span>|<span data-ttu-id="67c32-168">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-168">Int32</span></span>|<span data-ttu-id="67c32-169">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="67c32-169">The password expiration in days.</span></span>|
|<span data-ttu-id="67c32-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="67c32-170">passwordMinimumLength</span></span>|<span data-ttu-id="67c32-171">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-171">Int32</span></span>|<span data-ttu-id="67c32-172">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="67c32-172">The minimum password length.</span></span>|
|<span data-ttu-id="67c32-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="67c32-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="67c32-174">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-174">Int32</span></span>|<span data-ttu-id="67c32-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="67c32-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="67c32-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="67c32-176">passwordRequiredType</span></span>|[<span data-ttu-id="67c32-177">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="67c32-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="67c32-178">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="67c32-178">The required password type.</span></span> <span data-ttu-id="67c32-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="67c32-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="67c32-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="67c32-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="67c32-181">Int32</span><span class="sxs-lookup"><span data-stu-id="67c32-181">Int32</span></span>|<span data-ttu-id="67c32-182">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="67c32-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="67c32-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="67c32-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="67c32-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-184">Boolean</span></span>|<span data-ttu-id="67c32-185">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="67c32-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="67c32-186">osMinimumVersion</span></span>|<span data-ttu-id="67c32-187">String</span><span class="sxs-lookup"><span data-stu-id="67c32-187">String</span></span>|<span data-ttu-id="67c32-188">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="67c32-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="67c32-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="67c32-189">osMaximumVersion</span></span>|<span data-ttu-id="67c32-190">String</span><span class="sxs-lookup"><span data-stu-id="67c32-190">String</span></span>|<span data-ttu-id="67c32-191">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="67c32-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="67c32-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="67c32-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="67c32-193">String</span><span class="sxs-lookup"><span data-stu-id="67c32-193">String</span></span>|<span data-ttu-id="67c32-194">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="67c32-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="67c32-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="67c32-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="67c32-196">String</span><span class="sxs-lookup"><span data-stu-id="67c32-196">String</span></span>|<span data-ttu-id="67c32-197">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="67c32-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="67c32-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="67c32-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="67c32-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-199">Boolean</span></span>|<span data-ttu-id="67c32-200">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="67c32-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="67c32-201">bitLockerEnabled</span></span>|<span data-ttu-id="67c32-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-202">Boolean</span></span>|<span data-ttu-id="67c32-203">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="67c32-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="67c32-204">secureBootEnabled</span></span>|<span data-ttu-id="67c32-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-205">Boolean</span></span>|<span data-ttu-id="67c32-206">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="67c32-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="67c32-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="67c32-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-208">Boolean</span></span>|<span data-ttu-id="67c32-209">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="67c32-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="67c32-210">storageRequireEncryption</span></span>|<span data-ttu-id="67c32-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c32-211">Boolean</span></span>|<span data-ttu-id="67c32-212">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="67c32-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="67c32-213">応答</span><span class="sxs-lookup"><span data-stu-id="67c32-213">Response</span></span>
<span data-ttu-id="67c32-214">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="67c32-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c32-215">例</span><span class="sxs-lookup"><span data-stu-id="67c32-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="67c32-216">要求</span><span class="sxs-lookup"><span data-stu-id="67c32-216">Request</span></span>
<span data-ttu-id="67c32-217">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67c32-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="67c32-218">応答</span><span class="sxs-lookup"><span data-stu-id="67c32-218">Response</span></span>
<span data-ttu-id="67c32-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67c32-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



