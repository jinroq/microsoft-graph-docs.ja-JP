---
title: WindowsWifiEnterpriseEAPConfiguration を更新します。
description: WindowsWifiEnterpriseEAPConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4daa930e47c20f4a330ed9a860c2bc2c9224e742
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832642"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="494f2-103">WindowsWifiEnterpriseEAPConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="494f2-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="494f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="494f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="494f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="494f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="494f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="494f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="494f2-107">[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="494f2-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="494f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="494f2-108">Prerequisites</span></span>
<span data-ttu-id="494f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="494f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="494f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="494f2-111">Permission type</span></span>|<span data-ttu-id="494f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="494f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="494f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="494f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="494f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="494f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="494f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="494f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="494f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="494f2-116">Not supported.</span></span>|
|<span data-ttu-id="494f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="494f2-117">Application</span></span>|<span data-ttu-id="494f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="494f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="494f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="494f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="494f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="494f2-120">Request headers</span></span>
|<span data-ttu-id="494f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="494f2-121">Header</span></span>|<span data-ttu-id="494f2-122">値</span><span class="sxs-lookup"><span data-stu-id="494f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="494f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="494f2-123">Authorization</span></span>|<span data-ttu-id="494f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="494f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="494f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="494f2-125">Accept</span></span>|<span data-ttu-id="494f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="494f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="494f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="494f2-127">Request body</span></span>
<span data-ttu-id="494f2-128">要求の本文に[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="494f2-129">[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="494f2-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="494f2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="494f2-130">Property</span></span>|<span data-ttu-id="494f2-131">種類</span><span class="sxs-lookup"><span data-stu-id="494f2-131">Type</span></span>|<span data-ttu-id="494f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="494f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="494f2-133">ID</span><span class="sxs-lookup"><span data-stu-id="494f2-133">id</span></span>|<span data-ttu-id="494f2-134">String</span><span class="sxs-lookup"><span data-stu-id="494f2-134">String</span></span>|<span data-ttu-id="494f2-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="494f2-135">Key of the entity.</span></span> <span data-ttu-id="494f2-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="494f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="494f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="494f2-138">DateTimeOffset</span></span>|<span data-ttu-id="494f2-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="494f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="494f2-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="494f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="494f2-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="494f2-142">String collection</span></span>|<span data-ttu-id="494f2-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="494f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="494f2-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="494f2-145">supportsScopeTags</span></span>|<span data-ttu-id="494f2-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-146">Boolean</span></span>|<span data-ttu-id="494f2-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="494f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="494f2-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="494f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="494f2-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="494f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="494f2-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="494f2-150">This property is read-only.</span></span> <span data-ttu-id="494f2-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="494f2-152">createdDateTime</span></span>|<span data-ttu-id="494f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="494f2-153">DateTimeOffset</span></span>|<span data-ttu-id="494f2-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="494f2-154">DateTime the object was created.</span></span> <span data-ttu-id="494f2-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-156">説明</span><span class="sxs-lookup"><span data-stu-id="494f2-156">description</span></span>|<span data-ttu-id="494f2-157">String</span><span class="sxs-lookup"><span data-stu-id="494f2-157">String</span></span>|<span data-ttu-id="494f2-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="494f2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="494f2-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="494f2-160">displayName</span></span>|<span data-ttu-id="494f2-161">String</span><span class="sxs-lookup"><span data-stu-id="494f2-161">String</span></span>|<span data-ttu-id="494f2-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="494f2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="494f2-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-164">version</span><span class="sxs-lookup"><span data-stu-id="494f2-164">version</span></span>|<span data-ttu-id="494f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-165">Int32</span></span>|<span data-ttu-id="494f2-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="494f2-166">Version of the device configuration.</span></span> <span data-ttu-id="494f2-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="494f2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="494f2-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="494f2-168">preSharedKey</span></span>|<span data-ttu-id="494f2-169">String</span><span class="sxs-lookup"><span data-stu-id="494f2-169">String</span></span>|<span data-ttu-id="494f2-170">これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="494f2-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="494f2-171">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-171">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-172">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="494f2-172">wifiSecurityType</span></span>|[<span data-ttu-id="494f2-173">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="494f2-173">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="494f2-174">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-174">Specify the Wifi Security Type.</span></span> <span data-ttu-id="494f2-175">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="494f2-175">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="494f2-176">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="494f2-176">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="494f2-177">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="494f2-177">meteredConnectionLimit</span></span>|[<span data-ttu-id="494f2-178">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="494f2-178">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="494f2-179">Wifi 接続のメータリングされた接続の制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-179">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="494f2-180">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="494f2-180">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="494f2-181">可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="494f2-181">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="494f2-182">ssid</span><span class="sxs-lookup"><span data-stu-id="494f2-182">ssid</span></span>|<span data-ttu-id="494f2-183">String</span><span class="sxs-lookup"><span data-stu-id="494f2-183">String</span></span>|<span data-ttu-id="494f2-184">Wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-184">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="494f2-185">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-185">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-186">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="494f2-186">networkName</span></span>|<span data-ttu-id="494f2-187">String</span><span class="sxs-lookup"><span data-stu-id="494f2-187">String</span></span>|<span data-ttu-id="494f2-188">ネットワーク構成の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-188">Specify the network configuration name.</span></span> <span data-ttu-id="494f2-189">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-189">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-190">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="494f2-190">connectAutomatically</span></span>|<span data-ttu-id="494f2-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-191">Boolean</span></span>|<span data-ttu-id="494f2-192">範囲で wifi 接続が自動的に接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-192">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="494f2-193">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-193">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-194">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="494f2-194">connectToPreferredNetwork</span></span>|<span data-ttu-id="494f2-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-195">Boolean</span></span>|<span data-ttu-id="494f2-196">Wifi 接続は、この 1 つに既に接続されている場合より優先するネットワークに接続する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-196">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="494f2-197">True を指定する ConnectAutomatically が必要です。</span><span class="sxs-lookup"><span data-stu-id="494f2-197">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="494f2-198">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-198">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-199">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="494f2-199">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="494f2-200">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-200">Boolean</span></span>|<span data-ttu-id="494f2-201">かどうか、wifi 接続自動的にでもすると、SSID をブロードキャストしていないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-201">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="494f2-202">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-202">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-203">proxySetting</span><span class="sxs-lookup"><span data-stu-id="494f2-203">proxySetting</span></span>|[<span data-ttu-id="494f2-204">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="494f2-204">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="494f2-205">プロキシの[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から Wi-fi 設定の継承の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-205">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="494f2-206">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="494f2-206">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="494f2-207">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="494f2-207">proxyManualAddress</span></span>|<span data-ttu-id="494f2-208">String</span><span class="sxs-lookup"><span data-stu-id="494f2-208">String</span></span>|<span data-ttu-id="494f2-209">プロキシ サーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-209">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="494f2-210">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-211">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="494f2-211">proxyManualPort</span></span>|<span data-ttu-id="494f2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-212">Int32</span></span>|<span data-ttu-id="494f2-213">プロキシ サーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-213">Specify the port for the proxy server.</span></span> <span data-ttu-id="494f2-214">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-215">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="494f2-215">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="494f2-216">String</span><span class="sxs-lookup"><span data-stu-id="494f2-216">String</span></span>|<span data-ttu-id="494f2-217">プロキシ サーバーの構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-217">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="494f2-218">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-218">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="494f2-219">forceFIPSCompliance</span></span>|<span data-ttu-id="494f2-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-220">Boolean</span></span>|<span data-ttu-id="494f2-221">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-221">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="494f2-222">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="494f2-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="494f2-223">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="494f2-223">networkSingleSignOn</span></span>|[<span data-ttu-id="494f2-224">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="494f2-224">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="494f2-225">型のネットワークの 1 つの記号を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-225">Specify the network single sign on type.</span></span> <span data-ttu-id="494f2-226">可能な値は、`disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="494f2-226">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="494f2-227">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="494f2-227">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="494f2-228">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-228">Int32</span></span>|<span data-ttu-id="494f2-229">認証の最大タイムアウトを秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-229">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="494f2-230">有効範囲: 1 ~ 120</span><span class="sxs-lookup"><span data-stu-id="494f2-230">Valid range: 1-120</span></span>|
|<span data-ttu-id="494f2-231">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="494f2-231">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="494f2-232">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-232">Boolean</span></span>|<span data-ttu-id="494f2-233">Wifi 接続がその他の認証の資格情報を促す必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-233">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="494f2-234">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="494f2-234">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="494f2-235">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-235">Boolean</span></span>|<span data-ttu-id="494f2-236">Wifi 接続する必要がありますペアワイズ マスター_キーのキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-236">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="494f2-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="494f2-237">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="494f2-238">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-238">Int32</span></span>|<span data-ttu-id="494f2-239">ペアワイズ マスター_キーの最大キャッシュ時間 (分単位) を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-239">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="494f2-240">有効範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="494f2-240">Valid range: 5-1440</span></span>|
|<span data-ttu-id="494f2-241">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="494f2-241">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="494f2-242">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-242">Int32</span></span>|<span data-ttu-id="494f2-243">キャッシュでは、ペアワイズ マスター_キーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-243">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="494f2-244">有効範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="494f2-244">Valid range: 1-255</span></span>|
|<span data-ttu-id="494f2-245">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="494f2-245">enablePreAuthentication</span></span>|<span data-ttu-id="494f2-246">ブール型</span><span class="sxs-lookup"><span data-stu-id="494f2-246">Boolean</span></span>|<span data-ttu-id="494f2-247">事前認証を有効にする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-247">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="494f2-248">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="494f2-248">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="494f2-249">Int32</span><span class="sxs-lookup"><span data-stu-id="494f2-249">Int32</span></span>|<span data-ttu-id="494f2-250">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-250">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="494f2-251">有効範囲: 1 ~ 16</span><span class="sxs-lookup"><span data-stu-id="494f2-251">Valid range: 1-16</span></span>|
|<span data-ttu-id="494f2-252">eapType</span><span class="sxs-lookup"><span data-stu-id="494f2-252">eapType</span></span>|[<span data-ttu-id="494f2-253">eapType</span><span class="sxs-lookup"><span data-stu-id="494f2-253">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="494f2-254">拡張認証プロトコル (EAP) です。</span><span class="sxs-lookup"><span data-stu-id="494f2-254">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="494f2-255">[EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。</span><span class="sxs-lookup"><span data-stu-id="494f2-255">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="494f2-256">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="494f2-256">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="494f2-257">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="494f2-257">trustedServerCertificateNames</span></span>|<span data-ttu-id="494f2-258">String コレクション</span><span class="sxs-lookup"><span data-stu-id="494f2-258">String collection</span></span>|<span data-ttu-id="494f2-259">信頼されたサーバー証明書名を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-259">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="494f2-260">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="494f2-260">authenticationMethod</span></span>|[<span data-ttu-id="494f2-261">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="494f2-261">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="494f2-262">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-262">Specify the authentication method.</span></span> <span data-ttu-id="494f2-263">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="494f2-263">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="494f2-264">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="494f2-264">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="494f2-265">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="494f2-265">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="494f2-266">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-266">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="494f2-267">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="494f2-267">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="494f2-268">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="494f2-268">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="494f2-269">String</span><span class="sxs-lookup"><span data-stu-id="494f2-269">String</span></span>|<span data-ttu-id="494f2-270">EAP TTLS または PEAP を使用する場合は、プライバシー保護のためのユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="494f2-270">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="494f2-271">応答</span><span class="sxs-lookup"><span data-stu-id="494f2-271">Response</span></span>
<span data-ttu-id="494f2-272">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="494f2-272">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="494f2-273">例</span><span class="sxs-lookup"><span data-stu-id="494f2-273">Example</span></span>
### <a name="request"></a><span data-ttu-id="494f2-274">要求</span><span class="sxs-lookup"><span data-stu-id="494f2-274">Request</span></span>
<span data-ttu-id="494f2-275">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="494f2-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1492

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="494f2-276">応答</span><span class="sxs-lookup"><span data-stu-id="494f2-276">Response</span></span>
<span data-ttu-id="494f2-p132">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="494f2-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





