---
title: WindowsPhone81VpnConfiguration を作成する
description: 新しい windowsPhone81VpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82e7dd4e3737ba39790554c62f9bb6829ce2d206
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917591"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="95971-103">WindowsPhone81VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="95971-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="95971-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95971-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95971-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95971-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95971-106">新しい[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="95971-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95971-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95971-107">Prerequisites</span></span>
<span data-ttu-id="95971-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95971-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95971-110">Permission type</span></span>|<span data-ttu-id="95971-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95971-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95971-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95971-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95971-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95971-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95971-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95971-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95971-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95971-115">Not supported.</span></span>|
|<span data-ttu-id="95971-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95971-116">Application</span></span>|<span data-ttu-id="95971-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95971-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95971-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95971-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95971-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95971-119">Request headers</span></span>
|<span data-ttu-id="95971-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95971-120">Header</span></span>|<span data-ttu-id="95971-121">値</span><span class="sxs-lookup"><span data-stu-id="95971-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95971-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95971-122">Authorization</span></span>|<span data-ttu-id="95971-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95971-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95971-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95971-124">Accept</span></span>|<span data-ttu-id="95971-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95971-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95971-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95971-126">Request body</span></span>
<span data-ttu-id="95971-127">要求本文で、windowsPhone81VpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95971-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="95971-128">次の表に、windowsPhone81VpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95971-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="95971-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95971-129">Property</span></span>|<span data-ttu-id="95971-130">型</span><span class="sxs-lookup"><span data-stu-id="95971-130">Type</span></span>|<span data-ttu-id="95971-131">説明</span><span class="sxs-lookup"><span data-stu-id="95971-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95971-132">id</span><span class="sxs-lookup"><span data-stu-id="95971-132">id</span></span>|<span data-ttu-id="95971-133">文字列</span><span class="sxs-lookup"><span data-stu-id="95971-133">String</span></span>|<span data-ttu-id="95971-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95971-134">Key of the entity.</span></span> <span data-ttu-id="95971-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95971-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95971-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95971-137">DateTimeOffset</span></span>|<span data-ttu-id="95971-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="95971-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95971-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95971-140">roleScopeTagIds</span></span>|<span data-ttu-id="95971-141">String collection</span><span class="sxs-lookup"><span data-stu-id="95971-141">String collection</span></span>|<span data-ttu-id="95971-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="95971-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95971-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95971-144">supportsScopeTags</span></span>|<span data-ttu-id="95971-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-145">Boolean</span></span>|<span data-ttu-id="95971-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95971-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95971-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="95971-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95971-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="95971-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95971-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="95971-149">This property is read-only.</span></span> <span data-ttu-id="95971-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95971-151">createdDateTime</span></span>|<span data-ttu-id="95971-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95971-152">DateTimeOffset</span></span>|<span data-ttu-id="95971-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="95971-153">DateTime the object was created.</span></span> <span data-ttu-id="95971-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-155">description</span><span class="sxs-lookup"><span data-stu-id="95971-155">description</span></span>|<span data-ttu-id="95971-156">String</span><span class="sxs-lookup"><span data-stu-id="95971-156">String</span></span>|<span data-ttu-id="95971-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="95971-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95971-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95971-159">displayName</span></span>|<span data-ttu-id="95971-160">String</span><span class="sxs-lookup"><span data-stu-id="95971-160">String</span></span>|<span data-ttu-id="95971-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="95971-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95971-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-163">version</span><span class="sxs-lookup"><span data-stu-id="95971-163">version</span></span>|<span data-ttu-id="95971-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95971-164">Int32</span></span>|<span data-ttu-id="95971-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="95971-165">Version of the device configuration.</span></span> <span data-ttu-id="95971-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95971-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="95971-167">connectionName</span></span>|<span data-ttu-id="95971-168">String</span><span class="sxs-lookup"><span data-stu-id="95971-168">String</span></span>|<span data-ttu-id="95971-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="95971-169">Connection name displayed to the user.</span></span> <span data-ttu-id="95971-170">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-171">サーバ</span><span class="sxs-lookup"><span data-stu-id="95971-171">servers</span></span>|<span data-ttu-id="95971-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95971-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="95971-173">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="95971-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="95971-174">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="95971-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="95971-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="95971-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="95971-176">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-177">customXml</span><span class="sxs-lookup"><span data-stu-id="95971-177">customXml</span></span>|<span data-ttu-id="95971-178">Binary</span><span class="sxs-lookup"><span data-stu-id="95971-178">Binary</span></span>|<span data-ttu-id="95971-179">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="95971-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="95971-180">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="95971-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="95971-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="95971-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-182">Boolean</span></span>|<span data-ttu-id="95971-183">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="95971-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="95971-184">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95971-184">This property is read-only.</span></span> <span data-ttu-id="95971-185">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="95971-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="95971-186">connectionType</span></span>|[<span data-ttu-id="95971-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="95971-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="95971-188">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="95971-188">Connection type.</span></span> <span data-ttu-id="95971-189">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95971-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="95971-190">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="95971-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="95971-191">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="95971-191">loginGroupOrDomain</span></span>|<span data-ttu-id="95971-192">String</span><span class="sxs-lookup"><span data-stu-id="95971-192">String</span></span>|<span data-ttu-id="95971-193">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="95971-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="95971-194">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="95971-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-195">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="95971-195">enableSplitTunneling</span></span>|<span data-ttu-id="95971-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-196">Boolean</span></span>|<span data-ttu-id="95971-197">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="95971-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="95971-198">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="95971-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-199">proxyServer</span><span class="sxs-lookup"><span data-stu-id="95971-199">proxyServer</span></span>|[<span data-ttu-id="95971-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="95971-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="95971-201">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="95971-201">Proxy Server.</span></span> <span data-ttu-id="95971-202">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="95971-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="95971-203">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="95971-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="95971-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-204">Boolean</span></span>|<span data-ttu-id="95971-205">会社の Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="95971-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="95971-206">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="95971-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="95971-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-207">Boolean</span></span>|<span data-ttu-id="95971-208">自宅 Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="95971-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="95971-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="95971-209">authenticationMethod</span></span>|[<span data-ttu-id="95971-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="95971-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="95971-211">認証方法。</span><span class="sxs-lookup"><span data-stu-id="95971-211">Authentication method.</span></span> <span data-ttu-id="95971-212">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="95971-212">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="95971-213">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="95971-213">rememberUserCredentials</span></span>|<span data-ttu-id="95971-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="95971-214">Boolean</span></span>|<span data-ttu-id="95971-215">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="95971-215">Remember user credentials.</span></span>|
|<span data-ttu-id="95971-216">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="95971-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="95971-217">String collection</span><span class="sxs-lookup"><span data-stu-id="95971-217">String collection</span></span>|<span data-ttu-id="95971-218">DNS サフィックス検索一覧。</span><span class="sxs-lookup"><span data-stu-id="95971-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="95971-219">応答</span><span class="sxs-lookup"><span data-stu-id="95971-219">Response</span></span>
<span data-ttu-id="95971-220">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95971-220">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95971-221">例</span><span class="sxs-lookup"><span data-stu-id="95971-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="95971-222">要求</span><span class="sxs-lookup"><span data-stu-id="95971-222">Request</span></span>
<span data-ttu-id="95971-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95971-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="95971-224">応答</span><span class="sxs-lookup"><span data-stu-id="95971-224">Response</span></span>
<span data-ttu-id="95971-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95971-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```




