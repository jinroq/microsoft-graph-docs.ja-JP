---
title: windows10VpnConfiguration リソースの種類
description: このプロファイルに構成を指定することで、Windows 10 デバイス (デスクトップまたはモバイル) に対して、目的の VPN エンドポイントに接続するように指示することができます。 VPN エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに VPN 接続を確立できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9426ec065449d4cdd68da876977196a1fe5b44c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982120"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="393b1-104">windows10VpnConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="393b1-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="393b1-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="393b1-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="393b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="393b1-107">このプロファイルに構成を指定することで、Windows 10 デバイス (デスクトップまたはモバイル) に対して、目的の VPN エンドポイントに接続するように指示することができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="393b1-108">VPN エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに VPN 接続を確立できます。</span><span class="sxs-lookup"><span data-stu-id="393b1-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="393b1-109">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="393b1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="393b1-110">Methods</span></span>
|<span data-ttu-id="393b1-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="393b1-111">Method</span></span>|<span data-ttu-id="393b1-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="393b1-112">Return Type</span></span>|<span data-ttu-id="393b1-113">説明</span><span class="sxs-lookup"><span data-stu-id="393b1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="393b1-114">リスト windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="393b1-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="393b1-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="393b1-116">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="393b1-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="393b1-117">Windows10VpnConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="393b1-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="393b1-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="393b1-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="393b1-119">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="393b1-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="393b1-120">Windows10VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="393b1-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="393b1-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="393b1-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="393b1-122">新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="393b1-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="393b1-123">Windows10VpnConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="393b1-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="393b1-124">None</span><span class="sxs-lookup"><span data-stu-id="393b1-124">None</span></span>|<span data-ttu-id="393b1-125">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="393b1-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="393b1-126">Windows10VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="393b1-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="393b1-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="393b1-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="393b1-128">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="393b1-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="393b1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="393b1-129">Properties</span></span>
|<span data-ttu-id="393b1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="393b1-130">Property</span></span>|<span data-ttu-id="393b1-131">型</span><span class="sxs-lookup"><span data-stu-id="393b1-131">Type</span></span>|<span data-ttu-id="393b1-132">説明</span><span class="sxs-lookup"><span data-stu-id="393b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393b1-133">id</span><span class="sxs-lookup"><span data-stu-id="393b1-133">id</span></span>|<span data-ttu-id="393b1-134">文字列</span><span class="sxs-lookup"><span data-stu-id="393b1-134">String</span></span>|<span data-ttu-id="393b1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="393b1-135">Key of the entity.</span></span> <span data-ttu-id="393b1-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="393b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="393b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="393b1-138">DateTimeOffset</span></span>|<span data-ttu-id="393b1-139">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="393b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="393b1-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="393b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="393b1-142">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-142">String collection</span></span>|<span data-ttu-id="393b1-143">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="393b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="393b1-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="393b1-145">supportsScopeTags</span></span>|<span data-ttu-id="393b1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-146">Boolean</span></span>|<span data-ttu-id="393b1-147">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="393b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="393b1-148">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="393b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="393b1-149">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="393b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="393b1-150">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="393b1-150">This property is read-only.</span></span> <span data-ttu-id="393b1-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="393b1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="393b1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="393b1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="393b1-154">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="393b1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="393b1-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="393b1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="393b1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="393b1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="393b1-158">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="393b1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="393b1-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="393b1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="393b1-161">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="393b1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="393b1-162">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="393b1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="393b1-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="393b1-164">createdDateTime</span></span>|<span data-ttu-id="393b1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="393b1-165">DateTimeOffset</span></span>|<span data-ttu-id="393b1-166">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="393b1-166">DateTime the object was created.</span></span> <span data-ttu-id="393b1-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-168">description</span><span class="sxs-lookup"><span data-stu-id="393b1-168">description</span></span>|<span data-ttu-id="393b1-169">String</span><span class="sxs-lookup"><span data-stu-id="393b1-169">String</span></span>|<span data-ttu-id="393b1-170">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="393b1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="393b1-171">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-171">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="393b1-172">displayName</span></span>|<span data-ttu-id="393b1-173">String</span><span class="sxs-lookup"><span data-stu-id="393b1-173">String</span></span>|<span data-ttu-id="393b1-174">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="393b1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="393b1-175">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-175">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-176">version</span><span class="sxs-lookup"><span data-stu-id="393b1-176">version</span></span>|<span data-ttu-id="393b1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="393b1-177">Int32</span></span>|<span data-ttu-id="393b1-178">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="393b1-178">Version of the device configuration.</span></span> <span data-ttu-id="393b1-179">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="393b1-180">connectionName</span></span>|<span data-ttu-id="393b1-181">String</span><span class="sxs-lookup"><span data-stu-id="393b1-181">String</span></span>|<span data-ttu-id="393b1-182">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="393b1-182">Connection name displayed to the user.</span></span> <span data-ttu-id="393b1-183">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-184">サーバ</span><span class="sxs-lookup"><span data-stu-id="393b1-184">servers</span></span>|<span data-ttu-id="393b1-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="393b1-186">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="393b1-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="393b1-187">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="393b1-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="393b1-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="393b1-189">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-190">customXml</span><span class="sxs-lookup"><span data-stu-id="393b1-190">customXml</span></span>|<span data-ttu-id="393b1-191">Binary</span><span class="sxs-lookup"><span data-stu-id="393b1-191">Binary</span></span>|<span data-ttu-id="393b1-192">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="393b1-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="393b1-193">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="393b1-194">profileTarget</span></span>|[<span data-ttu-id="393b1-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="393b1-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="393b1-196">プロファイルのターゲットの種類。</span><span class="sxs-lookup"><span data-stu-id="393b1-196">Profile target type.</span></span> <span data-ttu-id="393b1-197">可能な値は、`user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="393b1-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="393b1-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="393b1-198">connectionType</span></span>|[<span data-ttu-id="393b1-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="393b1-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="393b1-200">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="393b1-200">Connection type.</span></span> <span data-ttu-id="393b1-201">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="393b1-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="393b1-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="393b1-202">enableSplitTunneling</span></span>|<span data-ttu-id="393b1-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-203">Boolean</span></span>|<span data-ttu-id="393b1-204">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="393b1-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="393b1-205">enableAlwaysOn</span></span>|<span data-ttu-id="393b1-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-206">Boolean</span></span>|<span data-ttu-id="393b1-207">Always On モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="393b1-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="393b1-208">enableDeviceTunnel</span></span>|<span data-ttu-id="393b1-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-209">Boolean</span></span>|<span data-ttu-id="393b1-210">デバイストンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="393b1-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="393b1-211">enableDnsRegistration</span></span>|<span data-ttu-id="393b1-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-212">Boolean</span></span>|<span data-ttu-id="393b1-213">内部 DNS での IP アドレス登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="393b1-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="393b1-214">dnsSuffixes</span></span>|<span data-ttu-id="393b1-215">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-215">String collection</span></span>|<span data-ttu-id="393b1-216">DNS の検索一覧に追加する DNS サフィックスを指定して、短い名前を適切にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="393b1-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="393b1-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="393b1-217">authenticationMethod</span></span>|[<span data-ttu-id="393b1-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="393b1-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="393b1-219">認証方法。</span><span class="sxs-lookup"><span data-stu-id="393b1-219">Authentication method.</span></span> <span data-ttu-id="393b1-220">可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="393b1-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="393b1-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="393b1-221">rememberUserCredentials</span></span>|<span data-ttu-id="393b1-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-222">Boolean</span></span>|<span data-ttu-id="393b1-223">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="393b1-223">Remember user credentials.</span></span>|
|<span data-ttu-id="393b1-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="393b1-224">enableConditionalAccess</span></span>|<span data-ttu-id="393b1-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-225">Boolean</span></span>|<span data-ttu-id="393b1-226">条件付きアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-226">Enable conditional access.</span></span>|
|<span data-ttu-id="393b1-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="393b1-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="393b1-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-228">Boolean</span></span>|<span data-ttu-id="393b1-229">代替証明書を使用してシングルサインオン (SSO) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="393b1-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="393b1-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="393b1-230">singleSignOnEku</span></span>|[<span data-ttu-id="393b1-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="393b1-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="393b1-232">シングルサインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="393b1-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="393b1-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="393b1-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="393b1-234">String</span><span class="sxs-lookup"><span data-stu-id="393b1-234">String</span></span>|<span data-ttu-id="393b1-235">シングルサインオン発行者ハッシュ。</span><span class="sxs-lookup"><span data-stu-id="393b1-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="393b1-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="393b1-236">eapXml</span></span>|<span data-ttu-id="393b1-237">Binary</span><span class="sxs-lookup"><span data-stu-id="393b1-237">Binary</span></span>|<span data-ttu-id="393b1-238">拡張認証プロトコル (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="393b1-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="393b1-239">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="393b1-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="393b1-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="393b1-240">proxyServer</span></span>|[<span data-ttu-id="393b1-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="393b1-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="393b1-242">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="393b1-242">Proxy Server.</span></span>|
|<span data-ttu-id="393b1-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="393b1-243">associatedApps</span></span>|<span data-ttu-id="393b1-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="393b1-245">関連付けられているアプリ。</span><span class="sxs-lookup"><span data-stu-id="393b1-245">Associated Apps.</span></span> <span data-ttu-id="393b1-246">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="393b1-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="393b1-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="393b1-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="393b1-248">Boolean</span></span>|<span data-ttu-id="393b1-249">関連付けられているアプリのみが接続 (アプリごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="393b1-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="393b1-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="393b1-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="393b1-251">String</span><span class="sxs-lookup"><span data-stu-id="393b1-251">String</span></span>|<span data-ttu-id="393b1-252">この接続に関連付ける Windows Information Protection (WIP) ドメイン。</span><span class="sxs-lookup"><span data-stu-id="393b1-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="393b1-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="393b1-253">trafficRules</span></span>|<span data-ttu-id="393b1-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="393b1-255">トラフィックルール。</span><span class="sxs-lookup"><span data-stu-id="393b1-255">Traffic rules.</span></span> <span data-ttu-id="393b1-256">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="393b1-257">返信</span><span class="sxs-lookup"><span data-stu-id="393b1-257">routes</span></span>|<span data-ttu-id="393b1-258">[Vpnroute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="393b1-259">ルート (サードパーティプロバイダーの場合はオプション)。</span><span class="sxs-lookup"><span data-stu-id="393b1-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="393b1-260">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="393b1-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="393b1-261">dnsRules</span></span>|<span data-ttu-id="393b1-262">[Vpndnsrule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="393b1-263">DNS ルール。</span><span class="sxs-lookup"><span data-stu-id="393b1-263">DNS rules.</span></span> <span data-ttu-id="393b1-264">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="393b1-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="393b1-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="393b1-265">trustedNetworkDomains</span></span>|<span data-ttu-id="393b1-266">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-266">String collection</span></span>|<span data-ttu-id="393b1-267">信頼されたネットワークドメイン</span><span class="sxs-lookup"><span data-stu-id="393b1-267">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="393b1-268">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="393b1-268">Relationships</span></span>
|<span data-ttu-id="393b1-269">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="393b1-269">Relationship</span></span>|<span data-ttu-id="393b1-270">型</span><span class="sxs-lookup"><span data-stu-id="393b1-270">Type</span></span>|<span data-ttu-id="393b1-271">説明</span><span class="sxs-lookup"><span data-stu-id="393b1-271">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393b1-272">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="393b1-272">groupAssignments</span></span>|<span data-ttu-id="393b1-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="393b1-274">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="393b1-274">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="393b1-275">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-276">assignments</span><span class="sxs-lookup"><span data-stu-id="393b1-276">assignments</span></span>|<span data-ttu-id="393b1-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="393b1-278">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="393b1-278">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="393b1-279">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-279">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-280">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="393b1-280">deviceStatuses</span></span>|<span data-ttu-id="393b1-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="393b1-282">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="393b1-282">Device configuration installation status by device.</span></span> <span data-ttu-id="393b1-283">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-283">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-284">userStatuses</span><span class="sxs-lookup"><span data-stu-id="393b1-284">userStatuses</span></span>|<span data-ttu-id="393b1-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="393b1-286">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="393b1-286">Device configuration installation status by user.</span></span> <span data-ttu-id="393b1-287">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="393b1-287">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-288">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="393b1-288">deviceStatusOverview</span></span>|[<span data-ttu-id="393b1-289">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="393b1-289">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="393b1-290">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="393b1-290">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-291">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="393b1-291">userStatusOverview</span></span>|[<span data-ttu-id="393b1-292">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="393b1-292">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="393b1-293">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="393b1-293">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-294">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="393b1-294">deviceSettingStateSummaries</span></span>|<span data-ttu-id="393b1-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="393b1-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="393b1-296">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="393b1-296">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="393b1-297">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="393b1-297">identityCertificate</span></span>|[<span data-ttu-id="393b1-298">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="393b1-298">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="393b1-299">認証方法が証明書の場合にクライアント認証を行うための id 証明書。</span><span class="sxs-lookup"><span data-stu-id="393b1-299">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="393b1-300">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="393b1-300">JSON Representation</span></span>
<span data-ttu-id="393b1-301">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="393b1-301">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ]
}
```





