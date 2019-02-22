---
title: windowsPhone81VpnConfiguration の更新
description: windowsPhone81VpnConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c12b314b2b7971cd0f85d0ef7908fde7c1181af6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163519"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="0069e-103">windowsPhone81VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0069e-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="0069e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0069e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0069e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0069e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0069e-106">[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0069e-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0069e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0069e-107">Prerequisites</span></span>
<span data-ttu-id="0069e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0069e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0069e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0069e-110">Permission type</span></span>|<span data-ttu-id="0069e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0069e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0069e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0069e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0069e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0069e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0069e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0069e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0069e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0069e-115">Not supported.</span></span>|
|<span data-ttu-id="0069e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0069e-116">Application</span></span>|<span data-ttu-id="0069e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0069e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0069e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0069e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0069e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0069e-119">Request headers</span></span>
|<span data-ttu-id="0069e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0069e-120">Header</span></span>|<span data-ttu-id="0069e-121">値</span><span class="sxs-lookup"><span data-stu-id="0069e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0069e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0069e-122">Authorization</span></span>|<span data-ttu-id="0069e-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0069e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0069e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0069e-124">Accept</span></span>|<span data-ttu-id="0069e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0069e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0069e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0069e-126">Request body</span></span>
<span data-ttu-id="0069e-127">要求本文で、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0069e-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="0069e-128">次の表に、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0069e-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="0069e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0069e-129">Property</span></span>|<span data-ttu-id="0069e-130">型</span><span class="sxs-lookup"><span data-stu-id="0069e-130">Type</span></span>|<span data-ttu-id="0069e-131">説明</span><span class="sxs-lookup"><span data-stu-id="0069e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0069e-132">id</span><span class="sxs-lookup"><span data-stu-id="0069e-132">id</span></span>|<span data-ttu-id="0069e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0069e-133">String</span></span>|<span data-ttu-id="0069e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0069e-134">Key of the entity.</span></span> <span data-ttu-id="0069e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0069e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0069e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0069e-137">DateTimeOffset</span></span>|<span data-ttu-id="0069e-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0069e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0069e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0069e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0069e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0069e-141">String collection</span></span>|<span data-ttu-id="0069e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0069e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0069e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0069e-144">supportsScopeTags</span></span>|<span data-ttu-id="0069e-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="0069e-145">Boolean</span></span>|<span data-ttu-id="0069e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0069e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0069e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0069e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0069e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0069e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0069e-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0069e-149">This property is read-only.</span></span> <span data-ttu-id="0069e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0069e-151">createdDateTime</span></span>|<span data-ttu-id="0069e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0069e-152">DateTimeOffset</span></span>|<span data-ttu-id="0069e-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0069e-153">DateTime the object was created.</span></span> <span data-ttu-id="0069e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-155">説明</span><span class="sxs-lookup"><span data-stu-id="0069e-155">description</span></span>|<span data-ttu-id="0069e-156">String</span><span class="sxs-lookup"><span data-stu-id="0069e-156">String</span></span>|<span data-ttu-id="0069e-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0069e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0069e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0069e-159">displayName</span></span>|<span data-ttu-id="0069e-160">String</span><span class="sxs-lookup"><span data-stu-id="0069e-160">String</span></span>|<span data-ttu-id="0069e-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0069e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0069e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-163">version</span><span class="sxs-lookup"><span data-stu-id="0069e-163">version</span></span>|<span data-ttu-id="0069e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0069e-164">Int32</span></span>|<span data-ttu-id="0069e-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0069e-165">Version of the device configuration.</span></span> <span data-ttu-id="0069e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="0069e-167">connectionName</span></span>|<span data-ttu-id="0069e-168">String</span><span class="sxs-lookup"><span data-stu-id="0069e-168">String</span></span>|<span data-ttu-id="0069e-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="0069e-169">Connection name displayed to the user.</span></span> <span data-ttu-id="0069e-170">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-171">サーバー</span><span class="sxs-lookup"><span data-stu-id="0069e-171">servers</span></span>|<span data-ttu-id="0069e-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0069e-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0069e-173">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="0069e-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="0069e-174">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0069e-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0069e-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0069e-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0069e-176">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-177">customXml</span><span class="sxs-lookup"><span data-stu-id="0069e-177">customXml</span></span>|<span data-ttu-id="0069e-178">Binary</span><span class="sxs-lookup"><span data-stu-id="0069e-178">Binary</span></span>|<span data-ttu-id="0069e-179">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="0069e-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0069e-180">(UTF8 でエンコードされたバイト配列)[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0069e-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="0069e-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="0069e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0069e-182">Boolean</span></span>|<span data-ttu-id="0069e-183">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0069e-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="0069e-184">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0069e-184">This property is read-only.</span></span> <span data-ttu-id="0069e-185">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0069e-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="0069e-186">connectionType</span></span>|[<span data-ttu-id="0069e-187">windowsvpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="0069e-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="0069e-188">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="0069e-188">Connection type.</span></span> <span data-ttu-id="0069e-189">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0069e-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="0069e-190">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="0069e-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="0069e-191">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="0069e-191">loginGroupOrDomain</span></span>|<span data-ttu-id="0069e-192">String</span><span class="sxs-lookup"><span data-stu-id="0069e-192">String</span></span>|<span data-ttu-id="0069e-193">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="0069e-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0069e-194">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0069e-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-195">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="0069e-195">enableSplitTunneling</span></span>|<span data-ttu-id="0069e-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="0069e-196">Boolean</span></span>|<span data-ttu-id="0069e-197">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="0069e-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="0069e-198">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0069e-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-199">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0069e-199">proxyServer</span></span>|[<span data-ttu-id="0069e-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0069e-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="0069e-201">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="0069e-201">Proxy Server.</span></span> <span data-ttu-id="0069e-202">[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0069e-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0069e-203">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="0069e-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="0069e-204">ブール値</span><span class="sxs-lookup"><span data-stu-id="0069e-204">Boolean</span></span>|<span data-ttu-id="0069e-205">会社の wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="0069e-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="0069e-206">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="0069e-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="0069e-207">ブール値</span><span class="sxs-lookup"><span data-stu-id="0069e-207">Boolean</span></span>|<span data-ttu-id="0069e-208">自宅 wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="0069e-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="0069e-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0069e-209">authenticationMethod</span></span>|[<span data-ttu-id="0069e-210">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0069e-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0069e-211">認証方法。</span><span class="sxs-lookup"><span data-stu-id="0069e-211">Authentication method.</span></span> <span data-ttu-id="0069e-212">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="0069e-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0069e-213">rememberusercredentials</span><span class="sxs-lookup"><span data-stu-id="0069e-213">rememberUserCredentials</span></span>|<span data-ttu-id="0069e-214">ブール値</span><span class="sxs-lookup"><span data-stu-id="0069e-214">Boolean</span></span>|<span data-ttu-id="0069e-215">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="0069e-215">Remember user credentials.</span></span>|
|<span data-ttu-id="0069e-216">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="0069e-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="0069e-217">String collection</span><span class="sxs-lookup"><span data-stu-id="0069e-217">String collection</span></span>|<span data-ttu-id="0069e-218">DNS サフィックス検索一覧。</span><span class="sxs-lookup"><span data-stu-id="0069e-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="0069e-219">応答</span><span class="sxs-lookup"><span data-stu-id="0069e-219">Response</span></span>
<span data-ttu-id="0069e-220">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0069e-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0069e-221">例</span><span class="sxs-lookup"><span data-stu-id="0069e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="0069e-222">要求</span><span class="sxs-lookup"><span data-stu-id="0069e-222">Request</span></span>
<span data-ttu-id="0069e-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0069e-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0069e-224">応答</span><span class="sxs-lookup"><span data-stu-id="0069e-224">Response</span></span>
<span data-ttu-id="0069e-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0069e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




