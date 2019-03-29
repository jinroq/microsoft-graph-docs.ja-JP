---
title: macosvpnconfiguration の更新
description: macosvpnconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef693ccb098cc4b7e04b3bc8ccf26faccf106585
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973587"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="7d649-103">macosvpnconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="7d649-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="7d649-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d649-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d649-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d649-106">[macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d649-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d649-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d649-107">Prerequisites</span></span>
<span data-ttu-id="7d649-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d649-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d649-110">Permission type</span></span>|<span data-ttu-id="7d649-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d649-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d649-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d649-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d649-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d649-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d649-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d649-115">Not supported.</span></span>|
|<span data-ttu-id="7d649-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d649-116">Application</span></span>|<span data-ttu-id="7d649-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d649-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d649-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d649-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d649-119">Request headers</span></span>
|<span data-ttu-id="7d649-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d649-120">Header</span></span>|<span data-ttu-id="7d649-121">値</span><span class="sxs-lookup"><span data-stu-id="7d649-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d649-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d649-122">Authorization</span></span>|<span data-ttu-id="7d649-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d649-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d649-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7d649-124">Accept</span></span>|<span data-ttu-id="7d649-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d649-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d649-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d649-126">Request body</span></span>
<span data-ttu-id="7d649-127">要求本文で、 [macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d649-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="7d649-128">次の表に、 [macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d649-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="7d649-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d649-129">Property</span></span>|<span data-ttu-id="7d649-130">型</span><span class="sxs-lookup"><span data-stu-id="7d649-130">Type</span></span>|<span data-ttu-id="7d649-131">説明</span><span class="sxs-lookup"><span data-stu-id="7d649-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d649-132">id</span><span class="sxs-lookup"><span data-stu-id="7d649-132">id</span></span>|<span data-ttu-id="7d649-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d649-133">String</span></span>|<span data-ttu-id="7d649-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d649-134">Key of the entity.</span></span> <span data-ttu-id="7d649-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d649-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7d649-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d649-137">DateTimeOffset</span></span>|<span data-ttu-id="7d649-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7d649-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7d649-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d649-140">roleScopeTagIds</span></span>|<span data-ttu-id="7d649-141">String collection</span><span class="sxs-lookup"><span data-stu-id="7d649-141">String collection</span></span>|<span data-ttu-id="7d649-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7d649-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d649-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d649-144">supportsScopeTags</span></span>|<span data-ttu-id="7d649-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d649-145">Boolean</span></span>|<span data-ttu-id="7d649-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7d649-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d649-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7d649-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d649-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7d649-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d649-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7d649-149">This property is read-only.</span></span> <span data-ttu-id="7d649-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d649-151">createdDateTime</span></span>|<span data-ttu-id="7d649-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d649-152">DateTimeOffset</span></span>|<span data-ttu-id="7d649-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7d649-153">DateTime the object was created.</span></span> <span data-ttu-id="7d649-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-155">description</span><span class="sxs-lookup"><span data-stu-id="7d649-155">description</span></span>|<span data-ttu-id="7d649-156">String</span><span class="sxs-lookup"><span data-stu-id="7d649-156">String</span></span>|<span data-ttu-id="7d649-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7d649-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d649-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7d649-159">displayName</span></span>|<span data-ttu-id="7d649-160">String</span><span class="sxs-lookup"><span data-stu-id="7d649-160">String</span></span>|<span data-ttu-id="7d649-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7d649-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d649-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-163">version</span><span class="sxs-lookup"><span data-stu-id="7d649-163">version</span></span>|<span data-ttu-id="7d649-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7d649-164">Int32</span></span>|<span data-ttu-id="7d649-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7d649-165">Version of the device configuration.</span></span> <span data-ttu-id="7d649-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d649-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="7d649-167">connectionName</span></span>|<span data-ttu-id="7d649-168">String</span><span class="sxs-lookup"><span data-stu-id="7d649-168">String</span></span>|<span data-ttu-id="7d649-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="7d649-169">Connection name displayed to the user.</span></span> <span data-ttu-id="7d649-170">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="7d649-171">connectionType</span></span>|[<span data-ttu-id="7d649-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7d649-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="7d649-173">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="7d649-173">Connection type.</span></span> <span data-ttu-id="7d649-174">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7d649-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7d649-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、 `f5Access2018`、、、、、、、、、、、です。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="7d649-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="7d649-176">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="7d649-176">loginGroupOrDomain</span></span>|<span data-ttu-id="7d649-177">String</span><span class="sxs-lookup"><span data-stu-id="7d649-177">String</span></span>|<span data-ttu-id="7d649-178">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="7d649-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="7d649-179">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-180">role</span><span class="sxs-lookup"><span data-stu-id="7d649-180">role</span></span>|<span data-ttu-id="7d649-181">String</span><span class="sxs-lookup"><span data-stu-id="7d649-181">String</span></span>|<span data-ttu-id="7d649-182">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="7d649-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7d649-183">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-184">領域</span><span class="sxs-lookup"><span data-stu-id="7d649-184">realm</span></span>|<span data-ttu-id="7d649-185">String</span><span class="sxs-lookup"><span data-stu-id="7d649-185">String</span></span>|<span data-ttu-id="7d649-186">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="7d649-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7d649-187">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-188">server</span><span class="sxs-lookup"><span data-stu-id="7d649-188">server</span></span>|[<span data-ttu-id="7d649-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="7d649-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="7d649-190">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="7d649-190">VPN Server on the network.</span></span> <span data-ttu-id="7d649-191">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7d649-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="7d649-192">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-193">識別子</span><span class="sxs-lookup"><span data-stu-id="7d649-193">identifier</span></span>|<span data-ttu-id="7d649-194">String</span><span class="sxs-lookup"><span data-stu-id="7d649-194">String</span></span>|<span data-ttu-id="7d649-195">接続の種類がカスタム vpn に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="7d649-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7d649-196">例: Cisco anyconnect は、[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="7d649-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-197">customData</span><span class="sxs-lookup"><span data-stu-id="7d649-197">customData</span></span>|<span data-ttu-id="7d649-198">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7d649-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="7d649-199">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="7d649-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7d649-200">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7d649-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7d649-201">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="7d649-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7d649-202">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7d649-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7d649-203">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="7d649-204">customKeyValueData</span></span>|<span data-ttu-id="7d649-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7d649-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7d649-206">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="7d649-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="7d649-207">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7d649-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="7d649-208">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="7d649-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="7d649-209">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7d649-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="7d649-210">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-211">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="7d649-211">enableSplitTunneling</span></span>|<span data-ttu-id="7d649-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d649-212">Boolean</span></span>|<span data-ttu-id="7d649-213">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="7d649-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="7d649-214">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7d649-215">authenticationMethod</span></span>|[<span data-ttu-id="7d649-216">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="7d649-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7d649-217">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="7d649-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="7d649-218">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7d649-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="7d649-219">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="7d649-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="7d649-220">enableperapp</span><span class="sxs-lookup"><span data-stu-id="7d649-220">enablePerApp</span></span>|<span data-ttu-id="7d649-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d649-221">Boolean</span></span>|<span data-ttu-id="7d649-222">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの vpn 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="7d649-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="7d649-223">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-224">saf aridomains</span><span class="sxs-lookup"><span data-stu-id="7d649-224">safariDomains</span></span>|<span data-ttu-id="7d649-225">String collection</span><span class="sxs-lookup"><span data-stu-id="7d649-225">String collection</span></span>|<span data-ttu-id="7d649-226">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="7d649-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="7d649-227">この vpn に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの vpn 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="7d649-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="7d649-228">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="7d649-229">onDemandRules</span></span>|<span data-ttu-id="7d649-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7d649-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="7d649-231">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="7d649-231">On-Demand Rules.</span></span> <span data-ttu-id="7d649-232">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7d649-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7d649-233">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="7d649-234">proxyServer</span></span>|[<span data-ttu-id="7d649-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7d649-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="7d649-236">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="7d649-236">Proxy Server.</span></span> <span data-ttu-id="7d649-237">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="7d649-238">optintodeviceidsharing</span><span class="sxs-lookup"><span data-stu-id="7d649-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="7d649-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d649-239">Boolean</span></span>|<span data-ttu-id="7d649-240">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="7d649-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="7d649-241">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7d649-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7d649-242">応答</span><span class="sxs-lookup"><span data-stu-id="7d649-242">Response</span></span>
<span data-ttu-id="7d649-243">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d649-243">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d649-244">例</span><span class="sxs-lookup"><span data-stu-id="7d649-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d649-245">要求</span><span class="sxs-lookup"><span data-stu-id="7d649-245">Request</span></span>
<span data-ttu-id="7d649-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d649-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="7d649-247">応答</span><span class="sxs-lookup"><span data-stu-id="7d649-247">Response</span></span>
<span data-ttu-id="7d649-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d649-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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




