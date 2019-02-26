---
title: windows10EndpointProtectionConfiguration の作成
description: 新しい windows10EndpointProtectionConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8330a5bbce36d486d579a87b762d962a5fab2118
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140237"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="d8fd7-103">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="d8fd7-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d8fd7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8fd7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8fd7-106">新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8fd7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8fd7-107">Prerequisites</span></span>
<span data-ttu-id="d8fd7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8fd7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8fd7-110">Permission type</span></span>|<span data-ttu-id="d8fd7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8fd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8fd7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8fd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8fd7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8fd7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8fd7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8fd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8fd7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-115">Not supported.</span></span>|
|<span data-ttu-id="d8fd7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8fd7-116">Application</span></span>|<span data-ttu-id="d8fd7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8fd7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8fd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8fd7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8fd7-119">Request headers</span></span>
|<span data-ttu-id="d8fd7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8fd7-120">Header</span></span>|<span data-ttu-id="d8fd7-121">値</span><span class="sxs-lookup"><span data-stu-id="d8fd7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8fd7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8fd7-122">Authorization</span></span>|<span data-ttu-id="d8fd7-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8fd7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d8fd7-124">Accept</span></span>|<span data-ttu-id="d8fd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8fd7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8fd7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8fd7-126">Request body</span></span>
<span data-ttu-id="d8fd7-127">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="d8fd7-128">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="d8fd7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8fd7-129">Property</span></span>|<span data-ttu-id="d8fd7-130">型</span><span class="sxs-lookup"><span data-stu-id="d8fd7-130">Type</span></span>|<span data-ttu-id="d8fd7-131">説明</span><span class="sxs-lookup"><span data-stu-id="d8fd7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8fd7-132">id</span><span class="sxs-lookup"><span data-stu-id="d8fd7-132">id</span></span>|<span data-ttu-id="d8fd7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d8fd7-133">String</span></span>|<span data-ttu-id="d8fd7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-134">Key of the entity.</span></span> <span data-ttu-id="d8fd7-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8fd7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d8fd7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8fd7-137">DateTimeOffset</span></span>|<span data-ttu-id="d8fd7-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d8fd7-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8fd7-140">roleScopeTagIds</span></span>|<span data-ttu-id="d8fd7-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d8fd7-141">String collection</span></span>|<span data-ttu-id="d8fd7-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8fd7-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8fd7-144">supportsScopeTags</span></span>|<span data-ttu-id="d8fd7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-145">Boolean</span></span>|<span data-ttu-id="d8fd7-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8fd7-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8fd7-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8fd7-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-149">This property is read-only.</span></span> <span data-ttu-id="d8fd7-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8fd7-151">createdDateTime</span></span>|<span data-ttu-id="d8fd7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8fd7-152">DateTimeOffset</span></span>|<span data-ttu-id="d8fd7-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-153">DateTime the object was created.</span></span> <span data-ttu-id="d8fd7-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-155">説明</span><span class="sxs-lookup"><span data-stu-id="d8fd7-155">description</span></span>|<span data-ttu-id="d8fd7-156">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-156">String</span></span>|<span data-ttu-id="d8fd7-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8fd7-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d8fd7-159">displayName</span></span>|<span data-ttu-id="d8fd7-160">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-160">String</span></span>|<span data-ttu-id="d8fd7-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8fd7-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-163">version</span><span class="sxs-lookup"><span data-stu-id="d8fd7-163">version</span></span>|<span data-ttu-id="d8fd7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fd7-164">Int32</span></span>|<span data-ttu-id="d8fd7-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-165">Version of the device configuration.</span></span> <span data-ttu-id="d8fd7-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fd7-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="d8fd7-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="d8fd7-169">このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="d8fd7-170">これにより、dma リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="d8fd7-171">このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="d8fd7-172">カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="d8fd7-173">これは、製造時にシステムによってサポートされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="d8fd7-174">システムがカーネル dma 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「kernel dma 保護」フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="d8fd7-175">可能な値は `deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="d8fd7-176">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="d8fd7-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="d8fd7-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-178">このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="d8fd7-179">この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="d8fd7-180">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-181">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d8fd7-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="d8fd7-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-183">このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="d8fd7-184">State Allowed がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="d8fd7-185">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d8fd7-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="d8fd7-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-187">このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="d8fd7-188">ステートブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-188">State Block is supported.</span></span>|
|<span data-ttu-id="d8fd7-189">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8fd7-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="d8fd7-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-191">このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="d8fd7-192">そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="d8fd7-193">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-194">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="d8fd7-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="d8fd7-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-196">このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="d8fd7-197">NotConfigured、許可およびブロックされる状態のすべてがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="d8fd7-198">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="d8fd7-198">userRightsBackupData</span></span>|[<span data-ttu-id="d8fd7-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-200">このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="d8fd7-201">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-202">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="d8fd7-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="d8fd7-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-204">このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="d8fd7-205">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-206">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="d8fd7-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="d8fd7-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-208">このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="d8fd7-209">グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="d8fd7-210">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-211">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="d8fd7-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-213">このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="d8fd7-214">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-215">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="d8fd7-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="d8fd7-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-217">このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="d8fd7-218">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-219">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="d8fd7-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="d8fd7-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-221">このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="d8fd7-222">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-223">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="d8fd7-223">userRightsCreateToken</span></span>|[<span data-ttu-id="d8fd7-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-225">このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="d8fd7-226">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-227">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="d8fd7-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="d8fd7-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-229">このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="d8fd7-230">NotConfigured および許可されている状態のみがサポートされる</span><span class="sxs-lookup"><span data-stu-id="d8fd7-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d8fd7-231">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="d8fd7-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="d8fd7-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-233">このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="d8fd7-234">NotConfigured とブロックのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="d8fd7-235">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="d8fd7-235">userRightsDelegation</span></span>|[<span data-ttu-id="d8fd7-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-237">このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="d8fd7-238">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-239">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="d8fd7-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="d8fd7-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-241">このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="d8fd7-242">セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="d8fd7-243">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-244">user/シムの個人ユーザー</span><span class="sxs-lookup"><span data-stu-id="d8fd7-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="d8fd7-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-246">このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="d8fd7-247">この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="d8fd7-248">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-249">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="d8fd7-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="d8fd7-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-251">このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="d8fd7-252">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-253">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="d8fd7-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="d8fd7-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-255">このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="d8fd7-256">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-257">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="d8fd7-257">userRightsLockMemory</span></span>|[<span data-ttu-id="d8fd7-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-259">このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="d8fd7-260">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-261">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="d8fd7-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="d8fd7-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-263">このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="d8fd7-264">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-265">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="d8fd7-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="d8fd7-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-267">このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="d8fd7-268">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-269">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="d8fd7-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="d8fd7-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-271">このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="d8fd7-272">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-273">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="d8fd7-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="d8fd7-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-275">このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="d8fd7-276">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-277">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="d8fd7-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="d8fd7-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-279">このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="d8fd7-280">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-281">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="d8fd7-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="d8fd7-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-283">このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="d8fd7-284">このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="d8fd7-285">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-286">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="d8fd7-286">userRightsRestoreData</span></span>|[<span data-ttu-id="d8fd7-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-288">このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="d8fd7-289">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-290">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="d8fd7-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="d8fd7-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-292">このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="d8fd7-293">サポートされているのは、NotConfigured と許可の状態のみです。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d8fd7-294">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="d8fd7-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="d8fd7-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d8fd7-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d8fd7-296">このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="d8fd7-297">注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="d8fd7-298">サポートされている状態はブロックされます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="d8fd7-299">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="d8fd7-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="d8fd7-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-300">Boolean</span></span>|<span data-ttu-id="d8fd7-301">この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="d8fd7-302">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="d8fd7-303">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d8fd7-304">この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d8fd7-305">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-305">Default: Manual.</span></span> <span data-ttu-id="d8fd7-306">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d8fd7-307">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="d8fd7-308">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d8fd7-309">この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d8fd7-310">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-310">Default: Manual.</span></span> <span data-ttu-id="d8fd7-311">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d8fd7-312">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="d8fd7-313">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d8fd7-314">この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d8fd7-315">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-315">Default: Manual.</span></span> <span data-ttu-id="d8fd7-316">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d8fd7-317">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="d8fd7-318">servicestarttype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d8fd7-319">この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d8fd7-320">既定値: Manual。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-320">Default: Manual.</span></span> <span data-ttu-id="d8fd7-321">可能な値は `manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d8fd7-322">localsecurityoptionsenableadministratoraccount</span><span class="sxs-lookup"><span data-stu-id="d8fd7-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="d8fd7-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-323">Boolean</span></span>|<span data-ttu-id="d8fd7-324">ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="d8fd7-325">localsecurityoptionsblockremotelogonwithpassword</span><span class="sxs-lookup"><span data-stu-id="d8fd7-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="d8fd7-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-326">Boolean</span></span>|<span data-ttu-id="d8fd7-327">パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="d8fd7-328">localsecurityoptionsdisableアドミニストレーターアカウント</span><span class="sxs-lookup"><span data-stu-id="d8fd7-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="d8fd7-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-329">Boolean</span></span>|<span data-ttu-id="d8fd7-330">ローカル管理者アカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="d8fd7-331">localsecurityoptionsadministratoraccountname</span><span class="sxs-lookup"><span data-stu-id="d8fd7-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="d8fd7-332">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-332">String</span></span>|<span data-ttu-id="d8fd7-333">アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="d8fd7-334">localsecurityoptionsdisableguestaccount</span><span class="sxs-lookup"><span data-stu-id="d8fd7-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="d8fd7-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-335">Boolean</span></span>|<span data-ttu-id="d8fd7-336">ゲストアカウントを有効にするか無効にするかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="d8fd7-337">localsecurityoptionsguestaccountname</span><span class="sxs-lookup"><span data-stu-id="d8fd7-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="d8fd7-338">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-338">String</span></span>|<span data-ttu-id="d8fd7-339">アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="d8fd7-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="d8fd7-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="d8fd7-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-341">Boolean</span></span>|<span data-ttu-id="d8fd7-342">ログインせずに、ポータブルコンピューターをアンドックできないようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="d8fd7-343">localsecurityoptionsblockユーザーのドライバー</span><span class="sxs-lookup"><span data-stu-id="d8fd7-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="d8fd7-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-344">Boolean</span></span>|<span data-ttu-id="d8fd7-345">共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="d8fd7-346">localsecurityoptionsblockremoteop' aldrive access</span><span class="sxs-lookup"><span data-stu-id="d8fd7-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="d8fd7-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-347">Boolean</span></span>|<span data-ttu-id="d8fd7-348">この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="d8fd7-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="d8fd7-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="d8fd7-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="d8fd7-351">リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="d8fd7-352">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d8fd7-353">localsecurityoptionsmachineinactivitylimit</span><span class="sxs-lookup"><span data-stu-id="d8fd7-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="d8fd7-354">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fd7-354">Int32</span></span>|<span data-ttu-id="d8fd7-355">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d8fd7-356">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="d8fd7-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d8fd7-357">localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool</span><span class="sxs-lookup"><span data-stu-id="d8fd7-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="d8fd7-358">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fd7-358">Int32</span></span>|<span data-ttu-id="d8fd7-359">スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d8fd7-360">有効な値は 0 ~ 9999</span><span class="sxs-lookup"><span data-stu-id="d8fd7-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d8fd7-361">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="d8fd7-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="d8fd7-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-362">Boolean</span></span>|<span data-ttu-id="d8fd7-363">ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="d8fd7-364">localsecurityoption佐々木 delastsignedinuser</span><span class="sxs-lookup"><span data-stu-id="d8fd7-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="d8fd7-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-365">Boolean</span></span>|<span data-ttu-id="d8fd7-366">このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="d8fd7-367">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="d8fd7-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="d8fd7-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-368">Boolean</span></span>|<span data-ttu-id="d8fd7-369">資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="d8fd7-370">localsecurityoptionslogonmessagetitle</span><span class="sxs-lookup"><span data-stu-id="d8fd7-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="d8fd7-371">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-371">String</span></span>|<span data-ttu-id="d8fd7-372">ログインを試行するユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="d8fd7-373">localsecurityoptionslogonmessagetext</span><span class="sxs-lookup"><span data-stu-id="d8fd7-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="d8fd7-374">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-374">String</span></span>|<span data-ttu-id="d8fd7-375">ログインを試行するユーザーのメッセージテキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="d8fd7-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="d8fd7-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="d8fd7-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-377">Boolean</span></span>|<span data-ttu-id="d8fd7-378">オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="d8fd7-379">localsecurityoptionsinformationshownonlockscreen</span><span class="sxs-lookup"><span data-stu-id="d8fd7-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="d8fd7-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-380">Boolean</span></span>|<span data-ttu-id="d8fd7-381">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="d8fd7-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="d8fd7-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="d8fd7-383">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-383">String</span></span>|<span data-ttu-id="d8fd7-384">既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="d8fd7-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="d8fd7-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="d8fd7-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d8fd7-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d8fd7-387">このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d8fd7-388">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d8fd7-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="d8fd7-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="d8fd7-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d8fd7-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d8fd7-391">このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d8fd7-392">使用可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d8fd7-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d8fd7-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="d8fd7-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d8fd7-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="d8fd7-395">このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="d8fd7-396">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="d8fd7-397">lanmanagerwork ステーション disableinsecureguestログオン</span><span class="sxs-lookup"><span data-stu-id="d8fd7-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="d8fd7-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-398">Boolean</span></span>|<span data-ttu-id="d8fd7-399">有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="d8fd7-400">構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="d8fd7-401">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="d8fd7-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-402">Boolean</span></span>|<span data-ttu-id="d8fd7-403">このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="d8fd7-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="d8fd7-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="d8fd7-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-405">Boolean</span></span>|<span data-ttu-id="d8fd7-406">このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="d8fd7-407">localsecurityoptionsallowuiaccessapplicationelevation</span><span class="sxs-lookup"><span data-stu-id="d8fd7-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="d8fd7-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-408">Boolean</span></span>|<span data-ttu-id="d8fd7-409">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="d8fd7-410">localsecurityoptionsvirtualizefileandregistrywritefailurestoperuserlocations</span><span class="sxs-lookup"><span data-stu-id="d8fd7-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="d8fd7-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-411">Boolean</span></span>|<span data-ttu-id="d8fd7-412">ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する</span><span class="sxs-lookup"><span data-stu-id="d8fd7-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="d8fd7-413">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="d8fd7-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="d8fd7-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-414">Boolean</span></span>|<span data-ttu-id="d8fd7-415">指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="d8fd7-416">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d8fd7-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="d8fd7-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="d8fd7-418">管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="d8fd7-419">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="d8fd7-420">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d8fd7-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="d8fd7-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="d8fd7-422">標準ユーザーの昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="d8fd7-423">使用可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="d8fd7-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="d8fd7-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="d8fd7-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-425">Boolean</span></span>|<span data-ttu-id="d8fd7-426">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="d8fd7-427">管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="d8fd7-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="d8fd7-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="d8fd7-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-429">Boolean</span></span>|<span data-ttu-id="d8fd7-430">昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="d8fd7-431">localsecurityoptionsallowuiaccessapplicationsforsecurelocations</span><span class="sxs-lookup"><span data-stu-id="d8fd7-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="d8fd7-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-432">Boolean</span></span>|<span data-ttu-id="d8fd7-433">セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="d8fd7-434">localsecurityoptionsuseadminapprovalmode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="d8fd7-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-435">Boolean</span></span>|<span data-ttu-id="d8fd7-436">組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="d8fd7-437">localsecurityoptionsuseadminapprovalmodeforadministrators</span><span class="sxs-lookup"><span data-stu-id="d8fd7-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="d8fd7-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-438">Boolean</span></span>|<span data-ttu-id="d8fd7-439">管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="d8fd7-440">localsecurityoptionsinformationshownonlockscreen ロックアウト</span><span class="sxs-lookup"><span data-stu-id="d8fd7-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="d8fd7-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="d8fd7-442">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d8fd7-443">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d8fd7-444">使用可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="d8fd7-445">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d8fd7-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="d8fd7-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="d8fd7-447">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d8fd7-448">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d8fd7-449">使用可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d8fd7-450">localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers</span><span class="sxs-lookup"><span data-stu-id="d8fd7-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="d8fd7-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-451">Boolean</span></span>|<span data-ttu-id="d8fd7-452">このセキュリティ設定は、smb クライアントが smb パケット署名のネゴシエートを試行するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="d8fd7-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d8fd7-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d8fd7-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-454">Boolean</span></span>|<span data-ttu-id="d8fd7-455">このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="d8fd7-456">localsecurityoptionsdisableserverdigitallysigncommunicationsalways</span><span class="sxs-lookup"><span data-stu-id="d8fd7-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="d8fd7-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-457">Boolean</span></span>|<span data-ttu-id="d8fd7-458">このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="d8fd7-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d8fd7-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d8fd7-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-460">Boolean</span></span>|<span data-ttu-id="d8fd7-461">このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="d8fd7-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="d8fd7-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="d8fd7-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-463">Boolean</span></span>|<span data-ttu-id="d8fd7-464">このセキュリティ設定は、smb サーバーが smb パケットの署名を要求するクライアントとの間で smb パケットの署名をネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="d8fd7-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="d8fd7-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="d8fd7-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-466">Boolean</span></span>|<span data-ttu-id="d8fd7-467">既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="d8fd7-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="d8fd7-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="d8fd7-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-469">Boolean</span></span>|<span data-ttu-id="d8fd7-470">このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="d8fd7-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="d8fd7-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="d8fd7-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-472">Boolean</span></span>|<span data-ttu-id="d8fd7-473">このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="d8fd7-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="d8fd7-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="d8fd7-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-475">Boolean</span></span>|<span data-ttu-id="d8fd7-476">このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="d8fd7-477">既定では保存されません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="d8fd7-478">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="d8fd7-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="d8fd7-479">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-479">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="d8fd7-480">このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="d8fd7-481">使用可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="d8fd7-482">defendersecuritycenterdisablehealthui</span><span class="sxs-lookup"><span data-stu-id="d8fd7-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="d8fd7-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-483">Boolean</span></span>|<span data-ttu-id="d8fd7-484">アプリとブラウザーの保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="d8fd7-485">defendersecuritycenterdisablenetworkui</span><span class="sxs-lookup"><span data-stu-id="d8fd7-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="d8fd7-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-486">Boolean</span></span>|<span data-ttu-id="d8fd7-487">[ファミリオプション] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="d8fd7-488">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="d8fd7-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-489">Boolean</span></span>|<span data-ttu-id="d8fd7-490">[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="d8fd7-491">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="d8fd7-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-492">Boolean</span></span>|<span data-ttu-id="d8fd7-493">ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="d8fd7-494">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="d8fd7-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-495">Boolean</span></span>|<span data-ttu-id="d8fd7-496">ウイルスおよび脅威保護領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="d8fd7-497">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="d8fd7-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-498">Boolean</span></span>|<span data-ttu-id="d8fd7-499">[アカウントの保護] 領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="d8fd7-500">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-500">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="d8fd7-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-501">Boolean</span></span>|<span data-ttu-id="d8fd7-502">[TPM のクリア] ボタンの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-502">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="d8fd7-503">defendersecurityセンター disableハードウェア ui</span><span class="sxs-lookup"><span data-stu-id="d8fd7-503">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="d8fd7-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-504">Boolean</span></span>|<span data-ttu-id="d8fd7-505">[ハードウェア保護] 領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-505">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="d8fd7-506">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-506">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="d8fd7-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-507">Boolean</span></span>|<span data-ttu-id="d8fd7-508">通知領域コントロールの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-508">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="d8fd7-509">この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-509">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="d8fd7-510">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-510">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="d8fd7-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-511">Boolean</span></span>|<span data-ttu-id="d8fd7-512">ランサムウェア対策領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-512">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="d8fd7-513">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-513">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="d8fd7-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-514">Boolean</span></span>|<span data-ttu-id="d8fd7-515">デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-515">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="d8fd7-516">defendersecurityセンター disableトラブルシューティング ui</span><span class="sxs-lookup"><span data-stu-id="d8fd7-516">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="d8fd7-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-517">Boolean</span></span>|<span data-ttu-id="d8fd7-518">[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-518">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="d8fd7-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="d8fd7-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="d8fd7-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-520">Boolean</span></span>|<span data-ttu-id="d8fd7-521">脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-521">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="d8fd7-522">defendersecurityセンター組織 displayname</span><span class="sxs-lookup"><span data-stu-id="d8fd7-522">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="d8fd7-523">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-523">String</span></span>|<span data-ttu-id="d8fd7-524">ユーザーに表示される会社名。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-524">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="d8fd7-525">defendersecurityセンター helpemail</span><span class="sxs-lookup"><span data-stu-id="d8fd7-525">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="d8fd7-526">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-526">String</span></span>|<span data-ttu-id="d8fd7-527">ユーザーに表示される電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-527">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="d8fd7-528">defendersecurityセンター helpphone</span><span class="sxs-lookup"><span data-stu-id="d8fd7-528">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="d8fd7-529">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-529">String</span></span>|<span data-ttu-id="d8fd7-530">ユーザーに表示される電話番号または Skype ID。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-530">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="d8fd7-531">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="d8fd7-531">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="d8fd7-532">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-532">String</span></span>|<span data-ttu-id="d8fd7-533">ヘルプポータルの URL これは、ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-533">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="d8fd7-534">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="d8fd7-534">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="d8fd7-535">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-535">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="d8fd7-536">アプリの表示領域から表示する通知。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-536">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="d8fd7-537">可能な値は `notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-537">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="d8fd7-538">defendersecurityセンター itcontactdisplay</span><span class="sxs-lookup"><span data-stu-id="d8fd7-538">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="d8fd7-539">defendersecurityセンター itcontactdisplaytype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-539">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="d8fd7-540">エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-540">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="d8fd7-541">使用可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-541">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="d8fd7-542">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d8fd7-542">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d8fd7-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-543">Boolean</span></span>|<span data-ttu-id="d8fd7-544">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="d8fd7-544">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d8fd7-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d8fd7-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d8fd7-546">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fd7-546">Int32</span></span>|<span data-ttu-id="d8fd7-547">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-547">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d8fd7-548">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-548">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d8fd7-549">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="d8fd7-549">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d8fd7-550">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d8fd7-550">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d8fd7-551">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-551">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d8fd7-552">使用する事前共有キーのエンコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-552">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="d8fd7-553">可能な値は `deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-553">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d8fd7-554">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d8fd7-554">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d8fd7-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-555">Boolean</span></span>|<span data-ttu-id="d8fd7-556">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-556">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d8fd7-557">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d8fd7-557">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d8fd7-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-558">Boolean</span></span>|<span data-ttu-id="d8fd7-559">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-559">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d8fd7-560">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d8fd7-560">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d8fd7-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-561">Boolean</span></span>|<span data-ttu-id="d8fd7-562">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-562">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d8fd7-563">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d8fd7-563">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d8fd7-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-564">Boolean</span></span>|<span data-ttu-id="d8fd7-565">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-565">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d8fd7-566">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d8fd7-566">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d8fd7-567">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-567">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d8fd7-568">証明書失効リストの適用方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-568">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="d8fd7-569">使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-569">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d8fd7-570">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d8fd7-570">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d8fd7-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-571">Boolean</span></span>|<span data-ttu-id="d8fd7-572">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-572">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d8fd7-573">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d8fd7-573">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d8fd7-574">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-574">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d8fd7-575">トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-575">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="d8fd7-576">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-576">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d8fd7-577">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d8fd7-577">firewallProfileDomain</span></span>|[<span data-ttu-id="d8fd7-578">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-578">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d8fd7-579">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-579">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d8fd7-580">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d8fd7-580">firewallProfilePublic</span></span>|[<span data-ttu-id="d8fd7-581">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-581">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d8fd7-582">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-582">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d8fd7-583">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d8fd7-583">firewallProfilePrivate</span></span>|[<span data-ttu-id="d8fd7-584">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-584">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d8fd7-585">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-585">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d8fd7-586">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d8fd7-586">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="d8fd7-587">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-587">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-588">子プロセスの作成による Adobe Reader の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-588">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="d8fd7-589">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-589">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-590">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d8fd7-590">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d8fd7-591">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d8fd7-591">String collection</span></span>|<span data-ttu-id="d8fd7-592">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="d8fd7-592">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d8fd7-593">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-593">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="d8fd7-594">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-594">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-595">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-595">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="d8fd7-596">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-596">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-597">defenderofficeappsexecutablecontentcreationorlaunch</span><span class="sxs-lookup"><span data-stu-id="d8fd7-597">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="d8fd7-598">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-598">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-599">他のプロセスに挿入される Office アプリケーションの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-599">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="d8fd7-600">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-600">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-601">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d8fd7-601">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d8fd7-602">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-603">子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-603">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="d8fd7-604">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="d8fd7-606">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-606">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-607">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-607">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d8fd7-608">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-608">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-609">defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="d8fd7-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="d8fd7-610">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-611">Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d8fd7-612">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-613">defenderofficeappslaunchchildprocesstype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-613">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="d8fd7-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-615">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-615">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d8fd7-616">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-617">defenderofficeappslaunchchildprocess</span><span class="sxs-lookup"><span data-stu-id="d8fd7-617">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d8fd7-618">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-619">Office アプリケーションの開始子プロセスの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d8fd7-620">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-621">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-621">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="d8fd7-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-623">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-623">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d8fd7-624">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-625">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="d8fd7-625">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="d8fd7-626">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-627">Office のマクロコードからの Win32 インポートの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d8fd7-628">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-629">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-629">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="d8fd7-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-631">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-631">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d8fd7-632">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-633">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="d8fd7-633">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="d8fd7-634">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-635">難読化された js/vbs/ps/マクロコードの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d8fd7-636">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-637">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-637">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="d8fd7-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-639">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-639">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d8fd7-640">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-641">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="d8fd7-641">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="d8fd7-642">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-643">インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d8fd7-644">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-645">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-645">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="d8fd7-646">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-647">Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-647">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="d8fd7-648">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-649">defenderprocessの種類</span><span class="sxs-lookup"><span data-stu-id="d8fd7-649">defenderProcessCreationType</span></span>|[<span data-ttu-id="d8fd7-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-651">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-651">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d8fd7-652">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-653">defenderprocesscreation</span><span class="sxs-lookup"><span data-stu-id="d8fd7-653">defenderProcessCreation</span></span>|[<span data-ttu-id="d8fd7-654">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-655">PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d8fd7-656">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-657">defenderアン trustedusbprocesstype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-657">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="d8fd7-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-659">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-659">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d8fd7-660">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-661">defenderアン trustedusbプロセス</span><span class="sxs-lookup"><span data-stu-id="d8fd7-661">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="d8fd7-662">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-663">USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d8fd7-664">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-665">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-665">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="d8fd7-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-667">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-667">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d8fd7-668">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-669">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="d8fd7-669">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="d8fd7-670">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-671">流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d8fd7-672">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-673">defenderemailcontentexecutiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-673">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="d8fd7-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d8fd7-675">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-675">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d8fd7-676">可能な値は `userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-677">defenderemailcontentexecution</span><span class="sxs-lookup"><span data-stu-id="d8fd7-677">defenderEmailContentExecution</span></span>|[<span data-ttu-id="d8fd7-678">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-679">実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d8fd7-680">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-681">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-681">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="d8fd7-682">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-683">ranware に対して高度な保護を使用することを示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-683">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="d8fd7-684">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-685">defendergu/myfolderstype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-685">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="d8fd7-686">folderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-686">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="d8fd7-687">保護されたフォルダーの動作を示す値。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-687">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="d8fd7-688">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-688">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="d8fd7-689">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d8fd7-689">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d8fd7-690">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d8fd7-690">String collection</span></span>|<span data-ttu-id="d8fd7-691">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="d8fd7-691">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d8fd7-692">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d8fd7-692">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d8fd7-693">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d8fd7-693">String collection</span></span>|<span data-ttu-id="d8fd7-694">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="d8fd7-694">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d8fd7-695">defendernetworkprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-695">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="d8fd7-696">defenderprotectiontype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-696">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d8fd7-697">networkprotection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-697">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="d8fd7-698">可能な値は `userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-698">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d8fd7-699">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d8fd7-699">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d8fd7-700">Binary</span><span class="sxs-lookup"><span data-stu-id="d8fd7-700">Binary</span></span>|<span data-ttu-id="d8fd7-701">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-701">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d8fd7-702">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d8fd7-702">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d8fd7-703">String</span><span class="sxs-lookup"><span data-stu-id="d8fd7-703">String</span></span>|<span data-ttu-id="d8fd7-704">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-704">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d8fd7-705">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d8fd7-705">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d8fd7-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-706">Boolean</span></span>|<span data-ttu-id="d8fd7-707">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-707">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d8fd7-708">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d8fd7-708">appLockerApplicationControl</span></span>|[<span data-ttu-id="d8fd7-709">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-709">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="d8fd7-710">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-710">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="d8fd7-711">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-711">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d8fd7-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="d8fd7-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="d8fd7-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="d8fd7-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="d8fd7-714">セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-714">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="d8fd7-715">可能な値は `notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-715">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="d8fd7-716">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="d8fd7-716">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="d8fd7-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-717">Boolean</span></span>|<span data-ttu-id="d8fd7-718">仮想化ベースのセキュリティ (VBS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-718">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="d8fd7-719">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="d8fd7-719">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="d8fd7-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-720">Boolean</span></span>|<span data-ttu-id="d8fd7-721">次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-721">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="d8fd7-722">devicegu//systemguard</span><span class="sxs-lookup"><span data-stu-id="d8fd7-722">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="d8fd7-723">購入</span><span class="sxs-lookup"><span data-stu-id="d8fd7-723">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d8fd7-724">IT 管理者がシステムガードの起動を構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-724">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="d8fd7-725">可能な値は `notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-725">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d8fd7-726">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d8fd7-726">smartScreenEnableInShell</span></span>|<span data-ttu-id="d8fd7-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-727">Boolean</span></span>|<span data-ttu-id="d8fd7-728">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-728">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d8fd7-729">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d8fd7-729">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d8fd7-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-730">Boolean</span></span>|<span data-ttu-id="d8fd7-731">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-731">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d8fd7-732">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d8fd7-732">applicationGuardEnabled</span></span>|<span data-ttu-id="d8fd7-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-733">Boolean</span></span>|<span data-ttu-id="d8fd7-734">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="d8fd7-734">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d8fd7-735">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d8fd7-735">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="d8fd7-736">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d8fd7-736">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="d8fd7-737">新しい windows ビルドに対して windows Defender Application Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-737">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="d8fd7-738">使用可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-738">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="d8fd7-739">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d8fd7-739">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d8fd7-740">applicationgu/blockfiletransfertype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-740">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="d8fd7-741">画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-741">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="d8fd7-742">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-742">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d8fd7-743">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d8fd7-743">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d8fd7-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-744">Boolean</span></span>|<span data-ttu-id="d8fd7-745">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="d8fd7-745">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d8fd7-746">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d8fd7-746">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d8fd7-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-747">Boolean</span></span>|<span data-ttu-id="d8fd7-748">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-748">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d8fd7-749">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d8fd7-749">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d8fd7-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-750">Boolean</span></span>|<span data-ttu-id="d8fd7-751">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="d8fd7-751">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d8fd7-752">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d8fd7-752">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d8fd7-753">applicationgu/blockクリップボード sharingtype</span><span class="sxs-lookup"><span data-stu-id="d8fd7-753">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d8fd7-754">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-754">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="d8fd7-755">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-755">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d8fd7-756">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d8fd7-756">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d8fd7-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-757">Boolean</span></span>|<span data-ttu-id="d8fd7-758">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-758">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d8fd7-759">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d8fd7-759">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d8fd7-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-760">Boolean</span></span>|<span data-ttu-id="d8fd7-761">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-761">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d8fd7-762">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d8fd7-762">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d8fd7-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-763">Boolean</span></span>|<span data-ttu-id="d8fd7-764">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-764">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d8fd7-765">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d8fd7-765">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d8fd7-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-766">Boolean</span></span>|<span data-ttu-id="d8fd7-767">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="d8fd7-767">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d8fd7-768">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="d8fd7-768">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="d8fd7-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-769">Boolean</span></span>|<span data-ttu-id="d8fd7-770">application guard が仮想 GPU を使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="d8fd7-770">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="d8fd7-771">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="d8fd7-771">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="d8fd7-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-772">Boolean</span></span>|<span data-ttu-id="d8fd7-773">アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する</span><span class="sxs-lookup"><span data-stu-id="d8fd7-773">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="d8fd7-774">bitlockerallowstandarduserencryption</span><span class="sxs-lookup"><span data-stu-id="d8fd7-774">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="d8fd7-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-775">Boolean</span></span>|<span data-ttu-id="d8fd7-776">管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-776">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="d8fd7-777">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d8fd7-777">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d8fd7-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-778">Boolean</span></span>|<span data-ttu-id="d8fd7-779">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-779">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d8fd7-780">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d8fd7-780">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d8fd7-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-781">Boolean</span></span>|<span data-ttu-id="d8fd7-782">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-782">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d8fd7-783">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="d8fd7-783">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d8fd7-784">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d8fd7-784">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d8fd7-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fd7-785">Boolean</span></span>|<span data-ttu-id="d8fd7-786">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d8fd7-787">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-787">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="d8fd7-788">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-788">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="d8fd7-789">BitLocker システムドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-789">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="d8fd7-790">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-790">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="d8fd7-791">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-791">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="d8fd7-792">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-792">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="d8fd7-793">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-793">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d8fd7-794">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d8fd7-794">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d8fd7-795">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-795">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d8fd7-796">応答</span><span class="sxs-lookup"><span data-stu-id="d8fd7-796">Response</span></span>
<span data-ttu-id="d8fd7-797">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-797">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8fd7-798">例</span><span class="sxs-lookup"><span data-stu-id="d8fd7-798">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8fd7-799">要求</span><span class="sxs-lookup"><span data-stu-id="d8fd7-799">Request</span></span>
<span data-ttu-id="d8fd7-800">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-800">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d8fd7-801">応答</span><span class="sxs-lookup"><span data-stu-id="d8fd7-801">Response</span></span>
<span data-ttu-id="d8fd7-p198">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8fd7-p198">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




