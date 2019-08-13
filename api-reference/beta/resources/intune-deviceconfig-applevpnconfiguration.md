---
title: りんご Evpnconfiguration リソースの種類
description: Apple VPN 構成プロファイル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af50edfb0c098ed2fffabb7b736d8e0ab4dcb871
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333983"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="39707-103">りんご Evpnconfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39707-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="39707-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39707-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39707-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39707-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39707-106">Apple VPN 構成プロファイル。</span><span class="sxs-lookup"><span data-stu-id="39707-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="39707-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="39707-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="39707-108">Methods</span></span>
|<span data-ttu-id="39707-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="39707-109">Method</span></span>|<span data-ttu-id="39707-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39707-110">Return Type</span></span>|<span data-ttu-id="39707-111">説明</span><span class="sxs-lookup"><span data-stu-id="39707-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39707-112">りんごの構成を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="39707-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="39707-113">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="39707-114">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="39707-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="39707-115">作業環境の設定を取得する</span><span class="sxs-lookup"><span data-stu-id="39707-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="39707-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="39707-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="39707-117">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="39707-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39707-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39707-118">Properties</span></span>
|<span data-ttu-id="39707-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39707-119">Property</span></span>|<span data-ttu-id="39707-120">型</span><span class="sxs-lookup"><span data-stu-id="39707-120">Type</span></span>|<span data-ttu-id="39707-121">説明</span><span class="sxs-lookup"><span data-stu-id="39707-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39707-122">id</span><span class="sxs-lookup"><span data-stu-id="39707-122">id</span></span>|<span data-ttu-id="39707-123">文字列</span><span class="sxs-lookup"><span data-stu-id="39707-123">String</span></span>|<span data-ttu-id="39707-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="39707-124">Key of the entity.</span></span> <span data-ttu-id="39707-125">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39707-126">lastModifiedDateTime</span></span>|<span data-ttu-id="39707-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39707-127">DateTimeOffset</span></span>|<span data-ttu-id="39707-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="39707-128">DateTime the object was last modified.</span></span> <span data-ttu-id="39707-129">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39707-130">roleScopeTagIds</span></span>|<span data-ttu-id="39707-131">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-131">String collection</span></span>|<span data-ttu-id="39707-132">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="39707-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39707-133">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39707-134">supportsScopeTags</span></span>|<span data-ttu-id="39707-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="39707-135">Boolean</span></span>|<span data-ttu-id="39707-136">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="39707-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39707-137">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="39707-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39707-138">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="39707-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39707-139">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="39707-139">This property is read-only.</span></span> <span data-ttu-id="39707-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="39707-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="39707-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="39707-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="39707-143">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="39707-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="39707-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="39707-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="39707-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="39707-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="39707-147">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="39707-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="39707-148">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-149">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="39707-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="39707-150">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="39707-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="39707-151">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="39707-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="39707-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39707-153">createdDateTime</span></span>|<span data-ttu-id="39707-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39707-154">DateTimeOffset</span></span>|<span data-ttu-id="39707-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="39707-155">DateTime the object was created.</span></span> <span data-ttu-id="39707-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-157">description</span><span class="sxs-lookup"><span data-stu-id="39707-157">description</span></span>|<span data-ttu-id="39707-158">String</span><span class="sxs-lookup"><span data-stu-id="39707-158">String</span></span>|<span data-ttu-id="39707-159">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="39707-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39707-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-161">displayName</span><span class="sxs-lookup"><span data-stu-id="39707-161">displayName</span></span>|<span data-ttu-id="39707-162">String</span><span class="sxs-lookup"><span data-stu-id="39707-162">String</span></span>|<span data-ttu-id="39707-163">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="39707-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39707-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-165">version</span><span class="sxs-lookup"><span data-stu-id="39707-165">version</span></span>|<span data-ttu-id="39707-166">Int32</span><span class="sxs-lookup"><span data-stu-id="39707-166">Int32</span></span>|<span data-ttu-id="39707-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="39707-167">Version of the device configuration.</span></span> <span data-ttu-id="39707-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="39707-169">connectionName</span></span>|<span data-ttu-id="39707-170">String</span><span class="sxs-lookup"><span data-stu-id="39707-170">String</span></span>|<span data-ttu-id="39707-171">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="39707-171">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="39707-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="39707-172">connectionType</span></span>|[<span data-ttu-id="39707-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="39707-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="39707-174">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="39707-174">Connection type.</span></span> <span data-ttu-id="39707-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="39707-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="39707-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="39707-176">loginGroupOrDomain</span></span>|<span data-ttu-id="39707-177">String</span><span class="sxs-lookup"><span data-stu-id="39707-177">String</span></span>|<span data-ttu-id="39707-178">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="39707-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="39707-179">role</span><span class="sxs-lookup"><span data-stu-id="39707-179">role</span></span>|<span data-ttu-id="39707-180">String</span><span class="sxs-lookup"><span data-stu-id="39707-180">String</span></span>|<span data-ttu-id="39707-181">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="39707-181">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="39707-182">領域</span><span class="sxs-lookup"><span data-stu-id="39707-182">realm</span></span>|<span data-ttu-id="39707-183">String</span><span class="sxs-lookup"><span data-stu-id="39707-183">String</span></span>|<span data-ttu-id="39707-184">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="39707-184">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="39707-185">server</span><span class="sxs-lookup"><span data-stu-id="39707-185">server</span></span>|[<span data-ttu-id="39707-186">vpnServer</span><span class="sxs-lookup"><span data-stu-id="39707-186">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="39707-187">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="39707-187">VPN Server on the network.</span></span> <span data-ttu-id="39707-188">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="39707-188">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="39707-189">識別子</span><span class="sxs-lookup"><span data-stu-id="39707-189">identifier</span></span>|<span data-ttu-id="39707-190">String</span><span class="sxs-lookup"><span data-stu-id="39707-190">String</span></span>|<span data-ttu-id="39707-191">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="39707-191">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="39707-192">例: Cisco AnyConnect は、という形式の識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="39707-192">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="39707-193">customData</span><span class="sxs-lookup"><span data-stu-id="39707-193">customData</span></span>|<span data-ttu-id="39707-194">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="39707-195">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="39707-195">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="39707-196">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="39707-196">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="39707-197">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="39707-197">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="39707-198">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39707-198">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="39707-199">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="39707-199">customKeyValueData</span></span>|<span data-ttu-id="39707-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="39707-201">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="39707-201">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="39707-202">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="39707-202">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="39707-203">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="39707-203">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="39707-204">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39707-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="39707-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="39707-205">enableSplitTunneling</span></span>|<span data-ttu-id="39707-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="39707-206">Boolean</span></span>|<span data-ttu-id="39707-207">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="39707-207">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="39707-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="39707-208">authenticationMethod</span></span>|[<span data-ttu-id="39707-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="39707-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="39707-210">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="39707-210">Authentication method for this VPN connection.</span></span> <span data-ttu-id="39707-211">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="39707-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="39707-212">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="39707-212">enablePerApp</span></span>|<span data-ttu-id="39707-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="39707-213">Boolean</span></span>|<span data-ttu-id="39707-214">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="39707-214">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="39707-215">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="39707-215">safariDomains</span></span>|<span data-ttu-id="39707-216">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-216">String collection</span></span>|<span data-ttu-id="39707-217">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="39707-217">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="39707-218">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="39707-218">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="39707-219">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="39707-219">onDemandRules</span></span>|<span data-ttu-id="39707-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="39707-221">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="39707-221">On-Demand Rules.</span></span> <span data-ttu-id="39707-222">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39707-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39707-223">proxyServer</span><span class="sxs-lookup"><span data-stu-id="39707-223">proxyServer</span></span>|[<span data-ttu-id="39707-224">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="39707-224">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="39707-225">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="39707-225">Proxy Server.</span></span>|
|<span data-ttu-id="39707-226">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="39707-226">optInToDeviceIdSharing</span></span>|<span data-ttu-id="39707-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="39707-227">Boolean</span></span>|<span data-ttu-id="39707-228">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="39707-228">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39707-229">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39707-229">Relationships</span></span>
|<span data-ttu-id="39707-230">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39707-230">Relationship</span></span>|<span data-ttu-id="39707-231">型</span><span class="sxs-lookup"><span data-stu-id="39707-231">Type</span></span>|<span data-ttu-id="39707-232">説明</span><span class="sxs-lookup"><span data-stu-id="39707-232">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39707-233">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="39707-233">groupAssignments</span></span>|<span data-ttu-id="39707-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="39707-235">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="39707-235">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="39707-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-237">assignments</span><span class="sxs-lookup"><span data-stu-id="39707-237">assignments</span></span>|<span data-ttu-id="39707-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="39707-239">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="39707-239">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="39707-240">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-241">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="39707-241">deviceStatuses</span></span>|<span data-ttu-id="39707-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="39707-243">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="39707-243">Device configuration installation status by device.</span></span> <span data-ttu-id="39707-244">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-244">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-245">userStatuses</span><span class="sxs-lookup"><span data-stu-id="39707-245">userStatuses</span></span>|<span data-ttu-id="39707-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="39707-247">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="39707-247">Device configuration installation status by user.</span></span> <span data-ttu-id="39707-248">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39707-248">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-249">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="39707-249">deviceStatusOverview</span></span>|[<span data-ttu-id="39707-250">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="39707-250">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="39707-251">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="39707-251">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-252">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="39707-252">userStatusOverview</span></span>|[<span data-ttu-id="39707-253">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="39707-253">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="39707-254">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="39707-254">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39707-255">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="39707-255">deviceSettingStateSummaries</span></span>|<span data-ttu-id="39707-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39707-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="39707-257">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="39707-257">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39707-258">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39707-258">JSON Representation</span></span>
<span data-ttu-id="39707-259">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39707-259">Here is a JSON representation of the resource.</span></span>
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
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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



