---
title: MacOSEndpointProtectionConfiguration の作成
description: 新しい macOSEndpointProtectionConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce78f253dc3c0d22af78d9b6347c2f57546cb6a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338806"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="9e613-103">MacOSEndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="9e613-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="9e613-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e613-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e613-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e613-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e613-106">新しい[Macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e613-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e613-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e613-107">Prerequisites</span></span>
<span data-ttu-id="9e613-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e613-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e613-110">Permission type</span></span>|<span data-ttu-id="9e613-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e613-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e613-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e613-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e613-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e613-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e613-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e613-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e613-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e613-115">Not supported.</span></span>|
|<span data-ttu-id="9e613-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e613-116">Application</span></span>|<span data-ttu-id="9e613-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e613-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e613-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e613-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e613-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e613-119">Request headers</span></span>
|<span data-ttu-id="9e613-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e613-120">Header</span></span>|<span data-ttu-id="9e613-121">値</span><span class="sxs-lookup"><span data-stu-id="9e613-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e613-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e613-122">Authorization</span></span>|<span data-ttu-id="9e613-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e613-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e613-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9e613-124">Accept</span></span>|<span data-ttu-id="9e613-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e613-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e613-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e613-126">Request body</span></span>
<span data-ttu-id="9e613-127">要求本文で、macOSEndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e613-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="9e613-128">次の表に、macOSEndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e613-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="9e613-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e613-129">Property</span></span>|<span data-ttu-id="9e613-130">型</span><span class="sxs-lookup"><span data-stu-id="9e613-130">Type</span></span>|<span data-ttu-id="9e613-131">説明</span><span class="sxs-lookup"><span data-stu-id="9e613-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e613-132">id</span><span class="sxs-lookup"><span data-stu-id="9e613-132">id</span></span>|<span data-ttu-id="9e613-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9e613-133">String</span></span>|<span data-ttu-id="9e613-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e613-134">Key of the entity.</span></span> <span data-ttu-id="9e613-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e613-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e613-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e613-137">DateTimeOffset</span></span>|<span data-ttu-id="9e613-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9e613-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e613-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e613-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e613-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9e613-141">String collection</span></span>|<span data-ttu-id="9e613-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9e613-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e613-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e613-144">supportsScopeTags</span></span>|<span data-ttu-id="9e613-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-145">Boolean</span></span>|<span data-ttu-id="9e613-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9e613-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e613-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9e613-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e613-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9e613-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e613-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9e613-149">This property is read-only.</span></span> <span data-ttu-id="9e613-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e613-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9e613-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e613-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9e613-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="9e613-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9e613-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e613-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9e613-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e613-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9e613-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9e613-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9e613-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9e613-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9e613-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9e613-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9e613-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9e613-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9e613-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e613-163">createdDateTime</span></span>|<span data-ttu-id="9e613-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e613-164">DateTimeOffset</span></span>|<span data-ttu-id="9e613-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9e613-165">DateTime the object was created.</span></span> <span data-ttu-id="9e613-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-167">description</span><span class="sxs-lookup"><span data-stu-id="9e613-167">description</span></span>|<span data-ttu-id="9e613-168">String</span><span class="sxs-lookup"><span data-stu-id="9e613-168">String</span></span>|<span data-ttu-id="9e613-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9e613-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e613-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9e613-171">displayName</span></span>|<span data-ttu-id="9e613-172">String</span><span class="sxs-lookup"><span data-stu-id="9e613-172">String</span></span>|<span data-ttu-id="9e613-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9e613-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e613-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-175">version</span><span class="sxs-lookup"><span data-stu-id="9e613-175">version</span></span>|<span data-ttu-id="9e613-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9e613-176">Int32</span></span>|<span data-ttu-id="9e613-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e613-177">Version of the device configuration.</span></span> <span data-ttu-id="9e613-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e613-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e613-179">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="9e613-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="9e613-180">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="9e613-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="9e613-181">MacOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="9e613-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="9e613-182">使用可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="9e613-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="9e613-183">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="9e613-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="9e613-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-184">Boolean</span></span>|<span data-ttu-id="9e613-185">True に設定されている場合、ゲートキーパーのユーザーオーバーライドは無効になります。</span><span class="sxs-lookup"><span data-stu-id="9e613-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="9e613-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="9e613-186">firewallEnabled</span></span>|<span data-ttu-id="9e613-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-187">Boolean</span></span>|<span data-ttu-id="9e613-188">ファイアウォールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9e613-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="9e613-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="9e613-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="9e613-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-190">Boolean</span></span>|<span data-ttu-id="9e613-191">[着信接続をすべてブロックする] オプションに対応しています。</span><span class="sxs-lookup"><span data-stu-id="9e613-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="9e613-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="9e613-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="9e613-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-193">Boolean</span></span>|<span data-ttu-id="9e613-194">[ステルスモードを有効にする] に相当します。</span><span class="sxs-lookup"><span data-stu-id="9e613-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="9e613-195">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="9e613-195">firewallApplications</span></span>|<span data-ttu-id="9e613-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9e613-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="9e613-197">ファイアウォール設定のあるアプリケーションの一覧。</span><span class="sxs-lookup"><span data-stu-id="9e613-197">List of applications with firewall settings.</span></span> <span data-ttu-id="9e613-198">この一覧にないアプリケーションのファイアウォール設定は、ユーザーによって決まります。</span><span class="sxs-lookup"><span data-stu-id="9e613-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="9e613-199">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9e613-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9e613-200">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="9e613-200">fileVaultEnabled</span></span>|<span data-ttu-id="9e613-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-201">Boolean</span></span>|<span data-ttu-id="9e613-202">FileVault を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9e613-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="9e613-203">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="9e613-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="9e613-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="9e613-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="9e613-205">FileVault が有効になっている場合は必須。使用する回復キーの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="9e613-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="9e613-206">.</span><span class="sxs-lookup"><span data-stu-id="9e613-206"></span></span> <span data-ttu-id="9e613-207">可能な値は、`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey` です。</span><span class="sxs-lookup"><span data-stu-id="9e613-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="9e613-208">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="9e613-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="9e613-209">Binary</span><span class="sxs-lookup"><span data-stu-id="9e613-209">Binary</span></span>|<span data-ttu-id="9e613-210">選択した回復キーの種類 (s) に InstitutionalRecoveryKey が含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="9e613-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="9e613-211">証明機関の回復キーを設定するために使用する DER でエンコードされた証明書ファイル。</span><span class="sxs-lookup"><span data-stu-id="9e613-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="9e613-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="9e613-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="9e613-213">String</span><span class="sxs-lookup"><span data-stu-id="9e613-213">String</span></span>|<span data-ttu-id="9e613-214">UI に表示される、証明書の回復キー証明書のファイル名。</span><span class="sxs-lookup"><span data-stu-id="9e613-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="9e613-215">(\* der)</span><span class="sxs-lookup"><span data-stu-id="9e613-215">(\*.der).</span></span>|
|<span data-ttu-id="9e613-216">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="9e613-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="9e613-217">String</span><span class="sxs-lookup"><span data-stu-id="9e613-217">String</span></span>|<span data-ttu-id="9e613-218">選択されている回復キーの種類 (s) には、そのような回復キーが含まれている場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="9e613-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="9e613-219">ユーザーに対して、個人回復キーを取得する方法を説明する短いメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9e613-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="9e613-220">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="9e613-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="9e613-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-221">Boolean</span></span>|<span data-ttu-id="9e613-222">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9e613-222">Optional.</span></span> <span data-ttu-id="9e613-223">True に設定されている場合、ユーザーはサインアウトするまで FileVault の有効化を延期することができます。</span><span class="sxs-lookup"><span data-stu-id="9e613-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="9e613-224">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="9e613-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="9e613-225">Int32</span><span class="sxs-lookup"><span data-stu-id="9e613-225">Int32</span></span>|<span data-ttu-id="9e613-226">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9e613-226">Optional.</span></span> <span data-ttu-id="9e613-227">Defer オプションを使用する場合、ユーザーがサインインするために FileVault が必要になる前に、FileVault を有効にするように求めるプロンプトをユーザーが無視できる最大回数です。</span><span class="sxs-lookup"><span data-stu-id="9e613-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="9e613-228">-1 に設定すると、FileVault が有効になるまでは常に FileVault を有効にするかどうかを確認するメッセージが表示されます。ただし、ユーザーは FileVault の有効化をバイパスできます。</span><span class="sxs-lookup"><span data-stu-id="9e613-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="9e613-229">この値を0に設定すると、機能が無効になります。</span><span class="sxs-lookup"><span data-stu-id="9e613-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="9e613-230">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="9e613-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="9e613-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e613-231">Boolean</span></span>|<span data-ttu-id="9e613-232">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9e613-232">Optional.</span></span> <span data-ttu-id="9e613-233">Defer オプションを使用する場合、true に設定すると、ユーザーはサインアウト時に FileVault を有効にするかどうかを確認するメッセージを表示しません。</span><span class="sxs-lookup"><span data-stu-id="9e613-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="9e613-234">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="9e613-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="9e613-235">Int32</span><span class="sxs-lookup"><span data-stu-id="9e613-235">Int32</span></span>|<span data-ttu-id="9e613-236">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9e613-236">Optional.</span></span> <span data-ttu-id="9e613-237">選択した回復キーの種類 (s) には、そのキーを月単位で回転する頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e613-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|



## <a name="response"></a><span data-ttu-id="9e613-238">応答</span><span class="sxs-lookup"><span data-stu-id="9e613-238">Response</span></span>
<span data-ttu-id="9e613-239">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e613-239">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e613-240">例</span><span class="sxs-lookup"><span data-stu-id="9e613-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e613-241">要求</span><span class="sxs-lookup"><span data-stu-id="9e613-241">Request</span></span>
<span data-ttu-id="9e613-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e613-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2052

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```

### <a name="response"></a><span data-ttu-id="9e613-243">応答</span><span class="sxs-lookup"><span data-stu-id="9e613-243">Response</span></span>
<span data-ttu-id="9e613-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e613-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2224

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```






