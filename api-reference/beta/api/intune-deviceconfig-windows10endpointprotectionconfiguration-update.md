---
title: windows10EndpointProtectionConfiguration の更新
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 36d71a14900d3400874ac39bd1fa59c534208676
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983031"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="51440-103">windows10EndpointProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="51440-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="51440-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51440-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51440-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51440-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51440-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51440-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51440-107">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51440-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51440-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="51440-108">Prerequisites</span></span>
<span data-ttu-id="51440-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51440-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51440-111">Permission type</span></span>|<span data-ttu-id="51440-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51440-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51440-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51440-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51440-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51440-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51440-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51440-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51440-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51440-116">Not supported.</span></span>|
|<span data-ttu-id="51440-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51440-117">Application</span></span>|<span data-ttu-id="51440-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51440-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51440-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51440-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="51440-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51440-120">Request headers</span></span>
|<span data-ttu-id="51440-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51440-121">Header</span></span>|<span data-ttu-id="51440-122">値</span><span class="sxs-lookup"><span data-stu-id="51440-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51440-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51440-123">Authorization</span></span>|<span data-ttu-id="51440-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51440-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51440-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51440-125">Accept</span></span>|<span data-ttu-id="51440-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51440-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51440-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51440-127">Request body</span></span>
<span data-ttu-id="51440-128">要求本文で、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51440-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="51440-129">次の表に、[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51440-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="51440-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51440-130">Property</span></span>|<span data-ttu-id="51440-131">型</span><span class="sxs-lookup"><span data-stu-id="51440-131">Type</span></span>|<span data-ttu-id="51440-132">説明</span><span class="sxs-lookup"><span data-stu-id="51440-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51440-133">id</span><span class="sxs-lookup"><span data-stu-id="51440-133">id</span></span>|<span data-ttu-id="51440-134">String</span><span class="sxs-lookup"><span data-stu-id="51440-134">String</span></span>|<span data-ttu-id="51440-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51440-135">Key of the entity.</span></span> <span data-ttu-id="51440-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51440-137">lastModifiedDateTime</span></span>|<span data-ttu-id="51440-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51440-138">DateTimeOffset</span></span>|<span data-ttu-id="51440-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51440-139">DateTime the object was last modified.</span></span> <span data-ttu-id="51440-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51440-141">roleScopeTagIds</span></span>|<span data-ttu-id="51440-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51440-142">String collection</span></span>|<span data-ttu-id="51440-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="51440-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51440-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51440-145">supportsScopeTags</span></span>|<span data-ttu-id="51440-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-146">Boolean</span></span>|<span data-ttu-id="51440-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="51440-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51440-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="51440-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51440-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="51440-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51440-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="51440-150">This property is read-only.</span></span> <span data-ttu-id="51440-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51440-152">createdDateTime</span></span>|<span data-ttu-id="51440-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51440-153">DateTimeOffset</span></span>|<span data-ttu-id="51440-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51440-154">DateTime the object was created.</span></span> <span data-ttu-id="51440-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-156">説明</span><span class="sxs-lookup"><span data-stu-id="51440-156">description</span></span>|<span data-ttu-id="51440-157">String</span><span class="sxs-lookup"><span data-stu-id="51440-157">String</span></span>|<span data-ttu-id="51440-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="51440-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51440-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-160">displayName</span><span class="sxs-lookup"><span data-stu-id="51440-160">displayName</span></span>|<span data-ttu-id="51440-161">String</span><span class="sxs-lookup"><span data-stu-id="51440-161">String</span></span>|<span data-ttu-id="51440-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="51440-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51440-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-164">version</span><span class="sxs-lookup"><span data-stu-id="51440-164">version</span></span>|<span data-ttu-id="51440-165">Int32</span><span class="sxs-lookup"><span data-stu-id="51440-165">Int32</span></span>|<span data-ttu-id="51440-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="51440-166">Version of the device configuration.</span></span> <span data-ttu-id="51440-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51440-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51440-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="51440-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="51440-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-170">このユーザー権利のバックアップ/リストアの実行中に資格情報マネージャーで表示されます。</span><span class="sxs-lookup"><span data-stu-id="51440-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="51440-171">他のエンティティにこの特権が与えられた場合、ユーザーの保存された資格情報が危険にさらされる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="51440-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="51440-172">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="51440-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="51440-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-175">このユーザー権利は、どのユーザーを決定し、グループがネットワーク経由でコンピューターに接続できます。</span><span class="sxs-lookup"><span data-stu-id="51440-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="51440-176">許可の状態がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="51440-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="51440-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="51440-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-179">このユーザー権利は、どのユーザーとグループは、ネットワーク経由でコンピューターへの接続からのブロックを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="51440-180">ステート ブロックがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-180">State Block is supported.</span></span>|
|<span data-ttu-id="51440-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51440-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="51440-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-183">このユーザー権利では、認証なしのすべてのユーザーを偽装するプロセスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="51440-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="51440-184">プロセスをユーザーと同じローカル リソースへのアクセスを得ることができます。</span><span class="sxs-lookup"><span data-stu-id="51440-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="51440-185">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="51440-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="51440-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-188">このユーザー権利は、コンピューターにログオンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="51440-189">状態 NotConfigured、許可とブロックのすべてをサポートします。</span><span class="sxs-lookup"><span data-stu-id="51440-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="51440-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="51440-190">userRightsBackupData</span></span>|[<span data-ttu-id="51440-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-192">このユーザー権利では、回避できるユーザー ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのアクセス許可ファイルとディレクトリをバックアップするときを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="51440-193">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="51440-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="51440-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-196">このユーザー権利は、どのユーザーとグループは、コンピューターの内部時計の日付と時刻を変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="51440-197">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="51440-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="51440-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-200">このセキュリティ設定は、ユーザーがすべてのセッションに使用可能なグローバル オブジェクトを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="51440-201">グローバル オブジェクトを作成できるユーザーに影響を与える他のユーザーのセッションは、アプリケーションの障害やデータの破損につながる可能性の下で実行するプロセスです。</span><span class="sxs-lookup"><span data-stu-id="51440-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="51440-202">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="51440-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="51440-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-205">このユーザー権利は、どのユーザーおよびグループを作成し、ページファイルのサイズを変更する内部 API を呼び出すことができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="51440-206">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="51440-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="51440-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-209">このユーザー権利では、マネージャー オブジェクトを使用してディレクトリ オブジェクトを作成するプロセスで使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="51440-210">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="51440-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="51440-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-213">このユーザー権利は、ユーザーが、ログオンしているコンピューターからシンボリック リンクを作成できるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="51440-214">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="51440-215">userRightsCreateToken</span></span>|[<span data-ttu-id="51440-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-217">このユーザー権利では、プロセスでは、内部の API を使用して、アクセス トークンを作成するときに、ローカル リソースへのアクセスを取得するために使用するトークンを作成するプロセスにするユーザーまたはグループを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="51440-218">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="51440-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="51440-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-221">このユーザー権利は、ユーザーが任意のプロセスまたはカーネルにデバッガーをアタッチできるを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="51440-222">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="51440-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="51440-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="51440-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-225">このユーザー権利では、リモート デスクトップ サービス クライアントとしてログオン拒否するユーザーとグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="51440-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="51440-226">NotConfigured および受信拒否の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="51440-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="51440-227">userRightsDelegation</span></span>|[<span data-ttu-id="51440-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-229">このユーザー権利は、ユーザーまたはコンピューター オブジェクトの委任に対して信頼されるように設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="51440-230">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="51440-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="51440-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-233">このユーザー権利では、セキュリティ ログにエントリを追加するのにはプロセスが使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="51440-234">セキュリティ ログは、承認されていないシステムへのアクセスを追跡に使用します。</span><span class="sxs-lookup"><span data-stu-id="51440-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="51440-235">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="51440-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="51440-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-238">ユーザーには、このユーザー権利を割り当てるには、クライアントを偽装するには、そのユーザーに代わって実行されるプログラムすることができます。</span><span class="sxs-lookup"><span data-stu-id="51440-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="51440-239">により承認されていないユーザーが自分が作成したサービスに接続するクライアントを納得させることと、偽装して、クライアントに許可されていないユーザーのアクセス許可を昇格させるという、この種の偽装にこのユーザー権利を必要とします。管理者レベルまたはシステム レベル。</span><span class="sxs-lookup"><span data-stu-id="51440-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="51440-240">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="51440-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="51440-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-243">このユーザー権利は、取引先企業は他のプロセスに割り当てられている実行の優先順位を上げる別のプロセスに対するプロパティの書き込みアクセスを持つプロセスを使用することができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="51440-244">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="51440-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="51440-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-247">このユーザー権利は、ユーザーが動的にロードおよびデバイス ドライバーやカーネル モードでは、他のコードをアンロードするを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="51440-248">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="51440-249">userRightsLockMemory</span></span>|[<span data-ttu-id="51440-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-251">このユーザー権利では、ディスク上の仮想メモリを物理メモリにデータを保持するプロセスを使用できるアカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="51440-252">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="51440-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="51440-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-255">このユーザー権利は、オブジェクト アクセスの監査ファイル、Active Directory オブジェクト、レジストリ キーなどの個々 のリソースのオプションを指定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="51440-256">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="51440-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="51440-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-259">このユーザー権利では、リモート最適化などのボリュームの保守タスクを実行できるユーザーおよびグループを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="51440-260">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="51440-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="51440-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-263">このユーザー権利では、ファームウェアの環境値を変更できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="51440-264">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="51440-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="51440-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-267">このユーザー権利は、ユーザー アカウントは、ファイル、レジストリ キー、またはその他のユーザーが所有するプロセスなどのオブジェクトの整合性ラベルを変更できますを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="51440-268">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="51440-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="51440-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-271">このユーザー権利では、システム プロセスのパフォーマンスを監視するパフォーマンス監視ツールを使用できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="51440-272">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="51440-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="51440-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-275">このユーザー権利は、ネットワーク上のリモートの場所からコンピューターをシャット ダウンできるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="51440-276">このユーザー権利が誤用されると、サービス拒否攻撃があります。</span><span class="sxs-lookup"><span data-stu-id="51440-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="51440-277">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="51440-278">userRightsRestoreData</span></span>|[<span data-ttu-id="51440-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-280">このユーザー権利では、ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのファイルおよびディレクトリをバックアップ、復元するときのアクセス許可を回避できるユーザーを決定し、オブジェクトの所有者として有効なセキュリティ プリンシパルを設定できるユーザーを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="51440-281">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="51440-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="51440-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-284">所有権をユーザーのセキュリティ保護可能なオブジェクトの Active Directory オブジェクト、ファイル、フォルダー、プリンター、レジストリ キー、プロセス、およびスレッドを含め、システムでこのユーザー権利を決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="51440-285">NotConfigured と許可の状態のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="51440-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="51440-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="51440-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="51440-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="51440-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="51440-288">このセキュリティ設定は、サービスとしてプロセスを登録できないサービス アカウントを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="51440-289">注: このセキュリティ設定は、システム、ローカル サービス、またはネットワーク サービス アカウントには適用されません。</span><span class="sxs-lookup"><span data-stu-id="51440-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="51440-290">ブロックがサポートされているだけの状態です。</span><span class="sxs-lookup"><span data-stu-id="51440-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="51440-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="51440-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="51440-292">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-292">Boolean</span></span>|<span data-ttu-id="51440-293">この設定は、xbox ゲームの保存が有効 (1) または無効 (0) かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="51440-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="51440-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="51440-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="51440-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="51440-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="51440-296">この設定は、付属品の管理サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="51440-297">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="51440-297">Default: Manual.</span></span> <span data-ttu-id="51440-298">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="51440-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="51440-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="51440-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="51440-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="51440-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="51440-301">この設定は、認証マネージャーの Live サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="51440-302">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="51440-302">Default: Manual.</span></span> <span data-ttu-id="51440-303">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="51440-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="51440-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="51440-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="51440-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="51440-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="51440-306">保存サービスの開始のタイプのゲームのライブは Automatic(2)、Manual(3)、Disabled(4) であるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="51440-307">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="51440-307">Default: Manual.</span></span> <span data-ttu-id="51440-308">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="51440-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="51440-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="51440-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="51440-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="51440-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="51440-311">この設定は、ネットワーク サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="51440-312">既定: マニュアルです。</span><span class="sxs-lookup"><span data-stu-id="51440-312">Default: Manual.</span></span> <span data-ttu-id="51440-313">可能な値は、`manual`、`automatic`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="51440-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="51440-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="51440-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="51440-315">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-315">Boolean</span></span>|<span data-ttu-id="51440-316">ユーザーがこのコンピューターに Microsoft の新しいアカウントを追加するを防ぐ。</span><span class="sxs-lookup"><span data-stu-id="51440-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="51440-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="51440-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="51440-318">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-318">Boolean</span></span>|<span data-ttu-id="51440-319">物理デバイス以外の場所からのログオンにパスワードで保護していないローカルのアカウントを有効にします。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="51440-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="51440-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="51440-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="51440-321">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-321">Boolean</span></span>|<span data-ttu-id="51440-322">ローカル管理者アカウントを有効または無効にするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="51440-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="51440-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="51440-324">String</span><span class="sxs-lookup"><span data-stu-id="51440-324">String</span></span>|<span data-ttu-id="51440-325">"Administrator"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="51440-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="51440-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="51440-327">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-327">Boolean</span></span>|<span data-ttu-id="51440-328">Guest アカウントが有効か無効になっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="51440-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="51440-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="51440-330">String</span><span class="sxs-lookup"><span data-stu-id="51440-330">String</span></span>|<span data-ttu-id="51440-331">"Guest"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="51440-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="51440-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="51440-333">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-333">Boolean</span></span>|<span data-ttu-id="51440-334">ポータブル コンピューターを防ぐため、ログインしなくても接続されているからです。</span><span class="sxs-lookup"><span data-stu-id="51440-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="51440-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="51440-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="51440-336">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-336">Boolean</span></span>|<span data-ttu-id="51440-337">管理者だけが使用する共有プリンターへの接続の一部としてプリンター ドライバーをインストールを制限します。</span><span class="sxs-lookup"><span data-stu-id="51440-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="51440-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="51440-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="51440-339">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-339">Boolean</span></span>|<span data-ttu-id="51440-340">CD-ROM メディアにアクセスする唯一の対話形式でログオンしているユーザーは、この設定を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="51440-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="51440-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="51440-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="51440-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="51440-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="51440-343">リムーバブル NTFS メディアを取り出すことができるユーザーを定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="51440-344">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="51440-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="51440-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="51440-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="51440-346">Int32</span><span class="sxs-lookup"><span data-stu-id="51440-346">Int32</span></span>|<span data-ttu-id="51440-347">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="51440-348">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="51440-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="51440-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="51440-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="51440-350">Int32</span><span class="sxs-lookup"><span data-stu-id="51440-350">Int32</span></span>|<span data-ttu-id="51440-351">対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="51440-352">有効な値の 0 から 9999 まで</span><span class="sxs-lookup"><span data-stu-id="51440-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="51440-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="51440-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="51440-354">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-354">Boolean</span></span>|<span data-ttu-id="51440-355">CTRL + ALT + DEL を押す前に、ユーザーがログオンできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="51440-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="51440-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="51440-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="51440-357">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-357">Boolean</span></span>|<span data-ttu-id="51440-358">このデバイス上で最後署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="51440-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="51440-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="51440-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="51440-360">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-360">Boolean</span></span>|<span data-ttu-id="51440-361">資格情報を入力した後、デバイスのデスクトップが表示される前にこのデバイスに署名した人のユーザー名は表示されません。</span><span class="sxs-lookup"><span data-stu-id="51440-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="51440-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="51440-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="51440-363">String</span><span class="sxs-lookup"><span data-stu-id="51440-363">String</span></span>|<span data-ttu-id="51440-364">ログオン ユーザーのメッセージのタイトルを設定します。</span><span class="sxs-lookup"><span data-stu-id="51440-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="51440-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="51440-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="51440-366">String</span><span class="sxs-lookup"><span data-stu-id="51440-366">String</span></span>|<span data-ttu-id="51440-367">ログオン ユーザーのメッセージ テキストを設定します。</span><span class="sxs-lookup"><span data-stu-id="51440-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="51440-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="51440-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="51440-369">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-369">Boolean</span></span>|<span data-ttu-id="51440-370">ブロック PKU2U 認証要求をこのデバイスにオンライン id を使用します。</span><span class="sxs-lookup"><span data-stu-id="51440-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="51440-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="51440-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="51440-372">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-372">Boolean</span></span>|<span data-ttu-id="51440-373">UI ヘルパー LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティのブール値</span><span class="sxs-lookup"><span data-stu-id="51440-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="51440-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="51440-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="51440-375">String</span><span class="sxs-lookup"><span data-stu-id="51440-375">String</span></span>|<span data-ttu-id="51440-376">または、SAM にリモート呼び出しを行うには、ユーザーとグループを拒否する既定のセキュリティ記述子定義言語の文字列を編集します。</span><span class="sxs-lookup"><span data-stu-id="51440-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="51440-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="51440-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="51440-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="51440-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="51440-379">このセキュリティ設定では、クライアントが 128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とすることができます。</span><span class="sxs-lookup"><span data-stu-id="51440-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="51440-380">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="51440-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="51440-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="51440-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="51440-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="51440-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="51440-383">このセキュリティ設定は、128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とするサーバーです。</span><span class="sxs-lookup"><span data-stu-id="51440-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="51440-384">可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。</span><span class="sxs-lookup"><span data-stu-id="51440-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="51440-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="51440-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="51440-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="51440-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="51440-387">このセキュリティ設定は、ネットワーク ログオン時に使用するチャレンジ/レスポンス認証プロトコルを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="51440-388">使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="51440-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="51440-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="51440-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="51440-390">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-390">Boolean</span></span>|<span data-ttu-id="51440-391">有効な場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="51440-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="51440-392">構成されていない場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを拒否します。</span><span class="sxs-lookup"><span data-stu-id="51440-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="51440-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="51440-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="51440-394">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-394">Boolean</span></span>|<span data-ttu-id="51440-395">このセキュリティ設定は、システムのシャット ダウン時に仮想メモリのページファイルがオフになっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="51440-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="51440-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="51440-397">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-397">Boolean</span></span>|<span data-ttu-id="51440-398">このセキュリティ設定は、Windows にログオンしなくてもコンピューターをシャット ダウンできるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="51440-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="51440-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="51440-400">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-400">Boolean</span></span>|<span data-ttu-id="51440-401">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="51440-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="51440-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="51440-403">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-403">Boolean</span></span>|<span data-ttu-id="51440-404">ファイルとレジストリの書き込みエラーをユーザーの場所ごとに仮想化します。</span><span class="sxs-lookup"><span data-stu-id="51440-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="51440-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="51440-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="51440-406">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-406">Boolean</span></span>|<span data-ttu-id="51440-407">実行が許可される前に、実行可能ファイルに、PKI 証明書パス検証を強制します。</span><span class="sxs-lookup"><span data-stu-id="51440-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="51440-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="51440-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="51440-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="51440-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="51440-410">管理者承認モードでは、管理者に対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="51440-411">可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。</span><span class="sxs-lookup"><span data-stu-id="51440-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="51440-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="51440-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="51440-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="51440-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="51440-414">標準ユーザーに対する昇格時のプロンプトの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="51440-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="51440-415">可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。</span><span class="sxs-lookup"><span data-stu-id="51440-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="51440-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="51440-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="51440-417">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-417">Boolean</span></span>|<span data-ttu-id="51440-418">セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップに移動するすべての昇格要求を有効にします。</span><span class="sxs-lookup"><span data-stu-id="51440-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="51440-419">管理者および標準ユーザーに対するプロンプトの動作ポリシー設定が使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="51440-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="51440-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="51440-421">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-421">Boolean</span></span>|<span data-ttu-id="51440-422">システム特権を必要とするアプリケーションのインストールは、管理者の資格情報を求められます。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="51440-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="51440-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="51440-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="51440-424">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-424">Boolean</span></span>|<span data-ttu-id="51440-425">UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="51440-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="51440-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="51440-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="51440-427">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-427">Boolean</span></span>|<span data-ttu-id="51440-428">ビルトイン管理者アカウントが管理者承認モードを使用して、または完全な管理者特権を持つすべてのアプリケーションを実行するかどうかを定義します。既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="51440-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="51440-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="51440-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="51440-430">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-430">Boolean</span></span>|<span data-ttu-id="51440-431">管理者承認モードおよびすべての UAC ポリシー設定を有効にするかどうかを定義する既定値が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="51440-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="51440-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="51440-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="51440-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="51440-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="51440-434">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="51440-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="51440-435">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="51440-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="51440-436">可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。</span><span class="sxs-lookup"><span data-stu-id="51440-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="51440-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="51440-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="51440-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="51440-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="51440-439">セッションがロックされているときに表示されるユーザー情報を構成します。</span><span class="sxs-lookup"><span data-stu-id="51440-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="51440-440">構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="51440-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="51440-441">可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。</span><span class="sxs-lookup"><span data-stu-id="51440-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="51440-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="51440-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="51440-443">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-443">Boolean</span></span>|<span data-ttu-id="51440-444">このセキュリティ設定は、SMB クライアントが SMB パケット署名をネゴシエートしようとしたかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="51440-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="51440-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="51440-446">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-446">Boolean</span></span>|<span data-ttu-id="51440-447">このセキュリティ設定は、SMB クライアント コンポーネントでパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="51440-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="51440-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="51440-449">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-449">Boolean</span></span>|<span data-ttu-id="51440-450">このセキュリティ設定が有効の場合、サーバー メッセージ ブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしない Microsoft 以外の SMB サーバーにプレーン テキスト パスワードを送信するのには。</span><span class="sxs-lookup"><span data-stu-id="51440-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="51440-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="51440-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="51440-452">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-452">Boolean</span></span>|<span data-ttu-id="51440-453">このセキュリティ設定は、SMB サーバー コンポーネントがパケット署名が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="51440-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="51440-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="51440-455">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-455">Boolean</span></span>|<span data-ttu-id="51440-456">このセキュリティ設定は、SMB サーバーが SMB パケット署名を要求するクライアントをネゴシエートするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="51440-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="51440-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="51440-458">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-458">Boolean</span></span>|<span data-ttu-id="51440-459">既定では、このセキュリティ設定は共有とパイプは匿名でアクセスできる名前付きパイプおよび匿名でアクセスできる共有の設定に匿名アクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="51440-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="51440-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="51440-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="51440-461">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-461">Boolean</span></span>|<span data-ttu-id="51440-462">このセキュリティ設定は、どのような追加のアクセス許可をコンピューターへの匿名接続を許可しますを指定します。</span><span class="sxs-lookup"><span data-stu-id="51440-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="51440-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="51440-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="51440-464">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-464">Boolean</span></span>|<span data-ttu-id="51440-465">このセキュリティ設定は、ドメイン アカウントやネットワーク共有の名前の列挙など、特定の操作を実行するのには匿名ユーザーを許可するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="51440-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="51440-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="51440-467">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-467">Boolean</span></span>|<span data-ttu-id="51440-468">このセキュリティ設定は、かどうかは、次のパスワードの変更で新しいパスワードの LAN Manager (LM) ハッシュ値が格納されているを決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="51440-469">既定では格納されません。</span><span class="sxs-lookup"><span data-stu-id="51440-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="51440-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="51440-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="51440-471">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="51440-471">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="51440-472">このセキュリティ設定は、ユーザーのログオン用のスマート カードがスマート カード リーダーから削除されたときの動作を決定します。</span><span class="sxs-lookup"><span data-stu-id="51440-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="51440-473">可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。</span><span class="sxs-lookup"><span data-stu-id="51440-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="51440-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="51440-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="51440-475">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-475">Boolean</span></span>|<span data-ttu-id="51440-476">アプリケーションとブラウザーの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="51440-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="51440-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="51440-478">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-478">Boolean</span></span>|<span data-ttu-id="51440-479">ファミリのオプション領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="51440-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="51440-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="51440-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="51440-481">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-481">Boolean</span></span>|<span data-ttu-id="51440-482">デバイスのパフォーマンスと稼働状態の領域の表示を無効にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="51440-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="51440-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="51440-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="51440-484">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-484">Boolean</span></span>|<span data-ttu-id="51440-485">ファイアウォールとネットワークの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="51440-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="51440-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="51440-487">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-487">Boolean</span></span>|<span data-ttu-id="51440-488">ウイルスと脅威の保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="51440-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="51440-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="51440-490">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-490">Boolean</span></span>|<span data-ttu-id="51440-491">アカウントの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="51440-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="51440-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="51440-493">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-493">Boolean</span></span>|<span data-ttu-id="51440-494">ハードウェアの保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="51440-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="51440-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="51440-496">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-496">Boolean</span></span>|<span data-ttu-id="51440-497">Ransomware 保護領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="51440-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="51440-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="51440-499">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-499">Boolean</span></span>|<span data-ttu-id="51440-500">[デバイスのセキュリティ、セキュリティで保護されたブート領域の表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="51440-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="51440-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="51440-502">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-502">Boolean</span></span>|<span data-ttu-id="51440-503">[デバイスのセキュリティのトラブルシューティング、セキュリティ プロセスの表示を無効にする場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="51440-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="51440-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="51440-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="51440-505">String</span><span class="sxs-lookup"><span data-stu-id="51440-505">String</span></span>|<span data-ttu-id="51440-506">ユーザーに表示される会社名です。</span><span class="sxs-lookup"><span data-stu-id="51440-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="51440-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="51440-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="51440-508">String</span><span class="sxs-lookup"><span data-stu-id="51440-508">String</span></span>|<span data-ttu-id="51440-509">ユーザーに表示される電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="51440-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="51440-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="51440-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="51440-511">String</span><span class="sxs-lookup"><span data-stu-id="51440-511">String</span></span>|<span data-ttu-id="51440-512">電話番号または Skype ID のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="51440-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="51440-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="51440-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="51440-514">String</span><span class="sxs-lookup"><span data-stu-id="51440-514">String</span></span>|<span data-ttu-id="51440-515">ヘルプ ポータルの URL をユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="51440-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="51440-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="51440-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="51440-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="51440-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="51440-518">アプリケーションの表示領域を表示するのに通知します。</span><span class="sxs-lookup"><span data-stu-id="51440-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="51440-519">可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="51440-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="51440-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="51440-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="51440-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="51440-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="51440-522">IT の連絡先を表示する場所を構成するエンド ・ ユーザーへの情報です。</span><span class="sxs-lookup"><span data-stu-id="51440-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="51440-523">可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。</span><span class="sxs-lookup"><span data-stu-id="51440-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="51440-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="51440-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="51440-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-525">Boolean</span></span>|<span data-ttu-id="51440-526">デバイスへのステートフル FTP 接続をブロックします</span><span class="sxs-lookup"><span data-stu-id="51440-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="51440-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="51440-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="51440-528">Int32</span><span class="sxs-lookup"><span data-stu-id="51440-528">Int32</span></span>|<span data-ttu-id="51440-529">セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。</span><span class="sxs-lookup"><span data-stu-id="51440-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="51440-530">これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。</span><span class="sxs-lookup"><span data-stu-id="51440-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="51440-531">有効な値は 300 から 3600 までです</span><span class="sxs-lookup"><span data-stu-id="51440-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="51440-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="51440-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="51440-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="51440-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="51440-534">事前共有キーを使用するエンコーディングを選択します。</span><span class="sxs-lookup"><span data-stu-id="51440-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="51440-535">可能な値は、`deviceDefault`、`none`、`utF8` です。</span><span class="sxs-lookup"><span data-stu-id="51440-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="51440-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="51440-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="51440-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-537">Boolean</span></span>|<span data-ttu-id="51440-538">IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="51440-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="51440-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="51440-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="51440-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-540">Boolean</span></span>|<span data-ttu-id="51440-541">IPSec 除外を構成し、ICMP を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="51440-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="51440-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="51440-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-543">Boolean</span></span>|<span data-ttu-id="51440-544">IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します</span><span class="sxs-lookup"><span data-stu-id="51440-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="51440-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="51440-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="51440-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-546">Boolean</span></span>|<span data-ttu-id="51440-547">IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します</span><span class="sxs-lookup"><span data-stu-id="51440-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="51440-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="51440-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="51440-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="51440-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="51440-550">証明書失効リストを適用する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="51440-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="51440-551">可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。</span><span class="sxs-lookup"><span data-stu-id="51440-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="51440-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="51440-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="51440-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-553">Boolean</span></span>|<span data-ttu-id="51440-554">認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します</span><span class="sxs-lookup"><span data-stu-id="51440-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="51440-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="51440-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="51440-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="51440-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="51440-557">トンネルのゲートウェイでパケットのキューイングを適用する方法を構成します。</span><span class="sxs-lookup"><span data-stu-id="51440-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="51440-558">可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。</span><span class="sxs-lookup"><span data-stu-id="51440-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="51440-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="51440-559">firewallProfileDomain</span></span>|[<span data-ttu-id="51440-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="51440-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="51440-561">ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="51440-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="51440-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="51440-562">firewallProfilePublic</span></span>|[<span data-ttu-id="51440-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="51440-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="51440-564">パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="51440-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="51440-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="51440-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="51440-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="51440-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="51440-567">プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します</span><span class="sxs-lookup"><span data-stu-id="51440-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="51440-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="51440-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="51440-569">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51440-569">String collection</span></span>|<span data-ttu-id="51440-570">攻撃回避規則から除外する exe ファイルとフォルダーのリスト</span><span class="sxs-lookup"><span data-stu-id="51440-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="51440-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="51440-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="51440-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-573">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="51440-574">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="51440-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="51440-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-577">他のプロセス内に挿入する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="51440-578">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="51440-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="51440-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-581">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="51440-582">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="51440-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="51440-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-585">Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="51440-586">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="51440-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="51440-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-589">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="51440-590">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="51440-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="51440-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-593">子プロセスを起動する Office アプリケーションの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="51440-594">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="51440-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="51440-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-597">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="51440-598">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="51440-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="51440-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-601">Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="51440-602">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="51440-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="51440-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-605">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="51440-606">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="51440-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="51440-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-609">Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="51440-610">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="51440-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="51440-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-613">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="51440-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="51440-614">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="51440-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="51440-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-617">Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="51440-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="51440-618">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="51440-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="51440-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-621">資格情報が Windows のローカル セキュリティ機関サブシステムから盗むことが許可されているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="51440-622">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="51440-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="51440-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-625">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="51440-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="51440-626">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="51440-627">defenderProcessCreation</span></span>|[<span data-ttu-id="51440-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-629">PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。</span><span class="sxs-lookup"><span data-stu-id="51440-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="51440-630">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="51440-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="51440-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-633">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="51440-634">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="51440-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="51440-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-637">USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="51440-638">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="51440-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="51440-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-641">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="51440-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="51440-642">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="51440-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="51440-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-645">蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。</span><span class="sxs-lookup"><span data-stu-id="51440-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="51440-646">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="51440-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="51440-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="51440-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="51440-649">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="51440-650">可能な値は、`userDefined`、`block`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="51440-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="51440-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-653">メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="51440-654">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="51440-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-657">Ransomeware に対して高度な保護の使用を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="51440-658">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="51440-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="51440-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="51440-661">保護されたフォルダーの動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="51440-662">可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。</span><span class="sxs-lookup"><span data-stu-id="51440-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="51440-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="51440-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="51440-664">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51440-664">String collection</span></span>|<span data-ttu-id="51440-665">保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト</span><span class="sxs-lookup"><span data-stu-id="51440-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="51440-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="51440-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="51440-667">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51440-667">String collection</span></span>|<span data-ttu-id="51440-668">保護されたフォルダーのリストに追加されるフォルダー パスのリスト</span><span class="sxs-lookup"><span data-stu-id="51440-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="51440-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="51440-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="51440-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="51440-671">NetworkProtection の動作を示す値です。</span><span class="sxs-lookup"><span data-stu-id="51440-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="51440-672">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="51440-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="51440-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="51440-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="51440-674">Binary</span><span class="sxs-lookup"><span data-stu-id="51440-674">Binary</span></span>|<span data-ttu-id="51440-675">Exploit Protection の詳細に関する情報を含む XML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="51440-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="51440-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="51440-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="51440-677">String</span><span class="sxs-lookup"><span data-stu-id="51440-677">String</span></span>|<span data-ttu-id="51440-678">DefenderExploitProtectionXml の取得元となるファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="51440-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="51440-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="51440-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="51440-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-680">Boolean</span></span>|<span data-ttu-id="51440-681">ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="51440-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="51440-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="51440-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="51440-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="51440-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="51440-684">管理者がデバイスで許可するアプリの種類を選択できるようにします。</span><span class="sxs-lookup"><span data-stu-id="51440-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="51440-685">可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。</span><span class="sxs-lookup"><span data-stu-id="51440-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="51440-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="51440-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="51440-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="51440-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="51440-688">プラットフォームのセキュリティ レベルとセキュリティで保護されたブートし、仮想化ベースのセキュリティの両方が有効である場合は、資格情報の保護にします。</span><span class="sxs-lookup"><span data-stu-id="51440-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="51440-689">可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。</span><span class="sxs-lookup"><span data-stu-id="51440-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="51440-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="51440-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="51440-691">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-691">Boolean</span></span>|<span data-ttu-id="51440-692">Security(VBS) を仮想化をオンに基づいています。</span><span class="sxs-lookup"><span data-stu-id="51440-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="51440-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="51440-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="51440-694">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-694">Boolean</span></span>|<span data-ttu-id="51440-695">プラットフォームのセキュリティ レベルが次の再起動時に有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="51440-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="51440-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="51440-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="51440-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-697">Boolean</span></span>|<span data-ttu-id="51440-698">IT 管理者が Windows 用の SmartScreen を構成することを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="51440-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="51440-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="51440-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-700">Boolean</span></span>|<span data-ttu-id="51440-701">ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="51440-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="51440-702">applicationGuardEnabled</span></span>|<span data-ttu-id="51440-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-703">Boolean</span></span>|<span data-ttu-id="51440-704">Windows Defender Application Guard を有効にします</span><span class="sxs-lookup"><span data-stu-id="51440-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="51440-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="51440-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="51440-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="51440-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="51440-707">新しい Windows のビルドの Windows Defender のアプリケーション保護を有効にします。</span><span class="sxs-lookup"><span data-stu-id="51440-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="51440-708">可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。</span><span class="sxs-lookup"><span data-stu-id="51440-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="51440-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="51440-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="51440-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="51440-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="51440-711">イメージ ファイルの転送、テキスト ファイルのいずれかにクリップボードをブロックします。</span><span class="sxs-lookup"><span data-stu-id="51440-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="51440-712">可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。</span><span class="sxs-lookup"><span data-stu-id="51440-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="51440-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="51440-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="51440-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-714">Boolean</span></span>|<span data-ttu-id="51440-715">サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします</span><span class="sxs-lookup"><span data-stu-id="51440-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="51440-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="51440-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="51440-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-717">Boolean</span></span>|<span data-ttu-id="51440-718">App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="51440-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="51440-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="51440-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-720">Boolean</span></span>|<span data-ttu-id="51440-721">監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます</span><span class="sxs-lookup"><span data-stu-id="51440-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="51440-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="51440-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="51440-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="51440-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="51440-724">ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。</span><span class="sxs-lookup"><span data-stu-id="51440-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="51440-725">可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。</span><span class="sxs-lookup"><span data-stu-id="51440-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="51440-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="51440-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="51440-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-727">Boolean</span></span>|<span data-ttu-id="51440-728">コンテナーから PDF への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="51440-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="51440-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="51440-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-730">Boolean</span></span>|<span data-ttu-id="51440-731">コンテナーから XPS への出力を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="51440-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="51440-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="51440-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-733">Boolean</span></span>|<span data-ttu-id="51440-734">コンテナーからローカル プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="51440-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="51440-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="51440-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-736">Boolean</span></span>|<span data-ttu-id="51440-737">コンテナーからネットワーク プリンターへの出力を許可します</span><span class="sxs-lookup"><span data-stu-id="51440-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="51440-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="51440-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="51440-739">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-739">Boolean</span></span>|<span data-ttu-id="51440-740">仮想 GPU を使用するアプリケーションの保護を許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="51440-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="51440-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="51440-742">ブール型</span><span class="sxs-lookup"><span data-stu-id="51440-742">Boolean</span></span>|<span data-ttu-id="51440-743">アプリケーション ガード コンテナーの端からファイルをダウンロードし、ホスト上でファイル システムを保存するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="51440-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="51440-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="51440-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-745">Boolean</span></span>|<span data-ttu-id="51440-746">管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="51440-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="51440-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="51440-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-748">Boolean</span></span>|<span data-ttu-id="51440-749">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="51440-750">このポリシーは、モバイルの SKU に対してのみ有効です。
</span><span class="sxs-lookup"><span data-stu-id="51440-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="51440-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="51440-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="51440-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="51440-752">Boolean</span></span>|<span data-ttu-id="51440-753">管理者が BitLocker を使用して暗号化をオンにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="51440-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="51440-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="51440-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="51440-756">BitLocker のシステム ドライブのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="51440-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="51440-757">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-757">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="51440-758">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-758">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="51440-759">BitLocker は、ドライブのポリシーを修正します。</span><span class="sxs-lookup"><span data-stu-id="51440-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="51440-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="51440-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="51440-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="51440-762">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="51440-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="51440-763">応答</span><span class="sxs-lookup"><span data-stu-id="51440-763">Response</span></span>
<span data-ttu-id="51440-764">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51440-764">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51440-765">例</span><span class="sxs-lookup"><span data-stu-id="51440-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="51440-766">要求</span><span class="sxs-lookup"><span data-stu-id="51440-766">Request</span></span>
<span data-ttu-id="51440-767">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51440-767">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26312

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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

### <a name="response"></a><span data-ttu-id="51440-768">応答</span><span class="sxs-lookup"><span data-stu-id="51440-768">Response</span></span>
<span data-ttu-id="51440-p194">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51440-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26499

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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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





