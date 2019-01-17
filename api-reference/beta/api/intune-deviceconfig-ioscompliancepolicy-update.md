---
title: iosCompliancePolicy の更新
description: iosCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9ee2476d85ec1446fea4b45fac834eb62f82bc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967883"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="e8efc-103">iosCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="e8efc-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="e8efc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8efc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8efc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8efc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8efc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8efc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8efc-107">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8efc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e8efc-108">Prerequisites</span></span>
<span data-ttu-id="e8efc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8efc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8efc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8efc-111">Permission type</span></span>|<span data-ttu-id="e8efc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8efc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8efc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8efc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8efc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8efc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8efc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8efc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8efc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8efc-116">Not supported.</span></span>|
|<span data-ttu-id="e8efc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8efc-117">Application</span></span>|<span data-ttu-id="e8efc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8efc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8efc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8efc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e8efc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8efc-120">Request headers</span></span>
|<span data-ttu-id="e8efc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8efc-121">Header</span></span>|<span data-ttu-id="e8efc-122">値</span><span class="sxs-lookup"><span data-stu-id="e8efc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8efc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8efc-123">Authorization</span></span>|<span data-ttu-id="e8efc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e8efc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8efc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8efc-125">Accept</span></span>|<span data-ttu-id="e8efc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8efc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8efc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8efc-127">Request body</span></span>
<span data-ttu-id="e8efc-128">要求本文で、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="e8efc-129">次の表に、[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="e8efc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8efc-130">Property</span></span>|<span data-ttu-id="e8efc-131">型</span><span class="sxs-lookup"><span data-stu-id="e8efc-131">Type</span></span>|<span data-ttu-id="e8efc-132">説明</span><span class="sxs-lookup"><span data-stu-id="e8efc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8efc-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8efc-133">roleScopeTagIds</span></span>|<span data-ttu-id="e8efc-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e8efc-134">String collection</span></span>|<span data-ttu-id="e8efc-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e8efc-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e8efc-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-137">id</span><span class="sxs-lookup"><span data-stu-id="e8efc-137">id</span></span>|<span data-ttu-id="e8efc-138">String</span><span class="sxs-lookup"><span data-stu-id="e8efc-138">String</span></span>|<span data-ttu-id="e8efc-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e8efc-139">Key of the entity.</span></span> <span data-ttu-id="e8efc-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8efc-141">createdDateTime</span></span>|<span data-ttu-id="e8efc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8efc-142">DateTimeOffset</span></span>|<span data-ttu-id="e8efc-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e8efc-143">DateTime the object was created.</span></span> <span data-ttu-id="e8efc-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-145">説明</span><span class="sxs-lookup"><span data-stu-id="e8efc-145">description</span></span>|<span data-ttu-id="e8efc-146">String</span><span class="sxs-lookup"><span data-stu-id="e8efc-146">String</span></span>|<span data-ttu-id="e8efc-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e8efc-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8efc-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8efc-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e8efc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8efc-150">DateTimeOffset</span></span>|<span data-ttu-id="e8efc-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e8efc-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e8efc-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e8efc-153">displayName</span></span>|<span data-ttu-id="e8efc-154">String</span><span class="sxs-lookup"><span data-stu-id="e8efc-154">String</span></span>|<span data-ttu-id="e8efc-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e8efc-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8efc-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-157">version</span><span class="sxs-lookup"><span data-stu-id="e8efc-157">version</span></span>|<span data-ttu-id="e8efc-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-158">Int32</span></span>|<span data-ttu-id="e8efc-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e8efc-159">Version of the device configuration.</span></span> <span data-ttu-id="e8efc-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8efc-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e8efc-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e8efc-161">passcodeBlockSimple</span></span>|<span data-ttu-id="e8efc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8efc-162">Boolean</span></span>|<span data-ttu-id="e8efc-163">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e8efc-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e8efc-164">passcodeExpirationDays</span></span>|<span data-ttu-id="e8efc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-165">Int32</span></span>|<span data-ttu-id="e8efc-166">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="e8efc-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="e8efc-167">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="e8efc-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e8efc-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e8efc-168">passcodeMinimumLength</span></span>|<span data-ttu-id="e8efc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-169">Int32</span></span>|<span data-ttu-id="e8efc-170">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="e8efc-170">Minimum length of passcode.</span></span> <span data-ttu-id="e8efc-171">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="e8efc-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e8efc-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e8efc-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e8efc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-173">Int32</span></span>|<span data-ttu-id="e8efc-174">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="e8efc-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e8efc-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e8efc-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e8efc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-176">Int32</span></span>|<span data-ttu-id="e8efc-177">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="e8efc-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e8efc-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e8efc-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e8efc-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-179">Int32</span></span>|<span data-ttu-id="e8efc-180">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="e8efc-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="e8efc-181">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="e8efc-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e8efc-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e8efc-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e8efc-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e8efc-183">Int32</span></span>|<span data-ttu-id="e8efc-184">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="e8efc-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e8efc-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e8efc-185">passcodeRequiredType</span></span>|[<span data-ttu-id="e8efc-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e8efc-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e8efc-187">要求されるパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="e8efc-187">The required passcode type.</span></span> <span data-ttu-id="e8efc-188">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="e8efc-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e8efc-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e8efc-189">passcodeRequired</span></span>|<span data-ttu-id="e8efc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8efc-190">Boolean</span></span>|<span data-ttu-id="e8efc-191">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e8efc-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e8efc-192">osMinimumVersion</span></span>|<span data-ttu-id="e8efc-193">String</span><span class="sxs-lookup"><span data-stu-id="e8efc-193">String</span></span>|<span data-ttu-id="e8efc-194">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e8efc-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="e8efc-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e8efc-195">osMaximumVersion</span></span>|<span data-ttu-id="e8efc-196">String</span><span class="sxs-lookup"><span data-stu-id="e8efc-196">String</span></span>|<span data-ttu-id="e8efc-197">iOS の最高バージョン。</span><span class="sxs-lookup"><span data-stu-id="e8efc-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="e8efc-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="e8efc-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="e8efc-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8efc-199">Boolean</span></span>|<span data-ttu-id="e8efc-200">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="e8efc-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="e8efc-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8efc-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e8efc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8efc-202">Boolean</span></span>|<span data-ttu-id="e8efc-203">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8efc-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="e8efc-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e8efc-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e8efc-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e8efc-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e8efc-206">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e8efc-207">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="e8efc-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e8efc-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="e8efc-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="e8efc-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8efc-209">Boolean</span></span>|<span data-ttu-id="e8efc-210">管理された電子メール プロファイルを必要とするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="e8efc-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e8efc-211">restrictedApps</span></span>|<span data-ttu-id="e8efc-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8efc-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e8efc-213">デバイスには、特定のアプリケーションがインストールされていない必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8efc-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="e8efc-214">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e8efc-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e8efc-215">応答</span><span class="sxs-lookup"><span data-stu-id="e8efc-215">Response</span></span>
<span data-ttu-id="e8efc-216">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e8efc-216">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8efc-217">例</span><span class="sxs-lookup"><span data-stu-id="e8efc-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8efc-218">要求</span><span class="sxs-lookup"><span data-stu-id="e8efc-218">Request</span></span>
<span data-ttu-id="e8efc-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8efc-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1123

{
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

### <a name="response"></a><span data-ttu-id="e8efc-220">応答</span><span class="sxs-lookup"><span data-stu-id="e8efc-220">Response</span></span>
<span data-ttu-id="e8efc-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8efc-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





