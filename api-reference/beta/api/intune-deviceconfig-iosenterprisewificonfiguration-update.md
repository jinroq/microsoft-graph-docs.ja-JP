---
title: iosEnterpriseWiFiConfiguration の更新
description: iosEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47006811f38fb3bc35ac0df3d23d53ddc6c9ba36
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977220"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="a9f90-103">iosEnterpriseWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a9f90-103">Update iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="a9f90-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9f90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f90-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f90-106">[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-106">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9f90-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9f90-107">Prerequisites</span></span>
<span data-ttu-id="a9f90-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9f90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9f90-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9f90-110">Permission type</span></span>|<span data-ttu-id="a9f90-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9f90-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f90-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9f90-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f90-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f90-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9f90-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9f90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f90-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9f90-115">Not supported.</span></span>|
|<span data-ttu-id="a9f90-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9f90-116">Application</span></span>|<span data-ttu-id="a9f90-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9f90-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f90-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9f90-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a9f90-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9f90-119">Request headers</span></span>
|<span data-ttu-id="a9f90-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9f90-120">Header</span></span>|<span data-ttu-id="a9f90-121">値</span><span class="sxs-lookup"><span data-stu-id="a9f90-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f90-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f90-122">Authorization</span></span>|<span data-ttu-id="a9f90-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9f90-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a9f90-124">Accept</span></span>|<span data-ttu-id="a9f90-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f90-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f90-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9f90-126">Request body</span></span>
<span data-ttu-id="a9f90-127">要求本文で、 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-127">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="a9f90-128">次の表に、 [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-128">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="a9f90-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9f90-129">Property</span></span>|<span data-ttu-id="a9f90-130">型</span><span class="sxs-lookup"><span data-stu-id="a9f90-130">Type</span></span>|<span data-ttu-id="a9f90-131">説明</span><span class="sxs-lookup"><span data-stu-id="a9f90-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f90-132">id</span><span class="sxs-lookup"><span data-stu-id="a9f90-132">id</span></span>|<span data-ttu-id="a9f90-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a9f90-133">String</span></span>|<span data-ttu-id="a9f90-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a9f90-134">Key of the entity.</span></span> <span data-ttu-id="a9f90-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f90-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a9f90-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f90-137">DateTimeOffset</span></span>|<span data-ttu-id="a9f90-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a9f90-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a9f90-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9f90-140">roleScopeTagIds</span></span>|<span data-ttu-id="a9f90-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a9f90-141">String collection</span></span>|<span data-ttu-id="a9f90-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a9f90-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9f90-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9f90-144">supportsScopeTags</span></span>|<span data-ttu-id="a9f90-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f90-145">Boolean</span></span>|<span data-ttu-id="a9f90-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9f90-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a9f90-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9f90-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9f90-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-149">This property is read-only.</span></span> <span data-ttu-id="a9f90-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f90-151">createdDateTime</span></span>|<span data-ttu-id="a9f90-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f90-152">DateTimeOffset</span></span>|<span data-ttu-id="a9f90-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a9f90-153">DateTime the object was created.</span></span> <span data-ttu-id="a9f90-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-155">description</span><span class="sxs-lookup"><span data-stu-id="a9f90-155">description</span></span>|<span data-ttu-id="a9f90-156">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-156">String</span></span>|<span data-ttu-id="a9f90-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a9f90-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9f90-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a9f90-159">displayName</span></span>|<span data-ttu-id="a9f90-160">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-160">String</span></span>|<span data-ttu-id="a9f90-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a9f90-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9f90-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-163">version</span><span class="sxs-lookup"><span data-stu-id="a9f90-163">version</span></span>|<span data-ttu-id="a9f90-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f90-164">Int32</span></span>|<span data-ttu-id="a9f90-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a9f90-165">Version of the device configuration.</span></span> <span data-ttu-id="a9f90-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a9f90-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-167">networkname</span><span class="sxs-lookup"><span data-stu-id="a9f90-167">networkName</span></span>|<span data-ttu-id="a9f90-168">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-168">String</span></span>|<span data-ttu-id="a9f90-169">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="a9f90-169">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-170">ssid</span><span class="sxs-lookup"><span data-stu-id="a9f90-170">ssid</span></span>|<span data-ttu-id="a9f90-171">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-171">String</span></span>|<span data-ttu-id="a9f90-172">これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="a9f90-173">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-173">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-174">connectautomatically に</span><span class="sxs-lookup"><span data-stu-id="a9f90-174">connectAutomatically</span></span>|<span data-ttu-id="a9f90-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f90-175">Boolean</span></span>|<span data-ttu-id="a9f90-176">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a9f90-177">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="a9f90-178">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-178">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a9f90-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a9f90-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f90-180">Boolean</span></span>|<span data-ttu-id="a9f90-181">ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-181">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="a9f90-182">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="a9f90-183">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-183">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a9f90-184">wiFiSecurityType</span></span>|[<span data-ttu-id="a9f90-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a9f90-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="a9f90-186">wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a9f90-187">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-187">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="a9f90-188">可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="a9f90-189">proxySettings</span><span class="sxs-lookup"><span data-stu-id="a9f90-189">proxySettings</span></span>|[<span data-ttu-id="a9f90-190">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="a9f90-190">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="a9f90-191">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されたこの wi-fi 接続のプロキシの種類。</span><span class="sxs-lookup"><span data-stu-id="a9f90-191">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="a9f90-192">使用可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-192">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="a9f90-193">proxymanualaddress</span><span class="sxs-lookup"><span data-stu-id="a9f90-193">proxyManualAddress</span></span>|<span data-ttu-id="a9f90-194">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-194">String</span></span>|<span data-ttu-id="a9f90-195">手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。</span><span class="sxs-lookup"><span data-stu-id="a9f90-195">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="a9f90-196">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-197">proxymanualport</span><span class="sxs-lookup"><span data-stu-id="a9f90-197">proxyManualPort</span></span>|<span data-ttu-id="a9f90-198">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f90-198">Int32</span></span>|<span data-ttu-id="a9f90-199">手動構成が選択されている場合のプロキシサーバーのポート。</span><span class="sxs-lookup"><span data-stu-id="a9f90-199">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="a9f90-200">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-201">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a9f90-201">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a9f90-202">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-202">String</span></span>|<span data-ttu-id="a9f90-203">自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。</span><span class="sxs-lookup"><span data-stu-id="a9f90-203">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="a9f90-204">この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-204">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="a9f90-205">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-205">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-206">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a9f90-206">preSharedKey</span></span>|<span data-ttu-id="a9f90-207">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-207">String</span></span>|<span data-ttu-id="a9f90-208">これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="a9f90-208">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="a9f90-209">[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="a9f90-210">eaptype</span><span class="sxs-lookup"><span data-stu-id="a9f90-210">eapType</span></span>|[<span data-ttu-id="a9f90-211">eaptype</span><span class="sxs-lookup"><span data-stu-id="a9f90-211">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="a9f90-212">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="a9f90-212">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="a9f90-213">wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-213">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="a9f90-214">可能な値は `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-214">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="a9f90-215">eapfastconfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f90-215">eapFastConfiguration</span></span>|[<span data-ttu-id="a9f90-216">eapfastconfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f90-216">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="a9f90-217">eap-fast が選択した eap の種類の場合、eap-fast 構成オプション。</span><span class="sxs-lookup"><span data-stu-id="a9f90-217">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="a9f90-218">可能な値は、`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-218">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="a9f90-219">trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="a9f90-219">trustedServerCertificateNames</span></span>|<span data-ttu-id="a9f90-220">String collection</span><span class="sxs-lookup"><span data-stu-id="a9f90-220">String collection</span></span>|<span data-ttu-id="a9f90-221">eap の種類が eap-tls/TTLS/ファストまたは PEAP に構成されている場合の、信頼されたサーバー証明書の名前。</span><span class="sxs-lookup"><span data-stu-id="a9f90-221">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="a9f90-222">これは、信頼できる証明機関 (CA) によって発行された証明書で使用される一般的な名前です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-222">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="a9f90-223">この情報を指定すると、エンドユーザーがこの wi-fi ネットワークに接続したときに、エンドユーザーのデバイスに表示される [動的信頼] ダイアログをバイパスすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-223">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="a9f90-224">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a9f90-224">authenticationMethod</span></span>|[<span data-ttu-id="a9f90-225">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a9f90-225">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="a9f90-226">eap の種類が PEAP または eap-tls に構成されている場合の認証方法。</span><span class="sxs-lookup"><span data-stu-id="a9f90-226">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="a9f90-227">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-227">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="a9f90-228">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="a9f90-228">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="a9f90-229">none apauthenticationmethod_ apttlstype</span><span class="sxs-lookup"><span data-stu-id="a9f90-229">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="a9f90-230">eap の種類が eap-tls で、Authenticationmethod がユーザー名とパスワードの場合に認証を行うための非 EAP メソッド。</span><span class="sxs-lookup"><span data-stu-id="a9f90-230">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="a9f90-231">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-231">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a9f90-232">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="a9f90-232">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="a9f90-233">String</span><span class="sxs-lookup"><span data-stu-id="a9f90-233">String</span></span>|<span data-ttu-id="a9f90-234">eap の種類が eap-tls、eap-fast、または PEAP に構成されている場合は、id プライバシー (外部 id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a9f90-234">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="a9f90-235">このプロパティは、入力したテキストでユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="a9f90-235">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="a9f90-236">たとえば、' anonymous ' を使用すると、この wi-fi 接続で実際のユーザー名を使用して認証する各ユーザーは、' anonymous ' と表示されます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-236">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="a9f90-237">応答</span><span class="sxs-lookup"><span data-stu-id="a9f90-237">Response</span></span>
<span data-ttu-id="a9f90-238">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9f90-238">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f90-239">例</span><span class="sxs-lookup"><span data-stu-id="a9f90-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9f90-240">要求</span><span class="sxs-lookup"><span data-stu-id="a9f90-240">Request</span></span>
<span data-ttu-id="a9f90-241">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9f90-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="a9f90-242">応答</span><span class="sxs-lookup"><span data-stu-id="a9f90-242">Response</span></span>
<span data-ttu-id="a9f90-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9f90-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




