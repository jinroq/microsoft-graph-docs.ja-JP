---
title: MacOSVpnConfiguration の作成
description: 新しい macOSVpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 724faafbb07a9e3d9083adad73bee273f7a684cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946998"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="2d9f2-103">MacOSVpnConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="2d9f2-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="2d9f2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d9f2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9f2-106">新しい[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d9f2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d9f2-107">Prerequisites</span></span>
<span data-ttu-id="2d9f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9f2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d9f2-110">Permission type</span></span>|<span data-ttu-id="2d9f2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d9f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9f2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d9f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d9f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d9f2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d9f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9f2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-115">Not supported.</span></span>|
|<span data-ttu-id="2d9f2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-116">Application</span></span>|<span data-ttu-id="2d9f2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d9f2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d9f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2d9f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d9f2-119">Request headers</span></span>
|<span data-ttu-id="2d9f2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d9f2-120">Header</span></span>|<span data-ttu-id="2d9f2-121">値</span><span class="sxs-lookup"><span data-stu-id="2d9f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d9f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9f2-122">Authorization</span></span>|<span data-ttu-id="2d9f2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d9f2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2d9f2-124">Accept</span></span>|<span data-ttu-id="2d9f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d9f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9f2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d9f2-126">Request body</span></span>
<span data-ttu-id="2d9f2-127">要求本文で、macOSVpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="2d9f2-128">次の表に、macOSVpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="2d9f2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d9f2-129">Property</span></span>|<span data-ttu-id="2d9f2-130">型</span><span class="sxs-lookup"><span data-stu-id="2d9f2-130">Type</span></span>|<span data-ttu-id="2d9f2-131">説明</span><span class="sxs-lookup"><span data-stu-id="2d9f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9f2-132">id</span><span class="sxs-lookup"><span data-stu-id="2d9f2-132">id</span></span>|<span data-ttu-id="2d9f2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2d9f2-133">String</span></span>|<span data-ttu-id="2d9f2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-134">Key of the entity.</span></span> <span data-ttu-id="2d9f2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d9f2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d9f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d9f2-137">DateTimeOffset</span></span>|<span data-ttu-id="2d9f2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d9f2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d9f2-140">roleScopeTagIds</span></span>|<span data-ttu-id="2d9f2-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-141">String collection</span></span>|<span data-ttu-id="2d9f2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d9f2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2d9f2-144">supportsScopeTags</span></span>|<span data-ttu-id="2d9f2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d9f2-145">Boolean</span></span>|<span data-ttu-id="2d9f2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2d9f2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2d9f2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2d9f2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-149">This property is read-only.</span></span> <span data-ttu-id="2d9f2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d9f2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2d9f2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d9f2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2d9f2-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2d9f2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d9f2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2d9f2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d9f2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2d9f2-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2d9f2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2d9f2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2d9f2-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="2d9f2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2d9f2-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2d9f2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d9f2-163">createdDateTime</span></span>|<span data-ttu-id="2d9f2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d9f2-164">DateTimeOffset</span></span>|<span data-ttu-id="2d9f2-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-165">DateTime the object was created.</span></span> <span data-ttu-id="2d9f2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-167">description</span><span class="sxs-lookup"><span data-stu-id="2d9f2-167">description</span></span>|<span data-ttu-id="2d9f2-168">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-168">String</span></span>|<span data-ttu-id="2d9f2-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d9f2-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2d9f2-171">displayName</span></span>|<span data-ttu-id="2d9f2-172">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-172">String</span></span>|<span data-ttu-id="2d9f2-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d9f2-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-175">version</span><span class="sxs-lookup"><span data-stu-id="2d9f2-175">version</span></span>|<span data-ttu-id="2d9f2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2d9f2-176">Int32</span></span>|<span data-ttu-id="2d9f2-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-177">Version of the device configuration.</span></span> <span data-ttu-id="2d9f2-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d9f2-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="2d9f2-179">connectionName</span></span>|<span data-ttu-id="2d9f2-180">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-180">String</span></span>|<span data-ttu-id="2d9f2-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-181">Connection name displayed to the user.</span></span> <span data-ttu-id="2d9f2-182">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="2d9f2-183">connectionType</span></span>|[<span data-ttu-id="2d9f2-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2d9f2-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2d9f2-185">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-185">Connection type.</span></span> <span data-ttu-id="2d9f2-186">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2d9f2-187">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="2d9f2-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="2d9f2-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="2d9f2-188">loginGroupOrDomain</span></span>|<span data-ttu-id="2d9f2-189">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-189">String</span></span>|<span data-ttu-id="2d9f2-190">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2d9f2-191">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-192">role</span><span class="sxs-lookup"><span data-stu-id="2d9f2-192">role</span></span>|<span data-ttu-id="2d9f2-193">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-193">String</span></span>|<span data-ttu-id="2d9f2-194">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2d9f2-195">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-196">領域</span><span class="sxs-lookup"><span data-stu-id="2d9f2-196">realm</span></span>|<span data-ttu-id="2d9f2-197">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-197">String</span></span>|<span data-ttu-id="2d9f2-198">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2d9f2-199">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-200">server</span><span class="sxs-lookup"><span data-stu-id="2d9f2-200">server</span></span>|[<span data-ttu-id="2d9f2-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2d9f2-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2d9f2-202">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-202">VPN Server on the network.</span></span> <span data-ttu-id="2d9f2-203">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="2d9f2-204">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-205">識別子</span><span class="sxs-lookup"><span data-stu-id="2d9f2-205">identifier</span></span>|<span data-ttu-id="2d9f2-206">String</span><span class="sxs-lookup"><span data-stu-id="2d9f2-206">String</span></span>|<span data-ttu-id="2d9f2-207">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2d9f2-208">例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-209">customData</span><span class="sxs-lookup"><span data-stu-id="2d9f2-209">customData</span></span>|<span data-ttu-id="2d9f2-210">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2d9f2-211">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2d9f2-212">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2d9f2-213">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2d9f2-214">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2d9f2-215">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2d9f2-216">customKeyValueData</span></span>|<span data-ttu-id="2d9f2-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2d9f2-218">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2d9f2-219">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2d9f2-220">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2d9f2-221">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2d9f2-222">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2d9f2-223">enableSplitTunneling</span></span>|<span data-ttu-id="2d9f2-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d9f2-224">Boolean</span></span>|<span data-ttu-id="2d9f2-225">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="2d9f2-226">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2d9f2-227">authenticationMethod</span></span>|[<span data-ttu-id="2d9f2-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2d9f2-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2d9f2-229">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2d9f2-230">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2d9f2-231">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2d9f2-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="2d9f2-232">enablePerApp</span></span>|<span data-ttu-id="2d9f2-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d9f2-233">Boolean</span></span>|<span data-ttu-id="2d9f2-234">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2d9f2-235">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-236">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="2d9f2-236">safariDomains</span></span>|<span data-ttu-id="2d9f2-237">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-237">String collection</span></span>|<span data-ttu-id="2d9f2-238">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="2d9f2-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2d9f2-239">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2d9f2-240">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2d9f2-241">onDemandRules</span></span>|<span data-ttu-id="2d9f2-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2d9f2-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2d9f2-243">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-243">On-Demand Rules.</span></span> <span data-ttu-id="2d9f2-244">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2d9f2-245">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2d9f2-246">proxyServer</span></span>|[<span data-ttu-id="2d9f2-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2d9f2-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2d9f2-248">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-248">Proxy Server.</span></span> <span data-ttu-id="2d9f2-249">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f2-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="2d9f2-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2d9f2-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d9f2-251">Boolean</span></span>|<span data-ttu-id="2d9f2-252">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2d9f2-253">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2d9f2-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2d9f2-254">応答</span><span class="sxs-lookup"><span data-stu-id="2d9f2-254">Response</span></span>
<span data-ttu-id="2d9f2-255">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-255">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d9f2-256">例</span><span class="sxs-lookup"><span data-stu-id="2d9f2-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d9f2-257">要求</span><span class="sxs-lookup"><span data-stu-id="2d9f2-257">Request</span></span>
<span data-ttu-id="2d9f2-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d9f2-259">応答</span><span class="sxs-lookup"><span data-stu-id="2d9f2-259">Response</span></span>
<span data-ttu-id="2d9f2-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d9f2-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





