---
title: Windows10VpnConfiguration を作成する
description: 新しい windows10VpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40a1462757a22030db0640606df270b4b7abf585
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975166"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="34586-103">Windows10VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="34586-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="34586-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34586-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34586-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34586-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34586-106">新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="34586-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34586-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="34586-107">Prerequisites</span></span>
<span data-ttu-id="34586-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34586-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34586-110">Permission type</span></span>|<span data-ttu-id="34586-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="34586-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34586-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34586-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34586-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34586-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34586-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34586-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34586-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34586-115">Not supported.</span></span>|
|<span data-ttu-id="34586-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34586-116">Application</span></span>|<span data-ttu-id="34586-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34586-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34586-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34586-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34586-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34586-119">Request headers</span></span>
|<span data-ttu-id="34586-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34586-120">Header</span></span>|<span data-ttu-id="34586-121">値</span><span class="sxs-lookup"><span data-stu-id="34586-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34586-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34586-122">Authorization</span></span>|<span data-ttu-id="34586-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="34586-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34586-124">承諾</span><span class="sxs-lookup"><span data-stu-id="34586-124">Accept</span></span>|<span data-ttu-id="34586-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34586-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34586-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="34586-126">Request body</span></span>
<span data-ttu-id="34586-127">要求本文で、windows10VpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34586-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="34586-128">次の表に、windows10VpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="34586-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="34586-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34586-129">Property</span></span>|<span data-ttu-id="34586-130">型</span><span class="sxs-lookup"><span data-stu-id="34586-130">Type</span></span>|<span data-ttu-id="34586-131">説明</span><span class="sxs-lookup"><span data-stu-id="34586-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34586-132">id</span><span class="sxs-lookup"><span data-stu-id="34586-132">id</span></span>|<span data-ttu-id="34586-133">文字列</span><span class="sxs-lookup"><span data-stu-id="34586-133">String</span></span>|<span data-ttu-id="34586-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="34586-134">Key of the entity.</span></span> <span data-ttu-id="34586-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34586-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34586-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34586-137">DateTimeOffset</span></span>|<span data-ttu-id="34586-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="34586-138">DateTime the object was last modified.</span></span> <span data-ttu-id="34586-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34586-140">roleScopeTagIds</span></span>|<span data-ttu-id="34586-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-141">String collection</span></span>|<span data-ttu-id="34586-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="34586-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34586-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34586-144">supportsScopeTags</span></span>|<span data-ttu-id="34586-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-145">Boolean</span></span>|<span data-ttu-id="34586-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="34586-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34586-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="34586-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34586-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="34586-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34586-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="34586-149">This property is read-only.</span></span> <span data-ttu-id="34586-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34586-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34586-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34586-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34586-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="34586-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="34586-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34586-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34586-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34586-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34586-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="34586-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="34586-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="34586-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34586-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="34586-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34586-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="34586-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="34586-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34586-163">createdDateTime</span></span>|<span data-ttu-id="34586-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34586-164">DateTimeOffset</span></span>|<span data-ttu-id="34586-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="34586-165">DateTime the object was created.</span></span> <span data-ttu-id="34586-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-167">description</span><span class="sxs-lookup"><span data-stu-id="34586-167">description</span></span>|<span data-ttu-id="34586-168">String</span><span class="sxs-lookup"><span data-stu-id="34586-168">String</span></span>|<span data-ttu-id="34586-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="34586-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34586-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-171">displayName</span><span class="sxs-lookup"><span data-stu-id="34586-171">displayName</span></span>|<span data-ttu-id="34586-172">String</span><span class="sxs-lookup"><span data-stu-id="34586-172">String</span></span>|<span data-ttu-id="34586-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="34586-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34586-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-175">version</span><span class="sxs-lookup"><span data-stu-id="34586-175">version</span></span>|<span data-ttu-id="34586-176">Int32</span><span class="sxs-lookup"><span data-stu-id="34586-176">Int32</span></span>|<span data-ttu-id="34586-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="34586-177">Version of the device configuration.</span></span> <span data-ttu-id="34586-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34586-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="34586-179">connectionName</span></span>|<span data-ttu-id="34586-180">String</span><span class="sxs-lookup"><span data-stu-id="34586-180">String</span></span>|<span data-ttu-id="34586-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="34586-181">Connection name displayed to the user.</span></span> <span data-ttu-id="34586-182">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="34586-183">サーバ</span><span class="sxs-lookup"><span data-stu-id="34586-183">servers</span></span>|<span data-ttu-id="34586-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="34586-185">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="34586-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="34586-186">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="34586-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="34586-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="34586-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="34586-188">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="34586-189">customXml</span><span class="sxs-lookup"><span data-stu-id="34586-189">customXml</span></span>|<span data-ttu-id="34586-190">Binary</span><span class="sxs-lookup"><span data-stu-id="34586-190">Binary</span></span>|<span data-ttu-id="34586-191">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="34586-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="34586-192">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="34586-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="34586-193">profileTarget</span><span class="sxs-lookup"><span data-stu-id="34586-193">profileTarget</span></span>|[<span data-ttu-id="34586-194">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="34586-194">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="34586-195">プロファイルのターゲットの種類。</span><span class="sxs-lookup"><span data-stu-id="34586-195">Profile target type.</span></span> <span data-ttu-id="34586-196">可能な値は、`user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="34586-196">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="34586-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="34586-197">connectionType</span></span>|[<span data-ttu-id="34586-198">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="34586-198">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="34586-199">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="34586-199">Connection type.</span></span> <span data-ttu-id="34586-200">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="34586-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="34586-201">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="34586-201">enableSplitTunneling</span></span>|<span data-ttu-id="34586-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-202">Boolean</span></span>|<span data-ttu-id="34586-203">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-203">Enable split tunneling.</span></span>|
|<span data-ttu-id="34586-204">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="34586-204">enableAlwaysOn</span></span>|<span data-ttu-id="34586-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-205">Boolean</span></span>|<span data-ttu-id="34586-206">Always On モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-206">Enable Always On mode.</span></span>|
|<span data-ttu-id="34586-207">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="34586-207">enableDeviceTunnel</span></span>|<span data-ttu-id="34586-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-208">Boolean</span></span>|<span data-ttu-id="34586-209">デバイストンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-209">Enable device tunnel.</span></span>|
|<span data-ttu-id="34586-210">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="34586-210">enableDnsRegistration</span></span>|<span data-ttu-id="34586-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-211">Boolean</span></span>|<span data-ttu-id="34586-212">内部 DNS での IP アドレス登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-212">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="34586-213">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="34586-213">dnsSuffixes</span></span>|<span data-ttu-id="34586-214">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-214">String collection</span></span>|<span data-ttu-id="34586-215">DNS の検索一覧に追加する DNS サフィックスを指定して、短い名前を適切にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="34586-215">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="34586-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34586-216">authenticationMethod</span></span>|[<span data-ttu-id="34586-217">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34586-217">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="34586-218">認証方法。</span><span class="sxs-lookup"><span data-stu-id="34586-218">Authentication method.</span></span> <span data-ttu-id="34586-219">可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="34586-219">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="34586-220">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="34586-220">rememberUserCredentials</span></span>|<span data-ttu-id="34586-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-221">Boolean</span></span>|<span data-ttu-id="34586-222">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="34586-222">Remember user credentials.</span></span>|
|<span data-ttu-id="34586-223">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="34586-223">enableConditionalAccess</span></span>|<span data-ttu-id="34586-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-224">Boolean</span></span>|<span data-ttu-id="34586-225">条件付きアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-225">Enable conditional access.</span></span>|
|<span data-ttu-id="34586-226">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="34586-226">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="34586-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-227">Boolean</span></span>|<span data-ttu-id="34586-228">代替証明書を使用してシングルサインオン (SSO) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="34586-228">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="34586-229">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="34586-229">singleSignOnEku</span></span>|[<span data-ttu-id="34586-230">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="34586-230">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="34586-231">シングルサインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="34586-231">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="34586-232">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="34586-232">singleSignOnIssuerHash</span></span>|<span data-ttu-id="34586-233">String</span><span class="sxs-lookup"><span data-stu-id="34586-233">String</span></span>|<span data-ttu-id="34586-234">シングルサインオン発行者ハッシュ。</span><span class="sxs-lookup"><span data-stu-id="34586-234">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="34586-235">eapXml</span><span class="sxs-lookup"><span data-stu-id="34586-235">eapXml</span></span>|<span data-ttu-id="34586-236">Binary</span><span class="sxs-lookup"><span data-stu-id="34586-236">Binary</span></span>|<span data-ttu-id="34586-237">拡張認証プロトコル (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="34586-237">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="34586-238">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="34586-238">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="34586-239">proxyServer</span><span class="sxs-lookup"><span data-stu-id="34586-239">proxyServer</span></span>|[<span data-ttu-id="34586-240">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="34586-240">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="34586-241">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="34586-241">Proxy Server.</span></span>|
|<span data-ttu-id="34586-242">associatedApps</span><span class="sxs-lookup"><span data-stu-id="34586-242">associatedApps</span></span>|<span data-ttu-id="34586-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="34586-244">関連付けられているアプリ。</span><span class="sxs-lookup"><span data-stu-id="34586-244">Associated Apps.</span></span> <span data-ttu-id="34586-245">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="34586-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="34586-246">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="34586-246">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="34586-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="34586-247">Boolean</span></span>|<span data-ttu-id="34586-248">関連付けられているアプリのみが接続 (アプリごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="34586-248">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="34586-249">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="34586-249">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="34586-250">String</span><span class="sxs-lookup"><span data-stu-id="34586-250">String</span></span>|<span data-ttu-id="34586-251">この接続に関連付ける Windows Information Protection (WIP) ドメイン。</span><span class="sxs-lookup"><span data-stu-id="34586-251">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="34586-252">trafficRules</span><span class="sxs-lookup"><span data-stu-id="34586-252">trafficRules</span></span>|<span data-ttu-id="34586-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="34586-254">トラフィックルール。</span><span class="sxs-lookup"><span data-stu-id="34586-254">Traffic rules.</span></span> <span data-ttu-id="34586-255">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="34586-255">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="34586-256">返信</span><span class="sxs-lookup"><span data-stu-id="34586-256">routes</span></span>|<span data-ttu-id="34586-257">[Vpnroute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-257">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="34586-258">ルート (サードパーティプロバイダーの場合はオプション)。</span><span class="sxs-lookup"><span data-stu-id="34586-258">Routes (optional for third-party providers).</span></span> <span data-ttu-id="34586-259">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="34586-259">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="34586-260">dnsRules</span><span class="sxs-lookup"><span data-stu-id="34586-260">dnsRules</span></span>|<span data-ttu-id="34586-261">[Vpndnsrule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-261">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="34586-262">DNS ルール。</span><span class="sxs-lookup"><span data-stu-id="34586-262">DNS rules.</span></span> <span data-ttu-id="34586-263">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="34586-263">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="34586-264">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="34586-264">trustedNetworkDomains</span></span>|<span data-ttu-id="34586-265">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="34586-265">String collection</span></span>|<span data-ttu-id="34586-266">信頼されたネットワークドメイン</span><span class="sxs-lookup"><span data-stu-id="34586-266">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="34586-267">応答</span><span class="sxs-lookup"><span data-stu-id="34586-267">Response</span></span>
<span data-ttu-id="34586-268">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34586-268">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34586-269">例</span><span class="sxs-lookup"><span data-stu-id="34586-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="34586-270">要求</span><span class="sxs-lookup"><span data-stu-id="34586-270">Request</span></span>
<span data-ttu-id="34586-271">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34586-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4160

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="34586-272">応答</span><span class="sxs-lookup"><span data-stu-id="34586-272">Response</span></span>
<span data-ttu-id="34586-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34586-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4332

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





