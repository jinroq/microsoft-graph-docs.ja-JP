---
title: IosVpnConfiguration の更新
description: IosVpnConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b17348b88bd6b388cf7c1b52a70996787651e5d0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947726"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="0a924-103">IosVpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0a924-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="0a924-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a924-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a924-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a924-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a924-106">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a924-106">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a924-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a924-107">Prerequisites</span></span>
<span data-ttu-id="0a924-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a924-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a924-110">Permission type</span></span>|<span data-ttu-id="0a924-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a924-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a924-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a924-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a924-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a924-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a924-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a924-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a924-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a924-115">Not supported.</span></span>|
|<span data-ttu-id="0a924-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a924-116">Application</span></span>|<span data-ttu-id="0a924-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a924-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a924-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a924-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0a924-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a924-119">Request headers</span></span>
|<span data-ttu-id="0a924-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a924-120">Header</span></span>|<span data-ttu-id="0a924-121">値</span><span class="sxs-lookup"><span data-stu-id="0a924-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a924-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a924-122">Authorization</span></span>|<span data-ttu-id="0a924-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a924-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a924-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0a924-124">Accept</span></span>|<span data-ttu-id="0a924-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a924-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a924-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a924-126">Request body</span></span>
<span data-ttu-id="0a924-127">要求本文で、 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a924-127">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="0a924-128">次の表に、 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0a924-128">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="0a924-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a924-129">Property</span></span>|<span data-ttu-id="0a924-130">型</span><span class="sxs-lookup"><span data-stu-id="0a924-130">Type</span></span>|<span data-ttu-id="0a924-131">説明</span><span class="sxs-lookup"><span data-stu-id="0a924-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a924-132">id</span><span class="sxs-lookup"><span data-stu-id="0a924-132">id</span></span>|<span data-ttu-id="0a924-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0a924-133">String</span></span>|<span data-ttu-id="0a924-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0a924-134">Key of the entity.</span></span> <span data-ttu-id="0a924-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a924-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0a924-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a924-137">DateTimeOffset</span></span>|<span data-ttu-id="0a924-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a924-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0a924-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a924-140">roleScopeTagIds</span></span>|<span data-ttu-id="0a924-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-141">String collection</span></span>|<span data-ttu-id="0a924-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0a924-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a924-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a924-144">supportsScopeTags</span></span>|<span data-ttu-id="0a924-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a924-145">Boolean</span></span>|<span data-ttu-id="0a924-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0a924-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a924-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0a924-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a924-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0a924-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a924-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="0a924-149">This property is read-only.</span></span> <span data-ttu-id="0a924-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0a924-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0a924-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0a924-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0a924-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="0a924-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0a924-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0a924-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0a924-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0a924-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0a924-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0a924-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0a924-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0a924-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0a924-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0a924-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0a924-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0a924-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0a924-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a924-163">createdDateTime</span></span>|<span data-ttu-id="0a924-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a924-164">DateTimeOffset</span></span>|<span data-ttu-id="0a924-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0a924-165">DateTime the object was created.</span></span> <span data-ttu-id="0a924-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-167">description</span><span class="sxs-lookup"><span data-stu-id="0a924-167">description</span></span>|<span data-ttu-id="0a924-168">String</span><span class="sxs-lookup"><span data-stu-id="0a924-168">String</span></span>|<span data-ttu-id="0a924-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0a924-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a924-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0a924-171">displayName</span></span>|<span data-ttu-id="0a924-172">String</span><span class="sxs-lookup"><span data-stu-id="0a924-172">String</span></span>|<span data-ttu-id="0a924-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0a924-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a924-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-175">version</span><span class="sxs-lookup"><span data-stu-id="0a924-175">version</span></span>|<span data-ttu-id="0a924-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0a924-176">Int32</span></span>|<span data-ttu-id="0a924-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0a924-177">Version of the device configuration.</span></span> <span data-ttu-id="0a924-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0a924-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="0a924-179">connectionName</span></span>|<span data-ttu-id="0a924-180">String</span><span class="sxs-lookup"><span data-stu-id="0a924-180">String</span></span>|<span data-ttu-id="0a924-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="0a924-181">Connection name displayed to the user.</span></span> <span data-ttu-id="0a924-182">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="0a924-183">connectionType</span></span>|[<span data-ttu-id="0a924-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0a924-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0a924-185">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="0a924-185">Connection type.</span></span> <span data-ttu-id="0a924-186">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a924-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0a924-187">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="0a924-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="0a924-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0a924-188">loginGroupOrDomain</span></span>|<span data-ttu-id="0a924-189">String</span><span class="sxs-lookup"><span data-stu-id="0a924-189">String</span></span>|<span data-ttu-id="0a924-190">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="0a924-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0a924-191">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-192">role</span><span class="sxs-lookup"><span data-stu-id="0a924-192">role</span></span>|<span data-ttu-id="0a924-193">String</span><span class="sxs-lookup"><span data-stu-id="0a924-193">String</span></span>|<span data-ttu-id="0a924-194">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="0a924-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0a924-195">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-196">領域</span><span class="sxs-lookup"><span data-stu-id="0a924-196">realm</span></span>|<span data-ttu-id="0a924-197">String</span><span class="sxs-lookup"><span data-stu-id="0a924-197">String</span></span>|<span data-ttu-id="0a924-198">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="0a924-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0a924-199">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-200">server</span><span class="sxs-lookup"><span data-stu-id="0a924-200">server</span></span>|[<span data-ttu-id="0a924-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0a924-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0a924-202">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="0a924-202">VPN Server on the network.</span></span> <span data-ttu-id="0a924-203">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0a924-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="0a924-204">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-205">識別子</span><span class="sxs-lookup"><span data-stu-id="0a924-205">identifier</span></span>|<span data-ttu-id="0a924-206">String</span><span class="sxs-lookup"><span data-stu-id="0a924-206">String</span></span>|<span data-ttu-id="0a924-207">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="0a924-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0a924-208">例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="0a924-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-209">customData</span><span class="sxs-lookup"><span data-stu-id="0a924-209">customData</span></span>|<span data-ttu-id="0a924-210">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0a924-211">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="0a924-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0a924-212">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0a924-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0a924-213">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="0a924-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0a924-214">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0a924-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0a924-215">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0a924-216">customKeyValueData</span></span>|<span data-ttu-id="0a924-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0a924-218">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="0a924-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0a924-219">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0a924-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0a924-220">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="0a924-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0a924-221">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0a924-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0a924-222">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0a924-223">enableSplitTunneling</span></span>|<span data-ttu-id="0a924-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a924-224">Boolean</span></span>|<span data-ttu-id="0a924-225">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="0a924-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="0a924-226">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0a924-227">authenticationMethod</span></span>|[<span data-ttu-id="0a924-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0a924-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0a924-229">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="0a924-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0a924-230">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a924-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0a924-231">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="0a924-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0a924-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0a924-232">enablePerApp</span></span>|<span data-ttu-id="0a924-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a924-233">Boolean</span></span>|<span data-ttu-id="0a924-234">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="0a924-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0a924-235">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-236">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="0a924-236">safariDomains</span></span>|<span data-ttu-id="0a924-237">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-237">String collection</span></span>|<span data-ttu-id="0a924-238">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="0a924-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0a924-239">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="0a924-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0a924-240">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0a924-241">onDemandRules</span></span>|<span data-ttu-id="0a924-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0a924-243">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="0a924-243">On-Demand Rules.</span></span> <span data-ttu-id="0a924-244">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0a924-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0a924-245">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0a924-246">proxyServer</span></span>|[<span data-ttu-id="0a924-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0a924-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0a924-248">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="0a924-248">Proxy Server.</span></span> <span data-ttu-id="0a924-249">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0a924-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0a924-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a924-251">Boolean</span></span>|<span data-ttu-id="0a924-252">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="0a924-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0a924-253">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0a924-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0a924-254">providerType</span><span class="sxs-lookup"><span data-stu-id="0a924-254">providerType</span></span>|[<span data-ttu-id="0a924-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0a924-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0a924-256">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="0a924-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="0a924-257">可能な値は、`notConfigured`、`appProxy`、`packetTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="0a924-257">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0a924-258">Userdomain に</span><span class="sxs-lookup"><span data-stu-id="0a924-258">userDomain</span></span>|<span data-ttu-id="0a924-259">String</span><span class="sxs-lookup"><span data-stu-id="0a924-259">String</span></span>|<span data-ttu-id="0a924-260">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="0a924-260">Zscaler only.</span></span> <span data-ttu-id="0a924-261">Zscaler アプリでログインフィールドに事前設定するには、静的ドメインを入力します。</span><span class="sxs-lookup"><span data-stu-id="0a924-261">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0a924-262">この指定を省略すると、代わりにユーザーの Azure Active Directory ドメインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="0a924-262">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="0a924-263">Cloudname</span><span class="sxs-lookup"><span data-stu-id="0a924-263">strictEnforcement</span></span>|<span data-ttu-id="0a924-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a924-264">Boolean</span></span>|<span data-ttu-id="0a924-265">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="0a924-265">Zscaler only.</span></span> <span data-ttu-id="0a924-266">ユーザーが Zscaler アプリにサインインするまでネットワークトラフィックをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0a924-266">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0a924-267">"True" はトラフィックがブロックされることを意味します。</span><span class="sxs-lookup"><span data-stu-id="0a924-267">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="0a924-268">cloudName</span><span class="sxs-lookup"><span data-stu-id="0a924-268">cloudName</span></span>|<span data-ttu-id="0a924-269">String</span><span class="sxs-lookup"><span data-stu-id="0a924-269">String</span></span>|<span data-ttu-id="0a924-270">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="0a924-270">Zscaler only.</span></span> <span data-ttu-id="0a924-271">ユーザーが割り当てられている Zscaler cloud。</span><span class="sxs-lookup"><span data-stu-id="0a924-271">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="0a924-272">excludeList</span><span class="sxs-lookup"><span data-stu-id="0a924-272">excludeList</span></span>|<span data-ttu-id="0a924-273">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0a924-273">String collection</span></span>|<span data-ttu-id="0a924-274">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="0a924-274">Zscaler only.</span></span> <span data-ttu-id="0a924-275">Zscaler クラウド経由で送信されないネットワークアドレスのリスト。</span><span class="sxs-lookup"><span data-stu-id="0a924-275">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="0a924-276">応答</span><span class="sxs-lookup"><span data-stu-id="0a924-276">Response</span></span>
<span data-ttu-id="0a924-277">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a924-277">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a924-278">例</span><span class="sxs-lookup"><span data-stu-id="0a924-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a924-279">要求</span><span class="sxs-lookup"><span data-stu-id="0a924-279">Request</span></span>
<span data-ttu-id="0a924-280">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a924-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2815

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="0a924-281">応答</span><span class="sxs-lookup"><span data-stu-id="0a924-281">Response</span></span>
<span data-ttu-id="0a924-p134">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a924-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2987

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  ]
}
```





