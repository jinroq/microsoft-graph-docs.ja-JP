---
title: windows81VpnConfiguration の更新
description: windows81VpnConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6af3b3f3fd6c0c78e73b1f8c869b2801c0b7d301
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788424"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="1a951-103">windows81VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1a951-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="1a951-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a951-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a951-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a951-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a951-106">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a951-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a951-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a951-107">Prerequisites</span></span>
<span data-ttu-id="1a951-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a951-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a951-110">Permission type</span></span>|<span data-ttu-id="1a951-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a951-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a951-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a951-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a951-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a951-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a951-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a951-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a951-115">Not supported.</span></span>|
|<span data-ttu-id="1a951-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a951-116">Application</span></span>|<span data-ttu-id="1a951-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a951-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a951-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a951-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a951-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a951-119">Request headers</span></span>
|<span data-ttu-id="1a951-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a951-120">Header</span></span>|<span data-ttu-id="1a951-121">値</span><span class="sxs-lookup"><span data-stu-id="1a951-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a951-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a951-122">Authorization</span></span>|<span data-ttu-id="1a951-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a951-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a951-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1a951-124">Accept</span></span>|<span data-ttu-id="1a951-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a951-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a951-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a951-126">Request body</span></span>
<span data-ttu-id="1a951-127">要求本文で、 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a951-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="1a951-128">次の表に、 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a951-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="1a951-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a951-129">Property</span></span>|<span data-ttu-id="1a951-130">型</span><span class="sxs-lookup"><span data-stu-id="1a951-130">Type</span></span>|<span data-ttu-id="1a951-131">説明</span><span class="sxs-lookup"><span data-stu-id="1a951-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a951-132">id</span><span class="sxs-lookup"><span data-stu-id="1a951-132">id</span></span>|<span data-ttu-id="1a951-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a951-133">String</span></span>|<span data-ttu-id="1a951-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a951-134">Key of the entity.</span></span> <span data-ttu-id="1a951-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a951-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a951-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a951-137">DateTimeOffset</span></span>|<span data-ttu-id="1a951-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a951-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1a951-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a951-140">roleScopeTagIds</span></span>|<span data-ttu-id="1a951-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1a951-141">String collection</span></span>|<span data-ttu-id="1a951-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1a951-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a951-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a951-144">supportsScopeTags</span></span>|<span data-ttu-id="1a951-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a951-145">Boolean</span></span>|<span data-ttu-id="1a951-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a951-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a951-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1a951-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a951-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1a951-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a951-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1a951-149">This property is read-only.</span></span> <span data-ttu-id="1a951-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a951-151">createdDateTime</span></span>|<span data-ttu-id="1a951-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a951-152">DateTimeOffset</span></span>|<span data-ttu-id="1a951-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a951-153">DateTime the object was created.</span></span> <span data-ttu-id="1a951-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-155">説明</span><span class="sxs-lookup"><span data-stu-id="1a951-155">description</span></span>|<span data-ttu-id="1a951-156">String</span><span class="sxs-lookup"><span data-stu-id="1a951-156">String</span></span>|<span data-ttu-id="1a951-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1a951-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a951-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1a951-159">displayName</span></span>|<span data-ttu-id="1a951-160">String</span><span class="sxs-lookup"><span data-stu-id="1a951-160">String</span></span>|<span data-ttu-id="1a951-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1a951-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a951-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-163">version</span><span class="sxs-lookup"><span data-stu-id="1a951-163">version</span></span>|<span data-ttu-id="1a951-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1a951-164">Int32</span></span>|<span data-ttu-id="1a951-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a951-165">Version of the device configuration.</span></span> <span data-ttu-id="1a951-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="1a951-167">connectionName</span></span>|<span data-ttu-id="1a951-168">文字列</span><span class="sxs-lookup"><span data-stu-id="1a951-168">String</span></span>|<span data-ttu-id="1a951-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="1a951-169">Connection name displayed to the user.</span></span> <span data-ttu-id="1a951-170">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-171">サーバ</span><span class="sxs-lookup"><span data-stu-id="1a951-171">servers</span></span>|<span data-ttu-id="1a951-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a951-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1a951-173">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="1a951-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="1a951-174">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a951-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1a951-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1a951-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1a951-176">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-177">customXml</span><span class="sxs-lookup"><span data-stu-id="1a951-177">customXml</span></span>|<span data-ttu-id="1a951-178">Binary</span><span class="sxs-lookup"><span data-stu-id="1a951-178">Binary</span></span>|<span data-ttu-id="1a951-179">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="1a951-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1a951-180">(UTF8 でエンコードされたバイト配列)[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1a951-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1a951-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="1a951-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="1a951-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a951-182">Boolean</span></span>|<span data-ttu-id="1a951-183">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="1a951-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="1a951-184">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1a951-184">This property is read-only.</span></span>|
|<span data-ttu-id="1a951-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="1a951-185">connectionType</span></span>|[<span data-ttu-id="1a951-186">windowsvpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="1a951-186">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="1a951-187">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="1a951-187">Connection type.</span></span> <span data-ttu-id="1a951-188">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="1a951-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="1a951-189">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="1a951-189">loginGroupOrDomain</span></span>|<span data-ttu-id="1a951-190">文字列</span><span class="sxs-lookup"><span data-stu-id="1a951-190">String</span></span>|<span data-ttu-id="1a951-191">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="1a951-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="1a951-192">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="1a951-192">enableSplitTunneling</span></span>|<span data-ttu-id="1a951-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a951-193">Boolean</span></span>|<span data-ttu-id="1a951-194">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="1a951-194">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="1a951-195">proxyServer</span><span class="sxs-lookup"><span data-stu-id="1a951-195">proxyServer</span></span>|[<span data-ttu-id="1a951-196">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1a951-196">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="1a951-197">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="1a951-197">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="1a951-198">応答</span><span class="sxs-lookup"><span data-stu-id="1a951-198">Response</span></span>
<span data-ttu-id="1a951-199">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a951-199">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a951-200">例</span><span class="sxs-lookup"><span data-stu-id="1a951-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a951-201">要求</span><span class="sxs-lookup"><span data-stu-id="1a951-201">Request</span></span>
<span data-ttu-id="1a951-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a951-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="1a951-203">応答</span><span class="sxs-lookup"><span data-stu-id="1a951-203">Response</span></span>
<span data-ttu-id="1a951-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a951-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





