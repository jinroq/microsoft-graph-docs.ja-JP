---
title: windows10VpnConfiguration リソースの種類
description: このプロファイルの構成を提供することによって必要な VPN エンドポイントへの接続に Windows 10 デバイス (デスクトップまたはモバイル) に指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75710eb8d969f4bfc751405ecf6eca50ced6cfe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406970"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="7403d-104">windows10VpnConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7403d-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="7403d-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7403d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7403d-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7403d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7403d-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7403d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7403d-108">このプロファイルの構成を提供することによって必要な VPN エンドポイントへの接続に Windows 10 デバイス (デスクトップまたはモバイル) に指示できます。</span><span class="sxs-lookup"><span data-stu-id="7403d-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="7403d-109">指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。</span><span class="sxs-lookup"><span data-stu-id="7403d-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="7403d-110">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7403d-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7403d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="7403d-111">Methods</span></span>
|<span data-ttu-id="7403d-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="7403d-112">Method</span></span>|<span data-ttu-id="7403d-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7403d-113">Return Type</span></span>|<span data-ttu-id="7403d-114">説明</span><span class="sxs-lookup"><span data-stu-id="7403d-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7403d-115">リスト windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="7403d-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="7403d-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="7403d-117">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7403d-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7403d-118">Windows10VpnConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="7403d-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="7403d-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7403d-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="7403d-120">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7403d-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7403d-121">Windows10VpnConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="7403d-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="7403d-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7403d-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="7403d-123">新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7403d-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7403d-124">Windows10VpnConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="7403d-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="7403d-125">なし</span><span class="sxs-lookup"><span data-stu-id="7403d-125">None</span></span>|<span data-ttu-id="7403d-126">の[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7403d-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="7403d-127">Windows10VpnConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="7403d-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="7403d-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7403d-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="7403d-129">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7403d-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7403d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7403d-130">Properties</span></span>
|<span data-ttu-id="7403d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7403d-131">Property</span></span>|<span data-ttu-id="7403d-132">型</span><span class="sxs-lookup"><span data-stu-id="7403d-132">Type</span></span>|<span data-ttu-id="7403d-133">説明</span><span class="sxs-lookup"><span data-stu-id="7403d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7403d-134">id</span><span class="sxs-lookup"><span data-stu-id="7403d-134">id</span></span>|<span data-ttu-id="7403d-135">String</span><span class="sxs-lookup"><span data-stu-id="7403d-135">String</span></span>|<span data-ttu-id="7403d-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7403d-136">Key of the entity.</span></span> <span data-ttu-id="7403d-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7403d-138">lastModifiedDateTime</span></span>|<span data-ttu-id="7403d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7403d-139">DateTimeOffset</span></span>|<span data-ttu-id="7403d-140">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7403d-140">DateTime the object was last modified.</span></span> <span data-ttu-id="7403d-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7403d-142">roleScopeTagIds</span></span>|<span data-ttu-id="7403d-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-143">String collection</span></span>|<span data-ttu-id="7403d-144">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="7403d-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7403d-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7403d-146">supportsScopeTags</span></span>|<span data-ttu-id="7403d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-147">Boolean</span></span>|<span data-ttu-id="7403d-148">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7403d-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7403d-149">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="7403d-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7403d-150">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="7403d-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7403d-151">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7403d-151">This property is read-only.</span></span> <span data-ttu-id="7403d-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7403d-153">createdDateTime</span></span>|<span data-ttu-id="7403d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7403d-154">DateTimeOffset</span></span>|<span data-ttu-id="7403d-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7403d-155">DateTime the object was created.</span></span> <span data-ttu-id="7403d-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-157">説明</span><span class="sxs-lookup"><span data-stu-id="7403d-157">description</span></span>|<span data-ttu-id="7403d-158">String</span><span class="sxs-lookup"><span data-stu-id="7403d-158">String</span></span>|<span data-ttu-id="7403d-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7403d-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7403d-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-161">displayName</span><span class="sxs-lookup"><span data-stu-id="7403d-161">displayName</span></span>|<span data-ttu-id="7403d-162">String</span><span class="sxs-lookup"><span data-stu-id="7403d-162">String</span></span>|<span data-ttu-id="7403d-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7403d-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7403d-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-165">version</span><span class="sxs-lookup"><span data-stu-id="7403d-165">version</span></span>|<span data-ttu-id="7403d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7403d-166">Int32</span></span>|<span data-ttu-id="7403d-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7403d-167">Version of the device configuration.</span></span> <span data-ttu-id="7403d-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="7403d-169">connectionName</span></span>|<span data-ttu-id="7403d-170">String</span><span class="sxs-lookup"><span data-stu-id="7403d-170">String</span></span>|<span data-ttu-id="7403d-171">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="7403d-171">Connection name displayed to the user.</span></span> <span data-ttu-id="7403d-172">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="7403d-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-173">サーバー</span><span class="sxs-lookup"><span data-stu-id="7403d-173">servers</span></span>|<span data-ttu-id="7403d-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="7403d-175">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="7403d-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="7403d-176">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7403d-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="7403d-177">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7403d-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7403d-178">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="7403d-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-179">customXml</span><span class="sxs-lookup"><span data-stu-id="7403d-179">customXml</span></span>|<span data-ttu-id="7403d-180">Binary</span><span class="sxs-lookup"><span data-stu-id="7403d-180">Binary</span></span>|<span data-ttu-id="7403d-181">VPN 接続を構成するユーザー設定の XML コマンドです。</span><span class="sxs-lookup"><span data-stu-id="7403d-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="7403d-182">(UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="7403d-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="7403d-183">profileTarget</span></span>|[<span data-ttu-id="7403d-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="7403d-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="7403d-185">プロファイル対象の型。</span><span class="sxs-lookup"><span data-stu-id="7403d-185">Profile target type.</span></span> <span data-ttu-id="7403d-186">可能な値は、`user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="7403d-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="7403d-187">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="7403d-187">connectionType</span></span>|[<span data-ttu-id="7403d-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7403d-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="7403d-189">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="7403d-189">Connection type.</span></span> <span data-ttu-id="7403d-190">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="7403d-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="7403d-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="7403d-191">enableSplitTunneling</span></span>|<span data-ttu-id="7403d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-192">Boolean</span></span>|<span data-ttu-id="7403d-193">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="7403d-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="7403d-194">enableAlwaysOn</span></span>|<span data-ttu-id="7403d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-195">Boolean</span></span>|<span data-ttu-id="7403d-196">常にモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="7403d-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="7403d-197">enableDeviceTunnel</span></span>|<span data-ttu-id="7403d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-198">Boolean</span></span>|<span data-ttu-id="7403d-199">デバイスのトンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="7403d-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="7403d-200">enableDnsRegistration</span></span>|<span data-ttu-id="7403d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-201">Boolean</span></span>|<span data-ttu-id="7403d-202">内部の DNS の IP アドレスの登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="7403d-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="7403d-203">dnsSuffixes</span></span>|<span data-ttu-id="7403d-204">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-204">String collection</span></span>|<span data-ttu-id="7403d-205">短い形式の名前を適切にルーティングするのには DNS 検索一覧に追加する DNS サフィックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="7403d-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="7403d-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7403d-206">authenticationMethod</span></span>|[<span data-ttu-id="7403d-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7403d-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="7403d-208">認証方法です。</span><span class="sxs-lookup"><span data-stu-id="7403d-208">Authentication method.</span></span> <span data-ttu-id="7403d-209">可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="7403d-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="7403d-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="7403d-210">rememberUserCredentials</span></span>|<span data-ttu-id="7403d-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-211">Boolean</span></span>|<span data-ttu-id="7403d-212">ユーザーの資格情報を覚えておいてください。</span><span class="sxs-lookup"><span data-stu-id="7403d-212">Remember user credentials.</span></span>|
|<span data-ttu-id="7403d-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="7403d-213">enableConditionalAccess</span></span>|<span data-ttu-id="7403d-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-214">Boolean</span></span>|<span data-ttu-id="7403d-215">条件付きのアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-215">Enable conditional access.</span></span>|
|<span data-ttu-id="7403d-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="7403d-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="7403d-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-217">Boolean</span></span>|<span data-ttu-id="7403d-218">シングル サインオン (SSO) 代替の証明書を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7403d-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="7403d-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="7403d-219">singleSignOnEku</span></span>|[<span data-ttu-id="7403d-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="7403d-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="7403d-221">シングル サインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="7403d-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="7403d-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="7403d-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="7403d-223">String</span><span class="sxs-lookup"><span data-stu-id="7403d-223">String</span></span>|<span data-ttu-id="7403d-224">シングル サインオンが発行元のハッシュです。</span><span class="sxs-lookup"><span data-stu-id="7403d-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="7403d-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="7403d-225">eapXml</span></span>|<span data-ttu-id="7403d-226">Binary</span><span class="sxs-lookup"><span data-stu-id="7403d-226">Binary</span></span>|<span data-ttu-id="7403d-227">プロトコル (EAP) の XML を拡張可能な認証です。</span><span class="sxs-lookup"><span data-stu-id="7403d-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="7403d-228">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="7403d-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="7403d-229">proxyServer</span><span class="sxs-lookup"><span data-stu-id="7403d-229">proxyServer</span></span>|[<span data-ttu-id="7403d-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7403d-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="7403d-231">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="7403d-231">Proxy Server.</span></span>|
|<span data-ttu-id="7403d-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="7403d-232">associatedApps</span></span>|<span data-ttu-id="7403d-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="7403d-234">関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="7403d-234">Associated Apps.</span></span> <span data-ttu-id="7403d-235">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7403d-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7403d-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="7403d-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="7403d-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="7403d-237">Boolean</span></span>|<span data-ttu-id="7403d-238">関連付けられているアプリケーションだけでは、接続 (アプリケーションごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="7403d-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="7403d-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="7403d-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="7403d-240">String</span><span class="sxs-lookup"><span data-stu-id="7403d-240">String</span></span>|<span data-ttu-id="7403d-241">この接続に関連付けるには Windows の情報の保護 (WIP) のドメインです。</span><span class="sxs-lookup"><span data-stu-id="7403d-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="7403d-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="7403d-242">trafficRules</span></span>|<span data-ttu-id="7403d-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="7403d-244">トラフィックの規則。</span><span class="sxs-lookup"><span data-stu-id="7403d-244">Traffic rules.</span></span> <span data-ttu-id="7403d-245">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7403d-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="7403d-246">ルート</span><span class="sxs-lookup"><span data-stu-id="7403d-246">routes</span></span>|<span data-ttu-id="7403d-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="7403d-248">(サード パーティのプロバイダーでは省略可能) にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="7403d-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="7403d-249">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7403d-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="7403d-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="7403d-250">dnsRules</span></span>|<span data-ttu-id="7403d-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="7403d-252">DNS の規則。</span><span class="sxs-lookup"><span data-stu-id="7403d-252">DNS rules.</span></span> <span data-ttu-id="7403d-253">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7403d-253">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="7403d-254">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="7403d-254">trustedNetworkDomains</span></span>|<span data-ttu-id="7403d-255">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-255">String collection</span></span>|<span data-ttu-id="7403d-256">信頼できるネットワーク ・ ドメイン</span><span class="sxs-lookup"><span data-stu-id="7403d-256">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="7403d-257">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7403d-257">Relationships</span></span>
|<span data-ttu-id="7403d-258">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7403d-258">Relationship</span></span>|<span data-ttu-id="7403d-259">型</span><span class="sxs-lookup"><span data-stu-id="7403d-259">Type</span></span>|<span data-ttu-id="7403d-260">説明</span><span class="sxs-lookup"><span data-stu-id="7403d-260">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7403d-261">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="7403d-261">groupAssignments</span></span>|<span data-ttu-id="7403d-262">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-262">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="7403d-263">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="7403d-263">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="7403d-264">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-264">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-265">assignments</span><span class="sxs-lookup"><span data-stu-id="7403d-265">assignments</span></span>|<span data-ttu-id="7403d-266">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-266">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7403d-267">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="7403d-267">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="7403d-268">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-268">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-269">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7403d-269">deviceStatuses</span></span>|<span data-ttu-id="7403d-270">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-270">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7403d-271">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="7403d-271">Device configuration installation status by device.</span></span> <span data-ttu-id="7403d-272">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-272">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-273">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7403d-273">userStatuses</span></span>|<span data-ttu-id="7403d-274">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-274">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7403d-275">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="7403d-275">Device configuration installation status by user.</span></span> <span data-ttu-id="7403d-276">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7403d-276">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-277">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7403d-277">deviceStatusOverview</span></span>|[<span data-ttu-id="7403d-278">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7403d-278">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7403d-279">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7403d-279">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-280">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7403d-280">userStatusOverview</span></span>|[<span data-ttu-id="7403d-281">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7403d-281">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7403d-282">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7403d-282">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-283">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7403d-283">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7403d-284">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7403d-284">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7403d-285">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7403d-285">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7403d-286">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="7403d-286">identityCertificate</span></span>|[<span data-ttu-id="7403d-287">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="7403d-287">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="7403d-288">認証は、証明書とクライアントの認証に証明します。</span><span class="sxs-lookup"><span data-stu-id="7403d-288">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7403d-289">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7403d-289">JSON Representation</span></span>
<span data-ttu-id="7403d-290">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7403d-290">Here is a JSON representation of the resource.</span></span>
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




