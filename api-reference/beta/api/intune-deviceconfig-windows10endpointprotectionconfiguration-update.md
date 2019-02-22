---
title: windows10EndpointProtectionConfiguration の更新
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2680e25560d8211067a37f160d1341fd94b28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155091"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="0ccc1-103">windows10EndpointProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0ccc1-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="0ccc1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ccc1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ccc1-106">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ccc1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ccc1-107">Prerequisites</span></span>
<span data-ttu-id="0ccc1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ccc1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ccc1-110">Permission type</span></span>|<span data-ttu-id="0ccc1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ccc1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ccc1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ccc1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ccc1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccc1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ccc1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ccc1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ccc1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-115">Not supported.</span></span>|
|<span data-ttu-id="0ccc1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ccc1-116">Application</span></span>|<span data-ttu-id="0ccc1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ccc1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ccc1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ccc1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ccc1-119">Request headers</span></span>
|<span data-ttu-id="0ccc1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ccc1-120">Header</span></span>|<span data-ttu-id="0ccc1-121">値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ccc1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ccc1-122">Authorization</span></span>|<span data-ttu-id="0ccc1-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ccc1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0ccc1-124">Accept</span></span>|<span data-ttu-id="0ccc1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ccc1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ccc1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ccc1-126">Request body</span></span>
<span data-ttu-id="0ccc1-127">要求本文で、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="0ccc1-128">次の表に、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="0ccc1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ccc1-129">Property</span></span>|<span data-ttu-id="0ccc1-130">型</span><span class="sxs-lookup"><span data-stu-id="0ccc1-130">Type</span></span>|<span data-ttu-id="0ccc1-131">説明</span><span class="sxs-lookup"><span data-stu-id="0ccc1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ccc1-132">id</span><span class="sxs-lookup"><span data-stu-id="0ccc1-132">id</span></span>|<span data-ttu-id="0ccc1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0ccc1-133">String</span></span>|<span data-ttu-id="0ccc1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-134">Key of the entity.</span></span> <span data-ttu-id="0ccc1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ccc1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ccc1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ccc1-137">DateTimeOffset</span></span>|<span data-ttu-id="0ccc1-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0ccc1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ccc1-140">roleScopeTagIds</span></span>|<span data-ttu-id="0ccc1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0ccc1-141">String collection</span></span>|<span data-ttu-id="0ccc1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ccc1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ccc1-144">supportsScopeTags</span></span>|<span data-ttu-id="0ccc1-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-145">Boolean</span></span>|<span data-ttu-id="0ccc1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ccc1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ccc1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ccc1-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-149">This property is read-only.</span></span> <span data-ttu-id="0ccc1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ccc1-151">createdDateTime</span></span>|<span data-ttu-id="0ccc1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ccc1-152">DateTimeOffset</span></span>|<span data-ttu-id="0ccc1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-153">DateTime the object was created.</span></span> <span data-ttu-id="0ccc1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-155">説明</span><span class="sxs-lookup"><span data-stu-id="0ccc1-155">description</span></span>|<span data-ttu-id="0ccc1-156">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-156">String</span></span>|<span data-ttu-id="0ccc1-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ccc1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0ccc1-159">displayName</span></span>|<span data-ttu-id="0ccc1-160">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-160">String</span></span>|<span data-ttu-id="0ccc1-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ccc1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-163">version</span><span class="sxs-lookup"><span data-stu-id="0ccc1-163">version</span></span>|<span data-ttu-id="0ccc1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0ccc1-164">Int32</span></span>|<span data-ttu-id="0ccc1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-165">Version of the device configuration.</span></span> <span data-ttu-id="0ccc1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ccc1-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="0ccc1-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="0ccc1-169">このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="0ccc1-170">これにより、dma リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="0ccc1-171">このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="0ccc1-172">カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="0ccc1-173">これは、製造時にシステムによってサポートされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="0ccc1-174">システムがカーネル dma 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「kernel dma 保護」フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="0ccc1-175">可能な値は `deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="0ccc1-176">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="0ccc1-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="0ccc1-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-178">このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="0ccc1-179">この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="0ccc1-180">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-181">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="0ccc1-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="0ccc1-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-183">このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="0ccc1-184">State Allowed がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="0ccc1-185">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="0ccc1-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="0ccc1-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-187">このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="0ccc1-188">ステートブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-188">State Block is supported.</span></span>|
|<span data-ttu-id="0ccc1-189">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0ccc1-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="0ccc1-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-191">このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="0ccc1-192">そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="0ccc1-193">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-194">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="0ccc1-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="0ccc1-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-196">このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="0ccc1-197">NotConfigured、許可およびブロックされる状態のすべてがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="0ccc1-198">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="0ccc1-198">userRightsBackupData</span></span>|[<span data-ttu-id="0ccc1-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-200">このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="0ccc1-201">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-202">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="0ccc1-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="0ccc1-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-204">このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="0ccc1-205">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-206">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="0ccc1-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="0ccc1-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-208">このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="0ccc1-209">グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="0ccc1-210">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-211">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="0ccc1-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-213">このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="0ccc1-214">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-215">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="0ccc1-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="0ccc1-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-217">このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="0ccc1-218">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-219">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="0ccc1-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="0ccc1-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-221">このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="0ccc1-222">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-223">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="0ccc1-223">userRightsCreateToken</span></span>|[<span data-ttu-id="0ccc1-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-225">このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="0ccc1-226">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-227">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="0ccc1-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="0ccc1-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-229">このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="0ccc1-230">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="0ccc1-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="0ccc1-231">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="0ccc1-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="0ccc1-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-233">このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="0ccc1-234">NotConfigured とブロックのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="0ccc1-235">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="0ccc1-235">userRightsDelegation</span></span>|[<span data-ttu-id="0ccc1-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-237">このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="0ccc1-238">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-239">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="0ccc1-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="0ccc1-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-241">このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="0ccc1-242">セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="0ccc1-243">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-244">user/シムの個人ユーザー</span><span class="sxs-lookup"><span data-stu-id="0ccc1-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="0ccc1-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-246">このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="0ccc1-247">この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="0ccc1-248">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-249">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="0ccc1-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="0ccc1-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-251">このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="0ccc1-252">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-253">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="0ccc1-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="0ccc1-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-255">このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="0ccc1-256">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-257">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="0ccc1-257">userRightsLockMemory</span></span>|[<span data-ttu-id="0ccc1-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-259">このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="0ccc1-260">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-261">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="0ccc1-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="0ccc1-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-263">このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="0ccc1-264">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-265">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="0ccc1-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="0ccc1-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-267">このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="0ccc1-268">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-269">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="0ccc1-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="0ccc1-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-271">このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="0ccc1-272">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-273">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="0ccc1-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="0ccc1-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-275">このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="0ccc1-276">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-277">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="0ccc1-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="0ccc1-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-279">このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="0ccc1-280">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-281">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="0ccc1-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="0ccc1-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-283">このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="0ccc1-284">このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="0ccc1-285">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-286">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="0ccc1-286">userRightsRestoreData</span></span>|[<span data-ttu-id="0ccc1-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-288">このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="0ccc1-289">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-290">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="0ccc1-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="0ccc1-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-292">このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="0ccc1-293">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="0ccc1-294">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="0ccc1-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="0ccc1-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0ccc1-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="0ccc1-296">このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="0ccc1-297">注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="0ccc1-298">サポートされている状態はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="0ccc1-299">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="0ccc1-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="0ccc1-300">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-300">Boolean</span></span>|<span data-ttu-id="0ccc1-301">この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="0ccc1-302">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="0ccc1-303">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="0ccc1-304">この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="0ccc1-305">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-305">Default: Manual.</span></span> <span data-ttu-id="0ccc1-306">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="0ccc1-307">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="0ccc1-308">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="0ccc1-309">この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="0ccc1-310">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-310">Default: Manual.</span></span> <span data-ttu-id="0ccc1-311">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="0ccc1-312">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="0ccc1-313">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="0ccc1-314">この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="0ccc1-315">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-315">Default: Manual.</span></span> <span data-ttu-id="0ccc1-316">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="0ccc1-317">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="0ccc1-318">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="0ccc1-319">この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="0ccc1-320">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-320">Default: Manual.</span></span> <span data-ttu-id="0ccc1-321">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="0ccc1-322">localsecurityoptionsenableadministratoraccount</span><span class="sxs-lookup"><span data-stu-id="0ccc1-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="0ccc1-323">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-323">Boolean</span></span>|<span data-ttu-id="0ccc1-324">ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="0ccc1-325">localsecurityoptionsblockremotelogonwithpassword</span><span class="sxs-lookup"><span data-stu-id="0ccc1-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="0ccc1-326">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-326">Boolean</span></span>|<span data-ttu-id="0ccc1-327">パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="0ccc1-328">localsecurityoptionsdisableアドミニストレーターアカウント</span><span class="sxs-lookup"><span data-stu-id="0ccc1-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="0ccc1-329">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-329">Boolean</span></span>|<span data-ttu-id="0ccc1-330">ローカル管理者アカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="0ccc1-331">localsecurityoptionsadministratoraccountname</span><span class="sxs-lookup"><span data-stu-id="0ccc1-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="0ccc1-332">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-332">String</span></span>|<span data-ttu-id="0ccc1-333">アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="0ccc1-334">localsecurityoptionsdisableguestaccount</span><span class="sxs-lookup"><span data-stu-id="0ccc1-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="0ccc1-335">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-335">Boolean</span></span>|<span data-ttu-id="0ccc1-336">ゲストアカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="0ccc1-337">localsecurityoptionsguestaccountname</span><span class="sxs-lookup"><span data-stu-id="0ccc1-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="0ccc1-338">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-338">String</span></span>|<span data-ttu-id="0ccc1-339">アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="0ccc1-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="0ccc1-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="0ccc1-341">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-341">Boolean</span></span>|<span data-ttu-id="0ccc1-342">ログインせずに、ポータブルコンピューターをアンドックできないようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="0ccc1-343">localsecurityoptionsblockユーザーのドライバー</span><span class="sxs-lookup"><span data-stu-id="0ccc1-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="0ccc1-344">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-344">Boolean</span></span>|<span data-ttu-id="0ccc1-345">共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="0ccc1-346">localsecurityoptionsblockremoteop' aldrive access</span><span class="sxs-lookup"><span data-stu-id="0ccc1-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="0ccc1-347">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-347">Boolean</span></span>|<span data-ttu-id="0ccc1-348">この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="0ccc1-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="0ccc1-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="0ccc1-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="0ccc1-351">リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="0ccc1-352">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="0ccc1-353">localsecurityoptionsmachineinactivitylimit</span><span class="sxs-lookup"><span data-stu-id="0ccc1-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="0ccc1-354">Int32</span><span class="sxs-lookup"><span data-stu-id="0ccc1-354">Int32</span></span>|<span data-ttu-id="0ccc1-355">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="0ccc1-356">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="0ccc1-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="0ccc1-357">localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool</span><span class="sxs-lookup"><span data-stu-id="0ccc1-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="0ccc1-358">Int32</span><span class="sxs-lookup"><span data-stu-id="0ccc1-358">Int32</span></span>|<span data-ttu-id="0ccc1-359">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="0ccc1-360">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="0ccc1-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="0ccc1-361">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="0ccc1-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="0ccc1-362">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-362">Boolean</span></span>|<span data-ttu-id="0ccc1-363">ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="0ccc1-364">localsecurityoption佐々木 delastsignedinuser</span><span class="sxs-lookup"><span data-stu-id="0ccc1-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="0ccc1-365">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-365">Boolean</span></span>|<span data-ttu-id="0ccc1-366">このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="0ccc1-367">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="0ccc1-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="0ccc1-368">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-368">Boolean</span></span>|<span data-ttu-id="0ccc1-369">資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="0ccc1-370">localsecurityoptionslogonmessagetitle</span><span class="sxs-lookup"><span data-stu-id="0ccc1-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="0ccc1-371">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-371">String</span></span>|<span data-ttu-id="0ccc1-372">ログインを試行するユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="0ccc1-373">localsecurityoptionslogonmessagetext</span><span class="sxs-lookup"><span data-stu-id="0ccc1-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="0ccc1-374">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-374">String</span></span>|<span data-ttu-id="0ccc1-375">ログインを試行するユーザーのメッセージテキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="0ccc1-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="0ccc1-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="0ccc1-377">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-377">Boolean</span></span>|<span data-ttu-id="0ccc1-378">オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="0ccc1-379">localsecurityoptionsinformationshownonlockscreen</span><span class="sxs-lookup"><span data-stu-id="0ccc1-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="0ccc1-380">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-380">Boolean</span></span>|<span data-ttu-id="0ccc1-381">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="0ccc1-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="0ccc1-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="0ccc1-383">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-383">String</span></span>|<span data-ttu-id="0ccc1-384">既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="0ccc1-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="0ccc1-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="0ccc1-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="0ccc1-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="0ccc1-387">このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="0ccc1-388">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="0ccc1-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="0ccc1-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="0ccc1-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="0ccc1-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="0ccc1-391">このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="0ccc1-392">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="0ccc1-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="0ccc1-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="0ccc1-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="0ccc1-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="0ccc1-395">このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="0ccc1-396">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="0ccc1-397">lanmanagerwork ステーション disableinsecureguestログオン</span><span class="sxs-lookup"><span data-stu-id="0ccc1-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="0ccc1-398">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-398">Boolean</span></span>|<span data-ttu-id="0ccc1-399">有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="0ccc1-400">構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="0ccc1-401">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="0ccc1-402">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-402">Boolean</span></span>|<span data-ttu-id="0ccc1-403">このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="0ccc1-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="0ccc1-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="0ccc1-405">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-405">Boolean</span></span>|<span data-ttu-id="0ccc1-406">このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="0ccc1-407">localsecurityoptionsallowuiaccessapplicationelevation</span><span class="sxs-lookup"><span data-stu-id="0ccc1-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="0ccc1-408">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-408">Boolean</span></span>|<span data-ttu-id="0ccc1-409">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="0ccc1-410">localsecurityoptionsvirtualizefileandregistrywritefailurestoperuserlocations</span><span class="sxs-lookup"><span data-stu-id="0ccc1-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="0ccc1-411">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-411">Boolean</span></span>|<span data-ttu-id="0ccc1-412">ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する</span><span class="sxs-lookup"><span data-stu-id="0ccc1-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="0ccc1-413">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="0ccc1-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="0ccc1-414">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-414">Boolean</span></span>|<span data-ttu-id="0ccc1-415">指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="0ccc1-416">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="0ccc1-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="0ccc1-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="0ccc1-418">管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="0ccc1-419">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="0ccc1-420">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="0ccc1-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="0ccc1-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="0ccc1-422">標準ユーザーの昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="0ccc1-423">使用可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="0ccc1-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="0ccc1-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="0ccc1-425">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-425">Boolean</span></span>|<span data-ttu-id="0ccc1-426">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="0ccc1-427">管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="0ccc1-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="0ccc1-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="0ccc1-429">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-429">Boolean</span></span>|<span data-ttu-id="0ccc1-430">昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="0ccc1-431">localsecurityoptionsallowuiaccessapplicationsforsecurelocations</span><span class="sxs-lookup"><span data-stu-id="0ccc1-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="0ccc1-432">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-432">Boolean</span></span>|<span data-ttu-id="0ccc1-433">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="0ccc1-434">localsecurityoptionsuseadminapprovalmode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="0ccc1-435">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-435">Boolean</span></span>|<span data-ttu-id="0ccc1-436">組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="0ccc1-437">localsecurityoptionsuseadminapprovalmodeforadministrators</span><span class="sxs-lookup"><span data-stu-id="0ccc1-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="0ccc1-438">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-438">Boolean</span></span>|<span data-ttu-id="0ccc1-439">管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="0ccc1-440">localsecurityoptionsinformationshownonlockscreen ロックアウト</span><span class="sxs-lookup"><span data-stu-id="0ccc1-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="0ccc1-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="0ccc1-442">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="0ccc1-443">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="0ccc1-444">使用可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="0ccc1-445">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="0ccc1-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="0ccc1-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="0ccc1-447">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="0ccc1-448">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="0ccc1-449">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="0ccc1-450">localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers</span><span class="sxs-lookup"><span data-stu-id="0ccc1-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="0ccc1-451">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-451">Boolean</span></span>|<span data-ttu-id="0ccc1-452">このセキュリティ設定は、smb クライアントが smb パケット署名のネゴシエートを試行するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="0ccc1-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="0ccc1-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="0ccc1-454">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-454">Boolean</span></span>|<span data-ttu-id="0ccc1-455">このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="0ccc1-456">localsecurityoptionsdisableserverdigitallysigncommunicationsalways</span><span class="sxs-lookup"><span data-stu-id="0ccc1-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="0ccc1-457">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-457">Boolean</span></span>|<span data-ttu-id="0ccc1-458">このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="0ccc1-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="0ccc1-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="0ccc1-460">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-460">Boolean</span></span>|<span data-ttu-id="0ccc1-461">このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="0ccc1-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="0ccc1-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="0ccc1-463">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-463">Boolean</span></span>|<span data-ttu-id="0ccc1-464">このセキュリティ設定は、smb サーバーが smb パケットの署名を要求するクライアントとの間で smb パケットの署名をネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="0ccc1-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="0ccc1-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="0ccc1-466">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-466">Boolean</span></span>|<span data-ttu-id="0ccc1-467">既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="0ccc1-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="0ccc1-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="0ccc1-469">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-469">Boolean</span></span>|<span data-ttu-id="0ccc1-470">このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="0ccc1-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="0ccc1-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="0ccc1-472">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-472">Boolean</span></span>|<span data-ttu-id="0ccc1-473">このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="0ccc1-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="0ccc1-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="0ccc1-475">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-475">Boolean</span></span>|<span data-ttu-id="0ccc1-476">このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="0ccc1-477">既定では保存されません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="0ccc1-478">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="0ccc1-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="0ccc1-479">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-479">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="0ccc1-480">このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="0ccc1-481">使用可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="0ccc1-482">defendersecuritycenterdisablehealthui</span><span class="sxs-lookup"><span data-stu-id="0ccc1-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="0ccc1-483">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-483">Boolean</span></span>|<span data-ttu-id="0ccc1-484">アプリとブラウザーの保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="0ccc1-485">defendersecuritycenterdisablenetworkui</span><span class="sxs-lookup"><span data-stu-id="0ccc1-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="0ccc1-486">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-486">Boolean</span></span>|<span data-ttu-id="0ccc1-487">[ファミリオプション] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="0ccc1-488">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="0ccc1-489">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-489">Boolean</span></span>|<span data-ttu-id="0ccc1-490">[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="0ccc1-491">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="0ccc1-492">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-492">Boolean</span></span>|<span data-ttu-id="0ccc1-493">ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="0ccc1-494">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="0ccc1-495">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-495">Boolean</span></span>|<span data-ttu-id="0ccc1-496">ウイルスおよび脅威保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="0ccc1-497">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="0ccc1-498">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-498">Boolean</span></span>|<span data-ttu-id="0ccc1-499">[アカウントの保護] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="0ccc1-500">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-500">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="0ccc1-501">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-501">Boolean</span></span>|<span data-ttu-id="0ccc1-502">[TPM のクリア] ボタンの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-502">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="0ccc1-503">defendersecurityセンター disableハードウェア ui</span><span class="sxs-lookup"><span data-stu-id="0ccc1-503">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="0ccc1-504">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-504">Boolean</span></span>|<span data-ttu-id="0ccc1-505">[ハードウェア保護] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-505">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="0ccc1-506">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-506">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="0ccc1-507">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-507">Boolean</span></span>|<span data-ttu-id="0ccc1-508">通知領域コントロールの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-508">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="0ccc1-509">この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-509">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="0ccc1-510">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-510">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="0ccc1-511">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-511">Boolean</span></span>|<span data-ttu-id="0ccc1-512">ランサムウェア対策領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-512">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="0ccc1-513">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-513">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="0ccc1-514">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-514">Boolean</span></span>|<span data-ttu-id="0ccc1-515">デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-515">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="0ccc1-516">defendersecurityセンター disableトラブルシューティング ui</span><span class="sxs-lookup"><span data-stu-id="0ccc1-516">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="0ccc1-517">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-517">Boolean</span></span>|<span data-ttu-id="0ccc1-518">[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-518">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="0ccc1-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="0ccc1-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="0ccc1-520">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-520">Boolean</span></span>|<span data-ttu-id="0ccc1-521">脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-521">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="0ccc1-522">defendersecurityセンター組織 displayname</span><span class="sxs-lookup"><span data-stu-id="0ccc1-522">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="0ccc1-523">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-523">String</span></span>|<span data-ttu-id="0ccc1-524">ユーザーに表示される会社名。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-524">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="0ccc1-525">defendersecurityセンター helpemail</span><span class="sxs-lookup"><span data-stu-id="0ccc1-525">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="0ccc1-526">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-526">String</span></span>|<span data-ttu-id="0ccc1-527">ユーザーに表示される電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-527">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="0ccc1-528">defendersecurityセンター helpphone</span><span class="sxs-lookup"><span data-stu-id="0ccc1-528">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="0ccc1-529">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-529">String</span></span>|<span data-ttu-id="0ccc1-530">ユーザーに表示される電話番号または Skype ID。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-530">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="0ccc1-531">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="0ccc1-531">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="0ccc1-532">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-532">String</span></span>|<span data-ttu-id="0ccc1-533">ヘルプポータルの URL これは、ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-533">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="0ccc1-534">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="0ccc1-534">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="0ccc1-535">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-535">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="0ccc1-536">アプリの表示領域から表示する通知。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-536">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="0ccc1-537">可能な値は `notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-537">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="0ccc1-538">defendersecurityセンター itcontactdisplay</span><span class="sxs-lookup"><span data-stu-id="0ccc1-538">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="0ccc1-539">defendersecurityセンター itcontactdisplaytype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-539">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="0ccc1-540">エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-540">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="0ccc1-541">使用可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-541">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="0ccc1-542">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="0ccc1-542">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="0ccc1-543">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-543">Boolean</span></span>|<span data-ttu-id="0ccc1-544">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="0ccc1-544">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="0ccc1-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="0ccc1-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="0ccc1-546">Int32</span><span class="sxs-lookup"><span data-stu-id="0ccc1-546">Int32</span></span>|<span data-ttu-id="0ccc1-547">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-547">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="0ccc1-548">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-548">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="0ccc1-549">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="0ccc1-549">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="0ccc1-550">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="0ccc1-550">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="0ccc1-551">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-551">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="0ccc1-552">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-552">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="0ccc1-553">可能な値は `deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-553">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="0ccc1-554">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="0ccc1-554">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="0ccc1-555">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-555">Boolean</span></span>|<span data-ttu-id="0ccc1-556">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-556">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="0ccc1-557">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="0ccc1-557">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="0ccc1-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-558">Boolean</span></span>|<span data-ttu-id="0ccc1-559">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-559">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="0ccc1-560">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="0ccc1-560">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="0ccc1-561">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-561">Boolean</span></span>|<span data-ttu-id="0ccc1-562">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-562">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="0ccc1-563">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="0ccc1-563">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="0ccc1-564">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-564">Boolean</span></span>|<span data-ttu-id="0ccc1-565">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-565">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="0ccc1-566">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="0ccc1-566">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="0ccc1-567">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-567">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="0ccc1-568">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-568">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="0ccc1-569">使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-569">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="0ccc1-570">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="0ccc1-570">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="0ccc1-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-571">Boolean</span></span>|<span data-ttu-id="0ccc1-572">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-572">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="0ccc1-573">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="0ccc1-573">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="0ccc1-574">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-574">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="0ccc1-575">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-575">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="0ccc1-576">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-576">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="0ccc1-577">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="0ccc1-577">firewallProfileDomain</span></span>|[<span data-ttu-id="0ccc1-578">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-578">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0ccc1-579">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-579">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="0ccc1-580">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="0ccc1-580">firewallProfilePublic</span></span>|[<span data-ttu-id="0ccc1-581">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-581">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0ccc1-582">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-582">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="0ccc1-583">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="0ccc1-583">firewallProfilePrivate</span></span>|[<span data-ttu-id="0ccc1-584">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-584">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="0ccc1-585">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-585">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="0ccc1-586">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="0ccc1-586">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="0ccc1-587">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-587">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-588">子プロセスの作成による Adobe Reader の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-588">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="0ccc1-589">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-589">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-590">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="0ccc1-590">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="0ccc1-591">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0ccc1-591">String collection</span></span>|<span data-ttu-id="0ccc1-592">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="0ccc1-592">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="0ccc1-593">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-593">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="0ccc1-594">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-594">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-595">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-595">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="0ccc1-596">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-596">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-597">defenderofficeappsexecutablecontentcreationorlaunch</span><span class="sxs-lookup"><span data-stu-id="0ccc1-597">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="0ccc1-598">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-598">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-599">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-599">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="0ccc1-600">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-600">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-601">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="0ccc1-601">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="0ccc1-602">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-603">子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-603">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="0ccc1-604">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="0ccc1-606">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-606">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-607">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-607">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="0ccc1-608">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-608">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-609">defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="0ccc1-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="0ccc1-610">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-611">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="0ccc1-612">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-613">defenderofficeappslaunchchildprocesstype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-613">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="0ccc1-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-615">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-615">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="0ccc1-616">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-617">defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="0ccc1-617">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="0ccc1-618">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-619">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="0ccc1-620">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-621">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-621">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="0ccc1-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-623">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-623">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="0ccc1-624">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-625">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="0ccc1-625">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="0ccc1-626">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-627">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="0ccc1-628">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-629">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-629">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="0ccc1-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-631">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-631">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="0ccc1-632">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-633">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="0ccc1-633">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="0ccc1-634">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-635">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="0ccc1-636">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-637">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-637">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="0ccc1-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-639">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-639">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="0ccc1-640">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-641">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="0ccc1-641">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="0ccc1-642">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-643">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="0ccc1-644">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-645">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-645">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="0ccc1-646">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-647">Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-647">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="0ccc1-648">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-649">defenderprocessの種類</span><span class="sxs-lookup"><span data-stu-id="0ccc1-649">defenderProcessCreationType</span></span>|[<span data-ttu-id="0ccc1-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-651">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-651">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="0ccc1-652">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-653">defenderprocesscreation</span><span class="sxs-lookup"><span data-stu-id="0ccc1-653">defenderProcessCreation</span></span>|[<span data-ttu-id="0ccc1-654">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-655">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="0ccc1-656">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-657">defenderアン trustedusbprocesstype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-657">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="0ccc1-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-659">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-659">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="0ccc1-660">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-661">defenderアン trustedusbプロセス</span><span class="sxs-lookup"><span data-stu-id="0ccc1-661">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="0ccc1-662">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-663">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="0ccc1-664">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-665">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-665">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="0ccc1-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-667">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-667">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="0ccc1-668">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-669">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="0ccc1-669">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="0ccc1-670">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-671">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="0ccc1-672">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-673">defenderemailcontentexecutiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-673">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="0ccc1-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="0ccc1-675">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-675">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="0ccc1-676">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-677">defenderemailcontentexecution</span><span class="sxs-lookup"><span data-stu-id="0ccc1-677">defenderEmailContentExecution</span></span>|[<span data-ttu-id="0ccc1-678">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-679">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="0ccc1-680">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-681">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-681">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="0ccc1-682">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-683">ranware に対して高度な保護を使用することを示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-683">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="0ccc1-684">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-685">defendergu/myfolderstype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-685">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="0ccc1-686">folderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-686">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="0ccc1-687">保護されたフォルダーの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-687">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="0ccc1-688">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-688">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="0ccc1-689">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="0ccc1-689">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="0ccc1-690">String collection</span><span class="sxs-lookup"><span data-stu-id="0ccc1-690">String collection</span></span>|<span data-ttu-id="0ccc1-691">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="0ccc1-691">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="0ccc1-692">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="0ccc1-692">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="0ccc1-693">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0ccc1-693">String collection</span></span>|<span data-ttu-id="0ccc1-694">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="0ccc1-694">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="0ccc1-695">defendernetworkprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-695">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="0ccc1-696">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-696">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="0ccc1-697">networkprotection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-697">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="0ccc1-698">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-698">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="0ccc1-699">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="0ccc1-699">defenderExploitProtectionXml</span></span>|<span data-ttu-id="0ccc1-700">Binary</span><span class="sxs-lookup"><span data-stu-id="0ccc1-700">Binary</span></span>|<span data-ttu-id="0ccc1-701">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-701">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="0ccc1-702">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="0ccc1-702">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="0ccc1-703">String</span><span class="sxs-lookup"><span data-stu-id="0ccc1-703">String</span></span>|<span data-ttu-id="0ccc1-704">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-704">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="0ccc1-705">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="0ccc1-705">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="0ccc1-706">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-706">Boolean</span></span>|<span data-ttu-id="0ccc1-707">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-707">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="0ccc1-708">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="0ccc1-708">appLockerApplicationControl</span></span>|[<span data-ttu-id="0ccc1-709">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-709">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="0ccc1-710">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-710">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="0ccc1-711">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-711">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="0ccc1-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="0ccc1-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="0ccc1-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="0ccc1-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="0ccc1-714">セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-714">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="0ccc1-715">可能な値は `notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-715">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="0ccc1-716">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="0ccc1-716">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="0ccc1-717">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-717">Boolean</span></span>|<span data-ttu-id="0ccc1-718">仮想化ベースのセキュリティ (VBS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-718">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="0ccc1-719">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="0ccc1-719">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="0ccc1-720">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-720">Boolean</span></span>|<span data-ttu-id="0ccc1-721">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-721">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="0ccc1-722">devicegu//systemguard</span><span class="sxs-lookup"><span data-stu-id="0ccc1-722">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="0ccc1-723">購入</span><span class="sxs-lookup"><span data-stu-id="0ccc1-723">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0ccc1-724">IT 管理者がシステムガードの起動を構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-724">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="0ccc1-725">可能な値は `notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-725">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0ccc1-726">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="0ccc1-726">smartScreenEnableInShell</span></span>|<span data-ttu-id="0ccc1-727">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-727">Boolean</span></span>|<span data-ttu-id="0ccc1-728">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-728">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="0ccc1-729">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="0ccc1-729">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="0ccc1-730">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-730">Boolean</span></span>|<span data-ttu-id="0ccc1-731">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-731">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="0ccc1-732">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="0ccc1-732">applicationGuardEnabled</span></span>|<span data-ttu-id="0ccc1-733">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-733">Boolean</span></span>|<span data-ttu-id="0ccc1-734">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="0ccc1-734">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="0ccc1-735">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="0ccc1-735">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="0ccc1-736">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="0ccc1-736">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="0ccc1-737">新しい windows ビルドに対して windows Defender Application Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-737">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="0ccc1-738">使用可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-738">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="0ccc1-739">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="0ccc1-739">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="0ccc1-740">applicationgu/blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-740">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="0ccc1-741">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-741">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="0ccc1-742">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-742">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="0ccc1-743">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="0ccc1-743">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="0ccc1-744">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-744">Boolean</span></span>|<span data-ttu-id="0ccc1-745">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="0ccc1-745">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="0ccc1-746">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="0ccc1-746">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="0ccc1-747">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-747">Boolean</span></span>|<span data-ttu-id="0ccc1-748">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-748">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="0ccc1-749">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="0ccc1-749">applicationGuardForceAuditing</span></span>|<span data-ttu-id="0ccc1-750">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-750">Boolean</span></span>|<span data-ttu-id="0ccc1-751">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="0ccc1-751">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="0ccc1-752">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="0ccc1-752">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="0ccc1-753">applicationgu/blockクリップボード sharingtype</span><span class="sxs-lookup"><span data-stu-id="0ccc1-753">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="0ccc1-754">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-754">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="0ccc1-755">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-755">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="0ccc1-756">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="0ccc1-756">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="0ccc1-757">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-757">Boolean</span></span>|<span data-ttu-id="0ccc1-758">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-758">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="0ccc1-759">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="0ccc1-759">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="0ccc1-760">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-760">Boolean</span></span>|<span data-ttu-id="0ccc1-761">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-761">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="0ccc1-762">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="0ccc1-762">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="0ccc1-763">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-763">Boolean</span></span>|<span data-ttu-id="0ccc1-764">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-764">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="0ccc1-765">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="0ccc1-765">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="0ccc1-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-766">Boolean</span></span>|<span data-ttu-id="0ccc1-767">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="0ccc1-767">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="0ccc1-768">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="0ccc1-768">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="0ccc1-769">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-769">Boolean</span></span>|<span data-ttu-id="0ccc1-770">application guard が仮想 GPU を使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="0ccc1-770">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="0ccc1-771">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="0ccc1-771">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="0ccc1-772">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-772">Boolean</span></span>|<span data-ttu-id="0ccc1-773">アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する</span><span class="sxs-lookup"><span data-stu-id="0ccc1-773">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="0ccc1-774">bitlockerallowstandarduserencryption</span><span class="sxs-lookup"><span data-stu-id="0ccc1-774">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="0ccc1-775">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-775">Boolean</span></span>|<span data-ttu-id="0ccc1-776">管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-776">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="0ccc1-777">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="0ccc1-777">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="0ccc1-778">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ccc1-778">Boolean</span></span>|<span data-ttu-id="0ccc1-779">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-779">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="0ccc1-780">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="0ccc1-780">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="0ccc1-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-781">Boolean</span></span>|<span data-ttu-id="0ccc1-782">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-782">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="0ccc1-783">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="0ccc1-783">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="0ccc1-784">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="0ccc1-784">bitLockerEncryptDevice</span></span>|<span data-ttu-id="0ccc1-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccc1-785">Boolean</span></span>|<span data-ttu-id="0ccc1-786">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="0ccc1-787">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-787">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="0ccc1-788">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-788">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="0ccc1-789">BitLocker システムドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-789">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="0ccc1-790">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-790">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="0ccc1-791">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-791">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="0ccc1-792">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-792">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="0ccc1-793">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-793">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="0ccc1-794">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="0ccc1-794">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="0ccc1-795">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-795">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0ccc1-796">応答</span><span class="sxs-lookup"><span data-stu-id="0ccc1-796">Response</span></span>
<span data-ttu-id="0ccc1-797">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-797">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccc1-798">例</span><span class="sxs-lookup"><span data-stu-id="0ccc1-798">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ccc1-799">要求</span><span class="sxs-lookup"><span data-stu-id="0ccc1-799">Request</span></span>
<span data-ttu-id="0ccc1-800">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-800">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26778

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

### <a name="response"></a><span data-ttu-id="0ccc1-801">応答</span><span class="sxs-lookup"><span data-stu-id="0ccc1-801">Response</span></span>
<span data-ttu-id="0ccc1-p198">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ccc1-p198">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26950

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




