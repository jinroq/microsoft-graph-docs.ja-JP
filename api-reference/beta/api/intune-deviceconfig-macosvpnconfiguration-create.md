---
title: MacOSVpnConfiguration の作成
description: 新しい macOSVpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19c2ecaef5d23cacb15fb26e26b628144931410f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338659"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="e5e07-103">MacOSVpnConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="e5e07-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="e5e07-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5e07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5e07-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5e07-106">新しい[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5e07-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5e07-107">Prerequisites</span></span>
<span data-ttu-id="e5e07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5e07-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5e07-110">Permission type</span></span>|<span data-ttu-id="e5e07-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5e07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5e07-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5e07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5e07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5e07-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5e07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5e07-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5e07-115">Not supported.</span></span>|
|<span data-ttu-id="e5e07-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5e07-116">Application</span></span>|<span data-ttu-id="e5e07-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e07-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5e07-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5e07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5e07-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5e07-119">Request headers</span></span>
|<span data-ttu-id="e5e07-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5e07-120">Header</span></span>|<span data-ttu-id="e5e07-121">値</span><span class="sxs-lookup"><span data-stu-id="e5e07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5e07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5e07-122">Authorization</span></span>|<span data-ttu-id="e5e07-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5e07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5e07-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e5e07-124">Accept</span></span>|<span data-ttu-id="e5e07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5e07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5e07-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5e07-126">Request body</span></span>
<span data-ttu-id="e5e07-127">要求本文で、macOSVpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="e5e07-128">次の表に、macOSVpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="e5e07-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5e07-129">Property</span></span>|<span data-ttu-id="e5e07-130">型</span><span class="sxs-lookup"><span data-stu-id="e5e07-130">Type</span></span>|<span data-ttu-id="e5e07-131">説明</span><span class="sxs-lookup"><span data-stu-id="e5e07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e07-132">id</span><span class="sxs-lookup"><span data-stu-id="e5e07-132">id</span></span>|<span data-ttu-id="e5e07-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e5e07-133">String</span></span>|<span data-ttu-id="e5e07-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5e07-134">Key of the entity.</span></span> <span data-ttu-id="e5e07-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5e07-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5e07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e07-137">DateTimeOffset</span></span>|<span data-ttu-id="e5e07-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e5e07-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e5e07-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5e07-140">roleScopeTagIds</span></span>|<span data-ttu-id="e5e07-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e07-141">String collection</span></span>|<span data-ttu-id="e5e07-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e5e07-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5e07-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e5e07-144">supportsScopeTags</span></span>|<span data-ttu-id="e5e07-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e07-145">Boolean</span></span>|<span data-ttu-id="e5e07-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5e07-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e5e07-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5e07-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5e07-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-149">This property is read-only.</span></span> <span data-ttu-id="e5e07-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5e07-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e5e07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5e07-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e5e07-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="e5e07-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e5e07-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5e07-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e5e07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5e07-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e5e07-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e5e07-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e5e07-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e5e07-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e5e07-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e5e07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e5e07-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e5e07-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e5e07-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5e07-163">createdDateTime</span></span>|<span data-ttu-id="e5e07-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e07-164">DateTimeOffset</span></span>|<span data-ttu-id="e5e07-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e5e07-165">DateTime the object was created.</span></span> <span data-ttu-id="e5e07-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-167">description</span><span class="sxs-lookup"><span data-stu-id="e5e07-167">description</span></span>|<span data-ttu-id="e5e07-168">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-168">String</span></span>|<span data-ttu-id="e5e07-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e5e07-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5e07-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e5e07-171">displayName</span></span>|<span data-ttu-id="e5e07-172">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-172">String</span></span>|<span data-ttu-id="e5e07-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e5e07-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5e07-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-175">version</span><span class="sxs-lookup"><span data-stu-id="e5e07-175">version</span></span>|<span data-ttu-id="e5e07-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e5e07-176">Int32</span></span>|<span data-ttu-id="e5e07-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e5e07-177">Version of the device configuration.</span></span> <span data-ttu-id="e5e07-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e07-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="e5e07-179">connectionName</span></span>|<span data-ttu-id="e5e07-180">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-180">String</span></span>|<span data-ttu-id="e5e07-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="e5e07-181">Connection name displayed to the user.</span></span> <span data-ttu-id="e5e07-182">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="e5e07-183">connectionType</span></span>|[<span data-ttu-id="e5e07-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="e5e07-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="e5e07-185">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="e5e07-185">Connection type.</span></span> <span data-ttu-id="e5e07-186">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e5e07-187">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="e5e07-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="e5e07-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="e5e07-188">loginGroupOrDomain</span></span>|<span data-ttu-id="e5e07-189">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-189">String</span></span>|<span data-ttu-id="e5e07-190">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="e5e07-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="e5e07-191">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-192">role</span><span class="sxs-lookup"><span data-stu-id="e5e07-192">role</span></span>|<span data-ttu-id="e5e07-193">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-193">String</span></span>|<span data-ttu-id="e5e07-194">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="e5e07-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e5e07-195">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-196">領域</span><span class="sxs-lookup"><span data-stu-id="e5e07-196">realm</span></span>|<span data-ttu-id="e5e07-197">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-197">String</span></span>|<span data-ttu-id="e5e07-198">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="e5e07-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e5e07-199">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-200">server</span><span class="sxs-lookup"><span data-stu-id="e5e07-200">server</span></span>|[<span data-ttu-id="e5e07-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="e5e07-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="e5e07-202">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="e5e07-202">VPN Server on the network.</span></span> <span data-ttu-id="e5e07-203">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="e5e07-204">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-205">識別子</span><span class="sxs-lookup"><span data-stu-id="e5e07-205">identifier</span></span>|<span data-ttu-id="e5e07-206">String</span><span class="sxs-lookup"><span data-stu-id="e5e07-206">String</span></span>|<span data-ttu-id="e5e07-207">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="e5e07-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e5e07-208">例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="e5e07-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-209">customData</span><span class="sxs-lookup"><span data-stu-id="e5e07-209">customData</span></span>|<span data-ttu-id="e5e07-210">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e07-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e5e07-211">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="e5e07-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e5e07-212">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="e5e07-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e5e07-213">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="e5e07-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e5e07-214">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e5e07-215">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e5e07-216">customKeyValueData</span></span>|<span data-ttu-id="e5e07-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e07-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e5e07-218">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="e5e07-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e5e07-219">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="e5e07-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e5e07-220">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="e5e07-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e5e07-221">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e5e07-222">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="e5e07-223">enableSplitTunneling</span></span>|<span data-ttu-id="e5e07-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e07-224">Boolean</span></span>|<span data-ttu-id="e5e07-225">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="e5e07-226">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e5e07-227">authenticationMethod</span></span>|[<span data-ttu-id="e5e07-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e5e07-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e5e07-229">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="e5e07-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="e5e07-230">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e5e07-231">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="e5e07-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e5e07-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="e5e07-232">enablePerApp</span></span>|<span data-ttu-id="e5e07-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e07-233">Boolean</span></span>|<span data-ttu-id="e5e07-234">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="e5e07-235">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-236">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="e5e07-236">safariDomains</span></span>|<span data-ttu-id="e5e07-237">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e07-237">String collection</span></span>|<span data-ttu-id="e5e07-238">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="e5e07-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="e5e07-239">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="e5e07-240">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="e5e07-241">onDemandRules</span></span>|<span data-ttu-id="e5e07-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e07-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="e5e07-243">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="e5e07-243">On-Demand Rules.</span></span> <span data-ttu-id="e5e07-244">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e5e07-245">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="e5e07-246">proxyServer</span></span>|[<span data-ttu-id="e5e07-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="e5e07-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e5e07-248">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="e5e07-248">Proxy Server.</span></span> <span data-ttu-id="e5e07-249">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e5e07-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="e5e07-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="e5e07-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5e07-251">Boolean</span></span>|<span data-ttu-id="e5e07-252">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="e5e07-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="e5e07-253">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="e5e07-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e5e07-254">応答</span><span class="sxs-lookup"><span data-stu-id="e5e07-254">Response</span></span>
<span data-ttu-id="e5e07-255">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5e07-255">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5e07-256">例</span><span class="sxs-lookup"><span data-stu-id="e5e07-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5e07-257">要求</span><span class="sxs-lookup"><span data-stu-id="e5e07-257">Request</span></span>
<span data-ttu-id="e5e07-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5e07-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2630

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="e5e07-259">応答</span><span class="sxs-lookup"><span data-stu-id="e5e07-259">Response</span></span>
<span data-ttu-id="e5e07-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5e07-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2802

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```






