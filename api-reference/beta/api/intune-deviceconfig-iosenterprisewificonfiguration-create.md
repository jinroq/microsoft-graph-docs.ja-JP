---
title: IosEnterpriseWiFiConfiguration を作成します。
description: 新しい iosEnterpriseWiFiConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9017873be0175f08a17641787b3f84de2e3bc160
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881964"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="053f2-103">IosEnterpriseWiFiConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="053f2-103">Create iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="053f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="053f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="053f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="053f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="053f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="053f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="053f2-107">新しい[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="053f2-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="053f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="053f2-108">Prerequisites</span></span>
<span data-ttu-id="053f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="053f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="053f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="053f2-111">Permission type</span></span>|<span data-ttu-id="053f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="053f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="053f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="053f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="053f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="053f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="053f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="053f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="053f2-116">Not supported.</span></span>|
|<span data-ttu-id="053f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="053f2-117">Application</span></span>|<span data-ttu-id="053f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="053f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="053f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="053f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="053f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="053f2-120">Request headers</span></span>
|<span data-ttu-id="053f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="053f2-121">Header</span></span>|<span data-ttu-id="053f2-122">値</span><span class="sxs-lookup"><span data-stu-id="053f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="053f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="053f2-123">Authorization</span></span>|<span data-ttu-id="053f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="053f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="053f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="053f2-125">Accept</span></span>|<span data-ttu-id="053f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="053f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="053f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="053f2-127">Request body</span></span>
<span data-ttu-id="053f2-128">要求の本文に iosEnterpriseWiFiConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="053f2-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="053f2-129">次の表は、iosEnterpriseWiFiConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="053f2-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="053f2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="053f2-130">Property</span></span>|<span data-ttu-id="053f2-131">種類</span><span class="sxs-lookup"><span data-stu-id="053f2-131">Type</span></span>|<span data-ttu-id="053f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="053f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="053f2-133">ID</span><span class="sxs-lookup"><span data-stu-id="053f2-133">id</span></span>|<span data-ttu-id="053f2-134">String</span><span class="sxs-lookup"><span data-stu-id="053f2-134">String</span></span>|<span data-ttu-id="053f2-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="053f2-135">Key of the entity.</span></span> <span data-ttu-id="053f2-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="053f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="053f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="053f2-138">DateTimeOffset</span></span>|<span data-ttu-id="053f2-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="053f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="053f2-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="053f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="053f2-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="053f2-142">String collection</span></span>|<span data-ttu-id="053f2-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="053f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="053f2-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="053f2-145">supportsScopeTags</span></span>|<span data-ttu-id="053f2-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="053f2-146">Boolean</span></span>|<span data-ttu-id="053f2-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="053f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="053f2-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="053f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="053f2-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="053f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="053f2-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="053f2-150">This property is read-only.</span></span> <span data-ttu-id="053f2-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="053f2-152">createdDateTime</span></span>|<span data-ttu-id="053f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="053f2-153">DateTimeOffset</span></span>|<span data-ttu-id="053f2-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="053f2-154">DateTime the object was created.</span></span> <span data-ttu-id="053f2-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-156">説明</span><span class="sxs-lookup"><span data-stu-id="053f2-156">description</span></span>|<span data-ttu-id="053f2-157">String</span><span class="sxs-lookup"><span data-stu-id="053f2-157">String</span></span>|<span data-ttu-id="053f2-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="053f2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="053f2-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="053f2-160">displayName</span></span>|<span data-ttu-id="053f2-161">String</span><span class="sxs-lookup"><span data-stu-id="053f2-161">String</span></span>|<span data-ttu-id="053f2-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="053f2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="053f2-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-164">version</span><span class="sxs-lookup"><span data-stu-id="053f2-164">version</span></span>|<span data-ttu-id="053f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="053f2-165">Int32</span></span>|<span data-ttu-id="053f2-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="053f2-166">Version of the device configuration.</span></span> <span data-ttu-id="053f2-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="053f2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="053f2-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="053f2-168">networkName</span></span>|<span data-ttu-id="053f2-169">String</span><span class="sxs-lookup"><span data-stu-id="053f2-169">String</span></span>|<span data-ttu-id="053f2-170">ネットワーク名は、 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-170">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-171">ssid</span><span class="sxs-lookup"><span data-stu-id="053f2-171">ssid</span></span>|<span data-ttu-id="053f2-172">String</span><span class="sxs-lookup"><span data-stu-id="053f2-172">String</span></span>|<span data-ttu-id="053f2-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="053f2-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="053f2-174">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-174">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="053f2-175">connectAutomatically</span></span>|<span data-ttu-id="053f2-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="053f2-176">Boolean</span></span>|<span data-ttu-id="053f2-177">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="053f2-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="053f2-178">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="053f2-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="053f2-179">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-179">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="053f2-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="053f2-181">ブール型</span><span class="sxs-lookup"><span data-stu-id="053f2-181">Boolean</span></span>|<span data-ttu-id="053f2-182">ネットワーク名 (SSID) をブロードキャストしていないときに接続します。</span><span class="sxs-lookup"><span data-stu-id="053f2-182">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="053f2-183">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="053f2-183">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="053f2-184">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-184">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="053f2-185">wiFiSecurityType</span></span>|[<span data-ttu-id="053f2-186">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="053f2-186">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="053f2-187">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="053f2-187">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="053f2-188">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="053f2-188">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="053f2-189">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="053f2-189">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="053f2-190">型のオブジェクトで</span><span class="sxs-lookup"><span data-stu-id="053f2-190">proxySettings</span></span>|[<span data-ttu-id="053f2-191">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="053f2-191">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="053f2-192">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承される Wi-fi 接続のプロキシの種類です。</span><span class="sxs-lookup"><span data-stu-id="053f2-192">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="053f2-193">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="053f2-193">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="053f2-194">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="053f2-194">proxyManualAddress</span></span>|<span data-ttu-id="053f2-195">String</span><span class="sxs-lookup"><span data-stu-id="053f2-195">String</span></span>|<span data-ttu-id="053f2-196">手動の構成が選択されている時にプロキシ サーバーの IP アドレスまたは DNS ホスト名</span><span class="sxs-lookup"><span data-stu-id="053f2-196">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="053f2-197">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-197">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-198">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="053f2-198">proxyManualPort</span></span>|<span data-ttu-id="053f2-199">Int32</span><span class="sxs-lookup"><span data-stu-id="053f2-199">Int32</span></span>|<span data-ttu-id="053f2-200">手動の構成が選択されている時にプロキシ サーバーのポートです。</span><span class="sxs-lookup"><span data-stu-id="053f2-200">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="053f2-201">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-201">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-202">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="053f2-202">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="053f2-203">String</span><span class="sxs-lookup"><span data-stu-id="053f2-203">String</span></span>|<span data-ttu-id="053f2-204">自動構成を選択すると、プロキシ サーバーの自動構成スクリプトの URL です。</span><span class="sxs-lookup"><span data-stu-id="053f2-204">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="053f2-205">この URL は、通常、PAC (プロキシの自動構成) ファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="053f2-205">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="053f2-206">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-206">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-207">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="053f2-207">preSharedKey</span></span>|<span data-ttu-id="053f2-208">String</span><span class="sxs-lookup"><span data-stu-id="053f2-208">String</span></span>|<span data-ttu-id="053f2-209">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="053f2-209">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="053f2-210">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="053f2-210">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="053f2-211">eapType</span><span class="sxs-lookup"><span data-stu-id="053f2-211">eapType</span></span>|[<span data-ttu-id="053f2-212">eapType</span><span class="sxs-lookup"><span data-stu-id="053f2-212">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="053f2-213">拡張認証プロトコル (EAP) です。</span><span class="sxs-lookup"><span data-stu-id="053f2-213">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="053f2-214">[EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。</span><span class="sxs-lookup"><span data-stu-id="053f2-214">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="053f2-215">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="053f2-215">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="053f2-216">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="053f2-216">eapFastConfiguration</span></span>|[<span data-ttu-id="053f2-217">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="053f2-217">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="053f2-218">EAP-FAST 構成オプションには、EAP-FAST の場合は、選択した EAP の種類です。</span><span class="sxs-lookup"><span data-stu-id="053f2-218">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="053f2-219">可能な値は、`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously` です。</span><span class="sxs-lookup"><span data-stu-id="053f2-219">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="053f2-220">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="053f2-220">trustedServerCertificateNames</span></span>|<span data-ttu-id="053f2-221">String コレクション</span><span class="sxs-lookup"><span data-stu-id="053f2-221">String collection</span></span>|<span data-ttu-id="053f2-222">EAP-TLS または TTLS/高速または PEAP に EAP の種類が構成されている場合は、サーバー証明書の名前を信頼されています。</span><span class="sxs-lookup"><span data-stu-id="053f2-222">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="053f2-223">これは、信頼された証明機関 (CA) によって発行された証明書で使用される一般的な名前です。</span><span class="sxs-lookup"><span data-stu-id="053f2-223">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="053f2-224">この情報を入力する場合は、この Wi-fi ネットワークに接続するときに、エンド ・ ユーザーのデバイスに表示される動的な信頼] ダイアログを回避できます。</span><span class="sxs-lookup"><span data-stu-id="053f2-224">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="053f2-225">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="053f2-225">authenticationMethod</span></span>|[<span data-ttu-id="053f2-226">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="053f2-226">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="053f2-227">PEAP や EAP TTLS に EAP の種類が構成されている場合の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="053f2-227">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="053f2-228">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="053f2-228">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="053f2-229">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="053f2-229">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="053f2-230">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="053f2-230">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="053f2-231">EAP-TTLS では EAP の種類と Authenticationmethod は、ユーザー名とパスワードの認証のための非 EAP メソッドです。</span><span class="sxs-lookup"><span data-stu-id="053f2-231">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="053f2-232">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="053f2-232">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="053f2-233">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="053f2-233">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="053f2-234">String</span><span class="sxs-lookup"><span data-stu-id="053f2-234">String</span></span>|<span data-ttu-id="053f2-235">EAP - TTL、EAP - する EAP の種類が構成されている場合 (外部ユーザー) の [id プライバシーを有効にする高速または PEAP です。</span><span class="sxs-lookup"><span data-stu-id="053f2-235">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="053f2-236">このプロパティは、テキストを入力するユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="053f2-236">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="053f2-237">たとえば、'匿名' を使用する場合は、実際のユーザー名を使用してこの Wi-fi 接続で認証する各ユーザーが '匿名' として表示されます。</span><span class="sxs-lookup"><span data-stu-id="053f2-237">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="053f2-238">応答</span><span class="sxs-lookup"><span data-stu-id="053f2-238">Response</span></span>
<span data-ttu-id="053f2-239">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="053f2-239">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="053f2-240">例</span><span class="sxs-lookup"><span data-stu-id="053f2-240">Example</span></span>
### <a name="request"></a><span data-ttu-id="053f2-241">要求</span><span class="sxs-lookup"><span data-stu-id="053f2-241">Request</span></span>
<span data-ttu-id="053f2-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="053f2-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="053f2-243">応答</span><span class="sxs-lookup"><span data-stu-id="053f2-243">Response</span></span>
<span data-ttu-id="053f2-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="053f2-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





