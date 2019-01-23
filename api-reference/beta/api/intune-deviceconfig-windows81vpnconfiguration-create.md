---
title: Windows81VpnConfiguration を作成します。
description: 新しい windows81VpnConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f448d021c1135725cd372115acca1e5a0f8a807e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419780"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="e8cec-103">Windows81VpnConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="e8cec-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8cec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8cec-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8cec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8cec-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8cec-107">新しい[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8cec-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e8cec-108">Prerequisites</span></span>
<span data-ttu-id="e8cec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8cec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e8cec-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8cec-111">Permission type</span></span>|<span data-ttu-id="e8cec-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8cec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8cec-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8cec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8cec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8cec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8cec-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8cec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8cec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8cec-116">Not supported.</span></span>|
|<span data-ttu-id="e8cec-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8cec-117">Application</span></span>|<span data-ttu-id="e8cec-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8cec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8cec-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8cec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e8cec-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8cec-120">Request headers</span></span>
|<span data-ttu-id="e8cec-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8cec-121">Header</span></span>|<span data-ttu-id="e8cec-122">値</span><span class="sxs-lookup"><span data-stu-id="e8cec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8cec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8cec-123">Authorization</span></span>|<span data-ttu-id="e8cec-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e8cec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8cec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8cec-125">Accept</span></span>|<span data-ttu-id="e8cec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8cec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8cec-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8cec-127">Request body</span></span>
<span data-ttu-id="e8cec-128">要求の本文に windows81VpnConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="e8cec-129">次の表は、windows81VpnConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="e8cec-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8cec-130">Property</span></span>|<span data-ttu-id="e8cec-131">型</span><span class="sxs-lookup"><span data-stu-id="e8cec-131">Type</span></span>|<span data-ttu-id="e8cec-132">説明</span><span class="sxs-lookup"><span data-stu-id="e8cec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8cec-133">id</span><span class="sxs-lookup"><span data-stu-id="e8cec-133">id</span></span>|<span data-ttu-id="e8cec-134">String</span><span class="sxs-lookup"><span data-stu-id="e8cec-134">String</span></span>|<span data-ttu-id="e8cec-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e8cec-135">Key of the entity.</span></span> <span data-ttu-id="e8cec-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8cec-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e8cec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8cec-138">DateTimeOffset</span></span>|<span data-ttu-id="e8cec-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e8cec-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e8cec-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8cec-141">roleScopeTagIds</span></span>|<span data-ttu-id="e8cec-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e8cec-142">String collection</span></span>|<span data-ttu-id="e8cec-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e8cec-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e8cec-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e8cec-145">supportsScopeTags</span></span>|<span data-ttu-id="e8cec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8cec-146">Boolean</span></span>|<span data-ttu-id="e8cec-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e8cec-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e8cec-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e8cec-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="e8cec-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e8cec-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-150">This property is read-only.</span></span> <span data-ttu-id="e8cec-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8cec-152">createdDateTime</span></span>|<span data-ttu-id="e8cec-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8cec-153">DateTimeOffset</span></span>|<span data-ttu-id="e8cec-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e8cec-154">DateTime the object was created.</span></span> <span data-ttu-id="e8cec-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-156">説明</span><span class="sxs-lookup"><span data-stu-id="e8cec-156">description</span></span>|<span data-ttu-id="e8cec-157">String</span><span class="sxs-lookup"><span data-stu-id="e8cec-157">String</span></span>|<span data-ttu-id="e8cec-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e8cec-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8cec-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e8cec-160">displayName</span></span>|<span data-ttu-id="e8cec-161">String</span><span class="sxs-lookup"><span data-stu-id="e8cec-161">String</span></span>|<span data-ttu-id="e8cec-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e8cec-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8cec-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-164">version</span><span class="sxs-lookup"><span data-stu-id="e8cec-164">version</span></span>|<span data-ttu-id="e8cec-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e8cec-165">Int32</span></span>|<span data-ttu-id="e8cec-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e8cec-166">Version of the device configuration.</span></span> <span data-ttu-id="e8cec-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e8cec-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="e8cec-168">connectionName</span></span>|<span data-ttu-id="e8cec-169">String</span><span class="sxs-lookup"><span data-stu-id="e8cec-169">String</span></span>|<span data-ttu-id="e8cec-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e8cec-170">Connection name displayed to the user.</span></span> <span data-ttu-id="e8cec-171">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e8cec-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-172">サーバー</span><span class="sxs-lookup"><span data-stu-id="e8cec-172">servers</span></span>|<span data-ttu-id="e8cec-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e8cec-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="e8cec-174">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="e8cec-175">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e8cec-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="e8cec-176">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e8cec-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e8cec-177">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e8cec-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-178">customXml</span><span class="sxs-lookup"><span data-stu-id="e8cec-178">customXml</span></span>|<span data-ttu-id="e8cec-179">Binary</span><span class="sxs-lookup"><span data-stu-id="e8cec-179">Binary</span></span>|<span data-ttu-id="e8cec-180">VPN 接続を構成するユーザー設定の XML コマンドです。</span><span class="sxs-lookup"><span data-stu-id="e8cec-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="e8cec-181">(UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e8cec-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="e8cec-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="e8cec-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="e8cec-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8cec-183">Boolean</span></span>|<span data-ttu-id="e8cec-184">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e8cec-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="e8cec-185">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-185">This property is read-only.</span></span>|
|<span data-ttu-id="e8cec-186">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="e8cec-186">connectionType</span></span>|[<span data-ttu-id="e8cec-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="e8cec-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="e8cec-188">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-188">Connection type.</span></span> <span data-ttu-id="e8cec-189">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="e8cec-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="e8cec-190">loginGroupOrDomain</span></span>|<span data-ttu-id="e8cec-191">String</span><span class="sxs-lookup"><span data-stu-id="e8cec-191">String</span></span>|<span data-ttu-id="e8cec-192">ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。</span><span class="sxs-lookup"><span data-stu-id="e8cec-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="e8cec-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="e8cec-193">enableSplitTunneling</span></span>|<span data-ttu-id="e8cec-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8cec-194">Boolean</span></span>|<span data-ttu-id="e8cec-195">分割は、VPN のトンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e8cec-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="e8cec-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="e8cec-196">proxyServer</span></span>|[<span data-ttu-id="e8cec-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="e8cec-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="e8cec-198">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="e8cec-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="e8cec-199">応答</span><span class="sxs-lookup"><span data-stu-id="e8cec-199">Response</span></span>
<span data-ttu-id="e8cec-200">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e8cec-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8cec-201">例</span><span class="sxs-lookup"><span data-stu-id="e8cec-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8cec-202">要求</span><span class="sxs-lookup"><span data-stu-id="e8cec-202">Request</span></span>
<span data-ttu-id="e8cec-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8cec-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8cec-204">応答</span><span class="sxs-lookup"><span data-stu-id="e8cec-204">Response</span></span>
<span data-ttu-id="e8cec-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8cec-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




