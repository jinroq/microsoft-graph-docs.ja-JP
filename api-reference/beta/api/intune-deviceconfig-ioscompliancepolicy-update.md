---
title: iosCompliancePolicy の更新
description: iosCompliancePolicy オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a077c25710823b824435522b01fe28d16943f64c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923919"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="ba944-103">iosCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="ba944-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="ba944-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba944-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba944-106">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ba944-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba944-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ba944-107">Prerequisites</span></span>
<span data-ttu-id="ba944-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba944-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba944-110">Permission type</span></span>|<span data-ttu-id="ba944-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba944-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba944-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba944-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba944-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba944-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba944-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba944-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba944-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba944-115">Not supported.</span></span>|
|<span data-ttu-id="ba944-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba944-116">Application</span></span>|<span data-ttu-id="ba944-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba944-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba944-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba944-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ba944-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba944-119">Request headers</span></span>
|<span data-ttu-id="ba944-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba944-120">Header</span></span>|<span data-ttu-id="ba944-121">値</span><span class="sxs-lookup"><span data-stu-id="ba944-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba944-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba944-122">Authorization</span></span>|<span data-ttu-id="ba944-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba944-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba944-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ba944-124">Accept</span></span>|<span data-ttu-id="ba944-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba944-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba944-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba944-126">Request body</span></span>
<span data-ttu-id="ba944-127">要求本文で、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba944-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="ba944-128">次の表に、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ba944-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="ba944-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba944-129">Property</span></span>|<span data-ttu-id="ba944-130">型</span><span class="sxs-lookup"><span data-stu-id="ba944-130">Type</span></span>|<span data-ttu-id="ba944-131">説明</span><span class="sxs-lookup"><span data-stu-id="ba944-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba944-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ba944-132">roleScopeTagIds</span></span>|<span data-ttu-id="ba944-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ba944-133">String collection</span></span>|<span data-ttu-id="ba944-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ba944-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ba944-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-136">id</span><span class="sxs-lookup"><span data-stu-id="ba944-136">id</span></span>|<span data-ttu-id="ba944-137">文字列</span><span class="sxs-lookup"><span data-stu-id="ba944-137">String</span></span>|<span data-ttu-id="ba944-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ba944-138">Key of the entity.</span></span> <span data-ttu-id="ba944-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba944-140">createdDateTime</span></span>|<span data-ttu-id="ba944-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba944-141">DateTimeOffset</span></span>|<span data-ttu-id="ba944-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ba944-142">DateTime the object was created.</span></span> <span data-ttu-id="ba944-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-144">description</span><span class="sxs-lookup"><span data-stu-id="ba944-144">description</span></span>|<span data-ttu-id="ba944-145">String</span><span class="sxs-lookup"><span data-stu-id="ba944-145">String</span></span>|<span data-ttu-id="ba944-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ba944-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba944-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba944-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ba944-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba944-149">DateTimeOffset</span></span>|<span data-ttu-id="ba944-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ba944-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ba944-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ba944-152">displayName</span></span>|<span data-ttu-id="ba944-153">String</span><span class="sxs-lookup"><span data-stu-id="ba944-153">String</span></span>|<span data-ttu-id="ba944-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ba944-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba944-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-156">version</span><span class="sxs-lookup"><span data-stu-id="ba944-156">version</span></span>|<span data-ttu-id="ba944-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-157">Int32</span></span>|<span data-ttu-id="ba944-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ba944-158">Version of the device configuration.</span></span> <span data-ttu-id="ba944-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba944-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba944-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ba944-160">passcodeBlockSimple</span></span>|<span data-ttu-id="ba944-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba944-161">Boolean</span></span>|<span data-ttu-id="ba944-162">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba944-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ba944-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ba944-163">passcodeExpirationDays</span></span>|<span data-ttu-id="ba944-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-164">Int32</span></span>|<span data-ttu-id="ba944-165">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="ba944-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="ba944-166">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="ba944-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ba944-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ba944-167">passcodeMinimumLength</span></span>|<span data-ttu-id="ba944-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-168">Int32</span></span>|<span data-ttu-id="ba944-169">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="ba944-169">Minimum length of passcode.</span></span> <span data-ttu-id="ba944-170">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="ba944-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ba944-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ba944-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ba944-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-172">Int32</span></span>|<span data-ttu-id="ba944-173">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ba944-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ba944-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ba944-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ba944-175">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-175">Int32</span></span>|<span data-ttu-id="ba944-176">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ba944-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ba944-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ba944-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ba944-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-178">Int32</span></span>|<span data-ttu-id="ba944-179">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="ba944-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="ba944-180">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="ba944-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ba944-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ba944-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ba944-182">Int32</span><span class="sxs-lookup"><span data-stu-id="ba944-182">Int32</span></span>|<span data-ttu-id="ba944-183">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="ba944-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ba944-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ba944-184">passcodeRequiredType</span></span>|[<span data-ttu-id="ba944-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ba944-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ba944-186">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="ba944-186">The required passcode type.</span></span> <span data-ttu-id="ba944-187">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="ba944-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ba944-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ba944-188">passcodeRequired</span></span>|<span data-ttu-id="ba944-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba944-189">Boolean</span></span>|<span data-ttu-id="ba944-190">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ba944-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ba944-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ba944-191">osMinimumVersion</span></span>|<span data-ttu-id="ba944-192">String</span><span class="sxs-lookup"><span data-stu-id="ba944-192">String</span></span>|<span data-ttu-id="ba944-193">最小の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="ba944-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="ba944-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ba944-194">osMaximumVersion</span></span>|<span data-ttu-id="ba944-195">String</span><span class="sxs-lookup"><span data-stu-id="ba944-195">String</span></span>|<span data-ttu-id="ba944-196">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="ba944-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="ba944-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="ba944-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="ba944-198">String</span><span class="sxs-lookup"><span data-stu-id="ba944-198">String</span></span>|<span data-ttu-id="ba944-199">最小の IOS ビルドバージョン。</span><span class="sxs-lookup"><span data-stu-id="ba944-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="ba944-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="ba944-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="ba944-201">String</span><span class="sxs-lookup"><span data-stu-id="ba944-201">String</span></span>|<span data-ttu-id="ba944-202">IOS ビルドの最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="ba944-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="ba944-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="ba944-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="ba944-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba944-204">Boolean</span></span>|<span data-ttu-id="ba944-205">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="ba944-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="ba944-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ba944-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ba944-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba944-207">Boolean</span></span>|<span data-ttu-id="ba944-208">デバイスの脅威保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba944-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="ba944-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ba944-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ba944-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ba944-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ba944-211">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="ba944-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ba944-212">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="ba944-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ba944-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="ba944-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="ba944-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba944-214">Boolean</span></span>|<span data-ttu-id="ba944-215">管理された電子メール プロファイルを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba944-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="ba944-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="ba944-216">restrictedApps</span></span>|<span data-ttu-id="ba944-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ba944-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ba944-218">デバイスに、指定されたアプリがインストールされていないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="ba944-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="ba944-219">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ba944-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ba944-220">応答</span><span class="sxs-lookup"><span data-stu-id="ba944-220">Response</span></span>
<span data-ttu-id="ba944-221">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ba944-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba944-222">例</span><span class="sxs-lookup"><span data-stu-id="ba944-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba944-223">要求</span><span class="sxs-lookup"><span data-stu-id="ba944-223">Request</span></span>
<span data-ttu-id="ba944-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba944-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba944-225">応答</span><span class="sxs-lookup"><span data-stu-id="ba944-225">Response</span></span>
<span data-ttu-id="ba944-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba944-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




