---
title: Windows81VpnConfiguration を作成する
description: 新しい windows81VpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c4c87833abc3f736ef795708add36646ef55812
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918130"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="ad8f2-103">Windows81VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="ad8f2-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="ad8f2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad8f2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad8f2-106">新しい[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-106">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad8f2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad8f2-107">Prerequisites</span></span>
<span data-ttu-id="ad8f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8f2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad8f2-110">Permission type</span></span>|<span data-ttu-id="ad8f2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad8f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad8f2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad8f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad8f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad8f2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad8f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad8f2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-115">Not supported.</span></span>|
|<span data-ttu-id="ad8f2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad8f2-116">Application</span></span>|<span data-ttu-id="ad8f2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad8f2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad8f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ad8f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad8f2-119">Request headers</span></span>
|<span data-ttu-id="ad8f2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad8f2-120">Header</span></span>|<span data-ttu-id="ad8f2-121">値</span><span class="sxs-lookup"><span data-stu-id="ad8f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad8f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad8f2-122">Authorization</span></span>|<span data-ttu-id="ad8f2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad8f2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ad8f2-124">Accept</span></span>|<span data-ttu-id="ad8f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad8f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad8f2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad8f2-126">Request body</span></span>
<span data-ttu-id="ad8f2-127">要求本文で、windows81VpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-127">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="ad8f2-128">次の表に、windows81VpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-128">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="ad8f2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad8f2-129">Property</span></span>|<span data-ttu-id="ad8f2-130">型</span><span class="sxs-lookup"><span data-stu-id="ad8f2-130">Type</span></span>|<span data-ttu-id="ad8f2-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad8f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad8f2-132">id</span><span class="sxs-lookup"><span data-stu-id="ad8f2-132">id</span></span>|<span data-ttu-id="ad8f2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ad8f2-133">String</span></span>|<span data-ttu-id="ad8f2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-134">Key of the entity.</span></span> <span data-ttu-id="ad8f2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8f2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ad8f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8f2-137">DateTimeOffset</span></span>|<span data-ttu-id="ad8f2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ad8f2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad8f2-140">roleScopeTagIds</span></span>|<span data-ttu-id="ad8f2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ad8f2-141">String collection</span></span>|<span data-ttu-id="ad8f2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ad8f2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ad8f2-144">supportsScopeTags</span></span>|<span data-ttu-id="ad8f2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad8f2-145">Boolean</span></span>|<span data-ttu-id="ad8f2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ad8f2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ad8f2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ad8f2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-149">This property is read-only.</span></span> <span data-ttu-id="ad8f2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad8f2-151">createdDateTime</span></span>|<span data-ttu-id="ad8f2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad8f2-152">DateTimeOffset</span></span>|<span data-ttu-id="ad8f2-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-153">DateTime the object was created.</span></span> <span data-ttu-id="ad8f2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-155">description</span><span class="sxs-lookup"><span data-stu-id="ad8f2-155">description</span></span>|<span data-ttu-id="ad8f2-156">String</span><span class="sxs-lookup"><span data-stu-id="ad8f2-156">String</span></span>|<span data-ttu-id="ad8f2-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad8f2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ad8f2-159">displayName</span></span>|<span data-ttu-id="ad8f2-160">String</span><span class="sxs-lookup"><span data-stu-id="ad8f2-160">String</span></span>|<span data-ttu-id="ad8f2-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad8f2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-163">version</span><span class="sxs-lookup"><span data-stu-id="ad8f2-163">version</span></span>|<span data-ttu-id="ad8f2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ad8f2-164">Int32</span></span>|<span data-ttu-id="ad8f2-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-165">Version of the device configuration.</span></span> <span data-ttu-id="ad8f2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="ad8f2-167">connectionName</span></span>|<span data-ttu-id="ad8f2-168">String</span><span class="sxs-lookup"><span data-stu-id="ad8f2-168">String</span></span>|<span data-ttu-id="ad8f2-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-169">Connection name displayed to the user.</span></span> <span data-ttu-id="ad8f2-170">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-171">サーバ</span><span class="sxs-lookup"><span data-stu-id="ad8f2-171">servers</span></span>|<span data-ttu-id="ad8f2-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ad8f2-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ad8f2-173">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="ad8f2-174">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ad8f2-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ad8f2-176">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-177">customXml</span><span class="sxs-lookup"><span data-stu-id="ad8f2-177">customXml</span></span>|<span data-ttu-id="ad8f2-178">Binary</span><span class="sxs-lookup"><span data-stu-id="ad8f2-178">Binary</span></span>|<span data-ttu-id="ad8f2-179">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ad8f2-180">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ad8f2-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ad8f2-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ad8f2-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="ad8f2-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad8f2-182">Boolean</span></span>|<span data-ttu-id="ad8f2-183">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ad8f2-184">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-184">This property is read-only.</span></span>|
|<span data-ttu-id="ad8f2-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="ad8f2-185">connectionType</span></span>|[<span data-ttu-id="ad8f2-186">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ad8f2-186">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="ad8f2-187">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-187">Connection type.</span></span> <span data-ttu-id="ad8f2-188">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="ad8f2-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ad8f2-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ad8f2-190">String</span><span class="sxs-lookup"><span data-stu-id="ad8f2-190">String</span></span>|<span data-ttu-id="ad8f2-191">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ad8f2-192">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ad8f2-192">enableSplitTunneling</span></span>|<span data-ttu-id="ad8f2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad8f2-193">Boolean</span></span>|<span data-ttu-id="ad8f2-194">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-194">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="ad8f2-195">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ad8f2-195">proxyServer</span></span>|[<span data-ttu-id="ad8f2-196">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ad8f2-196">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="ad8f2-197">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-197">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="ad8f2-198">応答</span><span class="sxs-lookup"><span data-stu-id="ad8f2-198">Response</span></span>
<span data-ttu-id="ad8f2-199">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-199">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad8f2-200">例</span><span class="sxs-lookup"><span data-stu-id="ad8f2-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad8f2-201">要求</span><span class="sxs-lookup"><span data-stu-id="ad8f2-201">Request</span></span>
<span data-ttu-id="ad8f2-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1015

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="ad8f2-203">応答</span><span class="sxs-lookup"><span data-stu-id="ad8f2-203">Response</span></span>
<span data-ttu-id="ad8f2-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad8f2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




