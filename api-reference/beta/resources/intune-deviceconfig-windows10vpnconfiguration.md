---
title: windows10VpnConfiguration リソースの種類
description: このプロファイルに構成を指定することで、Windows 10 デバイス (デスクトップまたはモバイル) に対して、目的の VPN エンドポイントに接続するように指示することができます。 vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b1b906fc4a98895acc6e23a4b3e9a4d78ff28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148714"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="a7ede-104">windows10VpnConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7ede-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="a7ede-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ede-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7ede-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7ede-107">このプロファイルに構成を指定することで、Windows 10 デバイス (デスクトップまたはモバイル) に対して、目的の VPN エンドポイントに接続するように指示することができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="a7ede-108">vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="a7ede-109">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a7ede-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7ede-110">Methods</span></span>
|<span data-ttu-id="a7ede-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7ede-111">Method</span></span>|<span data-ttu-id="a7ede-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7ede-112">Return Type</span></span>|<span data-ttu-id="a7ede-113">説明</span><span class="sxs-lookup"><span data-stu-id="a7ede-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7ede-114">リスト windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="a7ede-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="a7ede-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="a7ede-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a7ede-117">windows10VpnConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="a7ede-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="a7ede-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7ede-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a7ede-119">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7ede-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a7ede-120">windows10VpnConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="a7ede-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="a7ede-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7ede-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a7ede-122">新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a7ede-123">windows10VpnConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="a7ede-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="a7ede-124">なし</span><span class="sxs-lookup"><span data-stu-id="a7ede-124">None</span></span>|<span data-ttu-id="a7ede-125">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="a7ede-126">windows10VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a7ede-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="a7ede-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7ede-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a7ede-128">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7ede-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7ede-129">Properties</span></span>
|<span data-ttu-id="a7ede-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7ede-130">Property</span></span>|<span data-ttu-id="a7ede-131">型</span><span class="sxs-lookup"><span data-stu-id="a7ede-131">Type</span></span>|<span data-ttu-id="a7ede-132">説明</span><span class="sxs-lookup"><span data-stu-id="a7ede-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ede-133">id</span><span class="sxs-lookup"><span data-stu-id="a7ede-133">id</span></span>|<span data-ttu-id="a7ede-134">文字列</span><span class="sxs-lookup"><span data-stu-id="a7ede-134">String</span></span>|<span data-ttu-id="a7ede-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a7ede-135">Key of the entity.</span></span> <span data-ttu-id="a7ede-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7ede-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a7ede-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7ede-138">DateTimeOffset</span></span>|<span data-ttu-id="a7ede-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a7ede-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a7ede-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7ede-141">roleScopeTagIds</span></span>|<span data-ttu-id="a7ede-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-142">String collection</span></span>|<span data-ttu-id="a7ede-143">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a7ede-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7ede-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7ede-145">supportsScopeTags</span></span>|<span data-ttu-id="a7ede-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-146">Boolean</span></span>|<span data-ttu-id="a7ede-147">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7ede-148">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a7ede-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7ede-149">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7ede-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-150">This property is read-only.</span></span> <span data-ttu-id="a7ede-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7ede-152">createdDateTime</span></span>|<span data-ttu-id="a7ede-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7ede-153">DateTimeOffset</span></span>|<span data-ttu-id="a7ede-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a7ede-154">DateTime the object was created.</span></span> <span data-ttu-id="a7ede-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-156">説明</span><span class="sxs-lookup"><span data-stu-id="a7ede-156">description</span></span>|<span data-ttu-id="a7ede-157">String</span><span class="sxs-lookup"><span data-stu-id="a7ede-157">String</span></span>|<span data-ttu-id="a7ede-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a7ede-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7ede-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a7ede-160">displayName</span></span>|<span data-ttu-id="a7ede-161">String</span><span class="sxs-lookup"><span data-stu-id="a7ede-161">String</span></span>|<span data-ttu-id="a7ede-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a7ede-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7ede-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-164">version</span><span class="sxs-lookup"><span data-stu-id="a7ede-164">version</span></span>|<span data-ttu-id="a7ede-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a7ede-165">Int32</span></span>|<span data-ttu-id="a7ede-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a7ede-166">Version of the device configuration.</span></span> <span data-ttu-id="a7ede-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="a7ede-168">connectionName</span></span>|<span data-ttu-id="a7ede-169">String</span><span class="sxs-lookup"><span data-stu-id="a7ede-169">String</span></span>|<span data-ttu-id="a7ede-170">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="a7ede-170">Connection name displayed to the user.</span></span> <span data-ttu-id="a7ede-171">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-172">サーバー</span><span class="sxs-lookup"><span data-stu-id="a7ede-172">servers</span></span>|<span data-ttu-id="a7ede-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a7ede-174">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="a7ede-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="a7ede-175">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a7ede-176">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a7ede-177">[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-178">customXml</span><span class="sxs-lookup"><span data-stu-id="a7ede-178">customXml</span></span>|<span data-ttu-id="a7ede-179">Binary</span><span class="sxs-lookup"><span data-stu-id="a7ede-179">Binary</span></span>|<span data-ttu-id="a7ede-180">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="a7ede-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a7ede-181">(UTF8 でエンコードされたバイト配列)[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-182">profiletarget</span><span class="sxs-lookup"><span data-stu-id="a7ede-182">profileTarget</span></span>|[<span data-ttu-id="a7ede-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="a7ede-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="a7ede-184">プロファイルのターゲットの種類。</span><span class="sxs-lookup"><span data-stu-id="a7ede-184">Profile target type.</span></span> <span data-ttu-id="a7ede-185">可能な値は `user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="a7ede-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="a7ede-186">connectionType</span></span>|[<span data-ttu-id="a7ede-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a7ede-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="a7ede-188">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="a7ede-188">Connection type.</span></span> <span data-ttu-id="a7ede-189">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="a7ede-190">enablesplittunneling</span><span class="sxs-lookup"><span data-stu-id="a7ede-190">enableSplitTunneling</span></span>|<span data-ttu-id="a7ede-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-191">Boolean</span></span>|<span data-ttu-id="a7ede-192">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="a7ede-193">enablealwayson</span><span class="sxs-lookup"><span data-stu-id="a7ede-193">enableAlwaysOn</span></span>|<span data-ttu-id="a7ede-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-194">Boolean</span></span>|<span data-ttu-id="a7ede-195">Always On モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="a7ede-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="a7ede-196">enableDeviceTunnel</span></span>|<span data-ttu-id="a7ede-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-197">Boolean</span></span>|<span data-ttu-id="a7ede-198">デバイストンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="a7ede-199">enablednsregistration</span><span class="sxs-lookup"><span data-stu-id="a7ede-199">enableDnsRegistration</span></span>|<span data-ttu-id="a7ede-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-200">Boolean</span></span>|<span data-ttu-id="a7ede-201">内部 DNS での IP アドレス登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="a7ede-202">dnssuffixes</span><span class="sxs-lookup"><span data-stu-id="a7ede-202">dnsSuffixes</span></span>|<span data-ttu-id="a7ede-203">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-203">String collection</span></span>|<span data-ttu-id="a7ede-204">dns の検索一覧に追加する dns サフィックスを指定して、短い名前を適切にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="a7ede-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a7ede-205">authenticationMethod</span></span>|[<span data-ttu-id="a7ede-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a7ede-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="a7ede-207">認証方法。</span><span class="sxs-lookup"><span data-stu-id="a7ede-207">Authentication method.</span></span> <span data-ttu-id="a7ede-208">可能な値は `certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="a7ede-209">rememberusercredentials</span><span class="sxs-lookup"><span data-stu-id="a7ede-209">rememberUserCredentials</span></span>|<span data-ttu-id="a7ede-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-210">Boolean</span></span>|<span data-ttu-id="a7ede-211">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="a7ede-211">Remember user credentials.</span></span>|
|<span data-ttu-id="a7ede-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="a7ede-212">enableConditionalAccess</span></span>|<span data-ttu-id="a7ede-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-213">Boolean</span></span>|<span data-ttu-id="a7ede-214">条件付きアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-214">Enable conditional access.</span></span>|
|<span data-ttu-id="a7ede-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="a7ede-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="a7ede-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-216">Boolean</span></span>|<span data-ttu-id="a7ede-217">代替証明書を使用してシングルサインオン (SSO) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a7ede-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="a7ede-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="a7ede-218">singleSignOnEku</span></span>|[<span data-ttu-id="a7ede-219">extendedkeyusage</span><span class="sxs-lookup"><span data-stu-id="a7ede-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="a7ede-220">シングルサインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="a7ede-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="a7ede-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="a7ede-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="a7ede-222">String</span><span class="sxs-lookup"><span data-stu-id="a7ede-222">String</span></span>|<span data-ttu-id="a7ede-223">シングルサインオン発行者ハッシュ。</span><span class="sxs-lookup"><span data-stu-id="a7ede-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="a7ede-224">eapxml</span><span class="sxs-lookup"><span data-stu-id="a7ede-224">eapXml</span></span>|<span data-ttu-id="a7ede-225">Binary</span><span class="sxs-lookup"><span data-stu-id="a7ede-225">Binary</span></span>|<span data-ttu-id="a7ede-226">拡張認証プロトコル (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="a7ede-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="a7ede-227">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="a7ede-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="a7ede-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a7ede-228">proxyServer</span></span>|[<span data-ttu-id="a7ede-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a7ede-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="a7ede-230">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="a7ede-230">Proxy Server.</span></span>|
|<span data-ttu-id="a7ede-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="a7ede-231">associatedApps</span></span>|<span data-ttu-id="a7ede-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="a7ede-233">関連付けられているアプリ。</span><span class="sxs-lookup"><span data-stu-id="a7ede-233">Associated Apps.</span></span> <span data-ttu-id="a7ede-234">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a7ede-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="a7ede-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="a7ede-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ede-236">Boolean</span></span>|<span data-ttu-id="a7ede-237">関連付けられているアプリのみが接続 (アプリごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="a7ede-238">windowsinformationprotectiondomain</span><span class="sxs-lookup"><span data-stu-id="a7ede-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="a7ede-239">String</span><span class="sxs-lookup"><span data-stu-id="a7ede-239">String</span></span>|<span data-ttu-id="a7ede-240">この接続に関連付ける Windows Information Protection (WIP) ドメイン。</span><span class="sxs-lookup"><span data-stu-id="a7ede-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="a7ede-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="a7ede-241">trafficRules</span></span>|<span data-ttu-id="a7ede-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="a7ede-243">トラフィックルール。</span><span class="sxs-lookup"><span data-stu-id="a7ede-243">Traffic rules.</span></span> <span data-ttu-id="a7ede-244">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a7ede-245">返信</span><span class="sxs-lookup"><span data-stu-id="a7ede-245">routes</span></span>|<span data-ttu-id="a7ede-246">[vpnroute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="a7ede-247">ルート (サードパーティプロバイダーの場合はオプション)。</span><span class="sxs-lookup"><span data-stu-id="a7ede-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="a7ede-248">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a7ede-249">dnsrules</span><span class="sxs-lookup"><span data-stu-id="a7ede-249">dnsRules</span></span>|<span data-ttu-id="a7ede-250">[vpndnsrule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="a7ede-251">DNS ルール。</span><span class="sxs-lookup"><span data-stu-id="a7ede-251">DNS rules.</span></span> <span data-ttu-id="a7ede-252">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a7ede-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a7ede-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="a7ede-253">trustedNetworkDomains</span></span>|<span data-ttu-id="a7ede-254">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-254">String collection</span></span>|<span data-ttu-id="a7ede-255">信頼されたネットワークドメイン</span><span class="sxs-lookup"><span data-stu-id="a7ede-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7ede-256">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7ede-256">Relationships</span></span>
|<span data-ttu-id="a7ede-257">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7ede-257">Relationship</span></span>|<span data-ttu-id="a7ede-258">型</span><span class="sxs-lookup"><span data-stu-id="a7ede-258">Type</span></span>|<span data-ttu-id="a7ede-259">説明</span><span class="sxs-lookup"><span data-stu-id="a7ede-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ede-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a7ede-260">groupAssignments</span></span>|<span data-ttu-id="a7ede-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a7ede-262">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a7ede-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a7ede-263">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-264">assignments</span><span class="sxs-lookup"><span data-stu-id="a7ede-264">assignments</span></span>|<span data-ttu-id="a7ede-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a7ede-266">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a7ede-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a7ede-267">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a7ede-268">deviceStatuses</span></span>|<span data-ttu-id="a7ede-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a7ede-270">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="a7ede-270">Device configuration installation status by device.</span></span> <span data-ttu-id="a7ede-271">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a7ede-272">userStatuses</span></span>|<span data-ttu-id="a7ede-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a7ede-274">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="a7ede-274">Device configuration installation status by user.</span></span> <span data-ttu-id="a7ede-275">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a7ede-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a7ede-276">deviceStatusOverview</span></span>|[<span data-ttu-id="a7ede-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a7ede-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a7ede-278">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a7ede-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a7ede-279">userStatusOverview</span></span>|[<span data-ttu-id="a7ede-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a7ede-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a7ede-281">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a7ede-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a7ede-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a7ede-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7ede-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a7ede-284">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a7ede-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7ede-285">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="a7ede-285">identityCertificate</span></span>|[<span data-ttu-id="a7ede-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="a7ede-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="a7ede-287">認証方法が証明書の場合にクライアント認証を行うための id 証明書。</span><span class="sxs-lookup"><span data-stu-id="a7ede-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7ede-288">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7ede-288">JSON Representation</span></span>
<span data-ttu-id="a7ede-289">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7ede-289">Here is a JSON representation of the resource.</span></span>
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




