---
title: IosWiFiConfiguration を更新します。
description: IosWiFiConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2ee5442dab64ef2d8d11d06ef16e439110ccc03
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393096"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="c4a83-103">IosWiFiConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="c4a83-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4a83-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4a83-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4a83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4a83-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4a83-107">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4a83-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4a83-108">Prerequisites</span></span>
<span data-ttu-id="c4a83-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4a83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4a83-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4a83-111">Permission type</span></span>|<span data-ttu-id="c4a83-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4a83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a83-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4a83-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a83-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4a83-116">Not supported.</span></span>|
|<span data-ttu-id="c4a83-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4a83-117">Application</span></span>|<span data-ttu-id="c4a83-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4a83-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a83-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4a83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c4a83-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a83-120">Request headers</span></span>
|<span data-ttu-id="c4a83-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a83-121">Header</span></span>|<span data-ttu-id="c4a83-122">値</span><span class="sxs-lookup"><span data-stu-id="c4a83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4a83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4a83-123">Authorization</span></span>|<span data-ttu-id="c4a83-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c4a83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4a83-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4a83-125">Accept</span></span>|<span data-ttu-id="c4a83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4a83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a83-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4a83-127">Request body</span></span>
<span data-ttu-id="c4a83-128">要求の本文に[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="c4a83-129">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="c4a83-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4a83-130">Property</span></span>|<span data-ttu-id="c4a83-131">型</span><span class="sxs-lookup"><span data-stu-id="c4a83-131">Type</span></span>|<span data-ttu-id="c4a83-132">説明</span><span class="sxs-lookup"><span data-stu-id="c4a83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4a83-133">id</span><span class="sxs-lookup"><span data-stu-id="c4a83-133">id</span></span>|<span data-ttu-id="c4a83-134">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-134">String</span></span>|<span data-ttu-id="c4a83-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c4a83-135">Key of the entity.</span></span> <span data-ttu-id="c4a83-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a83-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c4a83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a83-138">DateTimeOffset</span></span>|<span data-ttu-id="c4a83-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c4a83-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c4a83-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4a83-141">roleScopeTagIds</span></span>|<span data-ttu-id="c4a83-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c4a83-142">String collection</span></span>|<span data-ttu-id="c4a83-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c4a83-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4a83-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4a83-145">supportsScopeTags</span></span>|<span data-ttu-id="c4a83-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4a83-146">Boolean</span></span>|<span data-ttu-id="c4a83-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4a83-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c4a83-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4a83-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="c4a83-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4a83-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-150">This property is read-only.</span></span> <span data-ttu-id="c4a83-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4a83-152">createdDateTime</span></span>|<span data-ttu-id="c4a83-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4a83-153">DateTimeOffset</span></span>|<span data-ttu-id="c4a83-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c4a83-154">DateTime the object was created.</span></span> <span data-ttu-id="c4a83-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-156">説明</span><span class="sxs-lookup"><span data-stu-id="c4a83-156">description</span></span>|<span data-ttu-id="c4a83-157">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-157">String</span></span>|<span data-ttu-id="c4a83-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c4a83-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4a83-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c4a83-160">displayName</span></span>|<span data-ttu-id="c4a83-161">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-161">String</span></span>|<span data-ttu-id="c4a83-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c4a83-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4a83-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-164">version</span><span class="sxs-lookup"><span data-stu-id="c4a83-164">version</span></span>|<span data-ttu-id="c4a83-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c4a83-165">Int32</span></span>|<span data-ttu-id="c4a83-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c4a83-166">Version of the device configuration.</span></span> <span data-ttu-id="c4a83-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c4a83-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4a83-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="c4a83-168">networkName</span></span>|<span data-ttu-id="c4a83-169">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-169">String</span></span>|<span data-ttu-id="c4a83-170">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="c4a83-170">Network Name</span></span>|
|<span data-ttu-id="c4a83-171">ssid</span><span class="sxs-lookup"><span data-stu-id="c4a83-171">ssid</span></span>|<span data-ttu-id="c4a83-172">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-172">String</span></span>|<span data-ttu-id="c4a83-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="c4a83-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c4a83-174">connectAutomatically</span></span>|<span data-ttu-id="c4a83-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4a83-175">Boolean</span></span>|<span data-ttu-id="c4a83-176">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c4a83-177">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="c4a83-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c4a83-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c4a83-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4a83-179">Boolean</span></span>|<span data-ttu-id="c4a83-180">ネットワーク名 (SSID) をブロードキャストしていないときに接続します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="c4a83-181">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="c4a83-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4a83-182">wiFiSecurityType</span></span>|[<span data-ttu-id="c4a83-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c4a83-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c4a83-184">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4a83-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c4a83-185">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="c4a83-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c4a83-186">型のオブジェクトで</span><span class="sxs-lookup"><span data-stu-id="c4a83-186">proxySettings</span></span>|[<span data-ttu-id="c4a83-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="c4a83-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c4a83-188">この Wi-fi 接続のプロキシの種類です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="c4a83-189">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c4a83-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="c4a83-190">proxyManualAddress</span></span>|<span data-ttu-id="c4a83-191">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-191">String</span></span>|<span data-ttu-id="c4a83-192">手動の構成が選択されている時にプロキシ サーバーの IP アドレスまたは DNS ホスト名</span><span class="sxs-lookup"><span data-stu-id="c4a83-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="c4a83-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="c4a83-193">proxyManualPort</span></span>|<span data-ttu-id="c4a83-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c4a83-194">Int32</span></span>|<span data-ttu-id="c4a83-195">手動の構成が選択されている時にプロキシ サーバーのポートです。</span><span class="sxs-lookup"><span data-stu-id="c4a83-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="c4a83-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="c4a83-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c4a83-197">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-197">String</span></span>|<span data-ttu-id="c4a83-198">自動構成を選択すると、プロキシ サーバーの自動構成スクリプトの URL です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="c4a83-199">この URL は、通常、PAC (プロキシの自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="c4a83-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c4a83-200">preSharedKey</span></span>|<span data-ttu-id="c4a83-201">String</span><span class="sxs-lookup"><span data-stu-id="c4a83-201">String</span></span>|<span data-ttu-id="c4a83-202">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="c4a83-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="c4a83-203">応答</span><span class="sxs-lookup"><span data-stu-id="c4a83-203">Response</span></span>
<span data-ttu-id="c4a83-204">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c4a83-204">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a83-205">例</span><span class="sxs-lookup"><span data-stu-id="c4a83-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a83-206">要求</span><span class="sxs-lookup"><span data-stu-id="c4a83-206">Request</span></span>
<span data-ttu-id="c4a83-207">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a83-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 675

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="c4a83-208">応答</span><span class="sxs-lookup"><span data-stu-id="c4a83-208">Response</span></span>
<span data-ttu-id="c4a83-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4a83-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```




