---
title: macOSCompliancePolicy の作成
description: 新しい macOSCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68e4e59882a2d861a7a65c6077bfa685f8b5b86b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973679"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="68e66-103">macOSCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="68e66-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="68e66-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68e66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68e66-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68e66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68e66-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68e66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68e66-107">新しい [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="68e66-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68e66-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="68e66-108">Prerequisites</span></span>
<span data-ttu-id="68e66-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68e66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e66-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68e66-111">Permission type</span></span>|<span data-ttu-id="68e66-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="68e66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68e66-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68e66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68e66-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e66-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68e66-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68e66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68e66-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68e66-116">Not supported.</span></span>|
|<span data-ttu-id="68e66-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68e66-117">Application</span></span>|<span data-ttu-id="68e66-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68e66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68e66-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68e66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="68e66-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68e66-120">Request headers</span></span>
|<span data-ttu-id="68e66-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68e66-121">Header</span></span>|<span data-ttu-id="68e66-122">値</span><span class="sxs-lookup"><span data-stu-id="68e66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68e66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68e66-123">Authorization</span></span>|<span data-ttu-id="68e66-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="68e66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68e66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68e66-125">Accept</span></span>|<span data-ttu-id="68e66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68e66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68e66-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="68e66-127">Request body</span></span>
<span data-ttu-id="68e66-128">要求本文で、macOSCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="68e66-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="68e66-129">次の表に、macOSCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="68e66-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="68e66-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68e66-130">Property</span></span>|<span data-ttu-id="68e66-131">種類</span><span class="sxs-lookup"><span data-stu-id="68e66-131">Type</span></span>|<span data-ttu-id="68e66-132">説明</span><span class="sxs-lookup"><span data-stu-id="68e66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68e66-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68e66-133">roleScopeTagIds</span></span>|<span data-ttu-id="68e66-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="68e66-134">String collection</span></span>|<span data-ttu-id="68e66-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="68e66-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="68e66-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-137">id</span><span class="sxs-lookup"><span data-stu-id="68e66-137">id</span></span>|<span data-ttu-id="68e66-138">String</span><span class="sxs-lookup"><span data-stu-id="68e66-138">String</span></span>|<span data-ttu-id="68e66-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="68e66-139">Key of the entity.</span></span> <span data-ttu-id="68e66-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68e66-141">createdDateTime</span></span>|<span data-ttu-id="68e66-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e66-142">DateTimeOffset</span></span>|<span data-ttu-id="68e66-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="68e66-143">DateTime the object was created.</span></span> <span data-ttu-id="68e66-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-145">説明</span><span class="sxs-lookup"><span data-stu-id="68e66-145">description</span></span>|<span data-ttu-id="68e66-146">String</span><span class="sxs-lookup"><span data-stu-id="68e66-146">String</span></span>|<span data-ttu-id="68e66-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="68e66-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68e66-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68e66-149">lastModifiedDateTime</span></span>|<span data-ttu-id="68e66-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e66-150">DateTimeOffset</span></span>|<span data-ttu-id="68e66-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="68e66-151">DateTime the object was last modified.</span></span> <span data-ttu-id="68e66-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-153">displayName</span><span class="sxs-lookup"><span data-stu-id="68e66-153">displayName</span></span>|<span data-ttu-id="68e66-154">String</span><span class="sxs-lookup"><span data-stu-id="68e66-154">String</span></span>|<span data-ttu-id="68e66-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="68e66-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68e66-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-157">version</span><span class="sxs-lookup"><span data-stu-id="68e66-157">version</span></span>|<span data-ttu-id="68e66-158">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-158">Int32</span></span>|<span data-ttu-id="68e66-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="68e66-159">Version of the device configuration.</span></span> <span data-ttu-id="68e66-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68e66-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="68e66-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="68e66-161">passwordRequired</span></span>|<span data-ttu-id="68e66-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e66-162">Boolean</span></span>|<span data-ttu-id="68e66-163">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="68e66-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="68e66-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="68e66-164">passwordBlockSimple</span></span>|<span data-ttu-id="68e66-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e66-165">Boolean</span></span>|<span data-ttu-id="68e66-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="68e66-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="68e66-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="68e66-167">passwordExpirationDays</span></span>|<span data-ttu-id="68e66-168">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-168">Int32</span></span>|<span data-ttu-id="68e66-169">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="68e66-169">Number of days before the password expires.</span></span> <span data-ttu-id="68e66-170">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="68e66-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="68e66-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="68e66-171">passwordMinimumLength</span></span>|<span data-ttu-id="68e66-172">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-172">Int32</span></span>|<span data-ttu-id="68e66-173">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="68e66-173">Minimum length of password.</span></span> <span data-ttu-id="68e66-174">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="68e66-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="68e66-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="68e66-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="68e66-176">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-176">Int32</span></span>|<span data-ttu-id="68e66-177">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="68e66-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="68e66-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="68e66-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="68e66-179">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-179">Int32</span></span>|<span data-ttu-id="68e66-180">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="68e66-180">Number of previous passwords to block.</span></span> <span data-ttu-id="68e66-181">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="68e66-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="68e66-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="68e66-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="68e66-183">Int32</span><span class="sxs-lookup"><span data-stu-id="68e66-183">Int32</span></span>|<span data-ttu-id="68e66-184">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="68e66-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="68e66-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="68e66-185">passwordRequiredType</span></span>|[<span data-ttu-id="68e66-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="68e66-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="68e66-187">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="68e66-187">The required password type.</span></span> <span data-ttu-id="68e66-188">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="68e66-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="68e66-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="68e66-189">osMinimumVersion</span></span>|<span data-ttu-id="68e66-190">String</span><span class="sxs-lookup"><span data-stu-id="68e66-190">String</span></span>|<span data-ttu-id="68e66-191">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="68e66-191">Minimum IOS version.</span></span>|
|<span data-ttu-id="68e66-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="68e66-192">osMaximumVersion</span></span>|<span data-ttu-id="68e66-193">String</span><span class="sxs-lookup"><span data-stu-id="68e66-193">String</span></span>|<span data-ttu-id="68e66-194">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="68e66-194">Maximum IOS version.</span></span>|
|<span data-ttu-id="68e66-195">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="68e66-195">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="68e66-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e66-196">Boolean</span></span>|<span data-ttu-id="68e66-197">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68e66-197">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="68e66-198">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="68e66-198">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="68e66-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e66-199">Boolean</span></span>|<span data-ttu-id="68e66-200">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68e66-200">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="68e66-201">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68e66-201">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="68e66-202">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="68e66-202">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="68e66-203">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="68e66-203">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="68e66-204">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="68e66-204">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="68e66-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="68e66-205">storageRequireEncryption</span></span>|<span data-ttu-id="68e66-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e66-206">Boolean</span></span>|<span data-ttu-id="68e66-207">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="68e66-207">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="68e66-208">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="68e66-208">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="68e66-209">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="68e66-209">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="68e66-210">システムは、macOS のデバイスでどのダウンロード場所のアプリケーションから実行できるかを決定するプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="68e66-210">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="68e66-211">可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="68e66-211">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="68e66-212">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="68e66-212">firewallEnabled</span></span>|<span data-ttu-id="68e66-213">ブール型</span><span class="sxs-lookup"><span data-stu-id="68e66-213">Boolean</span></span>|<span data-ttu-id="68e66-214">かどうか、か、これらのファイアウォールは有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="68e66-214">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="68e66-215">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="68e66-215">firewallBlockAllIncoming</span></span>|<span data-ttu-id="68e66-216">ブール型</span><span class="sxs-lookup"><span data-stu-id="68e66-216">Boolean</span></span>|<span data-ttu-id="68e66-217">「すべての着信接続をブロックする] オプションに対応します。</span><span class="sxs-lookup"><span data-stu-id="68e66-217">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="68e66-218">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="68e66-218">firewallEnableStealthMode</span></span>|<span data-ttu-id="68e66-219">ブール型</span><span class="sxs-lookup"><span data-stu-id="68e66-219">Boolean</span></span>|<span data-ttu-id="68e66-220">「有効にするステルス モード」に対応</span><span class="sxs-lookup"><span data-stu-id="68e66-220">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="68e66-221">応答</span><span class="sxs-lookup"><span data-stu-id="68e66-221">Response</span></span>
<span data-ttu-id="68e66-222">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="68e66-222">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e66-223">例</span><span class="sxs-lookup"><span data-stu-id="68e66-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="68e66-224">要求</span><span class="sxs-lookup"><span data-stu-id="68e66-224">Request</span></span>
<span data-ttu-id="68e66-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="68e66-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1023

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="68e66-226">応答</span><span class="sxs-lookup"><span data-stu-id="68e66-226">Response</span></span>
<span data-ttu-id="68e66-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="68e66-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1131

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





