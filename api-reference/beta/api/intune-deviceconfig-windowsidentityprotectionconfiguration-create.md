---
title: WindowsIdentityProtectionConfiguration を作成します。
description: 新しい windowsIdentityProtectionConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: a0d588943f75694af159cfd835fc2e3a09b052e0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355392"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="67271-103">WindowsIdentityProtectionConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="67271-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="67271-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67271-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67271-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67271-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67271-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67271-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67271-107">新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67271-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67271-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="67271-108">Prerequisites</span></span>
<span data-ttu-id="67271-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67271-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67271-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67271-111">Permission type</span></span>|<span data-ttu-id="67271-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67271-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67271-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67271-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67271-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67271-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67271-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67271-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67271-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67271-116">Not supported.</span></span>|
|<span data-ttu-id="67271-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67271-117">Application</span></span>|<span data-ttu-id="67271-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67271-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67271-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67271-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="67271-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67271-120">Request headers</span></span>
|<span data-ttu-id="67271-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67271-121">Header</span></span>|<span data-ttu-id="67271-122">値</span><span class="sxs-lookup"><span data-stu-id="67271-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67271-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67271-123">Authorization</span></span>|<span data-ttu-id="67271-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67271-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67271-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67271-125">Accept</span></span>|<span data-ttu-id="67271-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67271-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67271-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="67271-127">Request body</span></span>
<span data-ttu-id="67271-128">要求の本文に windowsIdentityProtectionConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="67271-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="67271-129">次の表は、windowsIdentityProtectionConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67271-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="67271-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67271-130">Property</span></span>|<span data-ttu-id="67271-131">種類</span><span class="sxs-lookup"><span data-stu-id="67271-131">Type</span></span>|<span data-ttu-id="67271-132">説明</span><span class="sxs-lookup"><span data-stu-id="67271-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67271-133">ID</span><span class="sxs-lookup"><span data-stu-id="67271-133">id</span></span>|<span data-ttu-id="67271-134">String</span><span class="sxs-lookup"><span data-stu-id="67271-134">String</span></span>|<span data-ttu-id="67271-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67271-135">Key of the entity.</span></span> <span data-ttu-id="67271-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67271-137">lastModifiedDateTime</span></span>|<span data-ttu-id="67271-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67271-138">DateTimeOffset</span></span>|<span data-ttu-id="67271-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="67271-139">DateTime the object was last modified.</span></span> <span data-ttu-id="67271-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67271-141">roleScopeTagIds</span></span>|<span data-ttu-id="67271-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="67271-142">String collection</span></span>|<span data-ttu-id="67271-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="67271-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67271-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="67271-145">supportsScopeTags</span></span>|<span data-ttu-id="67271-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="67271-146">Boolean</span></span>|<span data-ttu-id="67271-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="67271-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67271-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="67271-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67271-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="67271-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67271-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="67271-150">This property is read-only.</span></span> <span data-ttu-id="67271-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67271-152">createdDateTime</span></span>|<span data-ttu-id="67271-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67271-153">DateTimeOffset</span></span>|<span data-ttu-id="67271-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="67271-154">DateTime the object was created.</span></span> <span data-ttu-id="67271-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-156">説明</span><span class="sxs-lookup"><span data-stu-id="67271-156">description</span></span>|<span data-ttu-id="67271-157">String</span><span class="sxs-lookup"><span data-stu-id="67271-157">String</span></span>|<span data-ttu-id="67271-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="67271-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67271-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-160">displayName</span><span class="sxs-lookup"><span data-stu-id="67271-160">displayName</span></span>|<span data-ttu-id="67271-161">String</span><span class="sxs-lookup"><span data-stu-id="67271-161">String</span></span>|<span data-ttu-id="67271-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="67271-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67271-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-164">version</span><span class="sxs-lookup"><span data-stu-id="67271-164">version</span></span>|<span data-ttu-id="67271-165">Int32</span><span class="sxs-lookup"><span data-stu-id="67271-165">Int32</span></span>|<span data-ttu-id="67271-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="67271-166">Version of the device configuration.</span></span> <span data-ttu-id="67271-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67271-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67271-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="67271-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="67271-169">ブール型</span><span class="sxs-lookup"><span data-stu-id="67271-169">Boolean</span></span>|<span data-ttu-id="67271-170">拡張スプーフィング対策 Windows こんにちは顔認証の facial の機能の認識を有効にするために使用するブール値です。</span><span class="sxs-lookup"><span data-stu-id="67271-170">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="67271-171">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="67271-171">pinMinimumLength</span></span>|<span data-ttu-id="67271-172">Int32</span><span class="sxs-lookup"><span data-stu-id="67271-172">Int32</span></span>|<span data-ttu-id="67271-173">ビジネスの暗証番号 (pin) は、Windows こんにちはに必要な文字の最小数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="67271-173">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="67271-174">有効な値は 4 ~ 127 包括的で、最大の暗証番号 (pin) の設定値に等しいかそれより小さい。</span><span class="sxs-lookup"><span data-stu-id="67271-174">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="67271-175">有効な値 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="67271-175">Valid values 4 to 127</span></span>|
|<span data-ttu-id="67271-176">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="67271-176">pinMaximumLength</span></span>|<span data-ttu-id="67271-177">Int32</span><span class="sxs-lookup"><span data-stu-id="67271-177">Int32</span></span>|<span data-ttu-id="67271-178">暗証番号 (pin) の作業に使用できる文字の最大数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="67271-178">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="67271-179">有効な値は、4 ~ 127 包括的以上の最小の暗証番号 (pin) の設定値と同じです。</span><span class="sxs-lookup"><span data-stu-id="67271-179">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="67271-180">有効な値 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="67271-180">Valid values 4 to 127</span></span>|
|<span data-ttu-id="67271-181">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67271-181">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="67271-182">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="67271-182">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="67271-183">この値は、ビジネスの暗証番号 (pin) の Windows こんにちはの文字の大文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="67271-183">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="67271-184">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="67271-184">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="67271-185">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67271-185">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="67271-186">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="67271-186">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="67271-187">この値は、ビジネスの暗証番号 (pin) の Windows こんにちはで小文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="67271-187">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="67271-188">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="67271-188">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="67271-189">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67271-189">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="67271-190">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="67271-190">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="67271-191">ビジネスの暗証番号 (pin) を Windows こんにちはで特殊文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="67271-191">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="67271-192">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="67271-192">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="67271-193">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="67271-193">pinExpirationInDays</span></span>|<span data-ttu-id="67271-194">Int32</span><span class="sxs-lookup"><span data-stu-id="67271-194">Int32</span></span>|<span data-ttu-id="67271-195">期間 (日数) を指定する整数値システムがそれを変更するユーザーを必要とする前に、暗証番号 (pin) を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="67271-195">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="67271-196">有効な値は、0 に 730 包括的です。</span><span class="sxs-lookup"><span data-stu-id="67271-196">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="67271-197">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="67271-197">Valid values 0 to 730</span></span>|
|<span data-ttu-id="67271-198">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="67271-198">pinPreviousBlockCount</span></span>|<span data-ttu-id="67271-199">Int32</span><span class="sxs-lookup"><span data-stu-id="67271-199">Int32</span></span>|<span data-ttu-id="67271-200">過去のピンを使用できないようにする機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="67271-200">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="67271-201">0 から 50、包括的で、これを設定する必要があり、その数にユーザーの現在の暗証番号 (pin) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="67271-201">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="67271-202">かどうかは 0 では、以前に設定ピンは格納されません。</span><span class="sxs-lookup"><span data-stu-id="67271-202">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="67271-203">PIN を通じて暗証番号 (pin) の履歴は保持されませんをリセットします。</span><span class="sxs-lookup"><span data-stu-id="67271-203">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="67271-204">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="67271-204">Valid values 0 to 50</span></span>|
|<span data-ttu-id="67271-205">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="67271-205">pinRecoveryEnabled</span></span>|<span data-ttu-id="67271-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="67271-206">Boolean</span></span>|<span data-ttu-id="67271-207">使用して、Windows こんにちはビジネス暗証番号 (pin) リカバリ ・ サービスの PIN を変更するユーザーを有効にするブール値です。</span><span class="sxs-lookup"><span data-stu-id="67271-207">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="67271-208">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="67271-208">securityDeviceRequired</span></span>|<span data-ttu-id="67271-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="67271-209">Boolean</span></span>|<span data-ttu-id="67271-210">Windows こんにちはビジネスのための準備のトラステッド プラットフォーム モジュール (TPM) を必要とするかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="67271-210">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="67271-211">TPM は、他のデバイス上に格納されているデータは使用できませんという点で、その他セキュリティ上の利点を提供します。</span><span class="sxs-lookup"><span data-stu-id="67271-211">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="67271-212">かどうかは False に設定すると、すべてのデバイスをプロビジョニングできる Windows こんにちはビジネスに使用可能な TPM がない場合でも。</span><span class="sxs-lookup"><span data-stu-id="67271-212">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="67271-213">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="67271-213">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="67271-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="67271-214">Boolean</span></span>|<span data-ttu-id="67271-215">代わりに、Windows こんにちはビジネス暗証番号 (pin) の顔や指紋などの生体認証のジェスチャの使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="67271-215">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="67271-216">場合は False、生体認証のジェスチャに設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="67271-216">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="67271-217">ユーザーは、障害が発生した場合のバックアップとして、暗証番号 (pin) を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="67271-217">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="67271-218">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="67271-218">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="67271-219">ブール型</span><span class="sxs-lookup"><span data-stu-id="67271-219">Boolean</span></span>|<span data-ttu-id="67271-220">Windows こんにちは設置型リソースの認証に証明書を使用するビジネスを可能にするブール値です。</span><span class="sxs-lookup"><span data-stu-id="67271-220">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="67271-221">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="67271-221">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="67271-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="67271-222">Boolean</span></span>|<span data-ttu-id="67271-223">Windows こんにちはの Windows へのサインイン方法としてビジネスをブロックするブール値です。</span><span class="sxs-lookup"><span data-stu-id="67271-223">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="67271-224">応答</span><span class="sxs-lookup"><span data-stu-id="67271-224">Response</span></span>
<span data-ttu-id="67271-225">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="67271-225">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67271-226">例</span><span class="sxs-lookup"><span data-stu-id="67271-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="67271-227">要求</span><span class="sxs-lookup"><span data-stu-id="67271-227">Request</span></span>
<span data-ttu-id="67271-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67271-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 838

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="67271-229">応答</span><span class="sxs-lookup"><span data-stu-id="67271-229">Response</span></span>
<span data-ttu-id="67271-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67271-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 946

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




