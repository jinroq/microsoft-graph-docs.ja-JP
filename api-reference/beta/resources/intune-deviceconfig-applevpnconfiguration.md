---
title: りんご Evpnconfiguration リソースの種類
description: Apple VPN 構成プロファイル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 57f3e7416dc984cf39b67638557aecf5a92a48a7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987678"
---
# <a name="applevpnconfiguration-resource-type"></a><span data-ttu-id="a218f-103">りんご Evpnconfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a218f-103">appleVpnConfiguration resource type</span></span>

> <span data-ttu-id="a218f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a218f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a218f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a218f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a218f-106">Apple VPN 構成プロファイル。</span><span class="sxs-lookup"><span data-stu-id="a218f-106">Apple VPN configuration profile.</span></span>


<span data-ttu-id="a218f-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a218f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a218f-108">Methods</span></span>
|<span data-ttu-id="a218f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a218f-109">Method</span></span>|<span data-ttu-id="a218f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a218f-110">Return Type</span></span>|<span data-ttu-id="a218f-111">説明</span><span class="sxs-lookup"><span data-stu-id="a218f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a218f-112">りんごの構成を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a218f-112">List appleVpnConfigurations</span></span>](../api/intune-deviceconfig-applevpnconfiguration-list.md)|<span data-ttu-id="a218f-113">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-113">[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) collection</span></span>|<span data-ttu-id="a218f-114">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a218f-114">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a218f-115">作業環境の設定を取得する</span><span class="sxs-lookup"><span data-stu-id="a218f-115">Get appleVpnConfiguration</span></span>](../api/intune-deviceconfig-applevpnconfiguration-get.md)|[<span data-ttu-id="a218f-116">appleVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a218f-116">appleVpnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnconfiguration.md)|<span data-ttu-id="a218f-117">[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a218f-117">Read properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a218f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a218f-118">Properties</span></span>
|<span data-ttu-id="a218f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a218f-119">Property</span></span>|<span data-ttu-id="a218f-120">型</span><span class="sxs-lookup"><span data-stu-id="a218f-120">Type</span></span>|<span data-ttu-id="a218f-121">説明</span><span class="sxs-lookup"><span data-stu-id="a218f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a218f-122">id</span><span class="sxs-lookup"><span data-stu-id="a218f-122">id</span></span>|<span data-ttu-id="a218f-123">文字列</span><span class="sxs-lookup"><span data-stu-id="a218f-123">String</span></span>|<span data-ttu-id="a218f-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a218f-124">Key of the entity.</span></span> <span data-ttu-id="a218f-125">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-125">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a218f-126">lastModifiedDateTime</span></span>|<span data-ttu-id="a218f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a218f-127">DateTimeOffset</span></span>|<span data-ttu-id="a218f-128">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a218f-128">DateTime the object was last modified.</span></span> <span data-ttu-id="a218f-129">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-129">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a218f-130">roleScopeTagIds</span></span>|<span data-ttu-id="a218f-131">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-131">String collection</span></span>|<span data-ttu-id="a218f-132">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a218f-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a218f-133">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-133">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a218f-134">supportsScopeTags</span></span>|<span data-ttu-id="a218f-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a218f-135">Boolean</span></span>|<span data-ttu-id="a218f-136">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a218f-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a218f-137">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a218f-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a218f-138">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a218f-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a218f-139">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a218f-139">This property is read-only.</span></span> <span data-ttu-id="a218f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a218f-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a218f-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a218f-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a218f-143">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="a218f-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a218f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a218f-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a218f-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a218f-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a218f-147">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a218f-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a218f-148">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-148">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-149">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a218f-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a218f-150">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="a218f-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a218f-151">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="a218f-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a218f-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a218f-153">createdDateTime</span></span>|<span data-ttu-id="a218f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a218f-154">DateTimeOffset</span></span>|<span data-ttu-id="a218f-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a218f-155">DateTime the object was created.</span></span> <span data-ttu-id="a218f-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-157">description</span><span class="sxs-lookup"><span data-stu-id="a218f-157">description</span></span>|<span data-ttu-id="a218f-158">String</span><span class="sxs-lookup"><span data-stu-id="a218f-158">String</span></span>|<span data-ttu-id="a218f-159">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a218f-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a218f-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-161">displayName</span><span class="sxs-lookup"><span data-stu-id="a218f-161">displayName</span></span>|<span data-ttu-id="a218f-162">String</span><span class="sxs-lookup"><span data-stu-id="a218f-162">String</span></span>|<span data-ttu-id="a218f-163">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a218f-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a218f-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-165">version</span><span class="sxs-lookup"><span data-stu-id="a218f-165">version</span></span>|<span data-ttu-id="a218f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a218f-166">Int32</span></span>|<span data-ttu-id="a218f-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a218f-167">Version of the device configuration.</span></span> <span data-ttu-id="a218f-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="a218f-169">connectionName</span></span>|<span data-ttu-id="a218f-170">String</span><span class="sxs-lookup"><span data-stu-id="a218f-170">String</span></span>|<span data-ttu-id="a218f-171">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="a218f-171">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="a218f-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="a218f-172">connectionType</span></span>|[<span data-ttu-id="a218f-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a218f-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="a218f-174">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="a218f-174">Connection type.</span></span> <span data-ttu-id="a218f-175">可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="a218f-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="a218f-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="a218f-176">loginGroupOrDomain</span></span>|<span data-ttu-id="a218f-177">String</span><span class="sxs-lookup"><span data-stu-id="a218f-177">String</span></span>|<span data-ttu-id="a218f-178">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="a218f-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a218f-179">role</span><span class="sxs-lookup"><span data-stu-id="a218f-179">role</span></span>|<span data-ttu-id="a218f-180">String</span><span class="sxs-lookup"><span data-stu-id="a218f-180">String</span></span>|<span data-ttu-id="a218f-181">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="a218f-181">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="a218f-182">領域</span><span class="sxs-lookup"><span data-stu-id="a218f-182">realm</span></span>|<span data-ttu-id="a218f-183">String</span><span class="sxs-lookup"><span data-stu-id="a218f-183">String</span></span>|<span data-ttu-id="a218f-184">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="a218f-184">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="a218f-185">server</span><span class="sxs-lookup"><span data-stu-id="a218f-185">server</span></span>|[<span data-ttu-id="a218f-186">vpnServer</span><span class="sxs-lookup"><span data-stu-id="a218f-186">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="a218f-187">ネットワーク上の VPN サーバー。</span><span class="sxs-lookup"><span data-stu-id="a218f-187">VPN Server on the network.</span></span> <span data-ttu-id="a218f-188">エンドユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a218f-188">Make sure end users can access this network location.</span></span>|
|<span data-ttu-id="a218f-189">識別子</span><span class="sxs-lookup"><span data-stu-id="a218f-189">identifier</span></span>|<span data-ttu-id="a218f-190">String</span><span class="sxs-lookup"><span data-stu-id="a218f-190">String</span></span>|<span data-ttu-id="a218f-191">接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。</span><span class="sxs-lookup"><span data-stu-id="a218f-191">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a218f-192">例: Cisco AnyConnect は、という形式の識別子を使用しています。</span><span class="sxs-lookup"><span data-stu-id="a218f-192">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin</span></span>|
|<span data-ttu-id="a218f-193">customData</span><span class="sxs-lookup"><span data-stu-id="a218f-193">customData</span></span>|<span data-ttu-id="a218f-194">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-194">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="a218f-195">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="a218f-195">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a218f-196">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a218f-196">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a218f-197">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="a218f-197">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a218f-198">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a218f-198">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="a218f-199">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="a218f-199">customKeyValueData</span></span>|<span data-ttu-id="a218f-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-200">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a218f-201">カスタムデータ接続の種類がカスタム VPN に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="a218f-201">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a218f-202">このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a218f-202">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a218f-203">これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="a218f-203">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a218f-204">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a218f-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="a218f-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a218f-205">enableSplitTunneling</span></span>|<span data-ttu-id="a218f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a218f-206">Boolean</span></span>|<span data-ttu-id="a218f-207">すべてのネットワークトラフィックを VPN 経由で送信します。</span><span class="sxs-lookup"><span data-stu-id="a218f-207">Send all network traffic through VPN.</span></span>|
|<span data-ttu-id="a218f-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a218f-208">authenticationMethod</span></span>|[<span data-ttu-id="a218f-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a218f-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="a218f-210">この VPN 接続の認証方法。</span><span class="sxs-lookup"><span data-stu-id="a218f-210">Authentication method for this VPN connection.</span></span> <span data-ttu-id="a218f-211">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="a218f-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a218f-212">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="a218f-212">enablePerApp</span></span>|<span data-ttu-id="a218f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a218f-213">Boolean</span></span>|<span data-ttu-id="a218f-214">この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。</span><span class="sxs-lookup"><span data-stu-id="a218f-214">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span>|
|<span data-ttu-id="a218f-215">Saf Aridomains</span><span class="sxs-lookup"><span data-stu-id="a218f-215">safariDomains</span></span>|<span data-ttu-id="a218f-216">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-216">String collection</span></span>|<span data-ttu-id="a218f-217">この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン</span><span class="sxs-lookup"><span data-stu-id="a218f-217">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="a218f-218">この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="a218f-218">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span>|
|<span data-ttu-id="a218f-219">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="a218f-219">onDemandRules</span></span>|<span data-ttu-id="a218f-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-220">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="a218f-221">オンデマンドルール。</span><span class="sxs-lookup"><span data-stu-id="a218f-221">On-Demand Rules.</span></span> <span data-ttu-id="a218f-222">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a218f-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a218f-223">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a218f-223">proxyServer</span></span>|[<span data-ttu-id="a218f-224">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a218f-224">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="a218f-225">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="a218f-225">Proxy Server.</span></span>|
|<span data-ttu-id="a218f-226">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="a218f-226">optInToDeviceIdSharing</span></span>|<span data-ttu-id="a218f-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="a218f-227">Boolean</span></span>|<span data-ttu-id="a218f-228">ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。</span><span class="sxs-lookup"><span data-stu-id="a218f-228">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a218f-229">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a218f-229">Relationships</span></span>
|<span data-ttu-id="a218f-230">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a218f-230">Relationship</span></span>|<span data-ttu-id="a218f-231">型</span><span class="sxs-lookup"><span data-stu-id="a218f-231">Type</span></span>|<span data-ttu-id="a218f-232">説明</span><span class="sxs-lookup"><span data-stu-id="a218f-232">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a218f-233">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a218f-233">groupAssignments</span></span>|<span data-ttu-id="a218f-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a218f-235">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a218f-235">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a218f-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-237">assignments</span><span class="sxs-lookup"><span data-stu-id="a218f-237">assignments</span></span>|<span data-ttu-id="a218f-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a218f-239">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a218f-239">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a218f-240">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-241">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a218f-241">deviceStatuses</span></span>|<span data-ttu-id="a218f-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a218f-243">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="a218f-243">Device configuration installation status by device.</span></span> <span data-ttu-id="a218f-244">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-244">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-245">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a218f-245">userStatuses</span></span>|<span data-ttu-id="a218f-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a218f-247">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="a218f-247">Device configuration installation status by user.</span></span> <span data-ttu-id="a218f-248">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a218f-248">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-249">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a218f-249">deviceStatusOverview</span></span>|[<span data-ttu-id="a218f-250">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a218f-250">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a218f-251">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a218f-251">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-252">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a218f-252">userStatusOverview</span></span>|[<span data-ttu-id="a218f-253">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a218f-253">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a218f-254">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a218f-254">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a218f-255">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a218f-255">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a218f-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a218f-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a218f-257">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a218f-257">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a218f-258">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a218f-258">JSON Representation</span></span>
<span data-ttu-id="a218f-259">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a218f-259">Here is a JSON representation of the resource.</span></span>
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





