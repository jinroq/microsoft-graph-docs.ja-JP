---
title: iosCompliancePolicy の更新
description: iosCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 524ffd9bbaf7b6a0e5d1e912d52af8137e59049f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167698"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="cfe3f-103">iosCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="cfe3f-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="cfe3f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfe3f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe3f-106">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfe3f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cfe3f-107">Prerequisites</span></span>
<span data-ttu-id="cfe3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cfe3f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfe3f-110">Permission type</span></span>|<span data-ttu-id="cfe3f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfe3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe3f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe3f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe3f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe3f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe3f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-115">Not supported.</span></span>|
|<span data-ttu-id="cfe3f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfe3f-116">Application</span></span>|<span data-ttu-id="cfe3f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe3f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfe3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="cfe3f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe3f-119">Request headers</span></span>
|<span data-ttu-id="cfe3f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe3f-120">Header</span></span>|<span data-ttu-id="cfe3f-121">値</span><span class="sxs-lookup"><span data-stu-id="cfe3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe3f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe3f-122">Authorization</span></span>|<span data-ttu-id="cfe3f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe3f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cfe3f-124">Accept</span></span>|<span data-ttu-id="cfe3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe3f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfe3f-126">Request body</span></span>
<span data-ttu-id="cfe3f-127">要求本文で、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="cfe3f-128">次の表に、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="cfe3f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfe3f-129">Property</span></span>|<span data-ttu-id="cfe3f-130">型</span><span class="sxs-lookup"><span data-stu-id="cfe3f-130">Type</span></span>|<span data-ttu-id="cfe3f-131">説明</span><span class="sxs-lookup"><span data-stu-id="cfe3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe3f-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfe3f-132">roleScopeTagIds</span></span>|<span data-ttu-id="cfe3f-133">String collection</span><span class="sxs-lookup"><span data-stu-id="cfe3f-133">String collection</span></span>|<span data-ttu-id="cfe3f-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cfe3f-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-136">id</span><span class="sxs-lookup"><span data-stu-id="cfe3f-136">id</span></span>|<span data-ttu-id="cfe3f-137">文字列</span><span class="sxs-lookup"><span data-stu-id="cfe3f-137">String</span></span>|<span data-ttu-id="cfe3f-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-138">Key of the entity.</span></span> <span data-ttu-id="cfe3f-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe3f-140">createdDateTime</span></span>|<span data-ttu-id="cfe3f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe3f-141">DateTimeOffset</span></span>|<span data-ttu-id="cfe3f-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-142">DateTime the object was created.</span></span> <span data-ttu-id="cfe3f-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-144">説明</span><span class="sxs-lookup"><span data-stu-id="cfe3f-144">description</span></span>|<span data-ttu-id="cfe3f-145">文字列</span><span class="sxs-lookup"><span data-stu-id="cfe3f-145">String</span></span>|<span data-ttu-id="cfe3f-146">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cfe3f-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe3f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cfe3f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe3f-149">DateTimeOffset</span></span>|<span data-ttu-id="cfe3f-150">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-150">DateTime the object was last modified.</span></span> <span data-ttu-id="cfe3f-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="cfe3f-152">displayName</span></span>|<span data-ttu-id="cfe3f-153">String</span><span class="sxs-lookup"><span data-stu-id="cfe3f-153">String</span></span>|<span data-ttu-id="cfe3f-154">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cfe3f-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-156">version</span><span class="sxs-lookup"><span data-stu-id="cfe3f-156">version</span></span>|<span data-ttu-id="cfe3f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-157">Int32</span></span>|<span data-ttu-id="cfe3f-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-158">Version of the device configuration.</span></span> <span data-ttu-id="cfe3f-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe3f-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cfe3f-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cfe3f-160">passcodeBlockSimple</span></span>|<span data-ttu-id="cfe3f-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="cfe3f-161">Boolean</span></span>|<span data-ttu-id="cfe3f-162">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="cfe3f-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cfe3f-163">passcodeExpirationDays</span></span>|<span data-ttu-id="cfe3f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-164">Int32</span></span>|<span data-ttu-id="cfe3f-165">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="cfe3f-166">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="cfe3f-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cfe3f-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cfe3f-167">passcodeMinimumLength</span></span>|<span data-ttu-id="cfe3f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-168">Int32</span></span>|<span data-ttu-id="cfe3f-169">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-169">Minimum length of passcode.</span></span> <span data-ttu-id="cfe3f-170">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="cfe3f-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="cfe3f-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cfe3f-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cfe3f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-172">Int32</span></span>|<span data-ttu-id="cfe3f-173">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="cfe3f-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cfe3f-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cfe3f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-175">Int32</span></span>|<span data-ttu-id="cfe3f-176">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="cfe3f-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="cfe3f-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="cfe3f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-178">Int32</span></span>|<span data-ttu-id="cfe3f-179">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="cfe3f-180">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="cfe3f-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cfe3f-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cfe3f-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="cfe3f-182">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe3f-182">Int32</span></span>|<span data-ttu-id="cfe3f-183">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cfe3f-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="cfe3f-184">passcodeRequiredType</span></span>|[<span data-ttu-id="cfe3f-185">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="cfe3f-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cfe3f-186">要求されるパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-186">The required passcode type.</span></span> <span data-ttu-id="cfe3f-187">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cfe3f-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="cfe3f-188">passcodeRequired</span></span>|<span data-ttu-id="cfe3f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe3f-189">Boolean</span></span>|<span data-ttu-id="cfe3f-190">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="cfe3f-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cfe3f-191">osMinimumVersion</span></span>|<span data-ttu-id="cfe3f-192">String</span><span class="sxs-lookup"><span data-stu-id="cfe3f-192">String</span></span>|<span data-ttu-id="cfe3f-193">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="cfe3f-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cfe3f-194">osMaximumVersion</span></span>|<span data-ttu-id="cfe3f-195">String</span><span class="sxs-lookup"><span data-stu-id="cfe3f-195">String</span></span>|<span data-ttu-id="cfe3f-196">iOS の最高バージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="cfe3f-197">osminimumbuildversion</span><span class="sxs-lookup"><span data-stu-id="cfe3f-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="cfe3f-198">String</span><span class="sxs-lookup"><span data-stu-id="cfe3f-198">String</span></span>|<span data-ttu-id="cfe3f-199">最小の IOS ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="cfe3f-200">osmaximumbuildversion</span><span class="sxs-lookup"><span data-stu-id="cfe3f-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="cfe3f-201">String</span><span class="sxs-lookup"><span data-stu-id="cfe3f-201">String</span></span>|<span data-ttu-id="cfe3f-202">IOS ビルドの最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="cfe3f-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="cfe3f-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="cfe3f-204">ブール値</span><span class="sxs-lookup"><span data-stu-id="cfe3f-204">Boolean</span></span>|<span data-ttu-id="cfe3f-205">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="cfe3f-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cfe3f-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cfe3f-207">ブール値</span><span class="sxs-lookup"><span data-stu-id="cfe3f-207">Boolean</span></span>|<span data-ttu-id="cfe3f-208">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="cfe3f-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cfe3f-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cfe3f-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cfe3f-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cfe3f-211">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cfe3f-212">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cfe3f-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="cfe3f-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="cfe3f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe3f-214">Boolean</span></span>|<span data-ttu-id="cfe3f-215">管理された電子メール プロファイルを必要とするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="cfe3f-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="cfe3f-216">restrictedApps</span></span>|<span data-ttu-id="cfe3f-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cfe3f-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cfe3f-218">デバイスに、指定されたアプリがインストールされていないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="cfe3f-219">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="cfe3f-220">応答</span><span class="sxs-lookup"><span data-stu-id="cfe3f-220">Response</span></span>
<span data-ttu-id="cfe3f-221">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe3f-222">例</span><span class="sxs-lookup"><span data-stu-id="cfe3f-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfe3f-223">要求</span><span class="sxs-lookup"><span data-stu-id="cfe3f-223">Request</span></span>
<span data-ttu-id="cfe3f-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cfe3f-225">応答</span><span class="sxs-lookup"><span data-stu-id="cfe3f-225">Response</span></span>
<span data-ttu-id="cfe3f-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfe3f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




