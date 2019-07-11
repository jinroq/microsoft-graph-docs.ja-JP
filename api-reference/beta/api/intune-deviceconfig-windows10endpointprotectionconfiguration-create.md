---
title: windows10EndpointProtectionConfiguration の作成
description: 新しい windows10EndpointProtectionConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1828bcd90fd3cefeead8f15dee09dc411a117300
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620382"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="2b02a-103">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="2b02a-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="2b02a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b02a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b02a-106">新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b02a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2b02a-107">Prerequisites</span></span>
<span data-ttu-id="2b02a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b02a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b02a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b02a-110">Permission type</span></span>|<span data-ttu-id="2b02a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b02a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b02a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b02a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b02a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b02a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b02a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b02a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b02a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-115">Not supported.</span></span>|
|<span data-ttu-id="2b02a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b02a-116">Application</span></span>|<span data-ttu-id="2b02a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b02a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b02a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b02a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b02a-119">Request headers</span></span>
|<span data-ttu-id="2b02a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b02a-120">Header</span></span>|<span data-ttu-id="2b02a-121">値</span><span class="sxs-lookup"><span data-stu-id="2b02a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b02a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b02a-122">Authorization</span></span>|<span data-ttu-id="2b02a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b02a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2b02a-124">Accept</span></span>|<span data-ttu-id="2b02a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b02a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b02a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b02a-126">Request body</span></span>
<span data-ttu-id="2b02a-127">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="2b02a-128">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="2b02a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b02a-129">Property</span></span>|<span data-ttu-id="2b02a-130">型</span><span class="sxs-lookup"><span data-stu-id="2b02a-130">Type</span></span>|<span data-ttu-id="2b02a-131">説明</span><span class="sxs-lookup"><span data-stu-id="2b02a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b02a-132">id</span><span class="sxs-lookup"><span data-stu-id="2b02a-132">id</span></span>|<span data-ttu-id="2b02a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2b02a-133">String</span></span>|<span data-ttu-id="2b02a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2b02a-134">Key of the entity.</span></span> <span data-ttu-id="2b02a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b02a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2b02a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b02a-137">DateTimeOffset</span></span>|<span data-ttu-id="2b02a-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2b02a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2b02a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b02a-140">roleScopeTagIds</span></span>|<span data-ttu-id="2b02a-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2b02a-141">String collection</span></span>|<span data-ttu-id="2b02a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2b02a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b02a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b02a-144">supportsScopeTags</span></span>|<span data-ttu-id="2b02a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-145">Boolean</span></span>|<span data-ttu-id="2b02a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b02a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b02a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b02a-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-149">This property is read-only.</span></span> <span data-ttu-id="2b02a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2b02a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2b02a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2b02a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2b02a-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="2b02a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2b02a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2b02a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2b02a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2b02a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2b02a-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2b02a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2b02a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2b02a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2b02a-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2b02a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2b02a-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2b02a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2b02a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b02a-163">createdDateTime</span></span>|<span data-ttu-id="2b02a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b02a-164">DateTimeOffset</span></span>|<span data-ttu-id="2b02a-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2b02a-165">DateTime the object was created.</span></span> <span data-ttu-id="2b02a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-167">description</span><span class="sxs-lookup"><span data-stu-id="2b02a-167">description</span></span>|<span data-ttu-id="2b02a-168">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-168">String</span></span>|<span data-ttu-id="2b02a-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2b02a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b02a-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2b02a-171">displayName</span></span>|<span data-ttu-id="2b02a-172">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-172">String</span></span>|<span data-ttu-id="2b02a-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2b02a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b02a-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-175">version</span><span class="sxs-lookup"><span data-stu-id="2b02a-175">version</span></span>|<span data-ttu-id="2b02a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2b02a-176">Int32</span></span>|<span data-ttu-id="2b02a-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2b02a-177">Version of the device configuration.</span></span> <span data-ttu-id="2b02a-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2b02a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b02a-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="2b02a-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="2b02a-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="2b02a-181">このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="2b02a-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="2b02a-182">これにより、DMA リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="2b02a-183">このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="2b02a-184">カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="2b02a-185">これは、製造時にシステムによってサポートされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="2b02a-186">システムがカーネル DMA 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「Kernel DMA 保護」フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2b02a-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="2b02a-187">可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="2b02a-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="2b02a-188">firewallRules</span></span>|<span data-ttu-id="2b02a-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b02a-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="2b02a-190">ファイアウォール規則の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="2b02a-191">このコレクションには、最大150個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="2b02a-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="2b02a-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="2b02a-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-194">このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="2b02a-195">この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="2b02a-196">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="2b02a-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="2b02a-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-199">このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="2b02a-200">State Allowed がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2b02a-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="2b02a-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="2b02a-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="2b02a-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-203">このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="2b02a-204">ステートブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2b02a-204">State Block is supported.</span></span>|
|<span data-ttu-id="2b02a-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2b02a-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="2b02a-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-207">このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="2b02a-208">そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="2b02a-209">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="2b02a-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="2b02a-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-212">このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="2b02a-213">NotConfigured、許可およびブロックされる状態のすべてがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2b02a-213">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="2b02a-214">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="2b02a-214">userRightsBackupData</span></span>|[<span data-ttu-id="2b02a-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-216">このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-216">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="2b02a-217">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-217">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-218">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="2b02a-218">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="2b02a-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-220">このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-220">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="2b02a-221">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-222">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="2b02a-222">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="2b02a-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-224">このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-224">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="2b02a-225">グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-225">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="2b02a-226">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-227">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="2b02a-227">userRightsCreatePageFile</span></span>|[<span data-ttu-id="2b02a-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-229">このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-229">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="2b02a-230">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-231">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="2b02a-231">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="2b02a-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-233">このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-233">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="2b02a-234">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-235">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="2b02a-235">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="2b02a-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-237">このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-237">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="2b02a-238">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-239">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="2b02a-239">userRightsCreateToken</span></span>|[<span data-ttu-id="2b02a-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-241">このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-241">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="2b02a-242">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-243">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="2b02a-243">userRightsDebugPrograms</span></span>|[<span data-ttu-id="2b02a-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-245">このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-245">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="2b02a-246">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="2b02a-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="2b02a-247">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="2b02a-247">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="2b02a-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-249">このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-249">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="2b02a-250">NotConfigured とブロックのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2b02a-250">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="2b02a-251">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="2b02a-251">userRightsDelegation</span></span>|[<span data-ttu-id="2b02a-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-253">このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-253">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="2b02a-254">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-254">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-255">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="2b02a-255">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="2b02a-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-257">このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-257">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="2b02a-258">セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-258">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="2b02a-259">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-260">User/シムの個人ユーザー</span><span class="sxs-lookup"><span data-stu-id="2b02a-260">userRightsImpersonateClient</span></span>|[<span data-ttu-id="2b02a-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-262">このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-262">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="2b02a-263">この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。</span><span class="sxs-lookup"><span data-stu-id="2b02a-263">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="2b02a-264">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-265">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="2b02a-265">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="2b02a-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-267">このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-267">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="2b02a-268">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-269">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="2b02a-269">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="2b02a-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-271">このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-271">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="2b02a-272">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-273">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="2b02a-273">userRightsLockMemory</span></span>|[<span data-ttu-id="2b02a-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-275">このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-275">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="2b02a-276">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-277">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="2b02a-277">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="2b02a-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-279">このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-279">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="2b02a-280">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-281">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="2b02a-281">userRightsManageVolumes</span></span>|[<span data-ttu-id="2b02a-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-283">このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-283">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="2b02a-284">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-285">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="2b02a-285">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="2b02a-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-287">このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-287">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="2b02a-288">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-289">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="2b02a-289">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="2b02a-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-291">このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-291">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="2b02a-292">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-293">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="2b02a-293">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="2b02a-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-295">このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-295">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="2b02a-296">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-297">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="2b02a-297">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="2b02a-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-299">このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-299">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="2b02a-300">このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-300">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="2b02a-301">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-302">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="2b02a-302">userRightsRestoreData</span></span>|[<span data-ttu-id="2b02a-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-304">このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-304">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="2b02a-305">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-306">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="2b02a-306">userRightsTakeOwnership</span></span>|[<span data-ttu-id="2b02a-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-308">このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-308">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="2b02a-309">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="2b02a-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="2b02a-310">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="2b02a-310">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="2b02a-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="2b02a-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="2b02a-312">このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-312">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="2b02a-313">注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-313">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="2b02a-314">サポートされている状態はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-314">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="2b02a-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="2b02a-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="2b02a-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-316">Boolean</span></span>|<span data-ttu-id="2b02a-317">この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="2b02a-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="2b02a-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="2b02a-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="2b02a-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="2b02a-320">この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="2b02a-321">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="2b02a-321">Default: Manual.</span></span> <span data-ttu-id="2b02a-322">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="2b02a-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="2b02a-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="2b02a-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="2b02a-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="2b02a-325">この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="2b02a-326">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="2b02a-326">Default: Manual.</span></span> <span data-ttu-id="2b02a-327">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="2b02a-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="2b02a-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="2b02a-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="2b02a-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="2b02a-330">この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="2b02a-331">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="2b02a-331">Default: Manual.</span></span> <span data-ttu-id="2b02a-332">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="2b02a-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="2b02a-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="2b02a-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="2b02a-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="2b02a-335">この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="2b02a-336">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="2b02a-336">Default: Manual.</span></span> <span data-ttu-id="2b02a-337">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="2b02a-338">Localsecurityoptionsenableadministratoraccount</span><span class="sxs-lookup"><span data-stu-id="2b02a-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="2b02a-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-339">Boolean</span></span>|<span data-ttu-id="2b02a-340">ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="2b02a-341">Localsecurityoptionsblockremotelogonwithpassword</span><span class="sxs-lookup"><span data-stu-id="2b02a-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="2b02a-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-342">Boolean</span></span>|<span data-ttu-id="2b02a-343">パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="2b02a-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="2b02a-344">Localsecurityoptionsdisableアドミニストレーターアカウント</span><span class="sxs-lookup"><span data-stu-id="2b02a-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="2b02a-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-345">Boolean</span></span>|<span data-ttu-id="2b02a-346">ローカル管理者アカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="2b02a-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="2b02a-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="2b02a-348">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-348">String</span></span>|<span data-ttu-id="2b02a-349">アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="2b02a-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="2b02a-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="2b02a-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-351">Boolean</span></span>|<span data-ttu-id="2b02a-352">ゲストアカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="2b02a-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="2b02a-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="2b02a-354">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-354">String</span></span>|<span data-ttu-id="2b02a-355">アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="2b02a-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="2b02a-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="2b02a-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-357">Boolean</span></span>|<span data-ttu-id="2b02a-358">ログインせずに、ポータブルコンピューターをアンドックできないようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="2b02a-359">Localsecurityoptionsblockユーザーのドライバー</span><span class="sxs-lookup"><span data-stu-id="2b02a-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="2b02a-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-360">Boolean</span></span>|<span data-ttu-id="2b02a-361">共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="2b02a-362">Localsecurityoptionsblockremoteop' Aldrive Access</span><span class="sxs-lookup"><span data-stu-id="2b02a-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="2b02a-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-363">Boolean</span></span>|<span data-ttu-id="2b02a-364">この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="2b02a-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="2b02a-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="2b02a-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="2b02a-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="2b02a-367">リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="2b02a-368">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="2b02a-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="2b02a-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="2b02a-370">Int32</span><span class="sxs-lookup"><span data-stu-id="2b02a-370">Int32</span></span>|<span data-ttu-id="2b02a-371">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="2b02a-372">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="2b02a-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="2b02a-373">Localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool</span><span class="sxs-lookup"><span data-stu-id="2b02a-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="2b02a-374">Int32</span><span class="sxs-lookup"><span data-stu-id="2b02a-374">Int32</span></span>|<span data-ttu-id="2b02a-375">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="2b02a-376">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="2b02a-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="2b02a-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="2b02a-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="2b02a-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-378">Boolean</span></span>|<span data-ttu-id="2b02a-379">ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="2b02a-380">Localsecurityoption佐々木 Delastsignedinuser</span><span class="sxs-lookup"><span data-stu-id="2b02a-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="2b02a-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-381">Boolean</span></span>|<span data-ttu-id="2b02a-382">このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="2b02a-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="2b02a-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="2b02a-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-384">Boolean</span></span>|<span data-ttu-id="2b02a-385">資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="2b02a-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="2b02a-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="2b02a-387">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-387">String</span></span>|<span data-ttu-id="2b02a-388">ログインを試行するユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="2b02a-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="2b02a-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="2b02a-390">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-390">String</span></span>|<span data-ttu-id="2b02a-391">ログインを試行するユーザーのメッセージテキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="2b02a-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="2b02a-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="2b02a-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-393">Boolean</span></span>|<span data-ttu-id="2b02a-394">オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="2b02a-395">Localsecurityoptionsinformationshownonlockscreen</span><span class="sxs-lookup"><span data-stu-id="2b02a-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="2b02a-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-396">Boolean</span></span>|<span data-ttu-id="2b02a-397">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="2b02a-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="2b02a-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="2b02a-399">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-399">String</span></span>|<span data-ttu-id="2b02a-400">既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="2b02a-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="2b02a-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="2b02a-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="2b02a-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="2b02a-403">このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="2b02a-404">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="2b02a-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="2b02a-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="2b02a-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="2b02a-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="2b02a-407">このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="2b02a-408">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="2b02a-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="2b02a-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="2b02a-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="2b02a-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="2b02a-411">このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="2b02a-412">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="2b02a-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="2b02a-413">Lanmanagerwork ステーション Disableinsecureguestログオン</span><span class="sxs-lookup"><span data-stu-id="2b02a-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="2b02a-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-414">Boolean</span></span>|<span data-ttu-id="2b02a-415">有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="2b02a-416">構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="2b02a-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="2b02a-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="2b02a-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-418">Boolean</span></span>|<span data-ttu-id="2b02a-419">このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="2b02a-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="2b02a-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="2b02a-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-421">Boolean</span></span>|<span data-ttu-id="2b02a-422">このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="2b02a-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="2b02a-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="2b02a-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-424">Boolean</span></span>|<span data-ttu-id="2b02a-425">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="2b02a-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="2b02a-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="2b02a-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-427">Boolean</span></span>|<span data-ttu-id="2b02a-428">ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する</span><span class="sxs-lookup"><span data-stu-id="2b02a-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="2b02a-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="2b02a-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="2b02a-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-430">Boolean</span></span>|<span data-ttu-id="2b02a-431">指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="2b02a-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="2b02a-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="2b02a-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="2b02a-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="2b02a-434">管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="2b02a-435">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="2b02a-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="2b02a-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="2b02a-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="2b02a-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="2b02a-438">標準ユーザーの昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="2b02a-439">使用可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="2b02a-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="2b02a-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="2b02a-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-441">Boolean</span></span>|<span data-ttu-id="2b02a-442">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="2b02a-443">管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="2b02a-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="2b02a-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="2b02a-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-445">Boolean</span></span>|<span data-ttu-id="2b02a-446">昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="2b02a-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="2b02a-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="2b02a-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="2b02a-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-448">Boolean</span></span>|<span data-ttu-id="2b02a-449">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="2b02a-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="2b02a-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="2b02a-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="2b02a-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-451">Boolean</span></span>|<span data-ttu-id="2b02a-452">組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="2b02a-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="2b02a-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="2b02a-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="2b02a-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-454">Boolean</span></span>|<span data-ttu-id="2b02a-455">管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="2b02a-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="2b02a-456">localSecurityOptionsInformationShownOnLockScreen ロックアウト</span><span class="sxs-lookup"><span data-stu-id="2b02a-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="2b02a-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="2b02a-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="2b02a-458">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="2b02a-459">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="2b02a-460">使用可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="2b02a-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="2b02a-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="2b02a-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="2b02a-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="2b02a-463">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="2b02a-464">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="2b02a-465">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="2b02a-466">Localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers</span><span class="sxs-lookup"><span data-stu-id="2b02a-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="2b02a-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-467">Boolean</span></span>|<span data-ttu-id="2b02a-468">このセキュリティ設定は、SMB クライアントが SMB パケット署名のネゴシエートを試行するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="2b02a-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="2b02a-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="2b02a-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-470">Boolean</span></span>|<span data-ttu-id="2b02a-471">このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="2b02a-472">Localsecurityoptionsdisableserverdigitallysigncommunicationsalways</span><span class="sxs-lookup"><span data-stu-id="2b02a-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="2b02a-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-473">Boolean</span></span>|<span data-ttu-id="2b02a-474">このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="2b02a-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="2b02a-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="2b02a-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-476">Boolean</span></span>|<span data-ttu-id="2b02a-477">このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="2b02a-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="2b02a-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="2b02a-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-479">Boolean</span></span>|<span data-ttu-id="2b02a-480">このセキュリティ設定は、SMB サーバーが SMB パケットの署名を要求するクライアントとの間で SMB パケットの署名をネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="2b02a-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="2b02a-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="2b02a-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-482">Boolean</span></span>|<span data-ttu-id="2b02a-483">既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="2b02a-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="2b02a-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="2b02a-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-485">Boolean</span></span>|<span data-ttu-id="2b02a-486">このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="2b02a-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="2b02a-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="2b02a-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-488">Boolean</span></span>|<span data-ttu-id="2b02a-489">このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="2b02a-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="2b02a-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="2b02a-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-491">Boolean</span></span>|<span data-ttu-id="2b02a-492">このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="2b02a-493">既定では保存されません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="2b02a-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="2b02a-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="2b02a-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="2b02a-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="2b02a-496">このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="2b02a-497">使用可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="2b02a-498">Defendersecuritycenterdisablehealthui</span><span class="sxs-lookup"><span data-stu-id="2b02a-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="2b02a-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-499">Boolean</span></span>|<span data-ttu-id="2b02a-500">アプリとブラウザーの保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="2b02a-501">Defendersecuritycenterdisablenetworkui</span><span class="sxs-lookup"><span data-stu-id="2b02a-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="2b02a-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-502">Boolean</span></span>|<span data-ttu-id="2b02a-503">[ファミリオプション] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="2b02a-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="2b02a-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-505">Boolean</span></span>|<span data-ttu-id="2b02a-506">[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="2b02a-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="2b02a-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-508">Boolean</span></span>|<span data-ttu-id="2b02a-509">ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="2b02a-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="2b02a-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-511">Boolean</span></span>|<span data-ttu-id="2b02a-512">ウイルスおよび脅威保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="2b02a-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="2b02a-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-514">Boolean</span></span>|<span data-ttu-id="2b02a-515">[アカウントの保護] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="2b02a-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="2b02a-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-517">Boolean</span></span>|<span data-ttu-id="2b02a-518">[TPM のクリア] ボタンの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="2b02a-519">Defendersecurityセンター Disableハードウェア Ui</span><span class="sxs-lookup"><span data-stu-id="2b02a-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="2b02a-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-520">Boolean</span></span>|<span data-ttu-id="2b02a-521">[ハードウェア保護] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="2b02a-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="2b02a-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-523">Boolean</span></span>|<span data-ttu-id="2b02a-524">通知領域コントロールの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="2b02a-525">この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b02a-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="2b02a-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="2b02a-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-527">Boolean</span></span>|<span data-ttu-id="2b02a-528">ランサムウェア対策領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="2b02a-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="2b02a-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-530">Boolean</span></span>|<span data-ttu-id="2b02a-531">デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="2b02a-532">Defendersecurityセンター Disableトラブルシューティング Ui</span><span class="sxs-lookup"><span data-stu-id="2b02a-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="2b02a-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-533">Boolean</span></span>|<span data-ttu-id="2b02a-534">[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="2b02a-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="2b02a-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="2b02a-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-536">Boolean</span></span>|<span data-ttu-id="2b02a-537">脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="2b02a-538">Defendersecurityセンター組織 Displayname</span><span class="sxs-lookup"><span data-stu-id="2b02a-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="2b02a-539">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-539">String</span></span>|<span data-ttu-id="2b02a-540">ユーザーに表示される会社名。</span><span class="sxs-lookup"><span data-stu-id="2b02a-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="2b02a-541">Defendersecurityセンター Helpemail</span><span class="sxs-lookup"><span data-stu-id="2b02a-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="2b02a-542">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-542">String</span></span>|<span data-ttu-id="2b02a-543">ユーザーに表示される電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="2b02a-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="2b02a-544">Defendersecurityセンター Helpphone</span><span class="sxs-lookup"><span data-stu-id="2b02a-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="2b02a-545">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-545">String</span></span>|<span data-ttu-id="2b02a-546">ユーザーに表示される電話番号または Skype ID。</span><span class="sxs-lookup"><span data-stu-id="2b02a-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="2b02a-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="2b02a-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="2b02a-548">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-548">String</span></span>|<span data-ttu-id="2b02a-549">ヘルプポータルの URL これは、ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="2b02a-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="2b02a-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="2b02a-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="2b02a-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="2b02a-552">アプリの表示領域から表示する通知。</span><span class="sxs-lookup"><span data-stu-id="2b02a-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="2b02a-553">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="2b02a-554">Defendersecurityセンター Itcontactdisplay</span><span class="sxs-lookup"><span data-stu-id="2b02a-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="2b02a-555">Defendersecurityセンター Itcontactdisplaytype</span><span class="sxs-lookup"><span data-stu-id="2b02a-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="2b02a-556">エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="2b02a-557">使用可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="2b02a-558">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="2b02a-558">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="2b02a-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-559">Boolean</span></span>|<span data-ttu-id="2b02a-560">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="2b02a-560">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="2b02a-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="2b02a-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="2b02a-562">Int32</span><span class="sxs-lookup"><span data-stu-id="2b02a-562">Int32</span></span>|<span data-ttu-id="2b02a-563">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-563">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="2b02a-564">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-564">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="2b02a-565">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="2b02a-565">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="2b02a-566">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="2b02a-566">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="2b02a-567">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="2b02a-567">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="2b02a-568">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-568">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="2b02a-569">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-569">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="2b02a-570">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="2b02a-570">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="2b02a-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-571">Boolean</span></span>|<span data-ttu-id="2b02a-572">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-572">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="2b02a-573">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="2b02a-573">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="2b02a-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-574">Boolean</span></span>|<span data-ttu-id="2b02a-575">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-575">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="2b02a-576">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="2b02a-576">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="2b02a-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-577">Boolean</span></span>|<span data-ttu-id="2b02a-578">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-578">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="2b02a-579">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="2b02a-579">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="2b02a-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-580">Boolean</span></span>|<span data-ttu-id="2b02a-581">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-581">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="2b02a-582">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="2b02a-582">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="2b02a-583">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="2b02a-583">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="2b02a-584">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-584">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="2b02a-585">使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-585">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="2b02a-586">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="2b02a-586">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="2b02a-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-587">Boolean</span></span>|<span data-ttu-id="2b02a-588">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="2b02a-588">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="2b02a-589">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="2b02a-589">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="2b02a-590">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="2b02a-590">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="2b02a-591">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-591">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="2b02a-592">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-592">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="2b02a-593">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="2b02a-593">firewallProfileDomain</span></span>|[<span data-ttu-id="2b02a-594">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b02a-594">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="2b02a-595">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="2b02a-595">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="2b02a-596">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="2b02a-596">firewallProfilePublic</span></span>|[<span data-ttu-id="2b02a-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b02a-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="2b02a-598">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="2b02a-598">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="2b02a-599">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="2b02a-599">firewallProfilePrivate</span></span>|[<span data-ttu-id="2b02a-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b02a-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="2b02a-601">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="2b02a-601">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="2b02a-602">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="2b02a-602">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="2b02a-603">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-603">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-604">子プロセスの作成による Adobe Reader の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-604">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="2b02a-605">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-605">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-606">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="2b02a-606">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="2b02a-607">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2b02a-607">String collection</span></span>|<span data-ttu-id="2b02a-608">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="2b02a-608">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="2b02a-609">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-609">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="2b02a-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-611">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-611">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="2b02a-612">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-613">Defenderofficeappsexecutablecontentcreationorlaunch</span><span class="sxs-lookup"><span data-stu-id="2b02a-613">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="2b02a-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-615">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-615">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="2b02a-616">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-617">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="2b02a-617">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="2b02a-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-619">子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-619">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="2b02a-620">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-621">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="2b02a-621">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="2b02a-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-623">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-623">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="2b02a-624">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-625">Defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="2b02a-625">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="2b02a-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-627">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="2b02a-628">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-629">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="2b02a-629">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="2b02a-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-631">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-631">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="2b02a-632">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-633">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="2b02a-633">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="2b02a-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-635">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="2b02a-636">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-637">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="2b02a-637">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="2b02a-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-639">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-639">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="2b02a-640">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-641">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="2b02a-641">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="2b02a-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-643">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="2b02a-644">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-645">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="2b02a-645">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="2b02a-646">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-647">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-647">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="2b02a-648">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-649">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="2b02a-649">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="2b02a-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-651">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="2b02a-652">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-653">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-653">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="2b02a-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-655">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-655">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="2b02a-656">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-657">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="2b02a-657">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="2b02a-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-659">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="2b02a-660">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-661">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="2b02a-661">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="2b02a-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-663">Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-663">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="2b02a-664">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-665">Defenderprocessの種類</span><span class="sxs-lookup"><span data-stu-id="2b02a-665">defenderProcessCreationType</span></span>|[<span data-ttu-id="2b02a-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-667">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-667">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="2b02a-668">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-669">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="2b02a-669">defenderProcessCreation</span></span>|[<span data-ttu-id="2b02a-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-671">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="2b02a-672">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-673">Defenderアン Trustedusbprocesstype</span><span class="sxs-lookup"><span data-stu-id="2b02a-673">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="2b02a-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-675">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-675">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="2b02a-676">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-677">Defenderアン Trustedusbプロセス</span><span class="sxs-lookup"><span data-stu-id="2b02a-677">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="2b02a-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-679">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="2b02a-680">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-681">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="2b02a-681">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="2b02a-682">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-683">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-683">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="2b02a-684">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-685">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="2b02a-685">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="2b02a-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-687">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="2b02a-688">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-689">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-689">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="2b02a-690">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="2b02a-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="2b02a-691">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-691">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="2b02a-692">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-693">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="2b02a-693">defenderEmailContentExecution</span></span>|[<span data-ttu-id="2b02a-694">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-695">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="2b02a-696">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-697">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-697">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="2b02a-698">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-699">Ranware に対して高度な保護を使用することを示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-699">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="2b02a-700">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-701">Defendergu/Myfolderstype</span><span class="sxs-lookup"><span data-stu-id="2b02a-701">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="2b02a-702">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-702">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="2b02a-703">保護されたフォルダーの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="2b02a-703">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="2b02a-704">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-704">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="2b02a-705">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="2b02a-705">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="2b02a-706">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2b02a-706">String collection</span></span>|<span data-ttu-id="2b02a-707">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="2b02a-707">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="2b02a-708">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="2b02a-708">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="2b02a-709">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2b02a-709">String collection</span></span>|<span data-ttu-id="2b02a-710">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="2b02a-710">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="2b02a-711">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-711">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="2b02a-712">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="2b02a-712">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="2b02a-713">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-713">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="2b02a-714">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-714">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="2b02a-715">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="2b02a-715">defenderExploitProtectionXml</span></span>|<span data-ttu-id="2b02a-716">Binary</span><span class="sxs-lookup"><span data-stu-id="2b02a-716">Binary</span></span>|<span data-ttu-id="2b02a-717">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="2b02a-717">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="2b02a-718">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="2b02a-718">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="2b02a-719">String</span><span class="sxs-lookup"><span data-stu-id="2b02a-719">String</span></span>|<span data-ttu-id="2b02a-720">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="2b02a-720">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="2b02a-721">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="2b02a-721">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="2b02a-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-722">Boolean</span></span>|<span data-ttu-id="2b02a-723">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-723">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="2b02a-724">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="2b02a-724">appLockerApplicationControl</span></span>|[<span data-ttu-id="2b02a-725">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="2b02a-725">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="2b02a-726">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-726">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="2b02a-727">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-727">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="2b02a-728">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="2b02a-728">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="2b02a-729">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="2b02a-729">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="2b02a-730">セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-730">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="2b02a-731">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-731">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="2b02a-732">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="2b02a-732">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="2b02a-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-733">Boolean</span></span>|<span data-ttu-id="2b02a-734">仮想化ベースのセキュリティ (VBS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-734">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="2b02a-735">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="2b02a-735">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="2b02a-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-736">Boolean</span></span>|<span data-ttu-id="2b02a-737">このプロパティは、2019年5月に廃止され、プロパティ DeviceGuardSecureBootWithDMA に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-737">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="2b02a-738">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-738">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="2b02a-739">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="2b02a-739">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="2b02a-740">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="2b02a-740">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="2b02a-741">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="2b02a-742">可能な値は、`notConfigured`、`withoutDMA`、`withDMA` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-742">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="2b02a-743">Devicegu//Systemguard</span><span class="sxs-lookup"><span data-stu-id="2b02a-743">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="2b02a-744">購入</span><span class="sxs-lookup"><span data-stu-id="2b02a-744">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="2b02a-745">IT 管理者がシステムガードの起動を構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-745">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="2b02a-746">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-746">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b02a-747">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="2b02a-747">smartScreenEnableInShell</span></span>|<span data-ttu-id="2b02a-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-748">Boolean</span></span>|<span data-ttu-id="2b02a-749">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-749">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="2b02a-750">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="2b02a-750">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="2b02a-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-751">Boolean</span></span>|<span data-ttu-id="2b02a-752">ユーザーが SmartScreen 警告を無視したり、悪意のあるファイルを実行したりできるかどうかを IT 管理者が制御できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-752">Allows IT Admins to control whether users can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="2b02a-753">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="2b02a-753">applicationGuardEnabled</span></span>|<span data-ttu-id="2b02a-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-754">Boolean</span></span>|<span data-ttu-id="2b02a-755">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="2b02a-755">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="2b02a-756">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="2b02a-756">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="2b02a-757">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="2b02a-757">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="2b02a-758">新しい Windows ビルドに対して Windows Defender Application Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-758">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="2b02a-759">使用可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-759">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="2b02a-760">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="2b02a-760">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="2b02a-761">Applicationgu/Blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="2b02a-761">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="2b02a-762">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2b02a-762">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="2b02a-763">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-763">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="2b02a-764">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="2b02a-764">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="2b02a-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-765">Boolean</span></span>|<span data-ttu-id="2b02a-766">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="2b02a-766">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="2b02a-767">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="2b02a-767">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="2b02a-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-768">Boolean</span></span>|<span data-ttu-id="2b02a-769">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-769">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="2b02a-770">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="2b02a-770">applicationGuardForceAuditing</span></span>|<span data-ttu-id="2b02a-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-771">Boolean</span></span>|<span data-ttu-id="2b02a-772">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="2b02a-772">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="2b02a-773">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="2b02a-773">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="2b02a-774">Applicationgu/Blockクリップボード Sharingtype</span><span class="sxs-lookup"><span data-stu-id="2b02a-774">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="2b02a-775">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="2b02a-775">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="2b02a-776">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-776">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="2b02a-777">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="2b02a-777">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="2b02a-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-778">Boolean</span></span>|<span data-ttu-id="2b02a-779">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-779">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="2b02a-780">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="2b02a-780">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="2b02a-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-781">Boolean</span></span>|<span data-ttu-id="2b02a-782">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-782">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="2b02a-783">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="2b02a-783">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="2b02a-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-784">Boolean</span></span>|<span data-ttu-id="2b02a-785">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-785">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="2b02a-786">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="2b02a-786">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="2b02a-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-787">Boolean</span></span>|<span data-ttu-id="2b02a-788">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="2b02a-788">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="2b02a-789">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="2b02a-789">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="2b02a-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-790">Boolean</span></span>|<span data-ttu-id="2b02a-791">Application guard が仮想 GPU を使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="2b02a-791">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="2b02a-792">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="2b02a-792">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="2b02a-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-793">Boolean</span></span>|<span data-ttu-id="2b02a-794">アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する</span><span class="sxs-lookup"><span data-stu-id="2b02a-794">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="2b02a-795">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="2b02a-795">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="2b02a-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-796">Boolean</span></span>|<span data-ttu-id="2b02a-797">管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-797">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="2b02a-798">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="2b02a-798">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="2b02a-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-799">Boolean</span></span>|<span data-ttu-id="2b02a-800">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-800">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="2b02a-801">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="2b02a-801">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="2b02a-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-802">Boolean</span></span>|<span data-ttu-id="2b02a-803">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-803">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="2b02a-804">このポリシーは、携帯電話の SKU に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-804">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="2b02a-805">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="2b02a-805">bitLockerEncryptDevice</span></span>|<span data-ttu-id="2b02a-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b02a-806">Boolean</span></span>|<span data-ttu-id="2b02a-807">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="2b02a-808">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-808">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="2b02a-809">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-809">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="2b02a-810">BitLocker システムドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="2b02a-810">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="2b02a-811">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-811">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="2b02a-812">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-812">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="2b02a-813">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="2b02a-813">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="2b02a-814">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-814">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="2b02a-815">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2b02a-815">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="2b02a-816">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="2b02a-816">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2b02a-817">応答</span><span class="sxs-lookup"><span data-stu-id="2b02a-817">Response</span></span>
<span data-ttu-id="2b02a-818">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2b02a-818">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b02a-819">例</span><span class="sxs-lookup"><span data-stu-id="2b02a-819">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b02a-820">要求</span><span class="sxs-lookup"><span data-stu-id="2b02a-820">Request</span></span>
<span data-ttu-id="2b02a-821">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b02a-821">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 28463

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="2b02a-822">応答</span><span class="sxs-lookup"><span data-stu-id="2b02a-822">Response</span></span>
<span data-ttu-id="2b02a-p204">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b02a-p204">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 28635

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```





