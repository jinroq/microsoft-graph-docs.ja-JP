---
title: りんご evpnconfiguration リソースの種類
description: Apple VPN 構成プロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d63fa3f8a93551be9c3180d4f8d6c7119838efd8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794898"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="62b78-103">りんご evpnconfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62b78-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="62b78-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62b78-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b78-106">Apple VPN 構成プロファイル。</span><span class="sxs-lookup"><span data-stu-id="62b78-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="62b78-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="62b78-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="62b78-108">Methods</span></span>
|<span data-ttu-id="62b78-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="62b78-109">Method</span></span>|<span data-ttu-id="62b78-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="62b78-110">Return Type</span></span>|<span data-ttu-id="62b78-111">説明</span><span class="sxs-lookup"><span data-stu-id="62b78-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62b78-112">りんごの構成を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="62b78-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="62b78-113">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="62b78-114">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="62b78-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="62b78-115">作業環境の設定を取得する</span><span class="sxs-lookup"><span data-stu-id="62b78-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="62b78-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="62b78-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="62b78-117">[りんご evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="62b78-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62b78-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b78-118">Properties</span></span>
|<span data-ttu-id="62b78-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b78-119">Property</span></span>|<span data-ttu-id="62b78-120">型</span><span class="sxs-lookup"><span data-stu-id="62b78-120">Type</span></span>|<span data-ttu-id="62b78-121">説明</span><span class="sxs-lookup"><span data-stu-id="62b78-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b78-122">id</span><span class="sxs-lookup"><span data-stu-id="62b78-122">id</span></span>|<span data-ttu-id="62b78-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="62b78-123">String</span></span>|<span data-ttu-id="62b78-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62b78-124">Key of the entity.</span></span> <span data-ttu-id="62b78-125">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62b78-126">lastModifiedDateTime</span></span>|<span data-ttu-id="62b78-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b78-127">DateTimeOffset</span></span>|<span data-ttu-id="62b78-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="62b78-128">DateTime the object was last modified.</span></span> <span data-ttu-id="62b78-129">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62b78-130">roleScopeTagIds</span></span>|<span data-ttu-id="62b78-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-131">String collection</span></span>|<span data-ttu-id="62b78-132">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="62b78-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62b78-133">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62b78-134">supportsScopeTags</span></span>|<span data-ttu-id="62b78-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="62b78-135">Boolean</span></span>|<span data-ttu-id="62b78-136">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62b78-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62b78-137">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="62b78-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62b78-138">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="62b78-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62b78-139">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="62b78-139">This property is read-only.</span></span> <span data-ttu-id="62b78-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62b78-141">createdDateTime</span></span>|<span data-ttu-id="62b78-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b78-142">DateTimeOffset</span></span>|<span data-ttu-id="62b78-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="62b78-143">DateTime the object was created.</span></span> <span data-ttu-id="62b78-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-145">説明</span><span class="sxs-lookup"><span data-stu-id="62b78-145">description</span></span>|<span data-ttu-id="62b78-146">String</span><span class="sxs-lookup"><span data-stu-id="62b78-146">String</span></span>|<span data-ttu-id="62b78-147">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="62b78-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62b78-148">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-149">displayName</span><span class="sxs-lookup"><span data-stu-id="62b78-149">displayName</span></span>|<span data-ttu-id="62b78-150">String</span><span class="sxs-lookup"><span data-stu-id="62b78-150">String</span></span>|<span data-ttu-id="62b78-151">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="62b78-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62b78-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-153">version</span><span class="sxs-lookup"><span data-stu-id="62b78-153">version</span></span>|<span data-ttu-id="62b78-154">Int32</span><span class="sxs-lookup"><span data-stu-id="62b78-154">Int32</span></span>|<span data-ttu-id="62b78-155">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="62b78-155">Version of the device configuration.</span></span> <span data-ttu-id="62b78-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-157">connectionName</span><span class="sxs-lookup"><span data-stu-id="62b78-157">connectionName</span></span>|<span data-ttu-id="62b78-158">文字列</span><span class="sxs-lookup"><span data-stu-id="62b78-158">String</span></span>|<span data-ttu-id="62b78-159">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="62b78-159">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="62b78-160">connectionType</span><span class="sxs-lookup"><span data-stu-id="62b78-160">connectionType</span></span>|[<span data-ttu-id="62b78-161">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="62b78-161">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="62b78-162">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="62b78-162">Connection type.</span></span> <span data-ttu-id="62b78-163">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、 `f5Access2018`、、、、、、、、、、、です。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="62b78-163">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="62b78-164">logingroupordomain</span><span class="sxs-lookup"><span data-stu-id="62b78-164">loginGroupOrDomain</span></span>|<span data-ttu-id="62b78-165">文字列</span><span class="sxs-lookup"><span data-stu-id="62b78-165">String</span></span>|<span data-ttu-id="62b78-166">接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="62b78-166">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="62b78-167">role</span><span class="sxs-lookup"><span data-stu-id="62b78-167">role</span></span>|<span data-ttu-id="62b78-168">文字列</span><span class="sxs-lookup"><span data-stu-id="62b78-168">String</span></span>|<span data-ttu-id="62b78-169">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="62b78-169">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="62b78-170">領域</span><span class="sxs-lookup"><span data-stu-id="62b78-170">realm</span></span>|<span data-ttu-id="62b78-171">文字列</span><span class="sxs-lookup"><span data-stu-id="62b78-171">String</span></span>|<span data-ttu-id="62b78-172">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="62b78-172">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="62b78-173">server</span><span class="sxs-lookup"><span data-stu-id="62b78-173">server</span></span>|[<span data-ttu-id="62b78-174">vpnServer</span><span class="sxs-lookup"><span data-stu-id="62b78-174">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="62b78-175">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="62b78-175">VPN Server on the network.</span></span> <span data-ttu-id="62b78-176">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="62b78-176">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="62b78-177">識別子</span><span class="sxs-lookup"><span data-stu-id="62b78-177">identifier</span></span>|<span data-ttu-id="62b78-178">文字列</span><span class="sxs-lookup"><span data-stu-id="62b78-178">String</span></span>|<span data-ttu-id="62b78-179">接続の種類がカスタム vpn に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="62b78-179">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="62b78-180">例: cisco anyconnect は、という形式の識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="62b78-180">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="62b78-181">customData</span><span class="sxs-lookup"><span data-stu-id="62b78-181">customData</span></span>|<span data-ttu-id="62b78-182">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-182">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="62b78-183">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="62b78-183">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="62b78-184">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="62b78-184">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="62b78-185">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="62b78-185">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="62b78-186">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62b78-186">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="62b78-187">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="62b78-187">customKeyValueData</span></span>|<span data-ttu-id="62b78-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-188">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="62b78-189">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="62b78-189">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="62b78-190">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="62b78-190">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="62b78-191">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="62b78-191">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="62b78-192">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62b78-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="62b78-193">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="62b78-193">enableSplitTunneling</span></span>|<span data-ttu-id="62b78-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="62b78-194">Boolean</span></span>|<span data-ttu-id="62b78-195">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="62b78-195">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="62b78-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="62b78-196">authenticationMethod</span></span>|[<span data-ttu-id="62b78-197">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="62b78-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="62b78-198">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="62b78-198">Authentication method for this VPN connection.</span></span> <span data-ttu-id="62b78-199">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="62b78-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="62b78-200">enableperapp</span><span class="sxs-lookup"><span data-stu-id="62b78-200">enablePerApp</span></span>|<span data-ttu-id="62b78-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="62b78-201">Boolean</span></span>|<span data-ttu-id="62b78-202">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの vpn 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="62b78-202">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="62b78-203">saf aridomains</span><span class="sxs-lookup"><span data-stu-id="62b78-203">safariDomains</span></span>|<span data-ttu-id="62b78-204">String コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-204">String collection</span></span>|<span data-ttu-id="62b78-205">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="62b78-205">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="62b78-206">この vpn に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの vpn 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="62b78-206">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="62b78-207">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="62b78-207">onDemandRules</span></span>|<span data-ttu-id="62b78-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-208">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="62b78-209">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="62b78-209">On-Demand Rules.</span></span> <span data-ttu-id="62b78-210">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="62b78-210">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="62b78-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="62b78-211">proxyServer</span></span>|[<span data-ttu-id="62b78-212">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="62b78-212">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="62b78-213">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="62b78-213">Proxy Server.</span></span>|
|<span data-ttu-id="62b78-214">optintodeviceidsharing</span><span class="sxs-lookup"><span data-stu-id="62b78-214">optInToDeviceIdSharing</span></span>|<span data-ttu-id="62b78-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="62b78-215">Boolean</span></span>|<span data-ttu-id="62b78-216">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="62b78-216">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62b78-217">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62b78-217">Relationships</span></span>
|<span data-ttu-id="62b78-218">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62b78-218">Relationship</span></span>|<span data-ttu-id="62b78-219">型</span><span class="sxs-lookup"><span data-stu-id="62b78-219">Type</span></span>|<span data-ttu-id="62b78-220">説明</span><span class="sxs-lookup"><span data-stu-id="62b78-220">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b78-221">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="62b78-221">groupAssignments</span></span>|<span data-ttu-id="62b78-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-222">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="62b78-223">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="62b78-223">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="62b78-224">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-224">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-225">assignments</span><span class="sxs-lookup"><span data-stu-id="62b78-225">assignments</span></span>|<span data-ttu-id="62b78-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-226">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="62b78-227">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="62b78-227">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="62b78-228">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-229">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="62b78-229">deviceStatuses</span></span>|<span data-ttu-id="62b78-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-230">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="62b78-231">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="62b78-231">Device configuration installation status by device.</span></span> <span data-ttu-id="62b78-232">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-233">userStatuses</span><span class="sxs-lookup"><span data-stu-id="62b78-233">userStatuses</span></span>|<span data-ttu-id="62b78-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-234">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="62b78-235">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="62b78-235">Device configuration installation status by user.</span></span> <span data-ttu-id="62b78-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62b78-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-237">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="62b78-237">deviceStatusOverview</span></span>|[<span data-ttu-id="62b78-238">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="62b78-238">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="62b78-239">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="62b78-239">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-240">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="62b78-240">userStatusOverview</span></span>|[<span data-ttu-id="62b78-241">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="62b78-241">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="62b78-242">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="62b78-242">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62b78-243">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="62b78-243">deviceSettingStateSummaries</span></span>|<span data-ttu-id="62b78-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62b78-244">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="62b78-245">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="62b78-245">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62b78-246">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62b78-246">JSON Representation</span></span>
<span data-ttu-id="62b78-247">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62b78-247">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```





