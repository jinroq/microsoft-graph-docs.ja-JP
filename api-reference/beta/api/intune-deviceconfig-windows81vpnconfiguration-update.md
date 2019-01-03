---
title: Windows81VpnConfiguration を更新します。
description: Windows81VpnConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: cabc382272c1943dce8361dd35c29c5b0f397826
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355343"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="32b29-103">Windows81VpnConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="32b29-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="32b29-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32b29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32b29-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32b29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32b29-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="32b29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32b29-107">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="32b29-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32b29-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="32b29-108">Prerequisites</span></span>
<span data-ttu-id="32b29-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32b29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b29-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32b29-111">Permission type</span></span>|<span data-ttu-id="32b29-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="32b29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32b29-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32b29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32b29-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b29-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32b29-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32b29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32b29-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32b29-116">Not supported.</span></span>|
|<span data-ttu-id="32b29-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32b29-117">Application</span></span>|<span data-ttu-id="32b29-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32b29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32b29-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32b29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="32b29-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32b29-120">Request headers</span></span>
|<span data-ttu-id="32b29-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32b29-121">Header</span></span>|<span data-ttu-id="32b29-122">値</span><span class="sxs-lookup"><span data-stu-id="32b29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32b29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b29-123">Authorization</span></span>|<span data-ttu-id="32b29-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="32b29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32b29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32b29-125">Accept</span></span>|<span data-ttu-id="32b29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32b29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32b29-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="32b29-127">Request body</span></span>
<span data-ttu-id="32b29-128">要求の本文に[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="32b29-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="32b29-129">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="32b29-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="32b29-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32b29-130">Property</span></span>|<span data-ttu-id="32b29-131">種類</span><span class="sxs-lookup"><span data-stu-id="32b29-131">Type</span></span>|<span data-ttu-id="32b29-132">説明</span><span class="sxs-lookup"><span data-stu-id="32b29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b29-133">ID</span><span class="sxs-lookup"><span data-stu-id="32b29-133">id</span></span>|<span data-ttu-id="32b29-134">String</span><span class="sxs-lookup"><span data-stu-id="32b29-134">String</span></span>|<span data-ttu-id="32b29-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="32b29-135">Key of the entity.</span></span> <span data-ttu-id="32b29-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32b29-137">lastModifiedDateTime</span></span>|<span data-ttu-id="32b29-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b29-138">DateTimeOffset</span></span>|<span data-ttu-id="32b29-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32b29-139">DateTime the object was last modified.</span></span> <span data-ttu-id="32b29-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32b29-141">roleScopeTagIds</span></span>|<span data-ttu-id="32b29-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="32b29-142">String collection</span></span>|<span data-ttu-id="32b29-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="32b29-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="32b29-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="32b29-145">supportsScopeTags</span></span>|<span data-ttu-id="32b29-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="32b29-146">Boolean</span></span>|<span data-ttu-id="32b29-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="32b29-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="32b29-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="32b29-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="32b29-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="32b29-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="32b29-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="32b29-150">This property is read-only.</span></span> <span data-ttu-id="32b29-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32b29-152">createdDateTime</span></span>|<span data-ttu-id="32b29-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b29-153">DateTimeOffset</span></span>|<span data-ttu-id="32b29-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32b29-154">DateTime the object was created.</span></span> <span data-ttu-id="32b29-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-156">説明</span><span class="sxs-lookup"><span data-stu-id="32b29-156">description</span></span>|<span data-ttu-id="32b29-157">String</span><span class="sxs-lookup"><span data-stu-id="32b29-157">String</span></span>|<span data-ttu-id="32b29-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="32b29-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32b29-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-160">displayName</span><span class="sxs-lookup"><span data-stu-id="32b29-160">displayName</span></span>|<span data-ttu-id="32b29-161">String</span><span class="sxs-lookup"><span data-stu-id="32b29-161">String</span></span>|<span data-ttu-id="32b29-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="32b29-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32b29-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-164">version</span><span class="sxs-lookup"><span data-stu-id="32b29-164">version</span></span>|<span data-ttu-id="32b29-165">Int32</span><span class="sxs-lookup"><span data-stu-id="32b29-165">Int32</span></span>|<span data-ttu-id="32b29-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="32b29-166">Version of the device configuration.</span></span> <span data-ttu-id="32b29-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32b29-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="32b29-168">connectionName</span></span>|<span data-ttu-id="32b29-169">String</span><span class="sxs-lookup"><span data-stu-id="32b29-169">String</span></span>|<span data-ttu-id="32b29-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="32b29-170">Connection name displayed to the user.</span></span> <span data-ttu-id="32b29-171">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="32b29-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-172">サーバー</span><span class="sxs-lookup"><span data-stu-id="32b29-172">servers</span></span>|<span data-ttu-id="32b29-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="32b29-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="32b29-174">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="32b29-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="32b29-175">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="32b29-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="32b29-176">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="32b29-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="32b29-177">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="32b29-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-178">customXml</span><span class="sxs-lookup"><span data-stu-id="32b29-178">customXml</span></span>|<span data-ttu-id="32b29-179">Binary</span><span class="sxs-lookup"><span data-stu-id="32b29-179">Binary</span></span>|<span data-ttu-id="32b29-180">VPN 接続を構成するユーザー設定の XML コマンドです。</span><span class="sxs-lookup"><span data-stu-id="32b29-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="32b29-181">(UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="32b29-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="32b29-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="32b29-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="32b29-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="32b29-183">Boolean</span></span>|<span data-ttu-id="32b29-184">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="32b29-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="32b29-185">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32b29-185">This property is read-only.</span></span>|
|<span data-ttu-id="32b29-186">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="32b29-186">connectionType</span></span>|[<span data-ttu-id="32b29-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="32b29-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="32b29-188">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="32b29-188">Connection type.</span></span> <span data-ttu-id="32b29-189">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="32b29-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="32b29-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="32b29-190">loginGroupOrDomain</span></span>|<span data-ttu-id="32b29-191">String</span><span class="sxs-lookup"><span data-stu-id="32b29-191">String</span></span>|<span data-ttu-id="32b29-192">ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。</span><span class="sxs-lookup"><span data-stu-id="32b29-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="32b29-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="32b29-193">enableSplitTunneling</span></span>|<span data-ttu-id="32b29-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="32b29-194">Boolean</span></span>|<span data-ttu-id="32b29-195">分割は、VPN のトンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="32b29-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="32b29-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="32b29-196">proxyServer</span></span>|[<span data-ttu-id="32b29-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="32b29-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="32b29-198">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="32b29-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="32b29-199">応答</span><span class="sxs-lookup"><span data-stu-id="32b29-199">Response</span></span>
<span data-ttu-id="32b29-200">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="32b29-200">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32b29-201">例</span><span class="sxs-lookup"><span data-stu-id="32b29-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="32b29-202">要求</span><span class="sxs-lookup"><span data-stu-id="32b29-202">Request</span></span>
<span data-ttu-id="32b29-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32b29-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1015

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="32b29-204">応答</span><span class="sxs-lookup"><span data-stu-id="32b29-204">Response</span></span>
<span data-ttu-id="32b29-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32b29-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```




