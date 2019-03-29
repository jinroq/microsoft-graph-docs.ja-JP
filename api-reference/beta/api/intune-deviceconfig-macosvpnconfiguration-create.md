---
title: macosvpnconfiguration の作成
description: 新しい macosvpnconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a9769bc59f69c5ed88679a7ead4e4bdd51840f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970801"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="81c36-103">macosvpnconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="81c36-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="81c36-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81c36-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81c36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81c36-106">新しい[macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="81c36-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81c36-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="81c36-107">Prerequisites</span></span>
<span data-ttu-id="81c36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81c36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c36-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81c36-110">Permission type</span></span>|<span data-ttu-id="81c36-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81c36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81c36-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81c36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81c36-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c36-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81c36-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81c36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81c36-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c36-115">Not supported.</span></span>|
|<span data-ttu-id="81c36-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81c36-116">Application</span></span>|<span data-ttu-id="81c36-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81c36-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81c36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="81c36-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81c36-119">Request headers</span></span>
|<span data-ttu-id="81c36-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81c36-120">Header</span></span>|<span data-ttu-id="81c36-121">値</span><span class="sxs-lookup"><span data-stu-id="81c36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81c36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c36-122">Authorization</span></span>|<span data-ttu-id="81c36-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="81c36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81c36-124">承諾</span><span class="sxs-lookup"><span data-stu-id="81c36-124">Accept</span></span>|<span data-ttu-id="81c36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81c36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c36-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="81c36-126">Request body</span></span>
<span data-ttu-id="81c36-127">要求本文で、macosvpnconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81c36-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="81c36-128">次の表に、macosvpnconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="81c36-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="81c36-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81c36-129">Property</span></span>|<span data-ttu-id="81c36-130">型</span><span class="sxs-lookup"><span data-stu-id="81c36-130">Type</span></span>|<span data-ttu-id="81c36-131">説明</span><span class="sxs-lookup"><span data-stu-id="81c36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81c36-132">id</span><span class="sxs-lookup"><span data-stu-id="81c36-132">id</span></span>|<span data-ttu-id="81c36-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81c36-133">String</span></span>|<span data-ttu-id="81c36-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="81c36-134">Key of the entity.</span></span> <span data-ttu-id="81c36-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81c36-136">lastModifiedDateTime</span></span>|<span data-ttu-id="81c36-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81c36-137">DateTimeOffset</span></span>|<span data-ttu-id="81c36-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="81c36-138">DateTime the object was last modified.</span></span> <span data-ttu-id="81c36-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81c36-140">roleScopeTagIds</span></span>|<span data-ttu-id="81c36-141">String collection</span><span class="sxs-lookup"><span data-stu-id="81c36-141">String collection</span></span>|<span data-ttu-id="81c36-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="81c36-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81c36-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="81c36-144">supportsScopeTags</span></span>|<span data-ttu-id="81c36-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="81c36-145">Boolean</span></span>|<span data-ttu-id="81c36-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="81c36-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="81c36-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="81c36-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="81c36-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="81c36-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="81c36-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="81c36-149">This property is read-only.</span></span> <span data-ttu-id="81c36-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81c36-151">createdDateTime</span></span>|<span data-ttu-id="81c36-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81c36-152">DateTimeOffset</span></span>|<span data-ttu-id="81c36-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="81c36-153">DateTime the object was created.</span></span> <span data-ttu-id="81c36-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-155">description</span><span class="sxs-lookup"><span data-stu-id="81c36-155">description</span></span>|<span data-ttu-id="81c36-156">String</span><span class="sxs-lookup"><span data-stu-id="81c36-156">String</span></span>|<span data-ttu-id="81c36-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="81c36-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="81c36-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-159">displayName</span><span class="sxs-lookup"><span data-stu-id="81c36-159">displayName</span></span>|<span data-ttu-id="81c36-160">String</span><span class="sxs-lookup"><span data-stu-id="81c36-160">String</span></span>|<span data-ttu-id="81c36-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="81c36-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="81c36-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-163">version</span><span class="sxs-lookup"><span data-stu-id="81c36-163">version</span></span>|<span data-ttu-id="81c36-164">Int32</span><span class="sxs-lookup"><span data-stu-id="81c36-164">Int32</span></span>|<span data-ttu-id="81c36-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="81c36-165">Version of the device configuration.</span></span> <span data-ttu-id="81c36-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="81c36-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="81c36-167">connectionName</span></span>|<span data-ttu-id="81c36-168">String</span><span class="sxs-lookup"><span data-stu-id="81c36-168">String</span></span>|<span data-ttu-id="81c36-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="81c36-169">Connection name displayed to the user.</span></span> <span data-ttu-id="81c36-170">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="81c36-171">connectionType</span></span>|[<span data-ttu-id="81c36-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="81c36-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="81c36-173">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="81c36-173">Connection type.</span></span> <span data-ttu-id="81c36-174">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="81c36-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="81c36-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、 `f5Access2018`、、、、、、、、、、、です。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="81c36-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="81c36-176">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="81c36-176">loginGroupOrDomain</span></span>|<span data-ttu-id="81c36-177">String</span><span class="sxs-lookup"><span data-stu-id="81c36-177">String</span></span>|<span data-ttu-id="81c36-178">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="81c36-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="81c36-179">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-180">role</span><span class="sxs-lookup"><span data-stu-id="81c36-180">role</span></span>|<span data-ttu-id="81c36-181">String</span><span class="sxs-lookup"><span data-stu-id="81c36-181">String</span></span>|<span data-ttu-id="81c36-182">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="81c36-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="81c36-183">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-184">領域</span><span class="sxs-lookup"><span data-stu-id="81c36-184">realm</span></span>|<span data-ttu-id="81c36-185">String</span><span class="sxs-lookup"><span data-stu-id="81c36-185">String</span></span>|<span data-ttu-id="81c36-186">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="81c36-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="81c36-187">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-188">server</span><span class="sxs-lookup"><span data-stu-id="81c36-188">server</span></span>|[<span data-ttu-id="81c36-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="81c36-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="81c36-190">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="81c36-190">VPN Server on the network.</span></span> <span data-ttu-id="81c36-191">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="81c36-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="81c36-192">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-193">識別子</span><span class="sxs-lookup"><span data-stu-id="81c36-193">identifier</span></span>|<span data-ttu-id="81c36-194">String</span><span class="sxs-lookup"><span data-stu-id="81c36-194">String</span></span>|<span data-ttu-id="81c36-195">接続の種類がカスタム vpn に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="81c36-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="81c36-196">例: Cisco anyconnect は、[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="81c36-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-197">customData</span><span class="sxs-lookup"><span data-stu-id="81c36-197">customData</span></span>|<span data-ttu-id="81c36-198">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81c36-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="81c36-199">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="81c36-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="81c36-200">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="81c36-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="81c36-201">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="81c36-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="81c36-202">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="81c36-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="81c36-203">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="81c36-204">customKeyValueData</span></span>|<span data-ttu-id="81c36-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81c36-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81c36-206">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="81c36-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="81c36-207">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="81c36-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="81c36-208">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="81c36-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="81c36-209">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="81c36-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="81c36-210">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-211">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="81c36-211">enableSplitTunneling</span></span>|<span data-ttu-id="81c36-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="81c36-212">Boolean</span></span>|<span data-ttu-id="81c36-213">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="81c36-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="81c36-214">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81c36-215">authenticationMethod</span></span>|[<span data-ttu-id="81c36-216">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="81c36-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="81c36-217">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="81c36-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="81c36-218">[[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="81c36-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="81c36-219">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="81c36-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="81c36-220">enableperapp</span><span class="sxs-lookup"><span data-stu-id="81c36-220">enablePerApp</span></span>|<span data-ttu-id="81c36-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="81c36-221">Boolean</span></span>|<span data-ttu-id="81c36-222">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの vpn 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="81c36-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="81c36-223">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-224">saf aridomains</span><span class="sxs-lookup"><span data-stu-id="81c36-224">safariDomains</span></span>|<span data-ttu-id="81c36-225">String collection</span><span class="sxs-lookup"><span data-stu-id="81c36-225">String collection</span></span>|<span data-ttu-id="81c36-226">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="81c36-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="81c36-227">この vpn に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの vpn 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="81c36-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="81c36-228">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="81c36-229">onDemandRules</span></span>|<span data-ttu-id="81c36-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="81c36-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="81c36-231">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="81c36-231">On-Demand Rules.</span></span> <span data-ttu-id="81c36-232">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="81c36-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="81c36-233">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="81c36-234">proxyServer</span></span>|[<span data-ttu-id="81c36-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="81c36-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="81c36-236">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="81c36-236">Proxy Server.</span></span> <span data-ttu-id="81c36-237">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="81c36-238">optintodeviceidsharing</span><span class="sxs-lookup"><span data-stu-id="81c36-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="81c36-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="81c36-239">Boolean</span></span>|<span data-ttu-id="81c36-240">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="81c36-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="81c36-241">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="81c36-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="81c36-242">応答</span><span class="sxs-lookup"><span data-stu-id="81c36-242">Response</span></span>
<span data-ttu-id="81c36-243">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81c36-243">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81c36-244">例</span><span class="sxs-lookup"><span data-stu-id="81c36-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="81c36-245">要求</span><span class="sxs-lookup"><span data-stu-id="81c36-245">Request</span></span>
<span data-ttu-id="81c36-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81c36-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="81c36-247">応答</span><span class="sxs-lookup"><span data-stu-id="81c36-247">Response</span></span>
<span data-ttu-id="81c36-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81c36-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




