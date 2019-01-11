---
title: Create iosCompliancePolicy
description: 新しい iosCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd5eca6a10492356f65449f2a1b98e6c79744b72
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873704"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="90731-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="90731-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="90731-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90731-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90731-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90731-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90731-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="90731-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90731-107">新しい [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="90731-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90731-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="90731-108">Prerequisites</span></span>
<span data-ttu-id="90731-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90731-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90731-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90731-111">Permission type</span></span>|<span data-ttu-id="90731-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90731-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90731-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90731-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90731-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90731-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90731-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90731-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90731-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90731-116">Not supported.</span></span>|
|<span data-ttu-id="90731-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90731-117">Application</span></span>|<span data-ttu-id="90731-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90731-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90731-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90731-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="90731-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90731-120">Request headers</span></span>
|<span data-ttu-id="90731-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90731-121">Header</span></span>|<span data-ttu-id="90731-122">値</span><span class="sxs-lookup"><span data-stu-id="90731-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90731-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90731-123">Authorization</span></span>|<span data-ttu-id="90731-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="90731-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90731-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90731-125">Accept</span></span>|<span data-ttu-id="90731-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90731-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90731-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="90731-127">Request body</span></span>
<span data-ttu-id="90731-128">要求本文で、iosCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="90731-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="90731-129">次の表に、iosCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90731-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="90731-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90731-130">Property</span></span>|<span data-ttu-id="90731-131">種類</span><span class="sxs-lookup"><span data-stu-id="90731-131">Type</span></span>|<span data-ttu-id="90731-132">説明</span><span class="sxs-lookup"><span data-stu-id="90731-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90731-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90731-133">roleScopeTagIds</span></span>|<span data-ttu-id="90731-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="90731-134">String collection</span></span>|<span data-ttu-id="90731-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="90731-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90731-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-137">id</span><span class="sxs-lookup"><span data-stu-id="90731-137">id</span></span>|<span data-ttu-id="90731-138">String</span><span class="sxs-lookup"><span data-stu-id="90731-138">String</span></span>|<span data-ttu-id="90731-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="90731-139">Key of the entity.</span></span> <span data-ttu-id="90731-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90731-141">createdDateTime</span></span>|<span data-ttu-id="90731-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90731-142">DateTimeOffset</span></span>|<span data-ttu-id="90731-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90731-143">DateTime the object was created.</span></span> <span data-ttu-id="90731-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-145">説明</span><span class="sxs-lookup"><span data-stu-id="90731-145">description</span></span>|<span data-ttu-id="90731-146">String</span><span class="sxs-lookup"><span data-stu-id="90731-146">String</span></span>|<span data-ttu-id="90731-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="90731-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90731-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90731-149">lastModifiedDateTime</span></span>|<span data-ttu-id="90731-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90731-150">DateTimeOffset</span></span>|<span data-ttu-id="90731-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="90731-151">DateTime the object was last modified.</span></span> <span data-ttu-id="90731-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-153">displayName</span><span class="sxs-lookup"><span data-stu-id="90731-153">displayName</span></span>|<span data-ttu-id="90731-154">String</span><span class="sxs-lookup"><span data-stu-id="90731-154">String</span></span>|<span data-ttu-id="90731-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="90731-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90731-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-157">version</span><span class="sxs-lookup"><span data-stu-id="90731-157">version</span></span>|<span data-ttu-id="90731-158">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-158">Int32</span></span>|<span data-ttu-id="90731-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="90731-159">Version of the device configuration.</span></span> <span data-ttu-id="90731-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="90731-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90731-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="90731-161">passcodeBlockSimple</span></span>|<span data-ttu-id="90731-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="90731-162">Boolean</span></span>|<span data-ttu-id="90731-163">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="90731-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="90731-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="90731-164">passcodeExpirationDays</span></span>|<span data-ttu-id="90731-165">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-165">Int32</span></span>|<span data-ttu-id="90731-166">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="90731-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="90731-167">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="90731-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="90731-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="90731-168">passcodeMinimumLength</span></span>|<span data-ttu-id="90731-169">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-169">Int32</span></span>|<span data-ttu-id="90731-170">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="90731-170">Minimum length of passcode.</span></span> <span data-ttu-id="90731-171">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="90731-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="90731-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="90731-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="90731-173">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-173">Int32</span></span>|<span data-ttu-id="90731-174">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="90731-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="90731-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="90731-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="90731-176">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-176">Int32</span></span>|<span data-ttu-id="90731-177">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="90731-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="90731-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="90731-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="90731-179">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-179">Int32</span></span>|<span data-ttu-id="90731-180">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="90731-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="90731-181">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="90731-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="90731-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="90731-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="90731-183">Int32</span><span class="sxs-lookup"><span data-stu-id="90731-183">Int32</span></span>|<span data-ttu-id="90731-184">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="90731-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="90731-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="90731-185">passcodeRequiredType</span></span>|[<span data-ttu-id="90731-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="90731-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="90731-187">要求されるパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="90731-187">The required passcode type.</span></span> <span data-ttu-id="90731-188">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="90731-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="90731-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="90731-189">passcodeRequired</span></span>|<span data-ttu-id="90731-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="90731-190">Boolean</span></span>|<span data-ttu-id="90731-191">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90731-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="90731-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="90731-192">osMinimumVersion</span></span>|<span data-ttu-id="90731-193">String</span><span class="sxs-lookup"><span data-stu-id="90731-193">String</span></span>|<span data-ttu-id="90731-194">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="90731-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="90731-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="90731-195">osMaximumVersion</span></span>|<span data-ttu-id="90731-196">String</span><span class="sxs-lookup"><span data-stu-id="90731-196">String</span></span>|<span data-ttu-id="90731-197">iOS の最高バージョン。</span><span class="sxs-lookup"><span data-stu-id="90731-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="90731-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="90731-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="90731-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="90731-199">Boolean</span></span>|<span data-ttu-id="90731-200">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="90731-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="90731-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="90731-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="90731-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="90731-202">Boolean</span></span>|<span data-ttu-id="90731-203">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="90731-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="90731-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="90731-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="90731-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="90731-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="90731-206">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="90731-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="90731-207">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="90731-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="90731-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="90731-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="90731-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="90731-209">Boolean</span></span>|<span data-ttu-id="90731-210">管理された電子メール プロファイルを必要とするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="90731-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="90731-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="90731-211">restrictedApps</span></span>|<span data-ttu-id="90731-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="90731-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="90731-213">デバイスには、特定のアプリケーションがインストールされていない必要があります。</span><span class="sxs-lookup"><span data-stu-id="90731-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="90731-214">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90731-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="90731-215">応答</span><span class="sxs-lookup"><span data-stu-id="90731-215">Response</span></span>
<span data-ttu-id="90731-216">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90731-216">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90731-217">例</span><span class="sxs-lookup"><span data-stu-id="90731-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="90731-218">要求</span><span class="sxs-lookup"><span data-stu-id="90731-218">Request</span></span>
<span data-ttu-id="90731-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90731-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1181

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="90731-220">応答</span><span class="sxs-lookup"><span data-stu-id="90731-220">Response</span></span>
<span data-ttu-id="90731-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90731-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1289

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





