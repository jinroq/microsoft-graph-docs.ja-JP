---
title: windows10EndpointProtectionConfiguration の更新
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bb398da325f6895eee7dd5e53938f8dafc5d5f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393621"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="b05ea-103">windows10EndpointProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="b05ea-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="b05ea-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b05ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b05ea-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b05ea-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b05ea-107">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b05ea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b05ea-108">Prerequisites</span></span>
<span data-ttu-id="b05ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b05ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b05ea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b05ea-111">Permission type</span></span>|<span data-ttu-id="b05ea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b05ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b05ea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b05ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b05ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b05ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b05ea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b05ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b05ea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-116">Not supported.</span></span>|
|<span data-ttu-id="b05ea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b05ea-117">Application</span></span>|<span data-ttu-id="b05ea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b05ea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b05ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b05ea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b05ea-120">Request headers</span></span>
|<span data-ttu-id="b05ea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b05ea-121">Header</span></span>|<span data-ttu-id="b05ea-122">値</span><span class="sxs-lookup"><span data-stu-id="b05ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b05ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b05ea-123">Authorization</span></span>|<span data-ttu-id="b05ea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b05ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b05ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b05ea-125">Accept</span></span>|<span data-ttu-id="b05ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b05ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b05ea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b05ea-127">Request body</span></span>
<span data-ttu-id="b05ea-128">要求本文で、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="b05ea-129">次の表に、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="b05ea-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b05ea-130">Property</span></span>|<span data-ttu-id="b05ea-131">型</span><span class="sxs-lookup"><span data-stu-id="b05ea-131">Type</span></span>|<span data-ttu-id="b05ea-132">説明</span><span class="sxs-lookup"><span data-stu-id="b05ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b05ea-133">id</span><span class="sxs-lookup"><span data-stu-id="b05ea-133">id</span></span>|<span data-ttu-id="b05ea-134">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-134">String</span></span>|<span data-ttu-id="b05ea-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b05ea-135">Key of the entity.</span></span> <span data-ttu-id="b05ea-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b05ea-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b05ea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b05ea-138">DateTimeOffset</span></span>|<span data-ttu-id="b05ea-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b05ea-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b05ea-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b05ea-141">roleScopeTagIds</span></span>|<span data-ttu-id="b05ea-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b05ea-142">String collection</span></span>|<span data-ttu-id="b05ea-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b05ea-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b05ea-145">supportsScopeTags</span></span>|<span data-ttu-id="b05ea-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-146">Boolean</span></span>|<span data-ttu-id="b05ea-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b05ea-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b05ea-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b05ea-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-150">This property is read-only.</span></span> <span data-ttu-id="b05ea-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b05ea-152">createdDateTime</span></span>|<span data-ttu-id="b05ea-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b05ea-153">DateTimeOffset</span></span>|<span data-ttu-id="b05ea-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b05ea-154">DateTime the object was created.</span></span> <span data-ttu-id="b05ea-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-156">説明</span><span class="sxs-lookup"><span data-stu-id="b05ea-156">description</span></span>|<span data-ttu-id="b05ea-157">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-157">String</span></span>|<span data-ttu-id="b05ea-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="b05ea-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b05ea-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b05ea-160">displayName</span></span>|<span data-ttu-id="b05ea-161">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-161">String</span></span>|<span data-ttu-id="b05ea-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="b05ea-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b05ea-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-164">version</span><span class="sxs-lookup"><span data-stu-id="b05ea-164">version</span></span>|<span data-ttu-id="b05ea-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b05ea-165">Int32</span></span>|<span data-ttu-id="b05ea-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b05ea-166">Version of the device configuration.</span></span> <span data-ttu-id="b05ea-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b05ea-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b05ea-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="b05ea-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="b05ea-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="b05ea-170">このポリシーは、外部の DMA 機能を持つデバイスに対して追加のセキュリティを提供します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="b05ea-171">これにより外部の DMA 対応デバイスの列挙体をより細かく制御互換性のないデバイスと DMA Remapping メモリの分離レベルとサンド ボックス化できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="b05ea-172">このポリシーは、カーネルの DMA の保護がサポートされていて、システムのファームウェアで有効になっている場合にのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="b05ea-173">カーネル DMA の保護は、ポリシーを使用して、またはエンド ・ ユーザーが制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="b05ea-174">製造時にシステムでサポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b05ea-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="b05ea-175">システムがカーネルの DMA の保護をサポートしているかを確認するには、MSINFO32.exe の概要] ページでカーネルの DMA 保護フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b05ea-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="b05ea-176">可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="b05ea-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="b05ea-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="b05ea-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-179">このユーザー権利のバックアップ/リストアの実行中に資格情報マネージャーで表示されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="b05ea-180">他のエンティティにこの特権が与えられた場合、ユーザーの保存された資格情報が危険にさらされる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b05ea-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="b05ea-181">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="b05ea-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="b05ea-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-184">このユーザー権利は、どのユーザーを決定し、グループがネットワーク経由でコンピューターに接続できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="b05ea-185">許可の状態がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="b05ea-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="b05ea-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="b05ea-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-188">このユーザー権利は、どのユーザーとグループは、ネットワーク経由でコンピューターへの接続からのブロックを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="b05ea-189">ステート ブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-189">State Block is supported.</span></span>|
|<span data-ttu-id="b05ea-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b05ea-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="b05ea-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-192">このユーザー権利では、認証なしのすべてのユーザーを偽装するプロセスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="b05ea-193">プロセスをユーザーと同じローカル リソースへのアクセスを得ることができます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="b05ea-194">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="b05ea-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="b05ea-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-197">このユーザー権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="b05ea-198">状態 NotConfigured、許可とブロックのすべてをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="b05ea-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="b05ea-199">userRightsBackupData</span></span>|[<span data-ttu-id="b05ea-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-201">このユーザー権利では、回避できるユーザー ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのアクセス許可ファイルとディレクトリをバックアップするときを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="b05ea-202">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="b05ea-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="b05ea-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-205">このユーザー権利は、どのユーザーとグループは、コンピューターの内部時計の日付と時刻を変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="b05ea-206">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="b05ea-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="b05ea-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-209">このセキュリティ設定は、ユーザーがすべてのセッションに使用可能なグローバル オブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="b05ea-210">グローバル オブジェクトを作成できるユーザーに影響を与える他のユーザーのセッションは、アプリケーションの障害やデータの破損につながる可能性の下で実行するプロセスです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="b05ea-211">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="b05ea-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="b05ea-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-214">このユーザー権利は、どのユーザーおよびグループを作成し、ページファイルのサイズを変更する内部 API を呼び出すことができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="b05ea-215">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="b05ea-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="b05ea-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-218">このユーザー権利では、マネージャー オブジェクトを使用してディレクトリ オブジェクトを作成するプロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="b05ea-219">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="b05ea-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="b05ea-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-222">このユーザー権利は、ユーザーが、ログオンしているコンピューターからシンボリック リンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="b05ea-223">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="b05ea-224">userRightsCreateToken</span></span>|[<span data-ttu-id="b05ea-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-226">このユーザー権利では、プロセスでは、内部の API を使用して、アクセス トークンを作成するときに、ローカル リソースへのアクセスを取得するために使用するトークンを作成するプロセスにするユーザーまたはグループを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="b05ea-227">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="b05ea-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="b05ea-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-230">このユーザー権利は、ユーザーが任意のプロセスまたはカーネルにデバッガーをアタッチできるを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="b05ea-231">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b05ea-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="b05ea-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="b05ea-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-234">このユーザー権利では、リモート デスクトップ サービス クライアントとしてログオン拒否するユーザーとグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="b05ea-235">NotConfigured および受信拒否の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="b05ea-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="b05ea-236">userRightsDelegation</span></span>|[<span data-ttu-id="b05ea-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-238">このユーザー権利は、ユーザーまたはコンピューター オブジェクトの委任に対して信頼されるように設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="b05ea-239">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="b05ea-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="b05ea-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-242">このユーザー権利では、セキュリティ ログにエントリを追加するのにはプロセスが使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="b05ea-243">セキュリティ ログは、承認されていないシステムへのアクセスを追跡に使用します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="b05ea-244">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="b05ea-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="b05ea-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-247">ユーザーには、このユーザー権利を割り当てるには、クライアントを偽装するには、そのユーザーに代わって実行されるプログラムすることができます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="b05ea-248">により承認されていないユーザーが自分が作成したサービスに接続するクライアントを納得させることと、偽装して、クライアントに許可されていないユーザーのアクセス許可を昇格させるという、この種の偽装にこのユーザー権利を必要とします。管理者レベルまたはシステム レベル。</span><span class="sxs-lookup"><span data-stu-id="b05ea-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="b05ea-249">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="b05ea-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="b05ea-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-252">このユーザー権利は、取引先企業は他のプロセスに割り当てられている実行の優先順位を上げる別のプロセスに対するプロパティの書き込みアクセスを持つプロセスを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="b05ea-253">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="b05ea-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="b05ea-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-256">このユーザー権利は、ユーザーが動的にロードおよびデバイス ドライバーやカーネル モードでは、他のコードをアンロードするを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="b05ea-257">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="b05ea-258">userRightsLockMemory</span></span>|[<span data-ttu-id="b05ea-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-260">このユーザー権利では、ディスク上の仮想メモリを物理メモリにデータを保持するプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="b05ea-261">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="b05ea-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="b05ea-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-264">このユーザー権利は、オブジェクト アクセスの監査ファイル、Active Directory オブジェクト、レジストリ キーなどの個々 のリソースのオプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="b05ea-265">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="b05ea-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="b05ea-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-268">このユーザー権利では、リモート最適化などのボリュームの保守タスクを実行できるユーザーおよびグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="b05ea-269">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="b05ea-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="b05ea-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-272">このユーザー権利では、ファームウェアの環境値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="b05ea-273">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="b05ea-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="b05ea-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-276">このユーザー権利は、ユーザー アカウントは、ファイル、レジストリ キー、またはその他のユーザーが所有するプロセスなどのオブジェクトの整合性ラベルを変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="b05ea-277">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="b05ea-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="b05ea-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-280">このユーザー権利では、システム プロセスのパフォーマンスを監視するパフォーマンス監視ツールを使用できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="b05ea-281">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="b05ea-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="b05ea-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-284">このユーザー権利は、ネットワーク上のリモートの場所からコンピューターをシャット ダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="b05ea-285">このユーザー権利が誤用されると、サービス拒否攻撃があります。</span><span class="sxs-lookup"><span data-stu-id="b05ea-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="b05ea-286">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="b05ea-287">userRightsRestoreData</span></span>|[<span data-ttu-id="b05ea-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-289">このユーザー権利では、ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのファイルおよびディレクトリをバックアップ、復元するときのアクセス許可を回避できるユーザーを決定し、オブジェクトの所有者として有効なセキュリティ プリンシパルを設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="b05ea-290">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="b05ea-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="b05ea-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-293">所有権をユーザーのセキュリティ保護可能なオブジェクトの Active Directory オブジェクト、ファイル、フォルダー、プリンター、レジストリ キー、プロセス、およびスレッドを含め、システムでこのユーザー権利を決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="b05ea-294">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b05ea-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="b05ea-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="b05ea-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b05ea-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b05ea-297">このセキュリティ設定は、サービスとしてプロセスを登録できないサービス アカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="b05ea-298">注: このセキュリティ設定は、システム、ローカル サービス、またはネットワーク サービス アカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="b05ea-299">ブロックがサポートされているだけの状態です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="b05ea-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="b05ea-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="b05ea-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-301">Boolean</span></span>|<span data-ttu-id="b05ea-302">この設定は、xbox ゲームの保存が有効 (1) または無効 (0) かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="b05ea-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b05ea-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="b05ea-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b05ea-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b05ea-305">この設定は、付属品の管理サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b05ea-306">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-306">Default: Manual.</span></span> <span data-ttu-id="b05ea-307">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b05ea-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b05ea-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="b05ea-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b05ea-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b05ea-310">この設定は、認証マネージャーの Live サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b05ea-311">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-311">Default: Manual.</span></span> <span data-ttu-id="b05ea-312">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b05ea-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b05ea-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="b05ea-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b05ea-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b05ea-315">保存サービスの開始のタイプのゲームのライブは Automatic(2)、Manual(3)、Disabled(4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b05ea-316">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-316">Default: Manual.</span></span> <span data-ttu-id="b05ea-317">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b05ea-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b05ea-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="b05ea-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b05ea-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b05ea-320">この設定は、ネットワーク サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b05ea-321">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-321">Default: Manual.</span></span> <span data-ttu-id="b05ea-322">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b05ea-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="b05ea-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="b05ea-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-324">Boolean</span></span>|<span data-ttu-id="b05ea-325">ユーザーがこのコンピューターに Microsoft の新しいアカウントを追加するを防ぐ。</span><span class="sxs-lookup"><span data-stu-id="b05ea-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="b05ea-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="b05ea-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="b05ea-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-327">Boolean</span></span>|<span data-ttu-id="b05ea-328">物理デバイス以外の場所からのログオンにパスワードで保護していないローカルのアカウントを有効にします。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="b05ea-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="b05ea-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="b05ea-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-330">Boolean</span></span>|<span data-ttu-id="b05ea-331">ローカル管理者アカウントを有効または無効にするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="b05ea-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="b05ea-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="b05ea-333">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-333">String</span></span>|<span data-ttu-id="b05ea-334">"Administrator"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="b05ea-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="b05ea-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="b05ea-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-336">Boolean</span></span>|<span data-ttu-id="b05ea-337">Guest アカウントが有効か無効になっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="b05ea-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="b05ea-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="b05ea-339">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-339">String</span></span>|<span data-ttu-id="b05ea-340">"Guest"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="b05ea-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="b05ea-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="b05ea-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-342">Boolean</span></span>|<span data-ttu-id="b05ea-343">ポータブル コンピューターを防ぐため、ログインしなくても接続されているからです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="b05ea-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="b05ea-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="b05ea-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-345">Boolean</span></span>|<span data-ttu-id="b05ea-346">管理者だけが使用する共有プリンターへの接続の一部としてプリンター ドライバーをインストールを制限します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="b05ea-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="b05ea-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="b05ea-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-348">Boolean</span></span>|<span data-ttu-id="b05ea-349">CD-ROM メディアにアクセスする唯一の対話形式でログオンしているユーザーは、この設定を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="b05ea-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="b05ea-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="b05ea-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="b05ea-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="b05ea-352">リムーバブル NTFS メディアを取り出すことができるユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="b05ea-353">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="b05ea-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="b05ea-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="b05ea-355">Int32</span><span class="sxs-lookup"><span data-stu-id="b05ea-355">Int32</span></span>|<span data-ttu-id="b05ea-356">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="b05ea-357">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="b05ea-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="b05ea-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="b05ea-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="b05ea-359">Int32</span><span class="sxs-lookup"><span data-stu-id="b05ea-359">Int32</span></span>|<span data-ttu-id="b05ea-360">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="b05ea-361">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="b05ea-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="b05ea-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="b05ea-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="b05ea-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-363">Boolean</span></span>|<span data-ttu-id="b05ea-364">CTRL + ALT + DEL を押す前に、ユーザーがログオンできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b05ea-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="b05ea-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="b05ea-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="b05ea-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-366">Boolean</span></span>|<span data-ttu-id="b05ea-367">このデバイス上で最後署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="b05ea-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="b05ea-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="b05ea-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-369">Boolean</span></span>|<span data-ttu-id="b05ea-370">資格情報を入力した後、デバイスのデスクトップが表示される前にこのデバイスに署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="b05ea-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="b05ea-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="b05ea-372">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-372">String</span></span>|<span data-ttu-id="b05ea-373">ログオン ユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="b05ea-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="b05ea-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="b05ea-375">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-375">String</span></span>|<span data-ttu-id="b05ea-376">ログオン ユーザーのメッセージ テキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="b05ea-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="b05ea-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="b05ea-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-378">Boolean</span></span>|<span data-ttu-id="b05ea-379">ブロック PKU2U 認証要求をこのデバイスにオンライン id を使用します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="b05ea-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="b05ea-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="b05ea-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-381">Boolean</span></span>|<span data-ttu-id="b05ea-382">UI ヘルパー LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティのブール値</span><span class="sxs-lookup"><span data-stu-id="b05ea-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="b05ea-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="b05ea-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="b05ea-384">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-384">String</span></span>|<span data-ttu-id="b05ea-385">または、SAM にリモート呼び出しを行うには、ユーザーとグループを拒否する既定のセキュリティ記述子定義言語の文字列を編集します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="b05ea-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="b05ea-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="b05ea-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b05ea-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="b05ea-388">このセキュリティ設定では、クライアントが 128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とすることができます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="b05ea-389">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="b05ea-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="b05ea-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="b05ea-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b05ea-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="b05ea-392">このセキュリティ設定は、128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とするサーバーです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="b05ea-393">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="b05ea-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="b05ea-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="b05ea-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="b05ea-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="b05ea-396">このセキュリティ設定は、ネットワーク ログオン時に使用するチャレンジ/レスポンス認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="b05ea-397">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="b05ea-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="b05ea-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="b05ea-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="b05ea-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-399">Boolean</span></span>|<span data-ttu-id="b05ea-400">有効な場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="b05ea-401">構成されていない場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="b05ea-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="b05ea-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="b05ea-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-403">Boolean</span></span>|<span data-ttu-id="b05ea-404">このセキュリティ設定は、システムのシャット ダウン時に仮想メモリのページファイルがオフになっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="b05ea-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="b05ea-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="b05ea-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-406">Boolean</span></span>|<span data-ttu-id="b05ea-407">このセキュリティ設定は、Windows にログオンしなくてもコンピューターをシャット ダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="b05ea-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="b05ea-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="b05ea-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-409">Boolean</span></span>|<span data-ttu-id="b05ea-410">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="b05ea-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="b05ea-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="b05ea-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-412">Boolean</span></span>|<span data-ttu-id="b05ea-413">ファイルとレジストリの書き込みエラーをユーザーの場所ごとに仮想化します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="b05ea-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="b05ea-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="b05ea-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-415">Boolean</span></span>|<span data-ttu-id="b05ea-416">実行が許可される前に、実行可能ファイルに、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="b05ea-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b05ea-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="b05ea-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b05ea-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="b05ea-419">管理者承認モードでは、管理者に対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="b05ea-420">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="b05ea-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b05ea-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="b05ea-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b05ea-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="b05ea-423">標準ユーザーに対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="b05ea-424">可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="b05ea-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="b05ea-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="b05ea-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-426">Boolean</span></span>|<span data-ttu-id="b05ea-427">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップに移動するすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="b05ea-428">管理者および標準ユーザーに対するプロンプトの動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="b05ea-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="b05ea-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="b05ea-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-430">Boolean</span></span>|<span data-ttu-id="b05ea-431">システム特権を必要とするアプリケーションのインストールは、管理者の資格情報を求められます。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="b05ea-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="b05ea-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="b05ea-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-433">Boolean</span></span>|<span data-ttu-id="b05ea-434">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="b05ea-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="b05ea-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="b05ea-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-436">Boolean</span></span>|<span data-ttu-id="b05ea-437">ビルトイン管理者アカウントが管理者承認モードを使用して、または完全な管理者特権を持つすべてのアプリケーションを実行するかどうかを定義します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="b05ea-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="b05ea-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="b05ea-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-439">Boolean</span></span>|<span data-ttu-id="b05ea-440">管理者承認モードおよびすべての UAC ポリシー設定を有効にするかどうかを定義する既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="b05ea-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b05ea-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="b05ea-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="b05ea-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="b05ea-443">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="b05ea-444">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="b05ea-445">可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="b05ea-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b05ea-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="b05ea-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="b05ea-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="b05ea-448">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="b05ea-449">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="b05ea-450">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="b05ea-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="b05ea-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="b05ea-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-452">Boolean</span></span>|<span data-ttu-id="b05ea-453">このセキュリティ設定は、SMB クライアントが SMB パケット署名をネゴシエートしようとしたかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="b05ea-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="b05ea-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="b05ea-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-455">Boolean</span></span>|<span data-ttu-id="b05ea-456">このセキュリティ設定は、SMB クライアント コンポーネントでパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="b05ea-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="b05ea-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="b05ea-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-458">Boolean</span></span>|<span data-ttu-id="b05ea-459">このセキュリティ設定が有効の場合、サーバー メッセージ ブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしない Microsoft 以外の SMB サーバーにプレーン テキスト パスワードを送信するのには。</span><span class="sxs-lookup"><span data-stu-id="b05ea-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="b05ea-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="b05ea-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="b05ea-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-461">Boolean</span></span>|<span data-ttu-id="b05ea-462">このセキュリティ設定は、SMB サーバー コンポーネントがパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="b05ea-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="b05ea-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="b05ea-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-464">Boolean</span></span>|<span data-ttu-id="b05ea-465">このセキュリティ設定は、SMB サーバーが SMB パケット署名を要求するクライアントをネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="b05ea-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="b05ea-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="b05ea-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-467">Boolean</span></span>|<span data-ttu-id="b05ea-468">既定では、このセキュリティ設定は共有とパイプは匿名でアクセスできる名前付きパイプおよび匿名でアクセスできる共有の設定に匿名アクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="b05ea-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="b05ea-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="b05ea-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-470">Boolean</span></span>|<span data-ttu-id="b05ea-471">このセキュリティ設定は、どのような追加のアクセス許可をコンピューターへの匿名接続を許可しますを指定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="b05ea-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="b05ea-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="b05ea-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-473">Boolean</span></span>|<span data-ttu-id="b05ea-474">このセキュリティ設定は、ドメイン アカウントやネットワーク共有の名前の列挙など、特定の操作を実行するのには匿名ユーザーを許可するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="b05ea-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="b05ea-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="b05ea-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-476">Boolean</span></span>|<span data-ttu-id="b05ea-477">このセキュリティ設定は、かどうかは、次のパスワードの変更で新しいパスワードの LAN Manager (LM) ハッシュ値が格納されているを決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="b05ea-478">既定では格納されません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="b05ea-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="b05ea-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="b05ea-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b05ea-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="b05ea-481">このセキュリティ設定は、ユーザーのログオン用のスマート カードがスマート カード リーダーから削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="b05ea-482">可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="b05ea-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="b05ea-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-484">Boolean</span></span>|<span data-ttu-id="b05ea-485">アプリケーションとブラウザーの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="b05ea-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="b05ea-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-487">Boolean</span></span>|<span data-ttu-id="b05ea-488">ファミリのオプション領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="b05ea-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="b05ea-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-490">Boolean</span></span>|<span data-ttu-id="b05ea-491">デバイスのパフォーマンスと稼働状態の領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="b05ea-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="b05ea-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-493">Boolean</span></span>|<span data-ttu-id="b05ea-494">ファイアウォールとネットワークの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="b05ea-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="b05ea-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-496">Boolean</span></span>|<span data-ttu-id="b05ea-497">ウイルスと脅威の保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="b05ea-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="b05ea-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-499">Boolean</span></span>|<span data-ttu-id="b05ea-500">アカウントの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="b05ea-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="b05ea-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-502">Boolean</span></span>|<span data-ttu-id="b05ea-503">ハードウェアの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="b05ea-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="b05ea-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-505">Boolean</span></span>|<span data-ttu-id="b05ea-506">Ransomware 保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="b05ea-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="b05ea-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-508">Boolean</span></span>|<span data-ttu-id="b05ea-509">[デバイスのセキュリティ、セキュリティで保護されたブート領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="b05ea-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="b05ea-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="b05ea-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-511">Boolean</span></span>|<span data-ttu-id="b05ea-512">[デバイスのセキュリティのトラブルシューティング、セキュリティ プロセスの表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="b05ea-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b05ea-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="b05ea-514">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-514">String</span></span>|<span data-ttu-id="b05ea-515">ユーザーに表示される会社名です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="b05ea-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="b05ea-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="b05ea-517">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-517">String</span></span>|<span data-ttu-id="b05ea-518">ユーザーに表示される電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="b05ea-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="b05ea-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="b05ea-520">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-520">String</span></span>|<span data-ttu-id="b05ea-521">電話番号または Skype ID のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="b05ea-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="b05ea-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="b05ea-523">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-523">String</span></span>|<span data-ttu-id="b05ea-524">ヘルプ ポータルの URL をユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="b05ea-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="b05ea-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="b05ea-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="b05ea-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="b05ea-527">アプリケーションの表示領域を表示するのに通知します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="b05ea-528">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="b05ea-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="b05ea-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="b05ea-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="b05ea-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="b05ea-531">IT の連絡先を表示する場所を構成するエンド ・ ユーザーへの情報です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="b05ea-532">可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="b05ea-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="b05ea-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="b05ea-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-534">Boolean</span></span>|<span data-ttu-id="b05ea-535">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="b05ea-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="b05ea-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b05ea-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="b05ea-537">Int32</span><span class="sxs-lookup"><span data-stu-id="b05ea-537">Int32</span></span>|<span data-ttu-id="b05ea-538">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="b05ea-539">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="b05ea-540">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="b05ea-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="b05ea-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="b05ea-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="b05ea-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="b05ea-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="b05ea-543">事前共有キーを使用するエンコーディングを選択します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="b05ea-544">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="b05ea-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="b05ea-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="b05ea-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-546">Boolean</span></span>|<span data-ttu-id="b05ea-547">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b05ea-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="b05ea-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="b05ea-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-549">Boolean</span></span>|<span data-ttu-id="b05ea-550">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="b05ea-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="b05ea-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="b05ea-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-552">Boolean</span></span>|<span data-ttu-id="b05ea-553">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b05ea-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="b05ea-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="b05ea-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-555">Boolean</span></span>|<span data-ttu-id="b05ea-556">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="b05ea-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="b05ea-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="b05ea-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="b05ea-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="b05ea-559">証明書失効リストを適用する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="b05ea-560">可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="b05ea-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="b05ea-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="b05ea-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-562">Boolean</span></span>|<span data-ttu-id="b05ea-563">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="b05ea-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="b05ea-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b05ea-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="b05ea-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="b05ea-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="b05ea-566">トンネルのゲートウェイでパケットのキューイングを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="b05ea-567">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="b05ea-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="b05ea-568">firewallProfileDomain</span></span>|[<span data-ttu-id="b05ea-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b05ea-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b05ea-570">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="b05ea-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="b05ea-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="b05ea-571">firewallProfilePublic</span></span>|[<span data-ttu-id="b05ea-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b05ea-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b05ea-573">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="b05ea-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="b05ea-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="b05ea-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="b05ea-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b05ea-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b05ea-576">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="b05ea-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="b05ea-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="b05ea-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="b05ea-578">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b05ea-578">String collection</span></span>|<span data-ttu-id="b05ea-579">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="b05ea-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="b05ea-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="b05ea-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-582">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="b05ea-583">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="b05ea-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="b05ea-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-586">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="b05ea-587">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="b05ea-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="b05ea-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-590">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="b05ea-591">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="b05ea-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="b05ea-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-594">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="b05ea-595">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="b05ea-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="b05ea-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-598">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="b05ea-599">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="b05ea-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="b05ea-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-602">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="b05ea-603">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="b05ea-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="b05ea-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-606">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="b05ea-607">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="b05ea-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="b05ea-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-610">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="b05ea-611">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="b05ea-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="b05ea-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-614">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="b05ea-615">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="b05ea-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="b05ea-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-618">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="b05ea-619">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="b05ea-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-622">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="b05ea-623">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="b05ea-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="b05ea-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-626">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="b05ea-627">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="b05ea-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="b05ea-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-630">資格情報が Windows のローカル セキュリティ機関サブシステムから盗むことが許可されているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="b05ea-631">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="b05ea-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="b05ea-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-634">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="b05ea-635">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="b05ea-636">defenderProcessCreation</span></span>|[<span data-ttu-id="b05ea-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-638">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="b05ea-639">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="b05ea-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="b05ea-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-642">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="b05ea-643">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="b05ea-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="b05ea-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-646">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="b05ea-647">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="b05ea-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="b05ea-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-650">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="b05ea-651">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="b05ea-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="b05ea-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-654">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="b05ea-655">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="b05ea-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b05ea-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b05ea-658">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="b05ea-659">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="b05ea-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="b05ea-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-662">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="b05ea-663">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="b05ea-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-666">Ransomeware に対して高度な保護の使用を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="b05ea-667">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="b05ea-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="b05ea-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="b05ea-670">保護されたフォルダーの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="b05ea-671">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="b05ea-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="b05ea-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="b05ea-673">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b05ea-673">String collection</span></span>|<span data-ttu-id="b05ea-674">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="b05ea-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="b05ea-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="b05ea-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="b05ea-676">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b05ea-676">String collection</span></span>|<span data-ttu-id="b05ea-677">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="b05ea-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="b05ea-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="b05ea-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b05ea-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b05ea-680">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="b05ea-681">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b05ea-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="b05ea-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="b05ea-683">Binary</span><span class="sxs-lookup"><span data-stu-id="b05ea-683">Binary</span></span>|<span data-ttu-id="b05ea-684">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="b05ea-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="b05ea-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="b05ea-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="b05ea-686">String</span><span class="sxs-lookup"><span data-stu-id="b05ea-686">String</span></span>|<span data-ttu-id="b05ea-687">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="b05ea-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="b05ea-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="b05ea-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="b05ea-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-689">Boolean</span></span>|<span data-ttu-id="b05ea-690">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="b05ea-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="b05ea-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="b05ea-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="b05ea-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="b05ea-693">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="b05ea-694">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="b05ea-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="b05ea-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="b05ea-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="b05ea-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="b05ea-697">プラットフォームのセキュリティ レベルとセキュリティで保護されたブートし、仮想化ベースのセキュリティの両方が有効である場合は、資格情報の保護にします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="b05ea-698">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="b05ea-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="b05ea-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="b05ea-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-700">Boolean</span></span>|<span data-ttu-id="b05ea-701">Security(VBS) を仮想化をオンに基づいています。</span><span class="sxs-lookup"><span data-stu-id="b05ea-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="b05ea-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="b05ea-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="b05ea-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-703">Boolean</span></span>|<span data-ttu-id="b05ea-704">プラットフォームのセキュリティ レベルが次の再起動時に有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="b05ea-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="b05ea-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="b05ea-706">[有効化](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="b05ea-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="b05ea-707">.md)</span><span class="sxs-lookup"><span data-stu-id="b05ea-707">.md)</span></span>|<span data-ttu-id="b05ea-708">ガードのシステムの起動を構成するのには IT 管理者を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="b05ea-709">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b05ea-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="b05ea-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="b05ea-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-711">Boolean</span></span>|<span data-ttu-id="b05ea-712">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="b05ea-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b05ea-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="b05ea-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-714">Boolean</span></span>|<span data-ttu-id="b05ea-715">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="b05ea-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="b05ea-716">applicationGuardEnabled</span></span>|<span data-ttu-id="b05ea-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-717">Boolean</span></span>|<span data-ttu-id="b05ea-718">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="b05ea-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="b05ea-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="b05ea-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="b05ea-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="b05ea-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="b05ea-721">新しい Windows のビルドの Windows Defender のアプリケーション保護を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="b05ea-722">可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="b05ea-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="b05ea-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="b05ea-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="b05ea-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="b05ea-725">イメージ ファイルの転送、テキスト ファイルのいずれかにクリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="b05ea-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="b05ea-726">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="b05ea-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="b05ea-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="b05ea-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-728">Boolean</span></span>|<span data-ttu-id="b05ea-729">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="b05ea-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="b05ea-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="b05ea-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="b05ea-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-731">Boolean</span></span>|<span data-ttu-id="b05ea-732">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="b05ea-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="b05ea-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="b05ea-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-734">Boolean</span></span>|<span data-ttu-id="b05ea-735">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="b05ea-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="b05ea-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="b05ea-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="b05ea-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="b05ea-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="b05ea-738">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="b05ea-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="b05ea-739">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="b05ea-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="b05ea-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="b05ea-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-741">Boolean</span></span>|<span data-ttu-id="b05ea-742">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="b05ea-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="b05ea-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="b05ea-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-744">Boolean</span></span>|<span data-ttu-id="b05ea-745">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="b05ea-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="b05ea-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="b05ea-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-747">Boolean</span></span>|<span data-ttu-id="b05ea-748">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="b05ea-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="b05ea-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="b05ea-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-750">Boolean</span></span>|<span data-ttu-id="b05ea-751">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="b05ea-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="b05ea-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="b05ea-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="b05ea-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-753">Boolean</span></span>|<span data-ttu-id="b05ea-754">仮想 GPU を使用するアプリケーションの保護を許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="b05ea-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="b05ea-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="b05ea-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-756">Boolean</span></span>|<span data-ttu-id="b05ea-757">アプリケーション ガード コンテナーの端からファイルをダウンロードし、ホスト上でファイル システムを保存するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="b05ea-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="b05ea-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="b05ea-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-759">Boolean</span></span>|<span data-ttu-id="b05ea-760">Azure AD に参加中に encrpytion を有効にする標準のユーザーに許可するのには管理者を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="b05ea-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="b05ea-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="b05ea-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-762">Boolean</span></span>|<span data-ttu-id="b05ea-763">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="b05ea-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="b05ea-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="b05ea-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-765">Boolean</span></span>|<span data-ttu-id="b05ea-766">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="b05ea-767">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="b05ea-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="b05ea-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="b05ea-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="b05ea-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="b05ea-769">Boolean</span></span>|<span data-ttu-id="b05ea-770">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="b05ea-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="b05ea-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="b05ea-773">BitLocker のシステム ドライブのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="b05ea-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="b05ea-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="b05ea-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="b05ea-776">BitLocker は、ドライブのポリシーを修正します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="b05ea-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="b05ea-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b05ea-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="b05ea-779">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="b05ea-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b05ea-780">応答</span><span class="sxs-lookup"><span data-stu-id="b05ea-780">Response</span></span>
<span data-ttu-id="b05ea-781">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b05ea-781">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b05ea-782">例</span><span class="sxs-lookup"><span data-stu-id="b05ea-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="b05ea-783">要求</span><span class="sxs-lookup"><span data-stu-id="b05ea-783">Request</span></span>
<span data-ttu-id="b05ea-784">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b05ea-784">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26475

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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

### <a name="response"></a><span data-ttu-id="b05ea-785">応答</span><span class="sxs-lookup"><span data-stu-id="b05ea-785">Response</span></span>
<span data-ttu-id="b05ea-p196">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b05ea-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26647

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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




