---
title: iosCompliancePolicy の更新
description: iosCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb8b8590fd59154fce31912d6275d23929a66f94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552842"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="f847c-103">iosCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="f847c-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="f847c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f847c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f847c-105">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f847c-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f847c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f847c-106">Prerequisites</span></span>
<span data-ttu-id="f847c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f847c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f847c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f847c-109">Permission type</span></span>|<span data-ttu-id="f847c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f847c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f847c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f847c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f847c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f847c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f847c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f847c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f847c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f847c-114">Not supported.</span></span>|
|<span data-ttu-id="f847c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f847c-115">Application</span></span>|<span data-ttu-id="f847c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f847c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f847c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f847c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f847c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f847c-118">Request headers</span></span>
|<span data-ttu-id="f847c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f847c-119">Header</span></span>|<span data-ttu-id="f847c-120">値</span><span class="sxs-lookup"><span data-stu-id="f847c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f847c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f847c-121">Authorization</span></span>|<span data-ttu-id="f847c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f847c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f847c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f847c-123">Accept</span></span>|<span data-ttu-id="f847c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f847c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f847c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f847c-125">Request body</span></span>
<span data-ttu-id="f847c-126">要求本文で、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f847c-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="f847c-127">次の表に、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f847c-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="f847c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f847c-128">Property</span></span>|<span data-ttu-id="f847c-129">型</span><span class="sxs-lookup"><span data-stu-id="f847c-129">Type</span></span>|<span data-ttu-id="f847c-130">説明</span><span class="sxs-lookup"><span data-stu-id="f847c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f847c-131">id</span><span class="sxs-lookup"><span data-stu-id="f847c-131">id</span></span>|<span data-ttu-id="f847c-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f847c-132">String</span></span>|<span data-ttu-id="f847c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f847c-133">Key of the entity.</span></span> <span data-ttu-id="f847c-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f847c-135">createdDateTime</span></span>|<span data-ttu-id="f847c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f847c-136">DateTimeOffset</span></span>|<span data-ttu-id="f847c-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f847c-137">DateTime the object was created.</span></span> <span data-ttu-id="f847c-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-139">description</span><span class="sxs-lookup"><span data-stu-id="f847c-139">description</span></span>|<span data-ttu-id="f847c-140">String</span><span class="sxs-lookup"><span data-stu-id="f847c-140">String</span></span>|<span data-ttu-id="f847c-141">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f847c-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f847c-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f847c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f847c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f847c-144">DateTimeOffset</span></span>|<span data-ttu-id="f847c-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f847c-145">DateTime the object was last modified.</span></span> <span data-ttu-id="f847c-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f847c-147">displayName</span></span>|<span data-ttu-id="f847c-148">String</span><span class="sxs-lookup"><span data-stu-id="f847c-148">String</span></span>|<span data-ttu-id="f847c-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f847c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f847c-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-151">version</span><span class="sxs-lookup"><span data-stu-id="f847c-151">version</span></span>|<span data-ttu-id="f847c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-152">Int32</span></span>|<span data-ttu-id="f847c-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f847c-153">Version of the device configuration.</span></span> <span data-ttu-id="f847c-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f847c-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f847c-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f847c-155">passcodeBlockSimple</span></span>|<span data-ttu-id="f847c-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="f847c-156">Boolean</span></span>|<span data-ttu-id="f847c-157">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f847c-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f847c-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f847c-158">passcodeExpirationDays</span></span>|<span data-ttu-id="f847c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-159">Int32</span></span>|<span data-ttu-id="f847c-160">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f847c-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="f847c-161">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="f847c-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f847c-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f847c-162">passcodeMinimumLength</span></span>|<span data-ttu-id="f847c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-163">Int32</span></span>|<span data-ttu-id="f847c-164">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="f847c-164">Minimum length of passcode.</span></span> <span data-ttu-id="f847c-165">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="f847c-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f847c-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f847c-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f847c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-167">Int32</span></span>|<span data-ttu-id="f847c-168">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f847c-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f847c-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f847c-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f847c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-170">Int32</span></span>|<span data-ttu-id="f847c-171">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="f847c-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="f847c-172">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f847c-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f847c-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f847c-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f847c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="f847c-174">Int32</span></span>|<span data-ttu-id="f847c-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="f847c-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f847c-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f847c-176">passcodeRequiredType</span></span>|[<span data-ttu-id="f847c-177">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="f847c-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f847c-178">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="f847c-178">The required passcode type.</span></span> <span data-ttu-id="f847c-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="f847c-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f847c-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f847c-180">passcodeRequired</span></span>|<span data-ttu-id="f847c-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="f847c-181">Boolean</span></span>|<span data-ttu-id="f847c-182">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f847c-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f847c-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f847c-183">osMinimumVersion</span></span>|<span data-ttu-id="f847c-184">String</span><span class="sxs-lookup"><span data-stu-id="f847c-184">String</span></span>|<span data-ttu-id="f847c-185">最小の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="f847c-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="f847c-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f847c-186">osMaximumVersion</span></span>|<span data-ttu-id="f847c-187">String</span><span class="sxs-lookup"><span data-stu-id="f847c-187">String</span></span>|<span data-ttu-id="f847c-188">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="f847c-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="f847c-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f847c-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f847c-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="f847c-190">Boolean</span></span>|<span data-ttu-id="f847c-191">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="f847c-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f847c-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f847c-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f847c-193">ブール値</span><span class="sxs-lookup"><span data-stu-id="f847c-193">Boolean</span></span>|<span data-ttu-id="f847c-194">デバイスの脅威保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f847c-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="f847c-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f847c-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f847c-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f847c-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f847c-197">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="f847c-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f847c-198">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="f847c-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f847c-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="f847c-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="f847c-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f847c-200">Boolean</span></span>|<span data-ttu-id="f847c-201">管理された電子メール プロファイルを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f847c-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="f847c-202">応答</span><span class="sxs-lookup"><span data-stu-id="f847c-202">Response</span></span>
<span data-ttu-id="f847c-203">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f847c-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f847c-204">例</span><span class="sxs-lookup"><span data-stu-id="f847c-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="f847c-205">要求</span><span class="sxs-lookup"><span data-stu-id="f847c-205">Request</span></span>
<span data-ttu-id="f847c-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f847c-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="f847c-207">応答</span><span class="sxs-lookup"><span data-stu-id="f847c-207">Response</span></span>
<span data-ttu-id="f847c-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f847c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
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
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



