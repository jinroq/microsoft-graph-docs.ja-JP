---
title: windows10EndpointProtectionConfiguration の作成
description: 新しい windows10EndpointProtectionConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74dc20bf9a160e68f81024ee1badeb95df9d717a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921773"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="bef79-103">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="bef79-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="bef79-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bef79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bef79-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bef79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bef79-106">新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bef79-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bef79-107">Prerequisites</span></span>
<span data-ttu-id="bef79-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bef79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef79-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bef79-110">Permission type</span></span>|<span data-ttu-id="bef79-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bef79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef79-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bef79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bef79-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef79-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bef79-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bef79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef79-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bef79-115">Not supported.</span></span>|
|<span data-ttu-id="bef79-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bef79-116">Application</span></span>|<span data-ttu-id="bef79-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bef79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef79-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bef79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bef79-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bef79-119">Request headers</span></span>
|<span data-ttu-id="bef79-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bef79-120">Header</span></span>|<span data-ttu-id="bef79-121">値</span><span class="sxs-lookup"><span data-stu-id="bef79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef79-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bef79-122">Authorization</span></span>|<span data-ttu-id="bef79-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bef79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef79-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bef79-124">Accept</span></span>|<span data-ttu-id="bef79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bef79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef79-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bef79-126">Request body</span></span>
<span data-ttu-id="bef79-127">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="bef79-128">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bef79-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="bef79-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bef79-129">Property</span></span>|<span data-ttu-id="bef79-130">型</span><span class="sxs-lookup"><span data-stu-id="bef79-130">Type</span></span>|<span data-ttu-id="bef79-131">説明</span><span class="sxs-lookup"><span data-stu-id="bef79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef79-132">id</span><span class="sxs-lookup"><span data-stu-id="bef79-132">id</span></span>|<span data-ttu-id="bef79-133">文字列</span><span class="sxs-lookup"><span data-stu-id="bef79-133">String</span></span>|<span data-ttu-id="bef79-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bef79-134">Key of the entity.</span></span> <span data-ttu-id="bef79-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bef79-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bef79-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef79-137">DateTimeOffset</span></span>|<span data-ttu-id="bef79-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="bef79-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bef79-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bef79-140">roleScopeTagIds</span></span>|<span data-ttu-id="bef79-141">String collection</span><span class="sxs-lookup"><span data-stu-id="bef79-141">String collection</span></span>|<span data-ttu-id="bef79-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="bef79-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bef79-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bef79-144">supportsScopeTags</span></span>|<span data-ttu-id="bef79-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-145">Boolean</span></span>|<span data-ttu-id="bef79-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bef79-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bef79-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="bef79-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bef79-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="bef79-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bef79-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="bef79-149">This property is read-only.</span></span> <span data-ttu-id="bef79-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bef79-151">createdDateTime</span></span>|<span data-ttu-id="bef79-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef79-152">DateTimeOffset</span></span>|<span data-ttu-id="bef79-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bef79-153">DateTime the object was created.</span></span> <span data-ttu-id="bef79-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-155">description</span><span class="sxs-lookup"><span data-stu-id="bef79-155">description</span></span>|<span data-ttu-id="bef79-156">String</span><span class="sxs-lookup"><span data-stu-id="bef79-156">String</span></span>|<span data-ttu-id="bef79-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="bef79-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bef79-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bef79-159">displayName</span></span>|<span data-ttu-id="bef79-160">String</span><span class="sxs-lookup"><span data-stu-id="bef79-160">String</span></span>|<span data-ttu-id="bef79-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="bef79-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bef79-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-163">version</span><span class="sxs-lookup"><span data-stu-id="bef79-163">version</span></span>|<span data-ttu-id="bef79-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bef79-164">Int32</span></span>|<span data-ttu-id="bef79-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="bef79-165">Version of the device configuration.</span></span> <span data-ttu-id="bef79-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bef79-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef79-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="bef79-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="bef79-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="bef79-169">このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="bef79-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="bef79-170">これにより、DMA リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="bef79-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="bef79-171">このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="bef79-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="bef79-172">カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="bef79-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="bef79-173">これは、製造時にシステムによってサポートされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="bef79-174">システムがカーネル DMA 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「Kernel DMA 保護」フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bef79-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="bef79-175">可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="bef79-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="bef79-176">firewallRules</span></span>|<span data-ttu-id="bef79-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bef79-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="bef79-178">ファイアウォール規則の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="bef79-179">このコレクションには、最大150個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bef79-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="bef79-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="bef79-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="bef79-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-182">このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="bef79-183">この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="bef79-184">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="bef79-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="bef79-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-187">このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="bef79-188">State Allowed がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bef79-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="bef79-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="bef79-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="bef79-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-191">このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="bef79-192">ステートブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bef79-192">State Block is supported.</span></span>|
|<span data-ttu-id="bef79-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bef79-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="bef79-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-195">このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。</span><span class="sxs-lookup"><span data-stu-id="bef79-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="bef79-196">そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="bef79-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="bef79-197">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="bef79-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="bef79-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-200">このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="bef79-201">NotConfigured、許可およびブロックされる状態のすべてがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bef79-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="bef79-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="bef79-202">userRightsBackupData</span></span>|[<span data-ttu-id="bef79-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-204">このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="bef79-205">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="bef79-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="bef79-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-208">このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="bef79-209">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="bef79-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="bef79-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-212">このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="bef79-213">グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="bef79-214">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="bef79-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="bef79-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-217">このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="bef79-218">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="bef79-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="bef79-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-221">このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="bef79-222">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="bef79-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="bef79-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-225">このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="bef79-226">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="bef79-227">userRightsCreateToken</span></span>|[<span data-ttu-id="bef79-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-229">このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="bef79-230">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="bef79-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="bef79-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-233">このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="bef79-234">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="bef79-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="bef79-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="bef79-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="bef79-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-237">このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="bef79-238">NotConfigured とブロックのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bef79-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="bef79-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="bef79-239">userRightsDelegation</span></span>|[<span data-ttu-id="bef79-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-241">このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="bef79-242">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="bef79-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="bef79-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-245">このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="bef79-246">セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="bef79-247">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-248">User/シムの個人ユーザー</span><span class="sxs-lookup"><span data-stu-id="bef79-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="bef79-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-250">このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。</span><span class="sxs-lookup"><span data-stu-id="bef79-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="bef79-251">この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。</span><span class="sxs-lookup"><span data-stu-id="bef79-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="bef79-252">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="bef79-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="bef79-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-255">このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="bef79-256">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="bef79-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="bef79-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-259">このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="bef79-260">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="bef79-261">userRightsLockMemory</span></span>|[<span data-ttu-id="bef79-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-263">このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。</span><span class="sxs-lookup"><span data-stu-id="bef79-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="bef79-264">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="bef79-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="bef79-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-267">このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="bef79-268">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="bef79-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="bef79-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-271">このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="bef79-272">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="bef79-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="bef79-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-275">このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="bef79-276">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="bef79-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="bef79-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-279">このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="bef79-280">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="bef79-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="bef79-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-283">このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="bef79-284">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="bef79-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="bef79-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-287">このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="bef79-288">このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="bef79-289">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="bef79-290">userRightsRestoreData</span></span>|[<span data-ttu-id="bef79-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-292">このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="bef79-293">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="bef79-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="bef79-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-296">このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="bef79-297">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="bef79-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="bef79-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="bef79-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="bef79-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="bef79-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="bef79-300">このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="bef79-301">注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="bef79-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="bef79-302">サポートされている状態はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="bef79-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="bef79-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="bef79-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="bef79-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-304">Boolean</span></span>|<span data-ttu-id="bef79-305">この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="bef79-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="bef79-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="bef79-307">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="bef79-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="bef79-308">この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="bef79-309">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="bef79-309">Default: Manual.</span></span> <span data-ttu-id="bef79-310">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="bef79-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="bef79-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="bef79-312">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="bef79-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="bef79-313">この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="bef79-314">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="bef79-314">Default: Manual.</span></span> <span data-ttu-id="bef79-315">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="bef79-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="bef79-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="bef79-317">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="bef79-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="bef79-318">この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="bef79-319">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="bef79-319">Default: Manual.</span></span> <span data-ttu-id="bef79-320">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="bef79-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="bef79-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="bef79-322">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="bef79-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="bef79-323">この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="bef79-324">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="bef79-324">Default: Manual.</span></span> <span data-ttu-id="bef79-325">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="bef79-326">Localsecurityoptionsenableadministratoraccount</span><span class="sxs-lookup"><span data-stu-id="bef79-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="bef79-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-327">Boolean</span></span>|<span data-ttu-id="bef79-328">ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="bef79-329">Localsecurityoptionsblockremotelogonwithpassword</span><span class="sxs-lookup"><span data-stu-id="bef79-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="bef79-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-330">Boolean</span></span>|<span data-ttu-id="bef79-331">パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef79-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="bef79-332">Localsecurityoptionsdisableアドミニストレーターアカウント</span><span class="sxs-lookup"><span data-stu-id="bef79-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="bef79-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-333">Boolean</span></span>|<span data-ttu-id="bef79-334">ローカル管理者アカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="bef79-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="bef79-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="bef79-336">String</span><span class="sxs-lookup"><span data-stu-id="bef79-336">String</span></span>|<span data-ttu-id="bef79-337">アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="bef79-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="bef79-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="bef79-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-339">Boolean</span></span>|<span data-ttu-id="bef79-340">ゲストアカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="bef79-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="bef79-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="bef79-342">String</span><span class="sxs-lookup"><span data-stu-id="bef79-342">String</span></span>|<span data-ttu-id="bef79-343">アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="bef79-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="bef79-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="bef79-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-345">Boolean</span></span>|<span data-ttu-id="bef79-346">ログインせずに、ポータブルコンピューターをアンドックできないようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="bef79-347">Localsecurityoptionsblockユーザーのドライバー</span><span class="sxs-lookup"><span data-stu-id="bef79-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="bef79-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-348">Boolean</span></span>|<span data-ttu-id="bef79-349">共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="bef79-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="bef79-350">Localsecurityoptionsblockremoteop' Aldrive Access</span><span class="sxs-lookup"><span data-stu-id="bef79-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="bef79-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-351">Boolean</span></span>|<span data-ttu-id="bef79-352">この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="bef79-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="bef79-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="bef79-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="bef79-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="bef79-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="bef79-355">リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="bef79-356">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="bef79-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="bef79-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="bef79-358">Int32</span><span class="sxs-lookup"><span data-stu-id="bef79-358">Int32</span></span>|<span data-ttu-id="bef79-359">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="bef79-360">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="bef79-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="bef79-361">Localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool</span><span class="sxs-lookup"><span data-stu-id="bef79-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="bef79-362">Int32</span><span class="sxs-lookup"><span data-stu-id="bef79-362">Int32</span></span>|<span data-ttu-id="bef79-363">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="bef79-364">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="bef79-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="bef79-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="bef79-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="bef79-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-366">Boolean</span></span>|<span data-ttu-id="bef79-367">ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="bef79-368">Localsecurityoption佐々木 Delastsignedinuser</span><span class="sxs-lookup"><span data-stu-id="bef79-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="bef79-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-369">Boolean</span></span>|<span data-ttu-id="bef79-370">このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="bef79-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="bef79-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="bef79-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="bef79-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-372">Boolean</span></span>|<span data-ttu-id="bef79-373">資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="bef79-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="bef79-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="bef79-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="bef79-375">String</span><span class="sxs-lookup"><span data-stu-id="bef79-375">String</span></span>|<span data-ttu-id="bef79-376">ログインを試行するユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="bef79-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="bef79-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="bef79-378">String</span><span class="sxs-lookup"><span data-stu-id="bef79-378">String</span></span>|<span data-ttu-id="bef79-379">ログインを試行するユーザーのメッセージテキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="bef79-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="bef79-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="bef79-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-381">Boolean</span></span>|<span data-ttu-id="bef79-382">オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。</span><span class="sxs-lookup"><span data-stu-id="bef79-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="bef79-383">Localsecurityoptionsinformationshownonlockscreen</span><span class="sxs-lookup"><span data-stu-id="bef79-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="bef79-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-384">Boolean</span></span>|<span data-ttu-id="bef79-385">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="bef79-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="bef79-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="bef79-387">String</span><span class="sxs-lookup"><span data-stu-id="bef79-387">String</span></span>|<span data-ttu-id="bef79-388">既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="bef79-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="bef79-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="bef79-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="bef79-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="bef79-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="bef79-391">このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。</span><span class="sxs-lookup"><span data-stu-id="bef79-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="bef79-392">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="bef79-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="bef79-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="bef79-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="bef79-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="bef79-395">このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="bef79-396">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="bef79-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="bef79-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="bef79-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="bef79-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="bef79-399">このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="bef79-400">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="bef79-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="bef79-401">Lanmanagerwork ステーション Disableinsecureguestログオン</span><span class="sxs-lookup"><span data-stu-id="bef79-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="bef79-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-402">Boolean</span></span>|<span data-ttu-id="bef79-403">有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="bef79-404">構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="bef79-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="bef79-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="bef79-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="bef79-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-406">Boolean</span></span>|<span data-ttu-id="bef79-407">このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="bef79-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="bef79-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="bef79-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-409">Boolean</span></span>|<span data-ttu-id="bef79-410">このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="bef79-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="bef79-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="bef79-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-412">Boolean</span></span>|<span data-ttu-id="bef79-413">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="bef79-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="bef79-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="bef79-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-415">Boolean</span></span>|<span data-ttu-id="bef79-416">ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する</span><span class="sxs-lookup"><span data-stu-id="bef79-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="bef79-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="bef79-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="bef79-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-418">Boolean</span></span>|<span data-ttu-id="bef79-419">指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="bef79-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="bef79-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="bef79-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="bef79-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="bef79-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="bef79-422">管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="bef79-423">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="bef79-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="bef79-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="bef79-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="bef79-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="bef79-426">標準ユーザーの昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="bef79-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="bef79-427">使用可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="bef79-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="bef79-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="bef79-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-429">Boolean</span></span>|<span data-ttu-id="bef79-430">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bef79-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="bef79-431">管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="bef79-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="bef79-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="bef79-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-433">Boolean</span></span>|<span data-ttu-id="bef79-434">昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef79-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="bef79-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="bef79-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="bef79-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-436">Boolean</span></span>|<span data-ttu-id="bef79-437">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef79-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="bef79-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="bef79-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="bef79-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-439">Boolean</span></span>|<span data-ttu-id="bef79-440">組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef79-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="bef79-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="bef79-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="bef79-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-442">Boolean</span></span>|<span data-ttu-id="bef79-443">管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef79-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="bef79-444">localSecurityOptionsInformationShownOnLockScreen ロックアウト</span><span class="sxs-lookup"><span data-stu-id="bef79-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="bef79-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="bef79-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="bef79-446">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="bef79-447">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="bef79-448">使用可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="bef79-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="bef79-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="bef79-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="bef79-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="bef79-451">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="bef79-452">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="bef79-453">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="bef79-454">Localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers</span><span class="sxs-lookup"><span data-stu-id="bef79-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="bef79-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-455">Boolean</span></span>|<span data-ttu-id="bef79-456">このセキュリティ設定は、SMB クライアントが SMB パケット署名のネゴシエートを試行するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="bef79-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="bef79-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="bef79-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-458">Boolean</span></span>|<span data-ttu-id="bef79-459">このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="bef79-460">Localsecurityoptionsdisableserverdigitallysigncommunicationsalways</span><span class="sxs-lookup"><span data-stu-id="bef79-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="bef79-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-461">Boolean</span></span>|<span data-ttu-id="bef79-462">このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="bef79-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="bef79-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="bef79-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-464">Boolean</span></span>|<span data-ttu-id="bef79-465">このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="bef79-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="bef79-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="bef79-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-467">Boolean</span></span>|<span data-ttu-id="bef79-468">このセキュリティ設定は、SMB サーバーが SMB パケットの署名を要求するクライアントとの間で SMB パケットの署名をネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="bef79-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="bef79-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="bef79-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-470">Boolean</span></span>|<span data-ttu-id="bef79-471">既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="bef79-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="bef79-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="bef79-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-473">Boolean</span></span>|<span data-ttu-id="bef79-474">このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="bef79-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="bef79-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="bef79-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-476">Boolean</span></span>|<span data-ttu-id="bef79-477">このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="bef79-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="bef79-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="bef79-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-479">Boolean</span></span>|<span data-ttu-id="bef79-480">このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="bef79-481">既定では保存されません。</span><span class="sxs-lookup"><span data-stu-id="bef79-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="bef79-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="bef79-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="bef79-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="bef79-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="bef79-484">このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="bef79-485">使用可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="bef79-486">Defendersecuritycenterdisablehealthui</span><span class="sxs-lookup"><span data-stu-id="bef79-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="bef79-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-487">Boolean</span></span>|<span data-ttu-id="bef79-488">アプリとブラウザーの保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="bef79-489">Defendersecuritycenterdisablenetworkui</span><span class="sxs-lookup"><span data-stu-id="bef79-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="bef79-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-490">Boolean</span></span>|<span data-ttu-id="bef79-491">[ファミリオプション] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="bef79-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="bef79-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="bef79-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="bef79-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-493">Boolean</span></span>|<span data-ttu-id="bef79-494">[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="bef79-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="bef79-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="bef79-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-496">Boolean</span></span>|<span data-ttu-id="bef79-497">ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="bef79-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="bef79-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="bef79-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-499">Boolean</span></span>|<span data-ttu-id="bef79-500">ウイルスおよび脅威保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="bef79-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="bef79-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="bef79-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-502">Boolean</span></span>|<span data-ttu-id="bef79-503">[アカウントの保護] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="bef79-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="bef79-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="bef79-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="bef79-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-505">Boolean</span></span>|<span data-ttu-id="bef79-506">[TPM のクリア] ボタンの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="bef79-507">Defendersecurityセンター Disableハードウェア Ui</span><span class="sxs-lookup"><span data-stu-id="bef79-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="bef79-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-508">Boolean</span></span>|<span data-ttu-id="bef79-509">[ハードウェア保護] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="bef79-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="bef79-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="bef79-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-511">Boolean</span></span>|<span data-ttu-id="bef79-512">通知領域コントロールの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="bef79-513">この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bef79-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="bef79-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="bef79-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="bef79-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-515">Boolean</span></span>|<span data-ttu-id="bef79-516">ランサムウェア対策領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="bef79-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="bef79-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="bef79-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-518">Boolean</span></span>|<span data-ttu-id="bef79-519">デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="bef79-520">Defendersecurityセンター Disableトラブルシューティング Ui</span><span class="sxs-lookup"><span data-stu-id="bef79-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="bef79-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-521">Boolean</span></span>|<span data-ttu-id="bef79-522">[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="bef79-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="bef79-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="bef79-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-524">Boolean</span></span>|<span data-ttu-id="bef79-525">脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="bef79-526">Defendersecurityセンター組織 Displayname</span><span class="sxs-lookup"><span data-stu-id="bef79-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="bef79-527">String</span><span class="sxs-lookup"><span data-stu-id="bef79-527">String</span></span>|<span data-ttu-id="bef79-528">ユーザーに表示される会社名。</span><span class="sxs-lookup"><span data-stu-id="bef79-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="bef79-529">Defendersecurityセンター Helpemail</span><span class="sxs-lookup"><span data-stu-id="bef79-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="bef79-530">String</span><span class="sxs-lookup"><span data-stu-id="bef79-530">String</span></span>|<span data-ttu-id="bef79-531">ユーザーに表示される電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="bef79-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="bef79-532">Defendersecurityセンター Helpphone</span><span class="sxs-lookup"><span data-stu-id="bef79-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="bef79-533">String</span><span class="sxs-lookup"><span data-stu-id="bef79-533">String</span></span>|<span data-ttu-id="bef79-534">ユーザーに表示される電話番号または Skype ID。</span><span class="sxs-lookup"><span data-stu-id="bef79-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="bef79-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="bef79-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="bef79-536">String</span><span class="sxs-lookup"><span data-stu-id="bef79-536">String</span></span>|<span data-ttu-id="bef79-537">ヘルプポータルの URL これは、ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="bef79-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="bef79-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="bef79-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="bef79-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="bef79-540">アプリの表示領域から表示する通知。</span><span class="sxs-lookup"><span data-stu-id="bef79-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="bef79-541">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="bef79-542">Defendersecurityセンター Itcontactdisplay</span><span class="sxs-lookup"><span data-stu-id="bef79-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="bef79-543">Defendersecurityセンター Itcontactdisplaytype</span><span class="sxs-lookup"><span data-stu-id="bef79-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="bef79-544">エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="bef79-545">使用可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="bef79-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="bef79-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="bef79-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-547">Boolean</span></span>|<span data-ttu-id="bef79-548">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="bef79-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="bef79-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="bef79-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="bef79-550">Int32</span><span class="sxs-lookup"><span data-stu-id="bef79-550">Int32</span></span>|<span data-ttu-id="bef79-551">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="bef79-552">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="bef79-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="bef79-553">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="bef79-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="bef79-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="bef79-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="bef79-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="bef79-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="bef79-556">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="bef79-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="bef79-557">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="bef79-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="bef79-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="bef79-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-559">Boolean</span></span>|<span data-ttu-id="bef79-560">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="bef79-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="bef79-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="bef79-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-562">Boolean</span></span>|<span data-ttu-id="bef79-563">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="bef79-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="bef79-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="bef79-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-565">Boolean</span></span>|<span data-ttu-id="bef79-566">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="bef79-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="bef79-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="bef79-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-568">Boolean</span></span>|<span data-ttu-id="bef79-569">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="bef79-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="bef79-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="bef79-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="bef79-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="bef79-572">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="bef79-573">使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="bef79-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="bef79-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="bef79-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-575">Boolean</span></span>|<span data-ttu-id="bef79-576">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="bef79-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="bef79-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="bef79-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="bef79-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="bef79-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="bef79-579">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="bef79-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="bef79-580">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="bef79-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="bef79-581">firewallProfileDomain</span></span>|[<span data-ttu-id="bef79-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bef79-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="bef79-583">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="bef79-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="bef79-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="bef79-584">firewallProfilePublic</span></span>|[<span data-ttu-id="bef79-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bef79-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="bef79-586">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="bef79-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="bef79-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="bef79-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="bef79-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="bef79-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="bef79-589">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="bef79-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="bef79-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="bef79-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="bef79-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-592">子プロセスの作成による Adobe Reader の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="bef79-593">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="bef79-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="bef79-595">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bef79-595">String collection</span></span>|<span data-ttu-id="bef79-596">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="bef79-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="bef79-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="bef79-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-599">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="bef79-600">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-601">Defenderofficeappsexecutablecontentcreationorlaunch</span><span class="sxs-lookup"><span data-stu-id="bef79-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="bef79-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-603">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="bef79-604">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="bef79-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="bef79-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-607">子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="bef79-608">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="bef79-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="bef79-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-611">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="bef79-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="bef79-612">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-613">Defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="bef79-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="bef79-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-615">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="bef79-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="bef79-616">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="bef79-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="bef79-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-619">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="bef79-620">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="bef79-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="bef79-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-623">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="bef79-624">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="bef79-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="bef79-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-627">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="bef79-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="bef79-628">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="bef79-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="bef79-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-631">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="bef79-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="bef79-632">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="bef79-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="bef79-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-635">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="bef79-636">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="bef79-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="bef79-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-639">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="bef79-640">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="bef79-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="bef79-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-643">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="bef79-644">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="bef79-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="bef79-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-647">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="bef79-648">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="bef79-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="bef79-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-651">Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="bef79-652">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-653">Defenderprocessの種類</span><span class="sxs-lookup"><span data-stu-id="bef79-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="bef79-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-655">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="bef79-656">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="bef79-657">defenderProcessCreation</span></span>|[<span data-ttu-id="bef79-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-659">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="bef79-660">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-661">Defenderアン Trustedusbprocesstype</span><span class="sxs-lookup"><span data-stu-id="bef79-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="bef79-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-663">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="bef79-664">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-665">Defenderアン Trustedusbプロセス</span><span class="sxs-lookup"><span data-stu-id="bef79-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="bef79-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-667">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="bef79-668">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="bef79-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="bef79-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-671">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="bef79-672">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="bef79-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="bef79-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-675">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="bef79-676">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="bef79-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="bef79-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="bef79-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="bef79-679">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="bef79-680">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="bef79-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="bef79-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-683">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="bef79-684">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="bef79-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-687">Ranware に対して高度な保護を使用することを示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="bef79-688">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-689">Defendergu/Myfolderstype</span><span class="sxs-lookup"><span data-stu-id="bef79-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="bef79-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="bef79-691">保護されたフォルダーの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="bef79-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="bef79-692">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="bef79-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="bef79-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="bef79-694">String collection</span><span class="sxs-lookup"><span data-stu-id="bef79-694">String collection</span></span>|<span data-ttu-id="bef79-695">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="bef79-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="bef79-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="bef79-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="bef79-697">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bef79-697">String collection</span></span>|<span data-ttu-id="bef79-698">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="bef79-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="bef79-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="bef79-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="bef79-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="bef79-701">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="bef79-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="bef79-702">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="bef79-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="bef79-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="bef79-704">Binary</span><span class="sxs-lookup"><span data-stu-id="bef79-704">Binary</span></span>|<span data-ttu-id="bef79-705">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="bef79-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="bef79-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="bef79-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="bef79-707">String</span><span class="sxs-lookup"><span data-stu-id="bef79-707">String</span></span>|<span data-ttu-id="bef79-708">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="bef79-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="bef79-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="bef79-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="bef79-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-710">Boolean</span></span>|<span data-ttu-id="bef79-711">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bef79-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="bef79-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="bef79-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="bef79-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="bef79-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="bef79-714">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="bef79-715">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="bef79-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="bef79-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="bef79-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="bef79-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="bef79-718">セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="bef79-719">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="bef79-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="bef79-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="bef79-721">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-721">Boolean</span></span>|<span data-ttu-id="bef79-722">仮想化ベースのセキュリティ (VBS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bef79-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="bef79-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="bef79-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="bef79-724">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-724">Boolean</span></span>|<span data-ttu-id="bef79-725">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bef79-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="bef79-726">Devicegu//Systemguard</span><span class="sxs-lookup"><span data-stu-id="bef79-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="bef79-727">購入</span><span class="sxs-lookup"><span data-stu-id="bef79-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bef79-728">IT 管理者がシステムガードの起動を構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bef79-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="bef79-729">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bef79-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="bef79-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="bef79-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-731">Boolean</span></span>|<span data-ttu-id="bef79-732">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="bef79-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="bef79-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="bef79-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-734">Boolean</span></span>|<span data-ttu-id="bef79-735">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="bef79-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="bef79-736">applicationGuardEnabled</span></span>|<span data-ttu-id="bef79-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-737">Boolean</span></span>|<span data-ttu-id="bef79-738">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="bef79-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="bef79-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="bef79-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="bef79-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="bef79-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="bef79-741">新しい Windows ビルドに対して Windows Defender Application Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bef79-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="bef79-742">使用可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="bef79-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="bef79-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="bef79-744">Applicationgu/Blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="bef79-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="bef79-745">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="bef79-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="bef79-746">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="bef79-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="bef79-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="bef79-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-748">Boolean</span></span>|<span data-ttu-id="bef79-749">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="bef79-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="bef79-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="bef79-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="bef79-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-751">Boolean</span></span>|<span data-ttu-id="bef79-752">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="bef79-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="bef79-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="bef79-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-754">Boolean</span></span>|<span data-ttu-id="bef79-755">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="bef79-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="bef79-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="bef79-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="bef79-757">Applicationgu/Blockクリップボード Sharingtype</span><span class="sxs-lookup"><span data-stu-id="bef79-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="bef79-758">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="bef79-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="bef79-759">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="bef79-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="bef79-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="bef79-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="bef79-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-761">Boolean</span></span>|<span data-ttu-id="bef79-762">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="bef79-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="bef79-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="bef79-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-764">Boolean</span></span>|<span data-ttu-id="bef79-765">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="bef79-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="bef79-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="bef79-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-767">Boolean</span></span>|<span data-ttu-id="bef79-768">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="bef79-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="bef79-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="bef79-770">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-770">Boolean</span></span>|<span data-ttu-id="bef79-771">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="bef79-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="bef79-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="bef79-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="bef79-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-773">Boolean</span></span>|<span data-ttu-id="bef79-774">Application guard が仮想 GPU を使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="bef79-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="bef79-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="bef79-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="bef79-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-776">Boolean</span></span>|<span data-ttu-id="bef79-777">アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する</span><span class="sxs-lookup"><span data-stu-id="bef79-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="bef79-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="bef79-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="bef79-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-779">Boolean</span></span>|<span data-ttu-id="bef79-780">管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="bef79-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="bef79-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="bef79-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-782">Boolean</span></span>|<span data-ttu-id="bef79-783">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="bef79-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="bef79-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="bef79-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-785">Boolean</span></span>|<span data-ttu-id="bef79-786">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="bef79-787">このポリシーは、携帯電話の SKU に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="bef79-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="bef79-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="bef79-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="bef79-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef79-789">Boolean</span></span>|<span data-ttu-id="bef79-790">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="bef79-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="bef79-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="bef79-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="bef79-793">BitLocker システムドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="bef79-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="bef79-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="bef79-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="bef79-796">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="bef79-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="bef79-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="bef79-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="bef79-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="bef79-799">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="bef79-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="bef79-800">応答</span><span class="sxs-lookup"><span data-stu-id="bef79-800">Response</span></span>
<span data-ttu-id="bef79-801">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bef79-801">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef79-802">例</span><span class="sxs-lookup"><span data-stu-id="bef79-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="bef79-803">要求</span><span class="sxs-lookup"><span data-stu-id="bef79-803">Request</span></span>
<span data-ttu-id="bef79-804">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bef79-804">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 27641

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="bef79-805">応答</span><span class="sxs-lookup"><span data-stu-id="bef79-805">Response</span></span>
<span data-ttu-id="bef79-p199">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bef79-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 27813

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




