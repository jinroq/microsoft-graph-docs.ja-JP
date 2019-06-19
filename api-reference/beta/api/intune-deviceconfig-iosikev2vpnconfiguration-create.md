---
title: IosikEv2VpnConfiguration を作成する
description: 新しい iosikEv2VpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c52cbfaa0895e5bccf2c892c5435460a1ebec30d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001763"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="f10f7-103">IosikEv2VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="f10f7-103">Create iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="f10f7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f10f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f10f7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10f7-106">新しい[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-106">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f10f7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f10f7-107">Prerequisites</span></span>
<span data-ttu-id="f10f7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f10f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f10f7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f10f7-110">Permission type</span></span>|<span data-ttu-id="f10f7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f10f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f10f7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f10f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f10f7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10f7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f10f7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f10f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f10f7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f10f7-115">Not supported.</span></span>|
|<span data-ttu-id="f10f7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f10f7-116">Application</span></span>|<span data-ttu-id="f10f7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f10f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f10f7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f10f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f10f7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f10f7-119">Request headers</span></span>
|<span data-ttu-id="f10f7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f10f7-120">Header</span></span>|<span data-ttu-id="f10f7-121">値</span><span class="sxs-lookup"><span data-stu-id="f10f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f10f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f10f7-122">Authorization</span></span>|<span data-ttu-id="f10f7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f10f7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f10f7-124">Accept</span></span>|<span data-ttu-id="f10f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f10f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10f7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f10f7-126">Request body</span></span>
<span data-ttu-id="f10f7-127">要求本文で、iosikEv2VpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-127">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="f10f7-128">次の表に、iosikEv2VpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-128">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="f10f7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f10f7-129">Property</span></span>|<span data-ttu-id="f10f7-130">型</span><span class="sxs-lookup"><span data-stu-id="f10f7-130">Type</span></span>|<span data-ttu-id="f10f7-131">説明</span><span class="sxs-lookup"><span data-stu-id="f10f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10f7-132">id</span><span class="sxs-lookup"><span data-stu-id="f10f7-132">id</span></span>|<span data-ttu-id="f10f7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f10f7-133">String</span></span>|<span data-ttu-id="f10f7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f10f7-134">Key of the entity.</span></span> <span data-ttu-id="f10f7-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f10f7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f10f7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f10f7-137">DateTimeOffset</span></span>|<span data-ttu-id="f10f7-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f10f7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f10f7-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f10f7-140">roleScopeTagIds</span></span>|<span data-ttu-id="f10f7-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-141">String collection</span></span>|<span data-ttu-id="f10f7-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f10f7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f10f7-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f10f7-144">supportsScopeTags</span></span>|<span data-ttu-id="f10f7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-145">Boolean</span></span>|<span data-ttu-id="f10f7-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f10f7-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f10f7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f10f7-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f10f7-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-149">This property is read-only.</span></span> <span data-ttu-id="f10f7-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f10f7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f10f7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f10f7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f10f7-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f10f7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f10f7-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f10f7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f10f7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f10f7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f10f7-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f10f7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f10f7-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f10f7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f10f7-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f10f7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f10f7-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f10f7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f10f7-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f10f7-163">createdDateTime</span></span>|<span data-ttu-id="f10f7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f10f7-164">DateTimeOffset</span></span>|<span data-ttu-id="f10f7-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f10f7-165">DateTime the object was created.</span></span> <span data-ttu-id="f10f7-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-167">description</span><span class="sxs-lookup"><span data-stu-id="f10f7-167">description</span></span>|<span data-ttu-id="f10f7-168">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-168">String</span></span>|<span data-ttu-id="f10f7-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f10f7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f10f7-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f10f7-171">displayName</span></span>|<span data-ttu-id="f10f7-172">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-172">String</span></span>|<span data-ttu-id="f10f7-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f10f7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f10f7-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-175">version</span><span class="sxs-lookup"><span data-stu-id="f10f7-175">version</span></span>|<span data-ttu-id="f10f7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f10f7-176">Int32</span></span>|<span data-ttu-id="f10f7-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f10f7-177">Version of the device configuration.</span></span> <span data-ttu-id="f10f7-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="f10f7-179">connectionName</span></span>|<span data-ttu-id="f10f7-180">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-180">String</span></span>|<span data-ttu-id="f10f7-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="f10f7-181">Connection name displayed to the user.</span></span> <span data-ttu-id="f10f7-182">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="f10f7-183">connectionType</span></span>|[<span data-ttu-id="f10f7-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f10f7-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f10f7-185">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="f10f7-185">Connection type.</span></span> <span data-ttu-id="f10f7-186">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f10f7-187">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="f10f7-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="f10f7-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f10f7-188">loginGroupOrDomain</span></span>|<span data-ttu-id="f10f7-189">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-189">String</span></span>|<span data-ttu-id="f10f7-190">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="f10f7-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f10f7-191">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-192">role</span><span class="sxs-lookup"><span data-stu-id="f10f7-192">role</span></span>|<span data-ttu-id="f10f7-193">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-193">String</span></span>|<span data-ttu-id="f10f7-194">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="f10f7-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f10f7-195">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-196">領域</span><span class="sxs-lookup"><span data-stu-id="f10f7-196">realm</span></span>|<span data-ttu-id="f10f7-197">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-197">String</span></span>|<span data-ttu-id="f10f7-198">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="f10f7-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f10f7-199">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-200">server</span><span class="sxs-lookup"><span data-stu-id="f10f7-200">server</span></span>|[<span data-ttu-id="f10f7-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f10f7-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f10f7-202">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="f10f7-202">VPN Server on the network.</span></span> <span data-ttu-id="f10f7-203">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="f10f7-204">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-205">識別子</span><span class="sxs-lookup"><span data-stu-id="f10f7-205">identifier</span></span>|<span data-ttu-id="f10f7-206">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-206">String</span></span>|<span data-ttu-id="f10f7-207">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="f10f7-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f10f7-208">例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="f10f7-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-209">customData</span><span class="sxs-lookup"><span data-stu-id="f10f7-209">customData</span></span>|<span data-ttu-id="f10f7-210">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f10f7-211">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="f10f7-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f10f7-212">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f10f7-213">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="f10f7-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f10f7-214">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f10f7-215">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f10f7-216">customKeyValueData</span></span>|<span data-ttu-id="f10f7-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f10f7-218">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="f10f7-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f10f7-219">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f10f7-220">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="f10f7-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f10f7-221">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f10f7-222">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f10f7-223">enableSplitTunneling</span></span>|<span data-ttu-id="f10f7-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-224">Boolean</span></span>|<span data-ttu-id="f10f7-225">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="f10f7-226">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f10f7-227">authenticationMethod</span></span>|[<span data-ttu-id="f10f7-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f10f7-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f10f7-229">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="f10f7-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f10f7-230">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f10f7-231">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f10f7-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f10f7-232">enablePerApp</span></span>|<span data-ttu-id="f10f7-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-233">Boolean</span></span>|<span data-ttu-id="f10f7-234">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f10f7-235">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-236">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="f10f7-236">safariDomains</span></span>|<span data-ttu-id="f10f7-237">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-237">String collection</span></span>|<span data-ttu-id="f10f7-238">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="f10f7-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f10f7-239">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f10f7-240">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f10f7-241">onDemandRules</span></span>|<span data-ttu-id="f10f7-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f10f7-243">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="f10f7-243">On-Demand Rules.</span></span> <span data-ttu-id="f10f7-244">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f10f7-245">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f10f7-246">proxyServer</span></span>|[<span data-ttu-id="f10f7-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f10f7-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f10f7-248">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="f10f7-248">Proxy Server.</span></span> <span data-ttu-id="f10f7-249">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f10f7-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f10f7-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-251">Boolean</span></span>|<span data-ttu-id="f10f7-252">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="f10f7-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f10f7-253">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f10f7-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-254">providerType</span><span class="sxs-lookup"><span data-stu-id="f10f7-254">providerType</span></span>|[<span data-ttu-id="f10f7-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f10f7-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="f10f7-256">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="f10f7-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="f10f7-257">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="f10f7-258">可能な値は、`notConfigured`、`appProxy`、`packetTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="f10f7-259">Userdomain に</span><span class="sxs-lookup"><span data-stu-id="f10f7-259">userDomain</span></span>|<span data-ttu-id="f10f7-260">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-260">String</span></span>|<span data-ttu-id="f10f7-261">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="f10f7-261">Zscaler only.</span></span> <span data-ttu-id="f10f7-262">Zscaler アプリでログインフィールドに事前設定するには、静的ドメインを入力します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="f10f7-263">この指定を省略すると、代わりにユーザーの Azure Active Directory ドメインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="f10f7-264">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-265">Cloudname</span><span class="sxs-lookup"><span data-stu-id="f10f7-265">strictEnforcement</span></span>|<span data-ttu-id="f10f7-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-266">Boolean</span></span>|<span data-ttu-id="f10f7-267">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="f10f7-267">Zscaler only.</span></span> <span data-ttu-id="f10f7-268">ユーザーが Zscaler アプリにサインインするまでネットワークトラフィックをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="f10f7-269">"True" はトラフィックがブロックされることを意味します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="f10f7-270">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-271">cloudName</span><span class="sxs-lookup"><span data-stu-id="f10f7-271">cloudName</span></span>|<span data-ttu-id="f10f7-272">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-272">String</span></span>|<span data-ttu-id="f10f7-273">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="f10f7-273">Zscaler only.</span></span> <span data-ttu-id="f10f7-274">ユーザーが割り当てられている Zscaler cloud。</span><span class="sxs-lookup"><span data-stu-id="f10f7-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="f10f7-275">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="f10f7-276">excludeList</span></span>|<span data-ttu-id="f10f7-277">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f10f7-277">String collection</span></span>|<span data-ttu-id="f10f7-278">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="f10f7-278">Zscaler only.</span></span> <span data-ttu-id="f10f7-279">Zscaler クラウド経由で送信されないネットワークアドレスのリスト。</span><span class="sxs-lookup"><span data-stu-id="f10f7-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="f10f7-280">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f10f7-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f10f7-281">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="f10f7-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f10f7-283">子のセキュリティアソシエーションのパラメーター</span><span class="sxs-lookup"><span data-stu-id="f10f7-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="f10f7-284">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f10f7-284">clientAuthenticationType</span></span>|[<span data-ttu-id="f10f7-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f10f7-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="f10f7-286">VPN クライアントが使用するクライアント認証の種類。</span><span class="sxs-lookup"><span data-stu-id="f10f7-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="f10f7-287">可能な値は、`userAuthentication`、`deviceAuthentication` です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="f10f7-288">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f10f7-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="f10f7-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f10f7-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="f10f7-290">ピア接続がまだアクティブであるかどうかを確認する頻度を決定します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="f10f7-291">.</span><span class="sxs-lookup"><span data-stu-id="f10f7-291"></span></span> <span data-ttu-id="f10f7-292">使用可能な値は、`medium`、`none`、`low`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="f10f7-293">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="f10f7-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="f10f7-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-294">Boolean</span></span>|<span data-ttu-id="f10f7-295">MOBIKE を無効にする</span><span class="sxs-lookup"><span data-stu-id="f10f7-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="f10f7-296">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="f10f7-296">disableRedirect</span></span>|<span data-ttu-id="f10f7-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-297">Boolean</span></span>|<span data-ttu-id="f10f7-298">リダイレクトを無効にする</span><span class="sxs-lookup"><span data-stu-id="f10f7-298">Disable Redirect</span></span>|
|<span data-ttu-id="f10f7-299">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="f10f7-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="f10f7-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-300">Boolean</span></span>|<span data-ttu-id="f10f7-301">ベストエフォート型の失効チェックを有効にします。サーバー応答のタイムアウトによって失敗しない</span><span class="sxs-lookup"><span data-stu-id="f10f7-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="f10f7-302">enableEAP</span><span class="sxs-lookup"><span data-stu-id="f10f7-302">enableEAP</span></span>|<span data-ttu-id="f10f7-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-303">Boolean</span></span>|<span data-ttu-id="f10f7-304">EAP のみの認証を有効にします</span><span class="sxs-lookup"><span data-stu-id="f10f7-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="f10f7-305">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="f10f7-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="f10f7-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-306">Boolean</span></span>|<span data-ttu-id="f10f7-307">完全な転送機密性 (PFS) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="f10f7-308">Enableuseinternalサブネット属性</span><span class="sxs-lookup"><span data-stu-id="f10f7-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="f10f7-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-309">Boolean</span></span>|<span data-ttu-id="f10f7-310">内部サブネット属性の使用を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="f10f7-311">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="f10f7-311">localIdentifier</span></span>|[<span data-ttu-id="f10f7-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="f10f7-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="f10f7-313">VPN 経由で接続しようとしているクライアントを識別する方法。</span><span class="sxs-lookup"><span data-stu-id="f10f7-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="f10f7-314">.</span><span class="sxs-lookup"><span data-stu-id="f10f7-314"></span></span> <span data-ttu-id="f10f7-315">可能な値は`deviceFQDN`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f10f7-315">Possible values are: `deviceFQDN`.</span></span>|
|<span data-ttu-id="f10f7-316">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="f10f7-316">remoteIdentifier</span></span>|<span data-ttu-id="f10f7-317">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-317">String</span></span>|<span data-ttu-id="f10f7-318">IKEv2 サーバーのアドレス。</span><span class="sxs-lookup"><span data-stu-id="f10f7-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="f10f7-319">FQDN、UserFQDN、ネットワークアドレス、または ASN1DN である必要があります。</span><span class="sxs-lookup"><span data-stu-id="f10f7-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="f10f7-320">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-320">securityAssociationParameters</span></span>|[<span data-ttu-id="f10f7-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f10f7-322">セキュリティアソシエーションパラメーター</span><span class="sxs-lookup"><span data-stu-id="f10f7-322">Security Association Parameters</span></span>|
|<span data-ttu-id="f10f7-323">Server指定 Ecommonname</span><span class="sxs-lookup"><span data-stu-id="f10f7-323">serverCertificateCommonName</span></span>|<span data-ttu-id="f10f7-324">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-324">String</span></span>|<span data-ttu-id="f10f7-325">サーバー認証で使用される IKEv2 サーバー証明書の共通名</span><span class="sxs-lookup"><span data-stu-id="f10f7-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="f10f7-326">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="f10f7-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="f10f7-327">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-327">String</span></span>|<span data-ttu-id="f10f7-328">認証で使用される IKEv2 サーバー証明書発行者の共通名</span><span class="sxs-lookup"><span data-stu-id="f10f7-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="f10f7-329">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="f10f7-329">serverCertificateType</span></span>|[<span data-ttu-id="f10f7-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="f10f7-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="f10f7-331">Vpn サーバーが認証のために VPN クライアントに提示する証明書の種類。</span><span class="sxs-lookup"><span data-stu-id="f10f7-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="f10f7-332">使用可能な値は、`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521` です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="f10f7-333">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="f10f7-333">sharedSecret</span></span>|<span data-ttu-id="f10f7-334">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-334">String</span></span>|<span data-ttu-id="f10f7-335">共有シークレット認証が選択されている場合に使用</span><span class="sxs-lookup"><span data-stu-id="f10f7-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="f10f7-336">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f10f7-336">tlsMaximumVersion</span></span>|<span data-ttu-id="f10f7-337">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-337">String</span></span>|<span data-ttu-id="f10f7-338">Eap-tls 認証で使用される最大 TLS バージョン</span><span class="sxs-lookup"><span data-stu-id="f10f7-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f10f7-339">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f10f7-339">tlsMinimumVersion</span></span>|<span data-ttu-id="f10f7-340">String</span><span class="sxs-lookup"><span data-stu-id="f10f7-340">String</span></span>|<span data-ttu-id="f10f7-341">Eap-tls 認証で使用する最低限の TLS バージョン</span><span class="sxs-lookup"><span data-stu-id="f10f7-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f10f7-342">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="f10f7-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-343">Boolean</span></span>|<span data-ttu-id="f10f7-344">明示的に指定されていない限り、すべてのパラメーターをデバイスの既定値に設定することによって、セキュリティアソシエーションパラメーターを使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="f10f7-345">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f10f7-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="f10f7-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="f10f7-346">Boolean</span></span>|<span data-ttu-id="f10f7-347">明示的に指定されていない限り、すべてのパラメーターをデバイスの既定値に設定することによって、子のセキュリティアソシエーションのパラメーターを使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f10f7-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|



## <a name="response"></a><span data-ttu-id="f10f7-348">応答</span><span class="sxs-lookup"><span data-stu-id="f10f7-348">Response</span></span>
<span data-ttu-id="f10f7-349">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f10f7-349">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f10f7-350">例</span><span class="sxs-lookup"><span data-stu-id="f10f7-350">Example</span></span>

### <a name="request"></a><span data-ttu-id="f10f7-351">要求</span><span class="sxs-lookup"><span data-stu-id="f10f7-351">Request</span></span>
<span data-ttu-id="f10f7-352">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f10f7-352">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4237

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "deviceFQDN",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a><span data-ttu-id="f10f7-353">応答</span><span class="sxs-lookup"><span data-stu-id="f10f7-353">Response</span></span>
<span data-ttu-id="f10f7-p139">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f10f7-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4409

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "deviceFQDN",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```




