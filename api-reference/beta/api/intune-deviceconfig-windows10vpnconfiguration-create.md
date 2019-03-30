---
title: windows10VpnConfiguration を作成する
description: 新しい windows10VpnConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa05bee08f30936ca496499090f8bdf9ee1877c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988659"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="55a86-103">windows10VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="55a86-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="55a86-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55a86-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55a86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55a86-106">新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="55a86-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55a86-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="55a86-107">Prerequisites</span></span>
<span data-ttu-id="55a86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55a86-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55a86-110">Permission type</span></span>|<span data-ttu-id="55a86-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="55a86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55a86-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55a86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55a86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55a86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55a86-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55a86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55a86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a86-115">Not supported.</span></span>|
|<span data-ttu-id="55a86-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55a86-116">Application</span></span>|<span data-ttu-id="55a86-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55a86-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55a86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="55a86-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55a86-119">Request headers</span></span>
|<span data-ttu-id="55a86-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55a86-120">Header</span></span>|<span data-ttu-id="55a86-121">値</span><span class="sxs-lookup"><span data-stu-id="55a86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55a86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55a86-122">Authorization</span></span>|<span data-ttu-id="55a86-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="55a86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55a86-124">承諾</span><span class="sxs-lookup"><span data-stu-id="55a86-124">Accept</span></span>|<span data-ttu-id="55a86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55a86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55a86-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="55a86-126">Request body</span></span>
<span data-ttu-id="55a86-127">要求本文で、windows10VpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="55a86-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="55a86-128">次の表に、windows10VpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="55a86-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="55a86-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55a86-129">Property</span></span>|<span data-ttu-id="55a86-130">型</span><span class="sxs-lookup"><span data-stu-id="55a86-130">Type</span></span>|<span data-ttu-id="55a86-131">説明</span><span class="sxs-lookup"><span data-stu-id="55a86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55a86-132">id</span><span class="sxs-lookup"><span data-stu-id="55a86-132">id</span></span>|<span data-ttu-id="55a86-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="55a86-133">String</span></span>|<span data-ttu-id="55a86-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="55a86-134">Key of the entity.</span></span> <span data-ttu-id="55a86-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55a86-136">lastModifiedDateTime</span></span>|<span data-ttu-id="55a86-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55a86-137">DateTimeOffset</span></span>|<span data-ttu-id="55a86-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="55a86-138">DateTime the object was last modified.</span></span> <span data-ttu-id="55a86-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="55a86-140">roleScopeTagIds</span></span>|<span data-ttu-id="55a86-141">String collection</span><span class="sxs-lookup"><span data-stu-id="55a86-141">String collection</span></span>|<span data-ttu-id="55a86-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="55a86-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="55a86-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="55a86-144">supportsScopeTags</span></span>|<span data-ttu-id="55a86-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-145">Boolean</span></span>|<span data-ttu-id="55a86-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="55a86-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="55a86-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="55a86-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="55a86-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="55a86-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="55a86-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="55a86-149">This property is read-only.</span></span> <span data-ttu-id="55a86-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55a86-151">createdDateTime</span></span>|<span data-ttu-id="55a86-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55a86-152">DateTimeOffset</span></span>|<span data-ttu-id="55a86-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="55a86-153">DateTime the object was created.</span></span> <span data-ttu-id="55a86-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-155">description</span><span class="sxs-lookup"><span data-stu-id="55a86-155">description</span></span>|<span data-ttu-id="55a86-156">String</span><span class="sxs-lookup"><span data-stu-id="55a86-156">String</span></span>|<span data-ttu-id="55a86-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="55a86-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55a86-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-159">displayName</span><span class="sxs-lookup"><span data-stu-id="55a86-159">displayName</span></span>|<span data-ttu-id="55a86-160">String</span><span class="sxs-lookup"><span data-stu-id="55a86-160">String</span></span>|<span data-ttu-id="55a86-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="55a86-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55a86-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-163">version</span><span class="sxs-lookup"><span data-stu-id="55a86-163">version</span></span>|<span data-ttu-id="55a86-164">Int32</span><span class="sxs-lookup"><span data-stu-id="55a86-164">Int32</span></span>|<span data-ttu-id="55a86-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="55a86-165">Version of the device configuration.</span></span> <span data-ttu-id="55a86-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="55a86-167">connectionName</span></span>|<span data-ttu-id="55a86-168">String</span><span class="sxs-lookup"><span data-stu-id="55a86-168">String</span></span>|<span data-ttu-id="55a86-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="55a86-169">Connection name displayed to the user.</span></span> <span data-ttu-id="55a86-170">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-171">サーバ</span><span class="sxs-lookup"><span data-stu-id="55a86-171">servers</span></span>|<span data-ttu-id="55a86-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="55a86-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="55a86-173">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="55a86-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="55a86-174">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="55a86-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="55a86-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="55a86-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="55a86-176">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-177">customXml</span><span class="sxs-lookup"><span data-stu-id="55a86-177">customXml</span></span>|<span data-ttu-id="55a86-178">Binary</span><span class="sxs-lookup"><span data-stu-id="55a86-178">Binary</span></span>|<span data-ttu-id="55a86-179">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="55a86-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="55a86-180">(UTF8 でエンコードされたバイト配列)[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="55a86-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="55a86-181">profiletarget</span><span class="sxs-lookup"><span data-stu-id="55a86-181">profileTarget</span></span>|[<span data-ttu-id="55a86-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="55a86-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="55a86-183">プロファイルのターゲットの種類。</span><span class="sxs-lookup"><span data-stu-id="55a86-183">Profile target type.</span></span> <span data-ttu-id="55a86-184">使用可能な値は、`user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="55a86-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="55a86-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="55a86-185">connectionType</span></span>|[<span data-ttu-id="55a86-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="55a86-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="55a86-187">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="55a86-187">Connection type.</span></span> <span data-ttu-id="55a86-188">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="55a86-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="55a86-189">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="55a86-189">enableSplitTunneling</span></span>|<span data-ttu-id="55a86-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-190">Boolean</span></span>|<span data-ttu-id="55a86-191">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="55a86-192">enablealwayson</span><span class="sxs-lookup"><span data-stu-id="55a86-192">enableAlwaysOn</span></span>|<span data-ttu-id="55a86-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-193">Boolean</span></span>|<span data-ttu-id="55a86-194">Always On モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="55a86-195">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="55a86-195">enableDeviceTunnel</span></span>|<span data-ttu-id="55a86-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-196">Boolean</span></span>|<span data-ttu-id="55a86-197">デバイストンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="55a86-198">enablednsregistration</span><span class="sxs-lookup"><span data-stu-id="55a86-198">enableDnsRegistration</span></span>|<span data-ttu-id="55a86-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-199">Boolean</span></span>|<span data-ttu-id="55a86-200">内部 DNS での IP アドレス登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="55a86-201">dnssuffixes</span><span class="sxs-lookup"><span data-stu-id="55a86-201">dnsSuffixes</span></span>|<span data-ttu-id="55a86-202">String collection</span><span class="sxs-lookup"><span data-stu-id="55a86-202">String collection</span></span>|<span data-ttu-id="55a86-203">dns の検索一覧に追加する dns サフィックスを指定して、短い名前を適切にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="55a86-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="55a86-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="55a86-204">authenticationMethod</span></span>|[<span data-ttu-id="55a86-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="55a86-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="55a86-206">認証方法。</span><span class="sxs-lookup"><span data-stu-id="55a86-206">Authentication method.</span></span> <span data-ttu-id="55a86-207">使用可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="55a86-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="55a86-208">rememberusercredentials</span><span class="sxs-lookup"><span data-stu-id="55a86-208">rememberUserCredentials</span></span>|<span data-ttu-id="55a86-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-209">Boolean</span></span>|<span data-ttu-id="55a86-210">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="55a86-210">Remember user credentials.</span></span>|
|<span data-ttu-id="55a86-211">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="55a86-211">enableConditionalAccess</span></span>|<span data-ttu-id="55a86-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-212">Boolean</span></span>|<span data-ttu-id="55a86-213">条件付きアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-213">Enable conditional access.</span></span>|
|<span data-ttu-id="55a86-214">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="55a86-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="55a86-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-215">Boolean</span></span>|<span data-ttu-id="55a86-216">代替証明書を使用してシングルサインオン (SSO) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="55a86-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="55a86-217">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="55a86-217">singleSignOnEku</span></span>|[<span data-ttu-id="55a86-218">extendedkeyusage</span><span class="sxs-lookup"><span data-stu-id="55a86-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="55a86-219">シングルサインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="55a86-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="55a86-220">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="55a86-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="55a86-221">String</span><span class="sxs-lookup"><span data-stu-id="55a86-221">String</span></span>|<span data-ttu-id="55a86-222">シングルサインオン発行者ハッシュ。</span><span class="sxs-lookup"><span data-stu-id="55a86-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="55a86-223">eapxml</span><span class="sxs-lookup"><span data-stu-id="55a86-223">eapXml</span></span>|<span data-ttu-id="55a86-224">Binary</span><span class="sxs-lookup"><span data-stu-id="55a86-224">Binary</span></span>|<span data-ttu-id="55a86-225">拡張認証プロトコル (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="55a86-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="55a86-226">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="55a86-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="55a86-227">proxyServer</span><span class="sxs-lookup"><span data-stu-id="55a86-227">proxyServer</span></span>|[<span data-ttu-id="55a86-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="55a86-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="55a86-229">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="55a86-229">Proxy Server.</span></span>|
|<span data-ttu-id="55a86-230">associatedApps</span><span class="sxs-lookup"><span data-stu-id="55a86-230">associatedApps</span></span>|<span data-ttu-id="55a86-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="55a86-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="55a86-232">関連付けられているアプリ。</span><span class="sxs-lookup"><span data-stu-id="55a86-232">Associated Apps.</span></span> <span data-ttu-id="55a86-233">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="55a86-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="55a86-234">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="55a86-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="55a86-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="55a86-235">Boolean</span></span>|<span data-ttu-id="55a86-236">関連付けられているアプリのみが接続 (アプリごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="55a86-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="55a86-237">windowsinformationprotectiondomain</span><span class="sxs-lookup"><span data-stu-id="55a86-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="55a86-238">String</span><span class="sxs-lookup"><span data-stu-id="55a86-238">String</span></span>|<span data-ttu-id="55a86-239">この接続に関連付ける Windows Information Protection (WIP) ドメイン。</span><span class="sxs-lookup"><span data-stu-id="55a86-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="55a86-240">trafficRules</span><span class="sxs-lookup"><span data-stu-id="55a86-240">trafficRules</span></span>|<span data-ttu-id="55a86-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="55a86-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="55a86-242">トラフィックルール。</span><span class="sxs-lookup"><span data-stu-id="55a86-242">Traffic rules.</span></span> <span data-ttu-id="55a86-243">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="55a86-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="55a86-244">返信</span><span class="sxs-lookup"><span data-stu-id="55a86-244">routes</span></span>|<span data-ttu-id="55a86-245">[vpnroute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="55a86-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="55a86-246">ルート (サードパーティプロバイダーの場合はオプション)。</span><span class="sxs-lookup"><span data-stu-id="55a86-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="55a86-247">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="55a86-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="55a86-248">dnsrules</span><span class="sxs-lookup"><span data-stu-id="55a86-248">dnsRules</span></span>|<span data-ttu-id="55a86-249">[vpndnsrule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="55a86-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="55a86-250">DNS ルール。</span><span class="sxs-lookup"><span data-stu-id="55a86-250">DNS rules.</span></span> <span data-ttu-id="55a86-251">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="55a86-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="55a86-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="55a86-252">trustedNetworkDomains</span></span>|<span data-ttu-id="55a86-253">String collection</span><span class="sxs-lookup"><span data-stu-id="55a86-253">String collection</span></span>|<span data-ttu-id="55a86-254">信頼されたネットワークドメイン</span><span class="sxs-lookup"><span data-stu-id="55a86-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="55a86-255">応答</span><span class="sxs-lookup"><span data-stu-id="55a86-255">Response</span></span>
<span data-ttu-id="55a86-256">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="55a86-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55a86-257">例</span><span class="sxs-lookup"><span data-stu-id="55a86-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="55a86-258">要求</span><span class="sxs-lookup"><span data-stu-id="55a86-258">Request</span></span>
<span data-ttu-id="55a86-259">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="55a86-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="55a86-260">応答</span><span class="sxs-lookup"><span data-stu-id="55a86-260">Response</span></span>
<span data-ttu-id="55a86-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="55a86-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3559

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```




