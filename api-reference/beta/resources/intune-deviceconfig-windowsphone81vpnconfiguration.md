---
title: windowsPhone81VpnConfiguration リソースの種類
description: このプロファイルの構成を提供することにより、必要な VPN エンドポイントへの接続に Windows Phone の 8.1 を指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。
author: tfitzmac
ms.openlocfilehash: 309a848965d666d8d89ee619441af8f5ca25b6fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317200"
---
# <a name="windowsphone81vpnconfiguration-resource-type"></a><span data-ttu-id="0b3c2-104">windowsPhone81VpnConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b3c2-104">windowsPhone81VpnConfiguration resource type</span></span>

> <span data-ttu-id="0b3c2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b3c2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b3c2-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b3c2-108">このプロファイルの構成を提供することにより、必要な VPN エンドポイントへの接続に Windows Phone の 8.1 を指示できます。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-108">By providing the configurations in this profile you can instruct the Windows Phone 8.1 to connect to desired VPN endpoint.</span></span> <span data-ttu-id="0b3c2-109">指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>

<span data-ttu-id="0b3c2-110">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-110">Inherits from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0b3c2-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b3c2-111">Methods</span></span>
|<span data-ttu-id="0b3c2-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b3c2-112">Method</span></span>|<span data-ttu-id="0b3c2-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-113">Return Type</span></span>|<span data-ttu-id="0b3c2-114">説明</span><span class="sxs-lookup"><span data-stu-id="0b3c2-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b3c2-115">リスト windowsPhone81VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="0b3c2-115">List windowsPhone81VpnConfigurations</span></span>](../api/intune-deviceconfig-windowsphone81vpnconfiguration-list.md)|<span data-ttu-id="0b3c2-116">[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-116">[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) collection</span></span>|<span data-ttu-id="0b3c2-117">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-117">List properties and relationships of the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0b3c2-118">WindowsPhone81VpnConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-118">Get windowsPhone81VpnConfiguration</span></span>](../api/intune-deviceconfig-windowsphone81vpnconfiguration-get.md)|[<span data-ttu-id="0b3c2-119">windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b3c2-119">windowsPhone81VpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|<span data-ttu-id="0b3c2-120">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-120">Read properties and relationships of the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0b3c2-121">WindowsPhone81VpnConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-121">Create windowsPhone81VpnConfiguration</span></span>](../api/intune-deviceconfig-windowsphone81vpnconfiguration-create.md)|[<span data-ttu-id="0b3c2-122">windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b3c2-122">windowsPhone81VpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|<span data-ttu-id="0b3c2-123">新しい[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-123">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0b3c2-124">WindowsPhone81VpnConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-124">Delete windowsPhone81VpnConfiguration</span></span>](../api/intune-deviceconfig-windowsphone81vpnconfiguration-delete.md)|<span data-ttu-id="0b3c2-125">なし</span><span class="sxs-lookup"><span data-stu-id="0b3c2-125">None</span></span>|<span data-ttu-id="0b3c2-126">の[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-126">Deletes a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="0b3c2-127">WindowsPhone81VpnConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-127">Update windowsPhone81VpnConfiguration</span></span>](../api/intune-deviceconfig-windowsphone81vpnconfiguration-update.md)|[<span data-ttu-id="0b3c2-128">windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b3c2-128">windowsPhone81VpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)|<span data-ttu-id="0b3c2-129">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-129">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b3c2-130">Properties</span><span class="sxs-lookup"><span data-stu-id="0b3c2-130">Properties</span></span>
|<span data-ttu-id="0b3c2-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b3c2-131">Property</span></span>|<span data-ttu-id="0b3c2-132">種類</span><span class="sxs-lookup"><span data-stu-id="0b3c2-132">Type</span></span>|<span data-ttu-id="0b3c2-133">説明</span><span class="sxs-lookup"><span data-stu-id="0b3c2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b3c2-134">ID</span><span class="sxs-lookup"><span data-stu-id="0b3c2-134">id</span></span>|<span data-ttu-id="0b3c2-135">String</span><span class="sxs-lookup"><span data-stu-id="0b3c2-135">String</span></span>|<span data-ttu-id="0b3c2-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-136">Key of the entity.</span></span> <span data-ttu-id="0b3c2-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3c2-138">lastModifiedDateTime</span></span>|<span data-ttu-id="0b3c2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3c2-139">DateTimeOffset</span></span>|<span data-ttu-id="0b3c2-140">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-140">DateTime the object was last modified.</span></span> <span data-ttu-id="0b3c2-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b3c2-142">roleScopeTagIds</span></span>|<span data-ttu-id="0b3c2-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-143">String collection</span></span>|<span data-ttu-id="0b3c2-144">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b3c2-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b3c2-146">supportsScopeTags</span></span>|<span data-ttu-id="0b3c2-147">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-147">Boolean</span></span>|<span data-ttu-id="0b3c2-148">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b3c2-149">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b3c2-150">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b3c2-151">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-151">This property is read-only.</span></span> <span data-ttu-id="0b3c2-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b3c2-153">createdDateTime</span></span>|<span data-ttu-id="0b3c2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3c2-154">DateTimeOffset</span></span>|<span data-ttu-id="0b3c2-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-155">DateTime the object was created.</span></span> <span data-ttu-id="0b3c2-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-157">説明</span><span class="sxs-lookup"><span data-stu-id="0b3c2-157">description</span></span>|<span data-ttu-id="0b3c2-158">String</span><span class="sxs-lookup"><span data-stu-id="0b3c2-158">String</span></span>|<span data-ttu-id="0b3c2-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b3c2-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-161">displayName</span><span class="sxs-lookup"><span data-stu-id="0b3c2-161">displayName</span></span>|<span data-ttu-id="0b3c2-162">String</span><span class="sxs-lookup"><span data-stu-id="0b3c2-162">String</span></span>|<span data-ttu-id="0b3c2-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b3c2-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-165">version</span><span class="sxs-lookup"><span data-stu-id="0b3c2-165">version</span></span>|<span data-ttu-id="0b3c2-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0b3c2-166">Int32</span></span>|<span data-ttu-id="0b3c2-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-167">Version of the device configuration.</span></span> <span data-ttu-id="0b3c2-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="0b3c2-169">connectionName</span></span>|<span data-ttu-id="0b3c2-170">String</span><span class="sxs-lookup"><span data-stu-id="0b3c2-170">String</span></span>|<span data-ttu-id="0b3c2-171">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-171">Connection name displayed to the user.</span></span> <span data-ttu-id="0b3c2-172">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-173">サーバー</span><span class="sxs-lookup"><span data-stu-id="0b3c2-173">servers</span></span>|<span data-ttu-id="0b3c2-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0b3c2-175">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="0b3c2-176">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0b3c2-177">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0b3c2-178">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-179">customXml</span><span class="sxs-lookup"><span data-stu-id="0b3c2-179">customXml</span></span>|<span data-ttu-id="0b3c2-180">Binary</span><span class="sxs-lookup"><span data-stu-id="0b3c2-180">Binary</span></span>|<span data-ttu-id="0b3c2-181">VPN 接続を構成するユーザー設定の XML コマンドです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0b3c2-182">(UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-183">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="0b3c2-183">applyOnlyToWindows81</span></span>|<span data-ttu-id="0b3c2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b3c2-184">Boolean</span></span>|<span data-ttu-id="0b3c2-185">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-185">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="0b3c2-186">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-186">This property is read-only.</span></span> <span data-ttu-id="0b3c2-187">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-187">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-188">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="0b3c2-188">connectionType</span></span>|[<span data-ttu-id="0b3c2-189">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0b3c2-189">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="0b3c2-190">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-190">Connection type.</span></span> <span data-ttu-id="0b3c2-191">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-191">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="0b3c2-192">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-192">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="0b3c2-193">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0b3c2-193">loginGroupOrDomain</span></span>|<span data-ttu-id="0b3c2-194">String</span><span class="sxs-lookup"><span data-stu-id="0b3c2-194">String</span></span>|<span data-ttu-id="0b3c2-195">ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-195">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0b3c2-196">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-196">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-197">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0b3c2-197">enableSplitTunneling</span></span>|<span data-ttu-id="0b3c2-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-198">Boolean</span></span>|<span data-ttu-id="0b3c2-199">分割は、VPN のトンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-199">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="0b3c2-200">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-200">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-201">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0b3c2-201">proxyServer</span></span>|[<span data-ttu-id="0b3c2-202">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0b3c2-202">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="0b3c2-203">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-203">Proxy Server.</span></span> <span data-ttu-id="0b3c2-204">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-204">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-205">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="0b3c2-205">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="0b3c2-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-206">Boolean</span></span>|<span data-ttu-id="0b3c2-207">Wi-fi の会社に VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-207">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="0b3c2-208">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="0b3c2-208">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="0b3c2-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-209">Boolean</span></span>|<span data-ttu-id="0b3c2-210">ホーム Wi-fi で VPN を使用しません。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-210">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="0b3c2-211">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b3c2-211">authenticationMethod</span></span>|[<span data-ttu-id="0b3c2-212">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b3c2-212">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0b3c2-213">認証方法です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-213">Authentication method.</span></span> <span data-ttu-id="0b3c2-214">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-214">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0b3c2-215">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="0b3c2-215">rememberUserCredentials</span></span>|<span data-ttu-id="0b3c2-216">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-216">Boolean</span></span>|<span data-ttu-id="0b3c2-217">ユーザーの資格情報を覚えておいてください。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-217">Remember user credentials.</span></span>|
|<span data-ttu-id="0b3c2-218">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="0b3c2-218">dnsSuffixSearchList</span></span>|<span data-ttu-id="0b3c2-219">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-219">String collection</span></span>|<span data-ttu-id="0b3c2-220">DNS サフィックス検索一覧です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-220">DNS suffix search list.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b3c2-221">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b3c2-221">Relationships</span></span>
|<span data-ttu-id="0b3c2-222">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b3c2-222">Relationship</span></span>|<span data-ttu-id="0b3c2-223">型</span><span class="sxs-lookup"><span data-stu-id="0b3c2-223">Type</span></span>|<span data-ttu-id="0b3c2-224">説明</span><span class="sxs-lookup"><span data-stu-id="0b3c2-224">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b3c2-225">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0b3c2-225">groupAssignments</span></span>|<span data-ttu-id="0b3c2-226">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-226">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0b3c2-227">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-227">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0b3c2-228">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-229">assignments</span><span class="sxs-lookup"><span data-stu-id="0b3c2-229">assignments</span></span>|<span data-ttu-id="0b3c2-230">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-230">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0b3c2-231">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-231">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0b3c2-232">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-233">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0b3c2-233">deviceStatuses</span></span>|<span data-ttu-id="0b3c2-234">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-234">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0b3c2-235">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-235">Device configuration installation status by device.</span></span> <span data-ttu-id="0b3c2-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-237">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0b3c2-237">userStatuses</span></span>|<span data-ttu-id="0b3c2-238">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-238">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0b3c2-239">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-239">Device configuration installation status by user.</span></span> <span data-ttu-id="0b3c2-240">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b3c2-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-241">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0b3c2-241">deviceStatusOverview</span></span>|[<span data-ttu-id="0b3c2-242">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0b3c2-242">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0b3c2-243">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0b3c2-243">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-244">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0b3c2-244">userStatusOverview</span></span>|[<span data-ttu-id="0b3c2-245">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0b3c2-245">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0b3c2-246">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0b3c2-246">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-247">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0b3c2-247">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0b3c2-248">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0b3c2-248">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0b3c2-249">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0b3c2-249">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b3c2-250">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="0b3c2-250">identityCertificate</span></span>|[<span data-ttu-id="0b3c2-251">windowsPhone81CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="0b3c2-251">windowsPhone81CertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)|<span data-ttu-id="0b3c2-252">認証は、証明書とクライアントの認証に証明します。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-252">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b3c2-253">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b3c2-253">JSON Representation</span></span>
<span data-ttu-id="0b3c2-254">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b3c2-254">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  "applyOnlyToWindows81": true,
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "String"
  ]
}
```




