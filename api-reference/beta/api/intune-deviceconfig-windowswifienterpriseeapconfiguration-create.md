---
title: WindowsWifiEnterpriseEAPConfiguration を作成します。
description: 新しい windowsWifiEnterpriseEAPConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f3ab25f8d74546bd75d4fdc65cc5306fd4c48d25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413480"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="6060e-103">WindowsWifiEnterpriseEAPConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="6060e-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="6060e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6060e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6060e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6060e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6060e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6060e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6060e-107">新しい[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6060e-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6060e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6060e-108">Prerequisites</span></span>
<span data-ttu-id="6060e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6060e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6060e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6060e-111">Permission type</span></span>|<span data-ttu-id="6060e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6060e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6060e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6060e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6060e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6060e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6060e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6060e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6060e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6060e-116">Not supported.</span></span>|
|<span data-ttu-id="6060e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6060e-117">Application</span></span>|<span data-ttu-id="6060e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6060e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6060e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6060e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6060e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6060e-120">Request headers</span></span>
|<span data-ttu-id="6060e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6060e-121">Header</span></span>|<span data-ttu-id="6060e-122">値</span><span class="sxs-lookup"><span data-stu-id="6060e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6060e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6060e-123">Authorization</span></span>|<span data-ttu-id="6060e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6060e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6060e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6060e-125">Accept</span></span>|<span data-ttu-id="6060e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6060e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6060e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6060e-127">Request body</span></span>
<span data-ttu-id="6060e-128">要求の本文に windowsWifiEnterpriseEAPConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="6060e-129">次の表は、windowsWifiEnterpriseEAPConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6060e-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="6060e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6060e-130">Property</span></span>|<span data-ttu-id="6060e-131">型</span><span class="sxs-lookup"><span data-stu-id="6060e-131">Type</span></span>|<span data-ttu-id="6060e-132">説明</span><span class="sxs-lookup"><span data-stu-id="6060e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6060e-133">id</span><span class="sxs-lookup"><span data-stu-id="6060e-133">id</span></span>|<span data-ttu-id="6060e-134">String</span><span class="sxs-lookup"><span data-stu-id="6060e-134">String</span></span>|<span data-ttu-id="6060e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6060e-135">Key of the entity.</span></span> <span data-ttu-id="6060e-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6060e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6060e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6060e-138">DateTimeOffset</span></span>|<span data-ttu-id="6060e-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6060e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6060e-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6060e-141">roleScopeTagIds</span></span>|<span data-ttu-id="6060e-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6060e-142">String collection</span></span>|<span data-ttu-id="6060e-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="6060e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6060e-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6060e-145">supportsScopeTags</span></span>|<span data-ttu-id="6060e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-146">Boolean</span></span>|<span data-ttu-id="6060e-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6060e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6060e-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="6060e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6060e-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="6060e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6060e-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6060e-150">This property is read-only.</span></span> <span data-ttu-id="6060e-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6060e-152">createdDateTime</span></span>|<span data-ttu-id="6060e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6060e-153">DateTimeOffset</span></span>|<span data-ttu-id="6060e-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6060e-154">DateTime the object was created.</span></span> <span data-ttu-id="6060e-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-156">説明</span><span class="sxs-lookup"><span data-stu-id="6060e-156">description</span></span>|<span data-ttu-id="6060e-157">String</span><span class="sxs-lookup"><span data-stu-id="6060e-157">String</span></span>|<span data-ttu-id="6060e-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6060e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6060e-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6060e-160">displayName</span></span>|<span data-ttu-id="6060e-161">String</span><span class="sxs-lookup"><span data-stu-id="6060e-161">String</span></span>|<span data-ttu-id="6060e-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6060e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6060e-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-164">version</span><span class="sxs-lookup"><span data-stu-id="6060e-164">version</span></span>|<span data-ttu-id="6060e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-165">Int32</span></span>|<span data-ttu-id="6060e-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6060e-166">Version of the device configuration.</span></span> <span data-ttu-id="6060e-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6060e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6060e-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="6060e-168">preSharedKey</span></span>|<span data-ttu-id="6060e-169">String</span><span class="sxs-lookup"><span data-stu-id="6060e-169">String</span></span>|<span data-ttu-id="6060e-170">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="6060e-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="6060e-171">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-171">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-172">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6060e-172">wifiSecurityType</span></span>|[<span data-ttu-id="6060e-173">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6060e-173">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="6060e-174">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-174">Specify the Wifi Security Type.</span></span> <span data-ttu-id="6060e-175">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6060e-175">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="6060e-176">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="6060e-176">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6060e-177">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="6060e-177">meteredConnectionLimit</span></span>|[<span data-ttu-id="6060e-178">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="6060e-178">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="6060e-179">Wifi 接続のメータリングされた接続の制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-179">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="6060e-180">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6060e-180">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="6060e-181">可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="6060e-181">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="6060e-182">ssid</span><span class="sxs-lookup"><span data-stu-id="6060e-182">ssid</span></span>|<span data-ttu-id="6060e-183">String</span><span class="sxs-lookup"><span data-stu-id="6060e-183">String</span></span>|<span data-ttu-id="6060e-184">Wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-184">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="6060e-185">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-185">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-186">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="6060e-186">networkName</span></span>|<span data-ttu-id="6060e-187">String</span><span class="sxs-lookup"><span data-stu-id="6060e-187">String</span></span>|<span data-ttu-id="6060e-188">ネットワーク構成の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-188">Specify the network configuration name.</span></span> <span data-ttu-id="6060e-189">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-189">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-190">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6060e-190">connectAutomatically</span></span>|<span data-ttu-id="6060e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-191">Boolean</span></span>|<span data-ttu-id="6060e-192">範囲で wifi 接続が自動的に接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-192">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="6060e-193">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-193">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-194">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="6060e-194">connectToPreferredNetwork</span></span>|<span data-ttu-id="6060e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-195">Boolean</span></span>|<span data-ttu-id="6060e-196">Wifi 接続は、この 1 つに既に接続されている場合より優先するネットワークに接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-196">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="6060e-197">True を指定する ConnectAutomatically が必要です。</span><span class="sxs-lookup"><span data-stu-id="6060e-197">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="6060e-198">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-198">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-199">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6060e-199">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6060e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-200">Boolean</span></span>|<span data-ttu-id="6060e-201">かどうか、wifi 接続自動的にでもすると、SSID をブロードキャストしていないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-201">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="6060e-202">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-202">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-203">proxySetting</span><span class="sxs-lookup"><span data-stu-id="6060e-203">proxySetting</span></span>|[<span data-ttu-id="6060e-204">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="6060e-204">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="6060e-205">プロキシの[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から Wi-fi 設定の継承の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-205">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="6060e-206">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="6060e-206">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="6060e-207">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="6060e-207">proxyManualAddress</span></span>|<span data-ttu-id="6060e-208">String</span><span class="sxs-lookup"><span data-stu-id="6060e-208">String</span></span>|<span data-ttu-id="6060e-209">プロキシ サーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-209">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="6060e-210">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-211">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="6060e-211">proxyManualPort</span></span>|<span data-ttu-id="6060e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-212">Int32</span></span>|<span data-ttu-id="6060e-213">プロキシ サーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-213">Specify the port for the proxy server.</span></span> <span data-ttu-id="6060e-214">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-215">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="6060e-215">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="6060e-216">String</span><span class="sxs-lookup"><span data-stu-id="6060e-216">String</span></span>|<span data-ttu-id="6060e-217">プロキシ サーバーの構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-217">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="6060e-218">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-218">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="6060e-219">forceFIPSCompliance</span></span>|<span data-ttu-id="6060e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-220">Boolean</span></span>|<span data-ttu-id="6060e-221">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-221">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="6060e-222">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6060e-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="6060e-223">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="6060e-223">networkSingleSignOn</span></span>|[<span data-ttu-id="6060e-224">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="6060e-224">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="6060e-225">型のネットワークの 1 つの記号を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-225">Specify the network single sign on type.</span></span> <span data-ttu-id="6060e-226">可能な値は、`disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="6060e-226">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="6060e-227">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="6060e-227">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="6060e-228">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-228">Int32</span></span>|<span data-ttu-id="6060e-229">認証の最大タイムアウトを秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-229">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="6060e-230">有効範囲: 1 ~ 120</span><span class="sxs-lookup"><span data-stu-id="6060e-230">Valid range: 1-120</span></span>|
|<span data-ttu-id="6060e-231">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="6060e-231">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="6060e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-232">Boolean</span></span>|<span data-ttu-id="6060e-233">Wifi 接続がその他の認証の資格情報を促す必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-233">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="6060e-234">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="6060e-234">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="6060e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-235">Boolean</span></span>|<span data-ttu-id="6060e-236">Wifi 接続する必要がありますペアワイズ マスター_キーのキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-236">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="6060e-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6060e-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="6060e-238">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-238">Int32</span></span>|<span data-ttu-id="6060e-239">ペアワイズ マスター_キーの最大キャッシュ時間 (分単位) を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-239">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="6060e-240">有効範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="6060e-240">Valid range: 5-1440</span></span>|
|<span data-ttu-id="6060e-241">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="6060e-241">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="6060e-242">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-242">Int32</span></span>|<span data-ttu-id="6060e-243">キャッシュでは、ペアワイズ マスター_キーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-243">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="6060e-244">有効範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="6060e-244">Valid range: 1-255</span></span>|
|<span data-ttu-id="6060e-245">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="6060e-245">enablePreAuthentication</span></span>|<span data-ttu-id="6060e-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="6060e-246">Boolean</span></span>|<span data-ttu-id="6060e-247">事前認証を有効にする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-247">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="6060e-248">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="6060e-248">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="6060e-249">Int32</span><span class="sxs-lookup"><span data-stu-id="6060e-249">Int32</span></span>|<span data-ttu-id="6060e-250">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-250">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="6060e-251">有効範囲: 1 ~ 16</span><span class="sxs-lookup"><span data-stu-id="6060e-251">Valid range: 1-16</span></span>|
|<span data-ttu-id="6060e-252">eapType</span><span class="sxs-lookup"><span data-stu-id="6060e-252">eapType</span></span>|[<span data-ttu-id="6060e-253">eapType</span><span class="sxs-lookup"><span data-stu-id="6060e-253">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="6060e-254">拡張認証プロトコル (EAP) です。</span><span class="sxs-lookup"><span data-stu-id="6060e-254">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="6060e-255">[EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。</span><span class="sxs-lookup"><span data-stu-id="6060e-255">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6060e-256">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="6060e-256">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="6060e-257">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="6060e-257">trustedServerCertificateNames</span></span>|<span data-ttu-id="6060e-258">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6060e-258">String collection</span></span>|<span data-ttu-id="6060e-259">信頼されたサーバー証明書名を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-259">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="6060e-260">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6060e-260">authenticationMethod</span></span>|[<span data-ttu-id="6060e-261">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6060e-261">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6060e-262">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-262">Specify the authentication method.</span></span> <span data-ttu-id="6060e-263">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="6060e-263">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6060e-264">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="6060e-264">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="6060e-265">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6060e-265">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6060e-266">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-266">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="6060e-267">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="6060e-267">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6060e-268">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6060e-268">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6060e-269">String</span><span class="sxs-lookup"><span data-stu-id="6060e-269">String</span></span>|<span data-ttu-id="6060e-270">EAP TTLS または PEAP を使用する場合は、プライバシー保護のためのユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="6060e-270">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="6060e-271">応答</span><span class="sxs-lookup"><span data-stu-id="6060e-271">Response</span></span>
<span data-ttu-id="6060e-272">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6060e-272">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6060e-273">例</span><span class="sxs-lookup"><span data-stu-id="6060e-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="6060e-274">要求</span><span class="sxs-lookup"><span data-stu-id="6060e-274">Request</span></span>
<span data-ttu-id="6060e-275">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6060e-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="6060e-276">応答</span><span class="sxs-lookup"><span data-stu-id="6060e-276">Response</span></span>
<span data-ttu-id="6060e-p132">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6060e-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




