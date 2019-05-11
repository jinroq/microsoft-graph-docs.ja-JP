---
title: IosVpnConfiguration の作成
description: 新しい iosVpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de7cbc2a357de7d4187379d2320b5718a85030ee
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923112"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="965bd-103">IosVpnConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="965bd-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="965bd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="965bd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="965bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="965bd-106">新しい[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="965bd-106">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="965bd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="965bd-107">Prerequisites</span></span>
<span data-ttu-id="965bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="965bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="965bd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="965bd-110">Permission type</span></span>|<span data-ttu-id="965bd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="965bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="965bd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="965bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="965bd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="965bd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="965bd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="965bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="965bd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965bd-115">Not supported.</span></span>|
|<span data-ttu-id="965bd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="965bd-116">Application</span></span>|<span data-ttu-id="965bd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="965bd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="965bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="965bd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="965bd-119">Request headers</span></span>
|<span data-ttu-id="965bd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="965bd-120">Header</span></span>|<span data-ttu-id="965bd-121">値</span><span class="sxs-lookup"><span data-stu-id="965bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="965bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="965bd-122">Authorization</span></span>|<span data-ttu-id="965bd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="965bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="965bd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="965bd-124">Accept</span></span>|<span data-ttu-id="965bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="965bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="965bd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="965bd-126">Request body</span></span>
<span data-ttu-id="965bd-127">要求本文で、iosVpnConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="965bd-127">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="965bd-128">次の表に、iosVpnConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="965bd-128">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="965bd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="965bd-129">Property</span></span>|<span data-ttu-id="965bd-130">型</span><span class="sxs-lookup"><span data-stu-id="965bd-130">Type</span></span>|<span data-ttu-id="965bd-131">説明</span><span class="sxs-lookup"><span data-stu-id="965bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="965bd-132">id</span><span class="sxs-lookup"><span data-stu-id="965bd-132">id</span></span>|<span data-ttu-id="965bd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="965bd-133">String</span></span>|<span data-ttu-id="965bd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="965bd-134">Key of the entity.</span></span> <span data-ttu-id="965bd-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="965bd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="965bd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="965bd-137">DateTimeOffset</span></span>|<span data-ttu-id="965bd-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="965bd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="965bd-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="965bd-140">roleScopeTagIds</span></span>|<span data-ttu-id="965bd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="965bd-141">String collection</span></span>|<span data-ttu-id="965bd-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="965bd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="965bd-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="965bd-144">supportsScopeTags</span></span>|<span data-ttu-id="965bd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="965bd-145">Boolean</span></span>|<span data-ttu-id="965bd-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="965bd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="965bd-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="965bd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="965bd-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="965bd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="965bd-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="965bd-149">This property is read-only.</span></span> <span data-ttu-id="965bd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="965bd-151">createdDateTime</span></span>|<span data-ttu-id="965bd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="965bd-152">DateTimeOffset</span></span>|<span data-ttu-id="965bd-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="965bd-153">DateTime the object was created.</span></span> <span data-ttu-id="965bd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-155">description</span><span class="sxs-lookup"><span data-stu-id="965bd-155">description</span></span>|<span data-ttu-id="965bd-156">String</span><span class="sxs-lookup"><span data-stu-id="965bd-156">String</span></span>|<span data-ttu-id="965bd-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="965bd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="965bd-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="965bd-159">displayName</span></span>|<span data-ttu-id="965bd-160">String</span><span class="sxs-lookup"><span data-stu-id="965bd-160">String</span></span>|<span data-ttu-id="965bd-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="965bd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="965bd-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-163">version</span><span class="sxs-lookup"><span data-stu-id="965bd-163">version</span></span>|<span data-ttu-id="965bd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="965bd-164">Int32</span></span>|<span data-ttu-id="965bd-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="965bd-165">Version of the device configuration.</span></span> <span data-ttu-id="965bd-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="965bd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="965bd-167">connectionName</span></span>|<span data-ttu-id="965bd-168">String</span><span class="sxs-lookup"><span data-stu-id="965bd-168">String</span></span>|<span data-ttu-id="965bd-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="965bd-169">Connection name displayed to the user.</span></span> <span data-ttu-id="965bd-170">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="965bd-171">connectionType</span></span>|[<span data-ttu-id="965bd-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="965bd-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="965bd-173">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="965bd-173">Connection type.</span></span> <span data-ttu-id="965bd-174">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="965bd-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="965bd-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、 `f5Access2018`、、、、、、、、、、、です。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="965bd-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="965bd-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="965bd-176">loginGroupOrDomain</span></span>|<span data-ttu-id="965bd-177">String</span><span class="sxs-lookup"><span data-stu-id="965bd-177">String</span></span>|<span data-ttu-id="965bd-178">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="965bd-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="965bd-179">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-180">role</span><span class="sxs-lookup"><span data-stu-id="965bd-180">role</span></span>|<span data-ttu-id="965bd-181">String</span><span class="sxs-lookup"><span data-stu-id="965bd-181">String</span></span>|<span data-ttu-id="965bd-182">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="965bd-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="965bd-183">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-184">領域</span><span class="sxs-lookup"><span data-stu-id="965bd-184">realm</span></span>|<span data-ttu-id="965bd-185">String</span><span class="sxs-lookup"><span data-stu-id="965bd-185">String</span></span>|<span data-ttu-id="965bd-186">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="965bd-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="965bd-187">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-188">server</span><span class="sxs-lookup"><span data-stu-id="965bd-188">server</span></span>|[<span data-ttu-id="965bd-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="965bd-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="965bd-190">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="965bd-190">VPN Server on the network.</span></span> <span data-ttu-id="965bd-191">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="965bd-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="965bd-192">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-193">識別子</span><span class="sxs-lookup"><span data-stu-id="965bd-193">identifier</span></span>|<span data-ttu-id="965bd-194">String</span><span class="sxs-lookup"><span data-stu-id="965bd-194">String</span></span>|<span data-ttu-id="965bd-195">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="965bd-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="965bd-196">例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="965bd-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-197">customData</span><span class="sxs-lookup"><span data-stu-id="965bd-197">customData</span></span>|<span data-ttu-id="965bd-198">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="965bd-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="965bd-199">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="965bd-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="965bd-200">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="965bd-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="965bd-201">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="965bd-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="965bd-202">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="965bd-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="965bd-203">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="965bd-204">customKeyValueData</span></span>|<span data-ttu-id="965bd-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="965bd-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="965bd-206">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="965bd-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="965bd-207">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="965bd-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="965bd-208">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="965bd-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="965bd-209">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="965bd-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="965bd-210">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="965bd-211">enableSplitTunneling</span></span>|<span data-ttu-id="965bd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="965bd-212">Boolean</span></span>|<span data-ttu-id="965bd-213">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="965bd-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="965bd-214">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="965bd-215">authenticationMethod</span></span>|[<span data-ttu-id="965bd-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="965bd-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="965bd-217">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="965bd-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="965bd-218">[[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="965bd-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="965bd-219">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="965bd-219">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="965bd-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="965bd-220">enablePerApp</span></span>|<span data-ttu-id="965bd-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="965bd-221">Boolean</span></span>|<span data-ttu-id="965bd-222">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="965bd-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="965bd-223">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-224">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="965bd-224">safariDomains</span></span>|<span data-ttu-id="965bd-225">String collection</span><span class="sxs-lookup"><span data-stu-id="965bd-225">String collection</span></span>|<span data-ttu-id="965bd-226">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="965bd-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="965bd-227">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="965bd-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="965bd-228">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="965bd-229">onDemandRules</span></span>|<span data-ttu-id="965bd-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="965bd-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="965bd-231">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="965bd-231">On-Demand Rules.</span></span> <span data-ttu-id="965bd-232">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="965bd-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="965bd-233">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="965bd-234">proxyServer</span></span>|[<span data-ttu-id="965bd-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="965bd-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="965bd-236">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="965bd-236">Proxy Server.</span></span> <span data-ttu-id="965bd-237">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="965bd-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="965bd-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="965bd-239">Boolean</span></span>|<span data-ttu-id="965bd-240">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="965bd-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="965bd-241">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="965bd-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="965bd-242">providerType</span><span class="sxs-lookup"><span data-stu-id="965bd-242">providerType</span></span>|[<span data-ttu-id="965bd-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="965bd-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="965bd-244">アプリごとの VPN のプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="965bd-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="965bd-245">可能な値は、`notConfigured`、`appProxy`、`packetTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="965bd-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="965bd-246">Userdomain に</span><span class="sxs-lookup"><span data-stu-id="965bd-246">userDomain</span></span>|<span data-ttu-id="965bd-247">String</span><span class="sxs-lookup"><span data-stu-id="965bd-247">String</span></span>|<span data-ttu-id="965bd-248">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="965bd-248">Zscaler only.</span></span> <span data-ttu-id="965bd-249">Zscaler アプリでログインフィールドに事前設定するには、静的ドメインを入力します。</span><span class="sxs-lookup"><span data-stu-id="965bd-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="965bd-250">この指定を省略すると、代わりにユーザーの Azure Active Directory ドメインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="965bd-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="965bd-251">Cloudname</span><span class="sxs-lookup"><span data-stu-id="965bd-251">strictEnforcement</span></span>|<span data-ttu-id="965bd-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="965bd-252">Boolean</span></span>|<span data-ttu-id="965bd-253">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="965bd-253">Zscaler only.</span></span> <span data-ttu-id="965bd-254">ユーザーが Zscaler アプリにサインインするまでネットワークトラフィックをブロックします。</span><span class="sxs-lookup"><span data-stu-id="965bd-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="965bd-255">"True" はトラフィックがブロックされることを意味します。</span><span class="sxs-lookup"><span data-stu-id="965bd-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="965bd-256">cloudName</span><span class="sxs-lookup"><span data-stu-id="965bd-256">cloudName</span></span>|<span data-ttu-id="965bd-257">String</span><span class="sxs-lookup"><span data-stu-id="965bd-257">String</span></span>|<span data-ttu-id="965bd-258">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="965bd-258">Zscaler only.</span></span> <span data-ttu-id="965bd-259">ユーザーが割り当てられている Zscaler cloud。</span><span class="sxs-lookup"><span data-stu-id="965bd-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="965bd-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="965bd-260">excludeList</span></span>|<span data-ttu-id="965bd-261">String collection</span><span class="sxs-lookup"><span data-stu-id="965bd-261">String collection</span></span>|<span data-ttu-id="965bd-262">Zscaler のみ。</span><span class="sxs-lookup"><span data-stu-id="965bd-262">Zscaler only.</span></span> <span data-ttu-id="965bd-263">Zscaler クラウド経由で送信されないネットワークアドレスのリスト。</span><span class="sxs-lookup"><span data-stu-id="965bd-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="965bd-264">応答</span><span class="sxs-lookup"><span data-stu-id="965bd-264">Response</span></span>
<span data-ttu-id="965bd-265">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="965bd-265">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="965bd-266">例</span><span class="sxs-lookup"><span data-stu-id="965bd-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="965bd-267">要求</span><span class="sxs-lookup"><span data-stu-id="965bd-267">Request</span></span>
<span data-ttu-id="965bd-268">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="965bd-268">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="965bd-269">応答</span><span class="sxs-lookup"><span data-stu-id="965bd-269">Response</span></span>
<span data-ttu-id="965bd-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="965bd-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




