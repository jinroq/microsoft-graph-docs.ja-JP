---
title: windows10EndpointProtectionConfiguration の作成
description: 新しい windows10EndpointProtectionConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6080578ae14d0446ca725247be6baa9d7633058e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976937"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="56f29-103">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="56f29-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="56f29-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56f29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56f29-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56f29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56f29-106">新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56f29-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="56f29-107">Prerequisites</span></span>
<span data-ttu-id="56f29-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56f29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56f29-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56f29-110">Permission type</span></span>|<span data-ttu-id="56f29-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56f29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56f29-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56f29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56f29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56f29-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56f29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56f29-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56f29-115">Not supported.</span></span>|
|<span data-ttu-id="56f29-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56f29-116">Application</span></span>|<span data-ttu-id="56f29-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56f29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56f29-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56f29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56f29-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56f29-119">Request headers</span></span>
|<span data-ttu-id="56f29-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56f29-120">Header</span></span>|<span data-ttu-id="56f29-121">値</span><span class="sxs-lookup"><span data-stu-id="56f29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56f29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="56f29-122">Authorization</span></span>|<span data-ttu-id="56f29-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="56f29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56f29-124">承諾</span><span class="sxs-lookup"><span data-stu-id="56f29-124">Accept</span></span>|<span data-ttu-id="56f29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56f29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56f29-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="56f29-126">Request body</span></span>
<span data-ttu-id="56f29-127">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="56f29-128">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="56f29-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="56f29-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56f29-129">Property</span></span>|<span data-ttu-id="56f29-130">型</span><span class="sxs-lookup"><span data-stu-id="56f29-130">Type</span></span>|<span data-ttu-id="56f29-131">説明</span><span class="sxs-lookup"><span data-stu-id="56f29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f29-132">id</span><span class="sxs-lookup"><span data-stu-id="56f29-132">id</span></span>|<span data-ttu-id="56f29-133">文字列</span><span class="sxs-lookup"><span data-stu-id="56f29-133">String</span></span>|<span data-ttu-id="56f29-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="56f29-134">Key of the entity.</span></span> <span data-ttu-id="56f29-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56f29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="56f29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56f29-137">DateTimeOffset</span></span>|<span data-ttu-id="56f29-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="56f29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="56f29-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56f29-140">roleScopeTagIds</span></span>|<span data-ttu-id="56f29-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="56f29-141">String collection</span></span>|<span data-ttu-id="56f29-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="56f29-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56f29-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="56f29-144">supportsScopeTags</span></span>|<span data-ttu-id="56f29-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-145">Boolean</span></span>|<span data-ttu-id="56f29-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56f29-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="56f29-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="56f29-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="56f29-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="56f29-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="56f29-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="56f29-149">This property is read-only.</span></span> <span data-ttu-id="56f29-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="56f29-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="56f29-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="56f29-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="56f29-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="56f29-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="56f29-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="56f29-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="56f29-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="56f29-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="56f29-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="56f29-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="56f29-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="56f29-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="56f29-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="56f29-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="56f29-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="56f29-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="56f29-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56f29-163">createdDateTime</span></span>|<span data-ttu-id="56f29-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56f29-164">DateTimeOffset</span></span>|<span data-ttu-id="56f29-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="56f29-165">DateTime the object was created.</span></span> <span data-ttu-id="56f29-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-167">description</span><span class="sxs-lookup"><span data-stu-id="56f29-167">description</span></span>|<span data-ttu-id="56f29-168">String</span><span class="sxs-lookup"><span data-stu-id="56f29-168">String</span></span>|<span data-ttu-id="56f29-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="56f29-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56f29-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-171">displayName</span><span class="sxs-lookup"><span data-stu-id="56f29-171">displayName</span></span>|<span data-ttu-id="56f29-172">String</span><span class="sxs-lookup"><span data-stu-id="56f29-172">String</span></span>|<span data-ttu-id="56f29-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="56f29-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56f29-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-175">version</span><span class="sxs-lookup"><span data-stu-id="56f29-175">version</span></span>|<span data-ttu-id="56f29-176">Int32</span><span class="sxs-lookup"><span data-stu-id="56f29-176">Int32</span></span>|<span data-ttu-id="56f29-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="56f29-177">Version of the device configuration.</span></span> <span data-ttu-id="56f29-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56f29-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56f29-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="56f29-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="56f29-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="56f29-181">このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="56f29-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="56f29-182">これにより、DMA リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="56f29-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="56f29-183">このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="56f29-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="56f29-184">カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="56f29-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="56f29-185">これは、製造時にシステムによってサポートされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="56f29-186">システムがカーネル DMA 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「Kernel DMA 保護」フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="56f29-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="56f29-187">可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="56f29-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="56f29-188">firewallRules</span></span>|<span data-ttu-id="56f29-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="56f29-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="56f29-190">ファイアウォール規則の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="56f29-191">このコレクションには、最大150個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="56f29-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="56f29-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="56f29-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="56f29-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-194">このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="56f29-195">この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="56f29-196">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="56f29-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="56f29-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-199">このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="56f29-200">State Allowed がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="56f29-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="56f29-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="56f29-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="56f29-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-203">このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="56f29-204">ステートブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="56f29-204">State Block is supported.</span></span>|
|<span data-ttu-id="56f29-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56f29-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="56f29-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-207">このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。</span><span class="sxs-lookup"><span data-stu-id="56f29-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="56f29-208">そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="56f29-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="56f29-209">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="56f29-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="56f29-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-212">このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="56f29-213">状態 NotConfigured、許可されているもの</span><span class="sxs-lookup"><span data-stu-id="56f29-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="56f29-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="56f29-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="56f29-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-216">このユーザーの権利は、コンピューターにログオンできないユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="56f29-217">状態 NotConfigured、ブロックされている</span><span class="sxs-lookup"><span data-stu-id="56f29-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="56f29-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="56f29-218">userRightsBackupData</span></span>|[<span data-ttu-id="56f29-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-220">このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="56f29-221">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="56f29-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="56f29-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-224">このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="56f29-225">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="56f29-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="56f29-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-228">このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="56f29-229">グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="56f29-230">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="56f29-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="56f29-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-233">このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="56f29-234">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="56f29-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="56f29-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-237">このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="56f29-238">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="56f29-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="56f29-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-241">このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="56f29-242">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="56f29-243">userRightsCreateToken</span></span>|[<span data-ttu-id="56f29-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-245">このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="56f29-246">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="56f29-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="56f29-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-249">このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="56f29-250">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="56f29-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="56f29-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="56f29-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="56f29-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-253">このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="56f29-254">NotConfigured とブロックのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="56f29-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="56f29-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="56f29-255">userRightsDelegation</span></span>|[<span data-ttu-id="56f29-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-257">このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="56f29-258">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="56f29-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="56f29-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-261">このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="56f29-262">セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="56f29-263">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-264">User/シムの個人ユーザー</span><span class="sxs-lookup"><span data-stu-id="56f29-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="56f29-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-266">このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。</span><span class="sxs-lookup"><span data-stu-id="56f29-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="56f29-267">この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。</span><span class="sxs-lookup"><span data-stu-id="56f29-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="56f29-268">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="56f29-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="56f29-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-271">このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="56f29-272">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="56f29-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="56f29-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-275">このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="56f29-276">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="56f29-277">userRightsLockMemory</span></span>|[<span data-ttu-id="56f29-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-279">このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。</span><span class="sxs-lookup"><span data-stu-id="56f29-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="56f29-280">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="56f29-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="56f29-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-283">このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="56f29-284">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="56f29-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="56f29-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-287">このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="56f29-288">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="56f29-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="56f29-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-291">このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="56f29-292">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="56f29-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="56f29-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-295">このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="56f29-296">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="56f29-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="56f29-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-299">このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="56f29-300">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="56f29-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="56f29-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-303">このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="56f29-304">このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="56f29-305">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="56f29-306">userRightsRestoreData</span></span>|[<span data-ttu-id="56f29-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-308">このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="56f29-309">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="56f29-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="56f29-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-312">このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="56f29-313">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="56f29-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="56f29-314">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="56f29-314">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="56f29-315">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="56f29-315">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="56f29-316">このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-316">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="56f29-317">注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="56f29-317">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="56f29-318">サポートされている状態はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="56f29-318">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="56f29-319">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="56f29-319">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="56f29-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-320">Boolean</span></span>|<span data-ttu-id="56f29-321">この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-321">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="56f29-322">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="56f29-322">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="56f29-323">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="56f29-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="56f29-324">この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-324">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="56f29-325">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="56f29-325">Default: Manual.</span></span> <span data-ttu-id="56f29-326">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="56f29-327">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="56f29-327">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="56f29-328">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="56f29-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="56f29-329">この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-329">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="56f29-330">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="56f29-330">Default: Manual.</span></span> <span data-ttu-id="56f29-331">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="56f29-332">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="56f29-332">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="56f29-333">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="56f29-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="56f29-334">この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-334">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="56f29-335">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="56f29-335">Default: Manual.</span></span> <span data-ttu-id="56f29-336">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="56f29-337">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="56f29-337">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="56f29-338">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="56f29-338">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="56f29-339">この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-339">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="56f29-340">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="56f29-340">Default: Manual.</span></span> <span data-ttu-id="56f29-341">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-341">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="56f29-342">Localsecurityoptionsenableadministratoraccount</span><span class="sxs-lookup"><span data-stu-id="56f29-342">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="56f29-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-343">Boolean</span></span>|<span data-ttu-id="56f29-344">ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-344">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="56f29-345">Localsecurityoptionsblockremotelogonwithpassword</span><span class="sxs-lookup"><span data-stu-id="56f29-345">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="56f29-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-346">Boolean</span></span>|<span data-ttu-id="56f29-347">パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="56f29-347">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="56f29-348">Localsecurityoptionsdisableアドミニストレーターアカウント</span><span class="sxs-lookup"><span data-stu-id="56f29-348">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="56f29-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-349">Boolean</span></span>|<span data-ttu-id="56f29-350">ローカル管理者アカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-350">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="56f29-351">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="56f29-351">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="56f29-352">String</span><span class="sxs-lookup"><span data-stu-id="56f29-352">String</span></span>|<span data-ttu-id="56f29-353">アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-353">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="56f29-354">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="56f29-354">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="56f29-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-355">Boolean</span></span>|<span data-ttu-id="56f29-356">ゲストアカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-356">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="56f29-357">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="56f29-357">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="56f29-358">String</span><span class="sxs-lookup"><span data-stu-id="56f29-358">String</span></span>|<span data-ttu-id="56f29-359">アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-359">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="56f29-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="56f29-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="56f29-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-361">Boolean</span></span>|<span data-ttu-id="56f29-362">ログインせずに、ポータブルコンピューターをアンドックできないようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-362">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="56f29-363">Localsecurityoptionsblockユーザーのドライバー</span><span class="sxs-lookup"><span data-stu-id="56f29-363">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="56f29-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-364">Boolean</span></span>|<span data-ttu-id="56f29-365">共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="56f29-365">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="56f29-366">Localsecurityoptionsblockremoteop' Aldrive Access</span><span class="sxs-lookup"><span data-stu-id="56f29-366">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="56f29-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-367">Boolean</span></span>|<span data-ttu-id="56f29-368">この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="56f29-368">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="56f29-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="56f29-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="56f29-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="56f29-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="56f29-371">リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-371">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="56f29-372">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-372">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="56f29-373">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="56f29-373">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="56f29-374">Int32</span><span class="sxs-lookup"><span data-stu-id="56f29-374">Int32</span></span>|<span data-ttu-id="56f29-375">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="56f29-376">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="56f29-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="56f29-377">Localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool</span><span class="sxs-lookup"><span data-stu-id="56f29-377">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="56f29-378">Int32</span><span class="sxs-lookup"><span data-stu-id="56f29-378">Int32</span></span>|<span data-ttu-id="56f29-379">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-379">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="56f29-380">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="56f29-380">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="56f29-381">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="56f29-381">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="56f29-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-382">Boolean</span></span>|<span data-ttu-id="56f29-383">ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-383">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="56f29-384">Localsecurityoption佐々木 Delastsignedinuser</span><span class="sxs-lookup"><span data-stu-id="56f29-384">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="56f29-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-385">Boolean</span></span>|<span data-ttu-id="56f29-386">このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="56f29-386">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="56f29-387">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="56f29-387">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="56f29-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-388">Boolean</span></span>|<span data-ttu-id="56f29-389">資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="56f29-389">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="56f29-390">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="56f29-390">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="56f29-391">String</span><span class="sxs-lookup"><span data-stu-id="56f29-391">String</span></span>|<span data-ttu-id="56f29-392">ログインを試行するユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-392">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="56f29-393">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="56f29-393">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="56f29-394">String</span><span class="sxs-lookup"><span data-stu-id="56f29-394">String</span></span>|<span data-ttu-id="56f29-395">ログインを試行するユーザーのメッセージテキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-395">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="56f29-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="56f29-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="56f29-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-397">Boolean</span></span>|<span data-ttu-id="56f29-398">オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。</span><span class="sxs-lookup"><span data-stu-id="56f29-398">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="56f29-399">Localsecurityoptionsinformationshownonlockscreen</span><span class="sxs-lookup"><span data-stu-id="56f29-399">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="56f29-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-400">Boolean</span></span>|<span data-ttu-id="56f29-401">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-401">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="56f29-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="56f29-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="56f29-403">String</span><span class="sxs-lookup"><span data-stu-id="56f29-403">String</span></span>|<span data-ttu-id="56f29-404">既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="56f29-404">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="56f29-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="56f29-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="56f29-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="56f29-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="56f29-407">このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。</span><span class="sxs-lookup"><span data-stu-id="56f29-407">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="56f29-408">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="56f29-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="56f29-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="56f29-410">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="56f29-410">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="56f29-411">このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-411">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="56f29-412">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-412">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="56f29-413">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="56f29-413">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="56f29-414">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="56f29-414">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="56f29-415">このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-415">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="56f29-416">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="56f29-416">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="56f29-417">Lanmanagerwork ステーション Disableinsecureguestログオン</span><span class="sxs-lookup"><span data-stu-id="56f29-417">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="56f29-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-418">Boolean</span></span>|<span data-ttu-id="56f29-419">有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-419">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="56f29-420">構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="56f29-420">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="56f29-421">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="56f29-421">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="56f29-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-422">Boolean</span></span>|<span data-ttu-id="56f29-423">このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-423">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="56f29-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="56f29-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="56f29-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-425">Boolean</span></span>|<span data-ttu-id="56f29-426">このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-426">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="56f29-427">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="56f29-427">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="56f29-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-428">Boolean</span></span>|<span data-ttu-id="56f29-429">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-429">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="56f29-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="56f29-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="56f29-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-431">Boolean</span></span>|<span data-ttu-id="56f29-432">ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する</span><span class="sxs-lookup"><span data-stu-id="56f29-432">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="56f29-433">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="56f29-433">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="56f29-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-434">Boolean</span></span>|<span data-ttu-id="56f29-435">指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="56f29-435">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="56f29-436">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="56f29-436">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="56f29-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="56f29-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="56f29-438">管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-438">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="56f29-439">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-439">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="56f29-440">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="56f29-440">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="56f29-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="56f29-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="56f29-442">標準ユーザーの昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f29-442">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="56f29-443">使用可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-443">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="56f29-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="56f29-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="56f29-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-445">Boolean</span></span>|<span data-ttu-id="56f29-446">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56f29-446">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="56f29-447">管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-447">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="56f29-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="56f29-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="56f29-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-449">Boolean</span></span>|<span data-ttu-id="56f29-450">昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="56f29-450">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="56f29-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="56f29-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="56f29-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-452">Boolean</span></span>|<span data-ttu-id="56f29-453">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="56f29-453">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="56f29-454">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="56f29-454">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="56f29-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-455">Boolean</span></span>|<span data-ttu-id="56f29-456">組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="56f29-456">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="56f29-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="56f29-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="56f29-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-458">Boolean</span></span>|<span data-ttu-id="56f29-459">管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="56f29-459">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="56f29-460">localSecurityOptionsInformationShownOnLockScreen ロックアウト</span><span class="sxs-lookup"><span data-stu-id="56f29-460">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="56f29-461">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="56f29-461">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="56f29-462">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="56f29-463">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="56f29-464">使用可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-464">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="56f29-465">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="56f29-465">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="56f29-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="56f29-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="56f29-467">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-467">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="56f29-468">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-468">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="56f29-469">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-469">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="56f29-470">Localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers</span><span class="sxs-lookup"><span data-stu-id="56f29-470">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="56f29-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-471">Boolean</span></span>|<span data-ttu-id="56f29-472">このセキュリティ設定は、SMB クライアントが SMB パケット署名のネゴシエートを試行するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-472">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="56f29-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="56f29-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="56f29-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-474">Boolean</span></span>|<span data-ttu-id="56f29-475">このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-475">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="56f29-476">Localsecurityoptionsdisableserverdigitallysigncommunicationsalways</span><span class="sxs-lookup"><span data-stu-id="56f29-476">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="56f29-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-477">Boolean</span></span>|<span data-ttu-id="56f29-478">このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-478">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="56f29-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="56f29-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="56f29-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-480">Boolean</span></span>|<span data-ttu-id="56f29-481">このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-481">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="56f29-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="56f29-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="56f29-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-483">Boolean</span></span>|<span data-ttu-id="56f29-484">このセキュリティ設定は、SMB サーバーが SMB パケットの署名を要求するクライアントとの間で SMB パケットの署名をネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-484">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="56f29-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="56f29-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="56f29-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-486">Boolean</span></span>|<span data-ttu-id="56f29-487">既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-487">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="56f29-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="56f29-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="56f29-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-489">Boolean</span></span>|<span data-ttu-id="56f29-490">このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-490">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="56f29-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="56f29-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="56f29-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-492">Boolean</span></span>|<span data-ttu-id="56f29-493">このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-493">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="56f29-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="56f29-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="56f29-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-495">Boolean</span></span>|<span data-ttu-id="56f29-496">このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-496">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="56f29-497">既定では保存されません。</span><span class="sxs-lookup"><span data-stu-id="56f29-497">It’s not stored by default.</span></span>|
|<span data-ttu-id="56f29-498">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="56f29-498">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="56f29-499">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="56f29-499">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="56f29-500">このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-500">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="56f29-501">使用可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-501">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="56f29-502">Defendersecuritycenterdisablehealthui</span><span class="sxs-lookup"><span data-stu-id="56f29-502">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="56f29-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-503">Boolean</span></span>|<span data-ttu-id="56f29-504">アプリとブラウザーの保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-504">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="56f29-505">Defendersecuritycenterdisablenetworkui</span><span class="sxs-lookup"><span data-stu-id="56f29-505">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="56f29-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-506">Boolean</span></span>|<span data-ttu-id="56f29-507">[ファミリオプション] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="56f29-507">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="56f29-508">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="56f29-508">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="56f29-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-509">Boolean</span></span>|<span data-ttu-id="56f29-510">[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-510">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="56f29-511">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="56f29-511">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="56f29-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-512">Boolean</span></span>|<span data-ttu-id="56f29-513">ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-513">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="56f29-514">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="56f29-514">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="56f29-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-515">Boolean</span></span>|<span data-ttu-id="56f29-516">ウイルスおよび脅威保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-516">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="56f29-517">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="56f29-517">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="56f29-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-518">Boolean</span></span>|<span data-ttu-id="56f29-519">[アカウントの保護] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="56f29-519">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="56f29-520">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="56f29-520">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="56f29-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-521">Boolean</span></span>|<span data-ttu-id="56f29-522">[TPM のクリア] ボタンの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-522">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="56f29-523">Defendersecurityセンター Disableハードウェア Ui</span><span class="sxs-lookup"><span data-stu-id="56f29-523">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="56f29-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-524">Boolean</span></span>|<span data-ttu-id="56f29-525">[ハードウェア保護] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-525">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="56f29-526">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="56f29-526">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="56f29-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-527">Boolean</span></span>|<span data-ttu-id="56f29-528">通知領域コントロールの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-528">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="56f29-529">この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56f29-529">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="56f29-530">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="56f29-530">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="56f29-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-531">Boolean</span></span>|<span data-ttu-id="56f29-532">ランサムウェア対策領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-532">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="56f29-533">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="56f29-533">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="56f29-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-534">Boolean</span></span>|<span data-ttu-id="56f29-535">デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-535">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="56f29-536">Defendersecurityセンター Disableトラブルシューティング Ui</span><span class="sxs-lookup"><span data-stu-id="56f29-536">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="56f29-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-537">Boolean</span></span>|<span data-ttu-id="56f29-538">[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-538">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="56f29-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="56f29-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="56f29-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-540">Boolean</span></span>|<span data-ttu-id="56f29-541">脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-541">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="56f29-542">Defendersecurityセンター組織 Displayname</span><span class="sxs-lookup"><span data-stu-id="56f29-542">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="56f29-543">String</span><span class="sxs-lookup"><span data-stu-id="56f29-543">String</span></span>|<span data-ttu-id="56f29-544">ユーザーに表示される会社名。</span><span class="sxs-lookup"><span data-stu-id="56f29-544">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="56f29-545">Defendersecurityセンター Helpemail</span><span class="sxs-lookup"><span data-stu-id="56f29-545">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="56f29-546">String</span><span class="sxs-lookup"><span data-stu-id="56f29-546">String</span></span>|<span data-ttu-id="56f29-547">ユーザーに表示される電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="56f29-547">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="56f29-548">Defendersecurityセンター Helpphone</span><span class="sxs-lookup"><span data-stu-id="56f29-548">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="56f29-549">String</span><span class="sxs-lookup"><span data-stu-id="56f29-549">String</span></span>|<span data-ttu-id="56f29-550">ユーザーに表示される電話番号または Skype ID。</span><span class="sxs-lookup"><span data-stu-id="56f29-550">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="56f29-551">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="56f29-551">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="56f29-552">String</span><span class="sxs-lookup"><span data-stu-id="56f29-552">String</span></span>|<span data-ttu-id="56f29-553">ヘルプポータルの URL これは、ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-553">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="56f29-554">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="56f29-554">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="56f29-555">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="56f29-555">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="56f29-556">アプリの表示領域から表示する通知。</span><span class="sxs-lookup"><span data-stu-id="56f29-556">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="56f29-557">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-557">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="56f29-558">Defendersecurityセンター Itcontactdisplay</span><span class="sxs-lookup"><span data-stu-id="56f29-558">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="56f29-559">Defendersecurityセンター Itcontactdisplaytype</span><span class="sxs-lookup"><span data-stu-id="56f29-559">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="56f29-560">エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-560">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="56f29-561">使用可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-561">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="56f29-562">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="56f29-562">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="56f29-563">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="56f29-563">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="56f29-564">Windows defender TamperProtection の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-564">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="56f29-565">可能な値は、`notConfigured`、`enable`、`disable` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-565">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="56f29-566">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="56f29-566">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="56f29-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-567">Boolean</span></span>|<span data-ttu-id="56f29-568">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="56f29-568">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="56f29-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="56f29-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="56f29-570">Int32</span><span class="sxs-lookup"><span data-stu-id="56f29-570">Int32</span></span>|<span data-ttu-id="56f29-571">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-571">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="56f29-572">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="56f29-572">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="56f29-573">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="56f29-573">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="56f29-574">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="56f29-574">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="56f29-575">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="56f29-575">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="56f29-576">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="56f29-576">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="56f29-577">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-577">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="56f29-578">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="56f29-578">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="56f29-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-579">Boolean</span></span>|<span data-ttu-id="56f29-580">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-580">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="56f29-581">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="56f29-581">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="56f29-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-582">Boolean</span></span>|<span data-ttu-id="56f29-583">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-583">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="56f29-584">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="56f29-584">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="56f29-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-585">Boolean</span></span>|<span data-ttu-id="56f29-586">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-586">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="56f29-587">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="56f29-587">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="56f29-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-588">Boolean</span></span>|<span data-ttu-id="56f29-589">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-589">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="56f29-590">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="56f29-590">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="56f29-591">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="56f29-591">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="56f29-592">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-592">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="56f29-593">使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-593">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="56f29-594">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="56f29-594">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="56f29-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-595">Boolean</span></span>|<span data-ttu-id="56f29-596">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="56f29-596">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="56f29-597">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="56f29-597">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="56f29-598">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="56f29-598">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="56f29-599">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="56f29-599">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="56f29-600">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-600">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="56f29-601">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="56f29-601">firewallProfileDomain</span></span>|[<span data-ttu-id="56f29-602">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="56f29-602">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="56f29-603">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="56f29-603">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="56f29-604">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="56f29-604">firewallProfilePublic</span></span>|[<span data-ttu-id="56f29-605">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="56f29-605">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="56f29-606">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="56f29-606">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="56f29-607">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="56f29-607">firewallProfilePrivate</span></span>|[<span data-ttu-id="56f29-608">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="56f29-608">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="56f29-609">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="56f29-609">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="56f29-610">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="56f29-610">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="56f29-611">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-611">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-612">子プロセスの作成による Adobe Reader の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-612">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="56f29-613">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-613">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-614">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="56f29-614">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="56f29-615">String コレクション</span><span class="sxs-lookup"><span data-stu-id="56f29-615">String collection</span></span>|<span data-ttu-id="56f29-616">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="56f29-616">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="56f29-617">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-617">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="56f29-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-619">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-619">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="56f29-620">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-621">Defenderofficeappsexecutablecontentcreationorlaunch</span><span class="sxs-lookup"><span data-stu-id="56f29-621">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="56f29-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-623">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-623">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="56f29-624">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-625">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="56f29-625">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="56f29-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-627">子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-627">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="56f29-628">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="56f29-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="56f29-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-631">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="56f29-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="56f29-632">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-633">Defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="56f29-633">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="56f29-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-635">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="56f29-635">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="56f29-636">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-637">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="56f29-637">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="56f29-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-639">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="56f29-640">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-641">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="56f29-641">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="56f29-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-643">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-643">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="56f29-644">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-645">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="56f29-645">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="56f29-646">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-647">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="56f29-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="56f29-648">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-649">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="56f29-649">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="56f29-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-651">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="56f29-651">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="56f29-652">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-653">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="56f29-653">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="56f29-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-655">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="56f29-656">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-657">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="56f29-657">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="56f29-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-659">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-659">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="56f29-660">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-661">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="56f29-661">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="56f29-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-663">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="56f29-664">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-665">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="56f29-665">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="56f29-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-667">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-667">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="56f29-668">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-669">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="56f29-669">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="56f29-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-671">Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-671">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="56f29-672">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-673">Defenderprocessの種類</span><span class="sxs-lookup"><span data-stu-id="56f29-673">defenderProcessCreationType</span></span>|[<span data-ttu-id="56f29-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-675">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="56f29-676">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-677">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="56f29-677">defenderProcessCreation</span></span>|[<span data-ttu-id="56f29-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-679">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-679">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="56f29-680">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-681">Defenderアン Trustedusbprocesstype</span><span class="sxs-lookup"><span data-stu-id="56f29-681">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="56f29-682">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-683">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="56f29-684">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-685">Defenderアン Trustedusbプロセス</span><span class="sxs-lookup"><span data-stu-id="56f29-685">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="56f29-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-687">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-687">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="56f29-688">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-689">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="56f29-689">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="56f29-690">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-691">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="56f29-692">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-693">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="56f29-693">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="56f29-694">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-695">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-695">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="56f29-696">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-697">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="56f29-697">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="56f29-698">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="56f29-698">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="56f29-699">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="56f29-700">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-700">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-701">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="56f29-701">defenderEmailContentExecution</span></span>|[<span data-ttu-id="56f29-702">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-703">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-703">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="56f29-704">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-705">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-705">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="56f29-706">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-706">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-707">Ranware に対して高度な保護を使用することを示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-707">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="56f29-708">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-708">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-709">Defendergu/Myfolderstype</span><span class="sxs-lookup"><span data-stu-id="56f29-709">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="56f29-710">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-710">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="56f29-711">保護されたフォルダーの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="56f29-711">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="56f29-712">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-712">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="56f29-713">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="56f29-713">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="56f29-714">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="56f29-714">String collection</span></span>|<span data-ttu-id="56f29-715">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="56f29-715">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="56f29-716">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="56f29-716">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="56f29-717">String コレクション</span><span class="sxs-lookup"><span data-stu-id="56f29-717">String collection</span></span>|<span data-ttu-id="56f29-718">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="56f29-718">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="56f29-719">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-719">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="56f29-720">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="56f29-720">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="56f29-721">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="56f29-721">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="56f29-722">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-722">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="56f29-723">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="56f29-723">defenderExploitProtectionXml</span></span>|<span data-ttu-id="56f29-724">Binary</span><span class="sxs-lookup"><span data-stu-id="56f29-724">Binary</span></span>|<span data-ttu-id="56f29-725">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="56f29-725">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="56f29-726">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="56f29-726">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="56f29-727">String</span><span class="sxs-lookup"><span data-stu-id="56f29-727">String</span></span>|<span data-ttu-id="56f29-728">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="56f29-728">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="56f29-729">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="56f29-729">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="56f29-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-730">Boolean</span></span>|<span data-ttu-id="56f29-731">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56f29-731">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="56f29-732">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="56f29-732">appLockerApplicationControl</span></span>|[<span data-ttu-id="56f29-733">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="56f29-733">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="56f29-734">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-734">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="56f29-735">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-735">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="56f29-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="56f29-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="56f29-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="56f29-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="56f29-738">セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-738">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="56f29-739">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-739">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="56f29-740">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="56f29-740">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="56f29-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-741">Boolean</span></span>|<span data-ttu-id="56f29-742">仮想化ベースのセキュリティ (VBS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56f29-742">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="56f29-743">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="56f29-743">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="56f29-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-744">Boolean</span></span>|<span data-ttu-id="56f29-745">このプロパティは、2019年5月に廃止され、プロパティ DeviceGuardSecureBootWithDMA に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="56f29-745">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="56f29-746">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-746">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="56f29-747">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="56f29-747">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="56f29-748">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="56f29-748">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="56f29-749">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="56f29-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="56f29-750">可能な値は、`notConfigured`、`withoutDMA`、`withDMA` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-750">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="56f29-751">Devicegu//Systemguard</span><span class="sxs-lookup"><span data-stu-id="56f29-751">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="56f29-752">購入</span><span class="sxs-lookup"><span data-stu-id="56f29-752">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="56f29-753">IT 管理者がシステムガードの起動を構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="56f29-753">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="56f29-754">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-754">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="56f29-755">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="56f29-755">smartScreenEnableInShell</span></span>|<span data-ttu-id="56f29-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-756">Boolean</span></span>|<span data-ttu-id="56f29-757">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-757">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="56f29-758">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="56f29-758">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="56f29-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-759">Boolean</span></span>|<span data-ttu-id="56f29-760">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-760">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="56f29-761">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="56f29-761">applicationGuardEnabled</span></span>|<span data-ttu-id="56f29-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-762">Boolean</span></span>|<span data-ttu-id="56f29-763">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="56f29-763">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="56f29-764">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="56f29-764">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="56f29-765">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="56f29-765">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="56f29-766">新しい Windows ビルドに対して Windows Defender Application Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56f29-766">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="56f29-767">使用可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-767">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="56f29-768">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="56f29-768">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="56f29-769">Applicationgu/Blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="56f29-769">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="56f29-770">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="56f29-770">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="56f29-771">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-771">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="56f29-772">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="56f29-772">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="56f29-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-773">Boolean</span></span>|<span data-ttu-id="56f29-774">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="56f29-774">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="56f29-775">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="56f29-775">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="56f29-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-776">Boolean</span></span>|<span data-ttu-id="56f29-777">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-777">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="56f29-778">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="56f29-778">applicationGuardForceAuditing</span></span>|<span data-ttu-id="56f29-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-779">Boolean</span></span>|<span data-ttu-id="56f29-780">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="56f29-780">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="56f29-781">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="56f29-781">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="56f29-782">Applicationgu/Blockクリップボード Sharingtype</span><span class="sxs-lookup"><span data-stu-id="56f29-782">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="56f29-783">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="56f29-783">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="56f29-784">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="56f29-784">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="56f29-785">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="56f29-785">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="56f29-786">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-786">Boolean</span></span>|<span data-ttu-id="56f29-787">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-787">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="56f29-788">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="56f29-788">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="56f29-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-789">Boolean</span></span>|<span data-ttu-id="56f29-790">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-790">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="56f29-791">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="56f29-791">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="56f29-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-792">Boolean</span></span>|<span data-ttu-id="56f29-793">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-793">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="56f29-794">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="56f29-794">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="56f29-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-795">Boolean</span></span>|<span data-ttu-id="56f29-796">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="56f29-796">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="56f29-797">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="56f29-797">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="56f29-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-798">Boolean</span></span>|<span data-ttu-id="56f29-799">Application guard が仮想 GPU を使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="56f29-799">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="56f29-800">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="56f29-800">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="56f29-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-801">Boolean</span></span>|<span data-ttu-id="56f29-802">アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する</span><span class="sxs-lookup"><span data-stu-id="56f29-802">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="56f29-803">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="56f29-803">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="56f29-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-804">Boolean</span></span>|<span data-ttu-id="56f29-805">管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-805">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="56f29-806">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="56f29-806">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="56f29-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-807">Boolean</span></span>|<span data-ttu-id="56f29-808">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-808">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="56f29-809">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="56f29-809">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="56f29-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-810">Boolean</span></span>|<span data-ttu-id="56f29-811">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="56f29-812">このポリシーは、携帯電話の SKU に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="56f29-812">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="56f29-813">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="56f29-813">bitLockerEncryptDevice</span></span>|<span data-ttu-id="56f29-814">Boolean</span><span class="sxs-lookup"><span data-stu-id="56f29-814">Boolean</span></span>|<span data-ttu-id="56f29-815">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="56f29-815">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="56f29-816">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-816">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="56f29-817">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-817">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="56f29-818">BitLocker システムドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="56f29-818">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="56f29-819">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-819">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="56f29-820">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-820">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="56f29-821">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="56f29-821">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="56f29-822">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-822">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="56f29-823">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="56f29-823">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="56f29-824">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="56f29-824">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="56f29-825">応答</span><span class="sxs-lookup"><span data-stu-id="56f29-825">Response</span></span>
<span data-ttu-id="56f29-826">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56f29-826">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56f29-827">例</span><span class="sxs-lookup"><span data-stu-id="56f29-827">Example</span></span>

### <a name="request"></a><span data-ttu-id="56f29-828">要求</span><span class="sxs-lookup"><span data-stu-id="56f29-828">Request</span></span>
<span data-ttu-id="56f29-829">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56f29-829">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 28958

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
      "edgeTraversal": "blocked",
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
  "userRightsDenyLocalLogOn": {
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
  "windowsDefenderTamperProtection": "enable",
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

### <a name="response"></a><span data-ttu-id="56f29-830">応答</span><span class="sxs-lookup"><span data-stu-id="56f29-830">Response</span></span>
<span data-ttu-id="56f29-p206">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56f29-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 29130

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
      "edgeTraversal": "blocked",
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
  "userRightsDenyLocalLogOn": {
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
  "windowsDefenderTamperProtection": "enable",
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





