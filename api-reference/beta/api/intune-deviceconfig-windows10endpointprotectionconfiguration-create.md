---
title: windows10EndpointProtectionConfiguration の作成
description: 新しい windows10EndpointProtectionConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bdc31fed7797a448239bc7ed19ac57750692646
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402588"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="f0f10-103">windows10EndpointProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="f0f10-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f0f10-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0f10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0f10-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0f10-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f10-107">新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0f10-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0f10-108">Prerequisites</span></span>
<span data-ttu-id="f0f10-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0f10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0f10-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0f10-111">Permission type</span></span>|<span data-ttu-id="f0f10-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0f10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f10-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f10-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f10-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-116">Not supported.</span></span>|
|<span data-ttu-id="f0f10-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0f10-117">Application</span></span>|<span data-ttu-id="f0f10-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f10-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0f10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0f10-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0f10-120">Request headers</span></span>
|<span data-ttu-id="f0f10-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0f10-121">Header</span></span>|<span data-ttu-id="f0f10-122">値</span><span class="sxs-lookup"><span data-stu-id="f0f10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f10-123">Authorization</span></span>|<span data-ttu-id="f0f10-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f0f10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0f10-125">Accept</span></span>|<span data-ttu-id="f0f10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f10-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0f10-127">Request body</span></span>
<span data-ttu-id="f0f10-128">要求本文で、windows10EndpointProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="f0f10-129">次の表に、windows10EndpointProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="f0f10-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0f10-130">Property</span></span>|<span data-ttu-id="f0f10-131">型</span><span class="sxs-lookup"><span data-stu-id="f0f10-131">Type</span></span>|<span data-ttu-id="f0f10-132">説明</span><span class="sxs-lookup"><span data-stu-id="f0f10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f10-133">id</span><span class="sxs-lookup"><span data-stu-id="f0f10-133">id</span></span>|<span data-ttu-id="f0f10-134">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-134">String</span></span>|<span data-ttu-id="f0f10-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f0f10-135">Key of the entity.</span></span> <span data-ttu-id="f0f10-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f10-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0f10-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f10-138">DateTimeOffset</span></span>|<span data-ttu-id="f0f10-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f0f10-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0f10-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0f10-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0f10-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f0f10-142">String collection</span></span>|<span data-ttu-id="f0f10-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0f10-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0f10-145">supportsScopeTags</span></span>|<span data-ttu-id="f0f10-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-146">Boolean</span></span>|<span data-ttu-id="f0f10-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0f10-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0f10-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0f10-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-150">This property is read-only.</span></span> <span data-ttu-id="f0f10-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f10-152">createdDateTime</span></span>|<span data-ttu-id="f0f10-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f10-153">DateTimeOffset</span></span>|<span data-ttu-id="f0f10-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f0f10-154">DateTime the object was created.</span></span> <span data-ttu-id="f0f10-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-156">説明</span><span class="sxs-lookup"><span data-stu-id="f0f10-156">description</span></span>|<span data-ttu-id="f0f10-157">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-157">String</span></span>|<span data-ttu-id="f0f10-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f0f10-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0f10-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f0f10-160">displayName</span></span>|<span data-ttu-id="f0f10-161">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-161">String</span></span>|<span data-ttu-id="f0f10-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f0f10-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0f10-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-164">version</span><span class="sxs-lookup"><span data-stu-id="f0f10-164">version</span></span>|<span data-ttu-id="f0f10-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f10-165">Int32</span></span>|<span data-ttu-id="f0f10-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f0f10-166">Version of the device configuration.</span></span> <span data-ttu-id="f0f10-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f0f10-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f10-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="f0f10-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="f0f10-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="f0f10-170">このポリシーは、外部の DMA 機能を持つデバイスに対して追加のセキュリティを提供します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="f0f10-171">これにより外部の DMA 対応デバイスの列挙体をより細かく制御互換性のないデバイスと DMA Remapping メモリの分離レベルとサンド ボックス化できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="f0f10-172">このポリシーは、カーネルの DMA の保護がサポートされていて、システムのファームウェアで有効になっている場合にのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="f0f10-173">カーネル DMA の保護は、ポリシーを使用して、またはエンド ・ ユーザーが制御できないプラットフォーム機能です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="f0f10-174">製造時にシステムでサポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0f10-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="f0f10-175">システムがカーネルの DMA の保護をサポートしているかを確認するには、MSINFO32.exe の概要] ページでカーネルの DMA 保護フィールドを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f0f10-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="f0f10-176">可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="f0f10-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="f0f10-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="f0f10-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-179">このユーザー権利のバックアップ/リストアの実行中に資格情報マネージャーで表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="f0f10-180">他のエンティティにこの特権が与えられた場合、ユーザーの保存された資格情報が危険にさらされる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f0f10-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="f0f10-181">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f0f10-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="f0f10-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-184">このユーザー権利は、どのユーザーを決定し、グループがネットワーク経由でコンピューターに接続できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="f0f10-185">許可の状態がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="f0f10-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f0f10-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="f0f10-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-188">このユーザー権利は、どのユーザーとグループは、ネットワーク経由でコンピューターへの接続からのブロックを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="f0f10-189">ステート ブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-189">State Block is supported.</span></span>|
|<span data-ttu-id="f0f10-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0f10-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="f0f10-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-192">このユーザー権利では、認証なしのすべてのユーザーを偽装するプロセスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="f0f10-193">プロセスをユーザーと同じローカル リソースへのアクセスを得ることができます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="f0f10-194">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="f0f10-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="f0f10-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-197">このユーザー権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="f0f10-198">状態 NotConfigured、許可とブロックのすべてをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="f0f10-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="f0f10-199">userRightsBackupData</span></span>|[<span data-ttu-id="f0f10-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-201">このユーザー権利では、回避できるユーザー ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのアクセス許可ファイルとディレクトリをバックアップするときを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="f0f10-202">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="f0f10-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="f0f10-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-205">このユーザー権利は、どのユーザーとグループは、コンピューターの内部時計の日付と時刻を変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="f0f10-206">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="f0f10-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="f0f10-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-209">このセキュリティ設定は、ユーザーがすべてのセッションに使用可能なグローバル オブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="f0f10-210">グローバル オブジェクトを作成できるユーザーに影響を与える他のユーザーのセッションは、アプリケーションの障害やデータの破損につながる可能性の下で実行するプロセスです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="f0f10-211">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="f0f10-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="f0f10-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-214">このユーザー権利は、どのユーザーおよびグループを作成し、ページファイルのサイズを変更する内部 API を呼び出すことができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="f0f10-215">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="f0f10-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="f0f10-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-218">このユーザー権利では、マネージャー オブジェクトを使用してディレクトリ オブジェクトを作成するプロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="f0f10-219">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="f0f10-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="f0f10-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-222">このユーザー権利は、ユーザーが、ログオンしているコンピューターからシンボリック リンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="f0f10-223">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="f0f10-224">userRightsCreateToken</span></span>|[<span data-ttu-id="f0f10-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-226">このユーザー権利では、プロセスでは、内部の API を使用して、アクセス トークンを作成するときに、ローカル リソースへのアクセスを取得するために使用するトークンを作成するプロセスにするユーザーまたはグループを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="f0f10-227">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="f0f10-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="f0f10-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-230">このユーザー権利は、ユーザーが任意のプロセスまたはカーネルにデバッガーをアタッチできるを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="f0f10-231">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f0f10-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="f0f10-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="f0f10-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-234">このユーザー権利では、リモート デスクトップ サービス クライアントとしてログオン拒否するユーザーとグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="f0f10-235">NotConfigured および受信拒否の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="f0f10-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="f0f10-236">userRightsDelegation</span></span>|[<span data-ttu-id="f0f10-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-238">このユーザー権利は、ユーザーまたはコンピューター オブジェクトの委任に対して信頼されるように設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="f0f10-239">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="f0f10-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="f0f10-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-242">このユーザー権利では、セキュリティ ログにエントリを追加するのにはプロセスが使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="f0f10-243">セキュリティ ログは、承認されていないシステムへのアクセスを追跡に使用します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="f0f10-244">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="f0f10-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="f0f10-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-247">ユーザーには、このユーザー権利を割り当てるには、クライアントを偽装するには、そのユーザーに代わって実行されるプログラムすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="f0f10-248">により承認されていないユーザーが自分が作成したサービスに接続するクライアントを納得させることと、偽装して、クライアントに許可されていないユーザーのアクセス許可を昇格させるという、この種の偽装にこのユーザー権利を必要とします。管理者レベルまたはシステム レベル。</span><span class="sxs-lookup"><span data-stu-id="f0f10-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="f0f10-249">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="f0f10-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="f0f10-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-252">このユーザー権利は、取引先企業は他のプロセスに割り当てられている実行の優先順位を上げる別のプロセスに対するプロパティの書き込みアクセスを持つプロセスを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="f0f10-253">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="f0f10-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="f0f10-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-256">このユーザー権利は、ユーザーが動的にロードおよびデバイス ドライバーやカーネル モードでは、他のコードをアンロードするを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="f0f10-257">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="f0f10-258">userRightsLockMemory</span></span>|[<span data-ttu-id="f0f10-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-260">このユーザー権利では、ディスク上の仮想メモリを物理メモリにデータを保持するプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="f0f10-261">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="f0f10-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="f0f10-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-264">このユーザー権利は、オブジェクト アクセスの監査ファイル、Active Directory オブジェクト、レジストリ キーなどの個々 のリソースのオプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="f0f10-265">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="f0f10-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="f0f10-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-268">このユーザー権利では、リモート最適化などのボリュームの保守タスクを実行できるユーザーおよびグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="f0f10-269">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="f0f10-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="f0f10-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-272">このユーザー権利では、ファームウェアの環境値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="f0f10-273">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="f0f10-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="f0f10-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-276">このユーザー権利は、ユーザー アカウントは、ファイル、レジストリ キー、またはその他のユーザーが所有するプロセスなどのオブジェクトの整合性ラベルを変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="f0f10-277">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="f0f10-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="f0f10-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-280">このユーザー権利では、システム プロセスのパフォーマンスを監視するパフォーマンス監視ツールを使用できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="f0f10-281">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="f0f10-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="f0f10-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-284">このユーザー権利は、ネットワーク上のリモートの場所からコンピューターをシャット ダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="f0f10-285">このユーザー権利が誤用されると、サービス拒否攻撃があります。</span><span class="sxs-lookup"><span data-stu-id="f0f10-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="f0f10-286">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="f0f10-287">userRightsRestoreData</span></span>|[<span data-ttu-id="f0f10-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-289">このユーザー権利では、ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのファイルおよびディレクトリをバックアップ、復元するときのアクセス許可を回避できるユーザーを決定し、オブジェクトの所有者として有効なセキュリティ プリンシパルを設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="f0f10-290">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="f0f10-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="f0f10-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-293">所有権をユーザーのセキュリティ保護可能なオブジェクトの Active Directory オブジェクト、ファイル、フォルダー、プリンター、レジストリ キー、プロセス、およびスレッドを含め、システムでこのユーザー権利を決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="f0f10-294">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f0f10-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="f0f10-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="f0f10-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f0f10-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f0f10-297">このセキュリティ設定は、サービスとしてプロセスを登録できないサービス アカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="f0f10-298">注: このセキュリティ設定は、システム、ローカル サービス、またはネットワーク サービス アカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="f0f10-299">ブロックがサポートされているだけの状態です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="f0f10-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="f0f10-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="f0f10-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-301">Boolean</span></span>|<span data-ttu-id="f0f10-302">この設定は、xbox ゲームの保存が有効 (1) または無効 (0) かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="f0f10-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f0f10-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="f0f10-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f0f10-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f0f10-305">この設定は、付属品の管理サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f0f10-306">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-306">Default: Manual.</span></span> <span data-ttu-id="f0f10-307">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f0f10-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f0f10-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="f0f10-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f0f10-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f0f10-310">この設定は、認証マネージャーの Live サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f0f10-311">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-311">Default: Manual.</span></span> <span data-ttu-id="f0f10-312">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f0f10-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f0f10-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="f0f10-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f0f10-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f0f10-315">保存サービスの開始のタイプのゲームのライブは Automatic(2)、Manual(3)、Disabled(4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f0f10-316">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-316">Default: Manual.</span></span> <span data-ttu-id="f0f10-317">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f0f10-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f0f10-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="f0f10-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f0f10-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f0f10-320">この設定は、ネットワーク サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f0f10-321">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-321">Default: Manual.</span></span> <span data-ttu-id="f0f10-322">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f0f10-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="f0f10-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="f0f10-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-324">Boolean</span></span>|<span data-ttu-id="f0f10-325">ユーザーがこのコンピューターに Microsoft の新しいアカウントを追加するを防ぐ。</span><span class="sxs-lookup"><span data-stu-id="f0f10-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="f0f10-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="f0f10-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="f0f10-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-327">Boolean</span></span>|<span data-ttu-id="f0f10-328">物理デバイス以外の場所からのログオンにパスワードで保護していないローカルのアカウントを有効にします。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="f0f10-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="f0f10-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="f0f10-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-330">Boolean</span></span>|<span data-ttu-id="f0f10-331">ローカル管理者アカウントを有効または無効にするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="f0f10-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="f0f10-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="f0f10-333">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-333">String</span></span>|<span data-ttu-id="f0f10-334">"Administrator"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="f0f10-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="f0f10-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="f0f10-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-336">Boolean</span></span>|<span data-ttu-id="f0f10-337">Guest アカウントが有効か無効になっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="f0f10-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f0f10-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="f0f10-339">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-339">String</span></span>|<span data-ttu-id="f0f10-340">"Guest"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="f0f10-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="f0f10-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="f0f10-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-342">Boolean</span></span>|<span data-ttu-id="f0f10-343">ポータブル コンピューターを防ぐため、ログインしなくても接続されているからです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="f0f10-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="f0f10-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="f0f10-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-345">Boolean</span></span>|<span data-ttu-id="f0f10-346">管理者だけが使用する共有プリンターへの接続の一部としてプリンター ドライバーをインストールを制限します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="f0f10-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="f0f10-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="f0f10-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-348">Boolean</span></span>|<span data-ttu-id="f0f10-349">CD-ROM メディアにアクセスする唯一の対話形式でログオンしているユーザーは、この設定を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="f0f10-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="f0f10-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="f0f10-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="f0f10-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="f0f10-352">リムーバブル NTFS メディアを取り出すことができるユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="f0f10-353">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f0f10-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="f0f10-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="f0f10-355">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f10-355">Int32</span></span>|<span data-ttu-id="f0f10-356">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f0f10-357">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="f0f10-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f0f10-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="f0f10-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="f0f10-359">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f10-359">Int32</span></span>|<span data-ttu-id="f0f10-360">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f0f10-361">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="f0f10-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f0f10-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="f0f10-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="f0f10-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-363">Boolean</span></span>|<span data-ttu-id="f0f10-364">CTRL + ALT + DEL を押す前に、ユーザーがログオンできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0f10-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="f0f10-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="f0f10-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="f0f10-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-366">Boolean</span></span>|<span data-ttu-id="f0f10-367">このデバイス上で最後署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="f0f10-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="f0f10-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="f0f10-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-369">Boolean</span></span>|<span data-ttu-id="f0f10-370">資格情報を入力した後、デバイスのデスクトップが表示される前にこのデバイスに署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="f0f10-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="f0f10-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="f0f10-372">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-372">String</span></span>|<span data-ttu-id="f0f10-373">ログオン ユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="f0f10-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="f0f10-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="f0f10-375">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-375">String</span></span>|<span data-ttu-id="f0f10-376">ログオン ユーザーのメッセージ テキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="f0f10-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="f0f10-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="f0f10-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-378">Boolean</span></span>|<span data-ttu-id="f0f10-379">ブロック PKU2U 認証要求をこのデバイスにオンライン id を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="f0f10-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="f0f10-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="f0f10-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-381">Boolean</span></span>|<span data-ttu-id="f0f10-382">UI ヘルパー LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティのブール値</span><span class="sxs-lookup"><span data-stu-id="f0f10-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="f0f10-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="f0f10-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="f0f10-384">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-384">String</span></span>|<span data-ttu-id="f0f10-385">または、SAM にリモート呼び出しを行うには、ユーザーとグループを拒否する既定のセキュリティ記述子定義言語の文字列を編集します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="f0f10-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="f0f10-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="f0f10-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f0f10-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f0f10-388">このセキュリティ設定では、クライアントが 128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f0f10-389">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f0f10-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="f0f10-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="f0f10-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f0f10-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f0f10-392">このセキュリティ設定は、128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とするサーバーです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f0f10-393">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f0f10-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f0f10-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="f0f10-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f0f10-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="f0f10-396">このセキュリティ設定は、ネットワーク ログオン時に使用するチャレンジ/レスポンス認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="f0f10-397">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="f0f10-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="f0f10-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="f0f10-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="f0f10-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-399">Boolean</span></span>|<span data-ttu-id="f0f10-400">有効な場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="f0f10-401">構成されていない場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="f0f10-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="f0f10-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="f0f10-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-403">Boolean</span></span>|<span data-ttu-id="f0f10-404">このセキュリティ設定は、システムのシャット ダウン時に仮想メモリのページファイルがオフになっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="f0f10-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="f0f10-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="f0f10-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-406">Boolean</span></span>|<span data-ttu-id="f0f10-407">このセキュリティ設定は、Windows にログオンしなくてもコンピューターをシャット ダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="f0f10-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="f0f10-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="f0f10-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-409">Boolean</span></span>|<span data-ttu-id="f0f10-410">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="f0f10-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="f0f10-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="f0f10-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-412">Boolean</span></span>|<span data-ttu-id="f0f10-413">ファイルとレジストリの書き込みエラーをユーザーの場所ごとに仮想化します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="f0f10-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="f0f10-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="f0f10-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-415">Boolean</span></span>|<span data-ttu-id="f0f10-416">実行が許可される前に、実行可能ファイルに、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="f0f10-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f0f10-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="f0f10-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f0f10-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="f0f10-419">管理者承認モードでは、管理者に対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="f0f10-420">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="f0f10-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f0f10-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="f0f10-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f0f10-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="f0f10-423">標準ユーザーに対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="f0f10-424">可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="f0f10-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="f0f10-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="f0f10-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-426">Boolean</span></span>|<span data-ttu-id="f0f10-427">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップに移動するすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="f0f10-428">管理者および標準ユーザーに対するプロンプトの動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="f0f10-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="f0f10-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="f0f10-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-430">Boolean</span></span>|<span data-ttu-id="f0f10-431">システム特権を必要とするアプリケーションのインストールは、管理者の資格情報を求められます。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="f0f10-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="f0f10-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="f0f10-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-433">Boolean</span></span>|<span data-ttu-id="f0f10-434">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="f0f10-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="f0f10-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="f0f10-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-436">Boolean</span></span>|<span data-ttu-id="f0f10-437">ビルトイン管理者アカウントが管理者承認モードを使用して、または完全な管理者特権を持つすべてのアプリケーションを実行するかどうかを定義します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="f0f10-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="f0f10-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="f0f10-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-439">Boolean</span></span>|<span data-ttu-id="f0f10-440">管理者承認モードおよびすべての UAC ポリシー設定を有効にするかどうかを定義する既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="f0f10-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f0f10-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="f0f10-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f0f10-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="f0f10-443">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f0f10-444">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f0f10-445">可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="f0f10-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f0f10-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="f0f10-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f0f10-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="f0f10-448">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f0f10-449">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f0f10-450">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f0f10-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="f0f10-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="f0f10-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-452">Boolean</span></span>|<span data-ttu-id="f0f10-453">このセキュリティ設定は、SMB クライアントが SMB パケット署名をネゴシエートしようとしたかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="f0f10-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f0f10-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f0f10-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-455">Boolean</span></span>|<span data-ttu-id="f0f10-456">このセキュリティ設定は、SMB クライアント コンポーネントでパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="f0f10-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="f0f10-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="f0f10-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-458">Boolean</span></span>|<span data-ttu-id="f0f10-459">このセキュリティ設定が有効の場合、サーバー メッセージ ブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしない Microsoft 以外の SMB サーバーにプレーン テキスト パスワードを送信するのには。</span><span class="sxs-lookup"><span data-stu-id="f0f10-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="f0f10-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f0f10-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f0f10-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-461">Boolean</span></span>|<span data-ttu-id="f0f10-462">このセキュリティ設定は、SMB サーバー コンポーネントがパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="f0f10-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="f0f10-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="f0f10-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-464">Boolean</span></span>|<span data-ttu-id="f0f10-465">このセキュリティ設定は、SMB サーバーが SMB パケット署名を要求するクライアントをネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="f0f10-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="f0f10-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="f0f10-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-467">Boolean</span></span>|<span data-ttu-id="f0f10-468">既定では、このセキュリティ設定は共有とパイプは匿名でアクセスできる名前付きパイプおよび匿名でアクセスできる共有の設定に匿名アクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="f0f10-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="f0f10-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="f0f10-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-470">Boolean</span></span>|<span data-ttu-id="f0f10-471">このセキュリティ設定は、どのような追加のアクセス許可をコンピューターへの匿名接続を許可しますを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="f0f10-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="f0f10-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="f0f10-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-473">Boolean</span></span>|<span data-ttu-id="f0f10-474">このセキュリティ設定は、ドメイン アカウントやネットワーク共有の名前の列挙など、特定の操作を実行するのには匿名ユーザーを許可するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="f0f10-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="f0f10-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="f0f10-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-476">Boolean</span></span>|<span data-ttu-id="f0f10-477">このセキュリティ設定は、かどうかは、次のパスワードの変更で新しいパスワードの LAN Manager (LM) ハッシュ値が格納されているを決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="f0f10-478">既定では格納されません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="f0f10-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="f0f10-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="f0f10-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f0f10-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="f0f10-481">このセキュリティ設定は、ユーザーのログオン用のスマート カードがスマート カード リーダーから削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="f0f10-482">可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="f0f10-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="f0f10-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-484">Boolean</span></span>|<span data-ttu-id="f0f10-485">アプリケーションとブラウザーの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="f0f10-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="f0f10-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-487">Boolean</span></span>|<span data-ttu-id="f0f10-488">ファミリのオプション領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="f0f10-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="f0f10-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-490">Boolean</span></span>|<span data-ttu-id="f0f10-491">デバイスのパフォーマンスと稼働状態の領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="f0f10-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="f0f10-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-493">Boolean</span></span>|<span data-ttu-id="f0f10-494">ファイアウォールとネットワークの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="f0f10-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="f0f10-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-496">Boolean</span></span>|<span data-ttu-id="f0f10-497">ウイルスと脅威の保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="f0f10-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="f0f10-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-499">Boolean</span></span>|<span data-ttu-id="f0f10-500">アカウントの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="f0f10-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="f0f10-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-502">Boolean</span></span>|<span data-ttu-id="f0f10-503">ハードウェアの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="f0f10-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="f0f10-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-505">Boolean</span></span>|<span data-ttu-id="f0f10-506">Ransomware 保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="f0f10-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="f0f10-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-508">Boolean</span></span>|<span data-ttu-id="f0f10-509">[デバイスのセキュリティ、セキュリティで保護されたブート領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="f0f10-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="f0f10-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="f0f10-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-511">Boolean</span></span>|<span data-ttu-id="f0f10-512">[デバイスのセキュリティのトラブルシューティング、セキュリティ プロセスの表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="f0f10-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0f10-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="f0f10-514">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-514">String</span></span>|<span data-ttu-id="f0f10-515">ユーザーに表示される会社名です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="f0f10-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="f0f10-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="f0f10-517">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-517">String</span></span>|<span data-ttu-id="f0f10-518">ユーザーに表示される電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="f0f10-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="f0f10-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="f0f10-520">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-520">String</span></span>|<span data-ttu-id="f0f10-521">電話番号または Skype ID のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="f0f10-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="f0f10-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="f0f10-523">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-523">String</span></span>|<span data-ttu-id="f0f10-524">ヘルプ ポータルの URL をユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="f0f10-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="f0f10-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="f0f10-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="f0f10-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="f0f10-527">アプリケーションの表示領域を表示するのに通知します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="f0f10-528">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="f0f10-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="f0f10-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="f0f10-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="f0f10-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="f0f10-531">IT の連絡先を表示する場所を構成するエンド ・ ユーザーへの情報です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="f0f10-532">可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="f0f10-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="f0f10-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="f0f10-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-534">Boolean</span></span>|<span data-ttu-id="f0f10-535">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="f0f10-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="f0f10-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="f0f10-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="f0f10-537">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f10-537">Int32</span></span>|<span data-ttu-id="f0f10-538">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="f0f10-539">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="f0f10-540">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="f0f10-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="f0f10-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f0f10-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="f0f10-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f0f10-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="f0f10-543">事前共有キーを使用するエンコーディングを選択します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="f0f10-544">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="f0f10-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="f0f10-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="f0f10-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-546">Boolean</span></span>|<span data-ttu-id="f0f10-547">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f0f10-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="f0f10-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="f0f10-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-549">Boolean</span></span>|<span data-ttu-id="f0f10-550">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="f0f10-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="f0f10-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="f0f10-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-552">Boolean</span></span>|<span data-ttu-id="f0f10-553">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f0f10-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="f0f10-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="f0f10-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-555">Boolean</span></span>|<span data-ttu-id="f0f10-556">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="f0f10-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f0f10-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="f0f10-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f0f10-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="f0f10-559">証明書失効リストを適用する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="f0f10-560">可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="f0f10-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="f0f10-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="f0f10-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-562">Boolean</span></span>|<span data-ttu-id="f0f10-563">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="f0f10-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="f0f10-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f0f10-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="f0f10-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="f0f10-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="f0f10-566">トンネルのゲートウェイでパケットのキューイングを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="f0f10-567">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="f0f10-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="f0f10-568">firewallProfileDomain</span></span>|[<span data-ttu-id="f0f10-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f0f10-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f0f10-570">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="f0f10-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="f0f10-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="f0f10-571">firewallProfilePublic</span></span>|[<span data-ttu-id="f0f10-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f0f10-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f0f10-573">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="f0f10-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="f0f10-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="f0f10-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="f0f10-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f0f10-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f0f10-576">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="f0f10-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="f0f10-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="f0f10-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="f0f10-578">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f0f10-578">String collection</span></span>|<span data-ttu-id="f0f10-579">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="f0f10-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="f0f10-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="f0f10-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-582">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="f0f10-583">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="f0f10-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="f0f10-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-586">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="f0f10-587">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="f0f10-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="f0f10-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-590">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f0f10-591">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="f0f10-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="f0f10-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-594">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f0f10-595">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="f0f10-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="f0f10-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-598">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f0f10-599">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f0f10-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f0f10-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-602">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f0f10-603">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="f0f10-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="f0f10-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-606">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f0f10-607">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="f0f10-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="f0f10-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-610">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f0f10-611">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="f0f10-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="f0f10-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-614">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f0f10-615">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="f0f10-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="f0f10-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-618">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f0f10-619">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="f0f10-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-622">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f0f10-623">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="f0f10-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="f0f10-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-626">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f0f10-627">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="f0f10-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="f0f10-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-630">資格情報が Windows のローカル セキュリティ機関サブシステムから盗むことが許可されているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="f0f10-631">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="f0f10-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="f0f10-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-634">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f0f10-635">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="f0f10-636">defenderProcessCreation</span></span>|[<span data-ttu-id="f0f10-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-638">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f0f10-639">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="f0f10-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="f0f10-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-642">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f0f10-643">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="f0f10-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="f0f10-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-646">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f0f10-647">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="f0f10-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="f0f10-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-650">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f0f10-651">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="f0f10-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="f0f10-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-654">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f0f10-655">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="f0f10-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f0f10-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f0f10-658">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f0f10-659">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="f0f10-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="f0f10-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-662">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f0f10-663">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="f0f10-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-666">Ransomeware に対して高度な保護の使用を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="f0f10-667">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="f0f10-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="f0f10-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="f0f10-670">保護されたフォルダーの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="f0f10-671">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="f0f10-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="f0f10-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="f0f10-673">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f0f10-673">String collection</span></span>|<span data-ttu-id="f0f10-674">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="f0f10-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="f0f10-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="f0f10-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="f0f10-676">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f0f10-676">String collection</span></span>|<span data-ttu-id="f0f10-677">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="f0f10-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="f0f10-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="f0f10-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f0f10-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f0f10-680">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="f0f10-681">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f0f10-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="f0f10-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="f0f10-683">Binary</span><span class="sxs-lookup"><span data-stu-id="f0f10-683">Binary</span></span>|<span data-ttu-id="f0f10-684">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="f0f10-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="f0f10-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="f0f10-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="f0f10-686">String</span><span class="sxs-lookup"><span data-stu-id="f0f10-686">String</span></span>|<span data-ttu-id="f0f10-687">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="f0f10-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="f0f10-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="f0f10-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="f0f10-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-689">Boolean</span></span>|<span data-ttu-id="f0f10-690">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="f0f10-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="f0f10-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="f0f10-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f0f10-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="f0f10-693">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="f0f10-694">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="f0f10-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="f0f10-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="f0f10-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="f0f10-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="f0f10-697">プラットフォームのセキュリティ レベルとセキュリティで保護されたブートし、仮想化ベースのセキュリティの両方が有効である場合は、資格情報の保護にします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="f0f10-698">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="f0f10-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="f0f10-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="f0f10-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-700">Boolean</span></span>|<span data-ttu-id="f0f10-701">Security(VBS) を仮想化をオンに基づいています。</span><span class="sxs-lookup"><span data-stu-id="f0f10-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="f0f10-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="f0f10-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="f0f10-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-703">Boolean</span></span>|<span data-ttu-id="f0f10-704">プラットフォームのセキュリティ レベルが次の再起動時に有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="f0f10-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="f0f10-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="f0f10-706">[有効化](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="f0f10-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="f0f10-707">.md)</span><span class="sxs-lookup"><span data-stu-id="f0f10-707">.md)</span></span>|<span data-ttu-id="f0f10-708">ガードのシステムの起動を構成するのには IT 管理者を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="f0f10-709">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f0f10-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="f0f10-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="f0f10-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-711">Boolean</span></span>|<span data-ttu-id="f0f10-712">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="f0f10-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f0f10-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="f0f10-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-714">Boolean</span></span>|<span data-ttu-id="f0f10-715">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="f0f10-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="f0f10-716">applicationGuardEnabled</span></span>|<span data-ttu-id="f0f10-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-717">Boolean</span></span>|<span data-ttu-id="f0f10-718">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="f0f10-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="f0f10-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f0f10-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="f0f10-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f0f10-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="f0f10-721">新しい Windows のビルドの Windows Defender のアプリケーション保護を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="f0f10-722">可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="f0f10-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f0f10-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="f0f10-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="f0f10-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="f0f10-725">イメージ ファイルの転送、テキスト ファイルのいずれかにクリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f0f10-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="f0f10-726">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="f0f10-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="f0f10-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="f0f10-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-728">Boolean</span></span>|<span data-ttu-id="f0f10-729">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="f0f10-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="f0f10-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="f0f10-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="f0f10-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-731">Boolean</span></span>|<span data-ttu-id="f0f10-732">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="f0f10-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="f0f10-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="f0f10-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-734">Boolean</span></span>|<span data-ttu-id="f0f10-735">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="f0f10-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="f0f10-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="f0f10-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="f0f10-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f0f10-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="f0f10-738">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="f0f10-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="f0f10-739">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="f0f10-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="f0f10-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="f0f10-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-741">Boolean</span></span>|<span data-ttu-id="f0f10-742">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="f0f10-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="f0f10-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="f0f10-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-744">Boolean</span></span>|<span data-ttu-id="f0f10-745">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="f0f10-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="f0f10-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="f0f10-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-747">Boolean</span></span>|<span data-ttu-id="f0f10-748">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="f0f10-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="f0f10-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="f0f10-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-750">Boolean</span></span>|<span data-ttu-id="f0f10-751">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="f0f10-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="f0f10-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="f0f10-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="f0f10-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-753">Boolean</span></span>|<span data-ttu-id="f0f10-754">仮想 GPU を使用するアプリケーションの保護を許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="f0f10-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="f0f10-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="f0f10-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-756">Boolean</span></span>|<span data-ttu-id="f0f10-757">アプリケーション ガード コンテナーの端からファイルをダウンロードし、ホスト上でファイル システムを保存するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="f0f10-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="f0f10-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="f0f10-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-759">Boolean</span></span>|<span data-ttu-id="f0f10-760">Azure AD に参加中に encrpytion を有効にする標準のユーザーに許可するのには管理者を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="f0f10-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="f0f10-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="f0f10-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-762">Boolean</span></span>|<span data-ttu-id="f0f10-763">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="f0f10-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="f0f10-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="f0f10-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-765">Boolean</span></span>|<span data-ttu-id="f0f10-766">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="f0f10-767">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="f0f10-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="f0f10-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="f0f10-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="f0f10-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0f10-769">Boolean</span></span>|<span data-ttu-id="f0f10-770">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="f0f10-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="f0f10-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="f0f10-773">BitLocker のシステム ドライブのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="f0f10-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="f0f10-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="f0f10-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="f0f10-776">BitLocker は、ドライブのポリシーを修正します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="f0f10-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="f0f10-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f0f10-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="f0f10-779">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="f0f10-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f0f10-780">応答</span><span class="sxs-lookup"><span data-stu-id="f0f10-780">Response</span></span>
<span data-ttu-id="f0f10-781">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0f10-781">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f10-782">例</span><span class="sxs-lookup"><span data-stu-id="f0f10-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f10-783">要求</span><span class="sxs-lookup"><span data-stu-id="f0f10-783">Request</span></span>
<span data-ttu-id="f0f10-784">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0f10-784">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f0f10-785">応答</span><span class="sxs-lookup"><span data-stu-id="f0f10-785">Response</span></span>
<span data-ttu-id="f0f10-p196">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0f10-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




