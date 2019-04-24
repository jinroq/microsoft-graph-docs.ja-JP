---
title: iosvpnconfiguration の作成
description: 新しい iosvpnconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7821db7f38a83a94092d54ba2c0ca2eb763a01dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519116"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="2da16-103">iosvpnconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="2da16-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="2da16-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2da16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2da16-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2da16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2da16-106">新しい[iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2da16-106">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2da16-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2da16-107">Prerequisites</span></span>
<span data-ttu-id="2da16-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2da16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2da16-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2da16-110">Permission type</span></span>|<span data-ttu-id="2da16-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2da16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2da16-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2da16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2da16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2da16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2da16-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2da16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2da16-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2da16-115">Not supported.</span></span>|
|<span data-ttu-id="2da16-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2da16-116">Application</span></span>|<span data-ttu-id="2da16-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2da16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2da16-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2da16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2da16-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2da16-119">Request headers</span></span>
|<span data-ttu-id="2da16-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2da16-120">Header</span></span>|<span data-ttu-id="2da16-121">値</span><span class="sxs-lookup"><span data-stu-id="2da16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2da16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da16-122">Authorization</span></span>|<span data-ttu-id="2da16-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2da16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2da16-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2da16-124">Accept</span></span>|<span data-ttu-id="2da16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2da16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2da16-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2da16-126">Request body</span></span>
<span data-ttu-id="2da16-127">要求本文で、iosvpnconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2da16-127">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="2da16-128">次の表に、iosvpnconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2da16-128">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="2da16-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2da16-129">Property</span></span>|<span data-ttu-id="2da16-130">型</span><span class="sxs-lookup"><span data-stu-id="2da16-130">Type</span></span>|<span data-ttu-id="2da16-131">説明</span><span class="sxs-lookup"><span data-stu-id="2da16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2da16-132">id</span><span class="sxs-lookup"><span data-stu-id="2da16-132">id</span></span>|<span data-ttu-id="2da16-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2da16-133">String</span></span>|<span data-ttu-id="2da16-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2da16-134">Key of the entity.</span></span> <span data-ttu-id="2da16-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2da16-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2da16-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2da16-137">DateTimeOffset</span></span>|<span data-ttu-id="2da16-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2da16-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2da16-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2da16-140">roleScopeTagIds</span></span>|<span data-ttu-id="2da16-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2da16-141">String collection</span></span>|<span data-ttu-id="2da16-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2da16-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2da16-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2da16-144">supportsScopeTags</span></span>|<span data-ttu-id="2da16-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da16-145">Boolean</span></span>|<span data-ttu-id="2da16-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2da16-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2da16-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2da16-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2da16-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2da16-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2da16-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2da16-149">This property is read-only.</span></span> <span data-ttu-id="2da16-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2da16-151">createdDateTime</span></span>|<span data-ttu-id="2da16-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2da16-152">DateTimeOffset</span></span>|<span data-ttu-id="2da16-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2da16-153">DateTime the object was created.</span></span> <span data-ttu-id="2da16-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-155">説明</span><span class="sxs-lookup"><span data-stu-id="2da16-155">description</span></span>|<span data-ttu-id="2da16-156">String</span><span class="sxs-lookup"><span data-stu-id="2da16-156">String</span></span>|<span data-ttu-id="2da16-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2da16-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2da16-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2da16-159">displayName</span></span>|<span data-ttu-id="2da16-160">String</span><span class="sxs-lookup"><span data-stu-id="2da16-160">String</span></span>|<span data-ttu-id="2da16-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2da16-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2da16-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-163">version</span><span class="sxs-lookup"><span data-stu-id="2da16-163">version</span></span>|<span data-ttu-id="2da16-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2da16-164">Int32</span></span>|<span data-ttu-id="2da16-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2da16-165">Version of the device configuration.</span></span> <span data-ttu-id="2da16-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2da16-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="2da16-167">connectionName</span></span>|<span data-ttu-id="2da16-168">String</span><span class="sxs-lookup"><span data-stu-id="2da16-168">String</span></span>|<span data-ttu-id="2da16-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="2da16-169">Connection name displayed to the user.</span></span> <span data-ttu-id="2da16-170">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="2da16-171">connectionType</span></span>|[<span data-ttu-id="2da16-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2da16-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2da16-173">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="2da16-173">Connection type.</span></span> <span data-ttu-id="2da16-174">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2da16-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2da16-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、 `f5Access2018`、、、、、、、、、、、です。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="2da16-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="2da16-176">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="2da16-176">loginGroupOrDomain</span></span>|<span data-ttu-id="2da16-177">String</span><span class="sxs-lookup"><span data-stu-id="2da16-177">String</span></span>|<span data-ttu-id="2da16-178">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="2da16-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2da16-179">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-180">role</span><span class="sxs-lookup"><span data-stu-id="2da16-180">role</span></span>|<span data-ttu-id="2da16-181">String</span><span class="sxs-lookup"><span data-stu-id="2da16-181">String</span></span>|<span data-ttu-id="2da16-182">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="2da16-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2da16-183">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-184">領域</span><span class="sxs-lookup"><span data-stu-id="2da16-184">realm</span></span>|<span data-ttu-id="2da16-185">String</span><span class="sxs-lookup"><span data-stu-id="2da16-185">String</span></span>|<span data-ttu-id="2da16-186">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="2da16-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2da16-187">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-188">server</span><span class="sxs-lookup"><span data-stu-id="2da16-188">server</span></span>|[<span data-ttu-id="2da16-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2da16-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2da16-190">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="2da16-190">VPN Server on the network.</span></span> <span data-ttu-id="2da16-191">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2da16-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="2da16-192">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-193">識別子</span><span class="sxs-lookup"><span data-stu-id="2da16-193">identifier</span></span>|<span data-ttu-id="2da16-194">String</span><span class="sxs-lookup"><span data-stu-id="2da16-194">String</span></span>|<span data-ttu-id="2da16-195">接続の種類がカスタム vpn に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="2da16-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2da16-196">例: Cisco anyconnect は、[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="2da16-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-197">customData</span><span class="sxs-lookup"><span data-stu-id="2da16-197">customData</span></span>|<span data-ttu-id="2da16-198">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2da16-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2da16-199">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="2da16-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2da16-200">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2da16-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2da16-201">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="2da16-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2da16-202">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2da16-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2da16-203">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2da16-204">customKeyValueData</span></span>|<span data-ttu-id="2da16-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2da16-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2da16-206">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="2da16-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2da16-207">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2da16-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2da16-208">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="2da16-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2da16-209">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2da16-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2da16-210">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-211">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="2da16-211">enableSplitTunneling</span></span>|<span data-ttu-id="2da16-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da16-212">Boolean</span></span>|<span data-ttu-id="2da16-213">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="2da16-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="2da16-214">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2da16-215">authenticationMethod</span></span>|[<span data-ttu-id="2da16-216">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2da16-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2da16-217">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="2da16-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2da16-218">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2da16-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2da16-219">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="2da16-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="2da16-220">enableperapp</span><span class="sxs-lookup"><span data-stu-id="2da16-220">enablePerApp</span></span>|<span data-ttu-id="2da16-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da16-221">Boolean</span></span>|<span data-ttu-id="2da16-222">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの vpn 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="2da16-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2da16-223">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-224">saf aridomains</span><span class="sxs-lookup"><span data-stu-id="2da16-224">safariDomains</span></span>|<span data-ttu-id="2da16-225">String collection</span><span class="sxs-lookup"><span data-stu-id="2da16-225">String collection</span></span>|<span data-ttu-id="2da16-226">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="2da16-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2da16-227">この vpn に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの vpn 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="2da16-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2da16-228">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2da16-229">onDemandRules</span></span>|<span data-ttu-id="2da16-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2da16-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2da16-231">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="2da16-231">On-Demand Rules.</span></span> <span data-ttu-id="2da16-232">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2da16-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2da16-233">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2da16-234">proxyServer</span></span>|[<span data-ttu-id="2da16-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2da16-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2da16-236">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="2da16-236">Proxy Server.</span></span> <span data-ttu-id="2da16-237">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-238">optintodeviceidsharing</span><span class="sxs-lookup"><span data-stu-id="2da16-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2da16-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da16-239">Boolean</span></span>|<span data-ttu-id="2da16-240">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="2da16-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2da16-241">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="2da16-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2da16-242">providerType</span><span class="sxs-lookup"><span data-stu-id="2da16-242">providerType</span></span>|[<span data-ttu-id="2da16-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="2da16-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="2da16-244">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="2da16-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="2da16-245">使用可能な値は、`notConfigured`、`appProxy`、`packetTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="2da16-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="2da16-246">userdomain に</span><span class="sxs-lookup"><span data-stu-id="2da16-246">userDomain</span></span>|<span data-ttu-id="2da16-247">String</span><span class="sxs-lookup"><span data-stu-id="2da16-247">String</span></span>|<span data-ttu-id="2da16-248">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="2da16-248">Zscaler only.</span></span> <span data-ttu-id="2da16-249">Zscaler アプリでログインフィールドに事前設定するには、静的ドメインを入力します。</span><span class="sxs-lookup"><span data-stu-id="2da16-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="2da16-250">この指定を省略すると、代わりにユーザーの Azure Active Directory ドメインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="2da16-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="2da16-251">cloudname</span><span class="sxs-lookup"><span data-stu-id="2da16-251">strictEnforcement</span></span>|<span data-ttu-id="2da16-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="2da16-252">Boolean</span></span>|<span data-ttu-id="2da16-253">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="2da16-253">Zscaler only.</span></span> <span data-ttu-id="2da16-254">ユーザーが Zscaler アプリにサインインするまでネットワークトラフィックをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2da16-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="2da16-255">"True" はトラフィックがブロックされることを意味します。</span><span class="sxs-lookup"><span data-stu-id="2da16-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="2da16-256">cloudname</span><span class="sxs-lookup"><span data-stu-id="2da16-256">cloudName</span></span>|<span data-ttu-id="2da16-257">String</span><span class="sxs-lookup"><span data-stu-id="2da16-257">String</span></span>|<span data-ttu-id="2da16-258">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="2da16-258">Zscaler only.</span></span> <span data-ttu-id="2da16-259">ユーザーが割り当てられている Zscaler cloud。</span><span class="sxs-lookup"><span data-stu-id="2da16-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="2da16-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="2da16-260">excludeList</span></span>|<span data-ttu-id="2da16-261">String collection</span><span class="sxs-lookup"><span data-stu-id="2da16-261">String collection</span></span>|<span data-ttu-id="2da16-262">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="2da16-262">Zscaler only.</span></span> <span data-ttu-id="2da16-263">Zscaler クラウド経由で送信されないネットワークアドレスのリスト。</span><span class="sxs-lookup"><span data-stu-id="2da16-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="2da16-264">応答</span><span class="sxs-lookup"><span data-stu-id="2da16-264">Response</span></span>
<span data-ttu-id="2da16-265">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2da16-265">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da16-266">例</span><span class="sxs-lookup"><span data-stu-id="2da16-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="2da16-267">要求</span><span class="sxs-lookup"><span data-stu-id="2da16-267">Request</span></span>
<span data-ttu-id="2da16-268">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2da16-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="2da16-269">応答</span><span class="sxs-lookup"><span data-stu-id="2da16-269">Response</span></span>
<span data-ttu-id="2da16-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2da16-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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





