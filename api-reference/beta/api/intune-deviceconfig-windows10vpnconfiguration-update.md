---
title: Windows10VpnConfiguration を更新します。
description: Windows10VpnConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: b55adee6a04eb3db09b12daa1e411a8d456ac73a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072365"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="f23e7-103">Windows10VpnConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-103">Update windows10VpnConfiguration</span></span>

> <span data-ttu-id="f23e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f23e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f23e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f23e7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f23e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f23e7-107">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f23e7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f23e7-108">Prerequisites</span></span>
<span data-ttu-id="f23e7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f23e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23e7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f23e7-111">Permission type</span></span>|<span data-ttu-id="f23e7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f23e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23e7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f23e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f23e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f23e7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f23e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23e7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23e7-116">Not supported.</span></span>|
|<span data-ttu-id="f23e7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f23e7-117">Application</span></span>|<span data-ttu-id="f23e7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23e7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f23e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f23e7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f23e7-120">Request headers</span></span>
|<span data-ttu-id="f23e7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f23e7-121">Header</span></span>|<span data-ttu-id="f23e7-122">値</span><span class="sxs-lookup"><span data-stu-id="f23e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23e7-123">Authorization</span></span>|<span data-ttu-id="f23e7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f23e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f23e7-125">Accept</span></span>|<span data-ttu-id="f23e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f23e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23e7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f23e7-127">Request body</span></span>
<span data-ttu-id="f23e7-128">要求の本文に[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="f23e7-129">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="f23e7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23e7-130">Property</span></span>|<span data-ttu-id="f23e7-131">型</span><span class="sxs-lookup"><span data-stu-id="f23e7-131">Type</span></span>|<span data-ttu-id="f23e7-132">説明</span><span class="sxs-lookup"><span data-stu-id="f23e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23e7-133">id</span><span class="sxs-lookup"><span data-stu-id="f23e7-133">id</span></span>|<span data-ttu-id="f23e7-134">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-134">String</span></span>|<span data-ttu-id="f23e7-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f23e7-135">Key of the entity.</span></span> <span data-ttu-id="f23e7-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f23e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f23e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23e7-138">DateTimeOffset</span></span>|<span data-ttu-id="f23e7-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f23e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f23e7-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f23e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="f23e7-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-142">String collection</span></span>|<span data-ttu-id="f23e7-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f23e7-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f23e7-145">supportsScopeTags</span></span>|<span data-ttu-id="f23e7-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-146">Boolean</span></span>|<span data-ttu-id="f23e7-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f23e7-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f23e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f23e7-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f23e7-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-150">This property is read-only.</span></span> <span data-ttu-id="f23e7-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f23e7-152">createdDateTime</span></span>|<span data-ttu-id="f23e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23e7-153">DateTimeOffset</span></span>|<span data-ttu-id="f23e7-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f23e7-154">DateTime the object was created.</span></span> <span data-ttu-id="f23e7-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-156">説明</span><span class="sxs-lookup"><span data-stu-id="f23e7-156">description</span></span>|<span data-ttu-id="f23e7-157">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-157">String</span></span>|<span data-ttu-id="f23e7-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f23e7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f23e7-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f23e7-160">displayName</span></span>|<span data-ttu-id="f23e7-161">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-161">String</span></span>|<span data-ttu-id="f23e7-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f23e7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f23e7-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-164">version</span><span class="sxs-lookup"><span data-stu-id="f23e7-164">version</span></span>|<span data-ttu-id="f23e7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f23e7-165">Int32</span></span>|<span data-ttu-id="f23e7-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f23e7-166">Version of the device configuration.</span></span> <span data-ttu-id="f23e7-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f23e7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f23e7-168">connectionName</span></span>|<span data-ttu-id="f23e7-169">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-169">String</span></span>|<span data-ttu-id="f23e7-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f23e7-171">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f23e7-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-172">サーバー</span><span class="sxs-lookup"><span data-stu-id="f23e7-172">servers</span></span>|<span data-ttu-id="f23e7-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f23e7-174">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="f23e7-175">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f23e7-176">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f23e7-177">[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f23e7-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-178">customXml</span><span class="sxs-lookup"><span data-stu-id="f23e7-178">customXml</span></span>|<span data-ttu-id="f23e7-179">バイナリ</span><span class="sxs-lookup"><span data-stu-id="f23e7-179">Binary</span></span>|<span data-ttu-id="f23e7-180">VPN 接続を構成するユーザー設定の XML コマンドです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f23e7-181">(UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="f23e7-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f23e7-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="f23e7-182">profileTarget</span></span>|[<span data-ttu-id="f23e7-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="f23e7-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="f23e7-184">プロファイル対象の型。</span><span class="sxs-lookup"><span data-stu-id="f23e7-184">Profile target type.</span></span> <span data-ttu-id="f23e7-185">可能な値は、`user`、`device`、`autoPilotDevice` です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="f23e7-186">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="f23e7-186">connectionType</span></span>|[<span data-ttu-id="f23e7-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f23e7-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="f23e7-188">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-188">Connection type.</span></span> <span data-ttu-id="f23e7-189">可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="f23e7-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f23e7-190">enableSplitTunneling</span></span>|<span data-ttu-id="f23e7-191">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-191">Boolean</span></span>|<span data-ttu-id="f23e7-192">分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="f23e7-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="f23e7-193">enableAlwaysOn</span></span>|<span data-ttu-id="f23e7-194">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-194">Boolean</span></span>|<span data-ttu-id="f23e7-195">常にモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="f23e7-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="f23e7-196">enableDeviceTunnel</span></span>|<span data-ttu-id="f23e7-197">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-197">Boolean</span></span>|<span data-ttu-id="f23e7-198">デバイスのトンネルを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="f23e7-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="f23e7-199">enableDnsRegistration</span></span>|<span data-ttu-id="f23e7-200">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-200">Boolean</span></span>|<span data-ttu-id="f23e7-201">内部の DNS の IP アドレスの登録を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="f23e7-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="f23e7-202">dnsSuffixes</span></span>|<span data-ttu-id="f23e7-203">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-203">String collection</span></span>|<span data-ttu-id="f23e7-204">短い形式の名前を適切にルーティングするのには DNS 検索一覧に追加する DNS サフィックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="f23e7-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="f23e7-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f23e7-205">authenticationMethod</span></span>|[<span data-ttu-id="f23e7-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f23e7-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="f23e7-207">認証方法です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-207">Authentication method.</span></span> <span data-ttu-id="f23e7-208">可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="f23e7-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="f23e7-209">rememberUserCredentials</span></span>|<span data-ttu-id="f23e7-210">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-210">Boolean</span></span>|<span data-ttu-id="f23e7-211">ユーザーの資格情報を覚えておいてください。</span><span class="sxs-lookup"><span data-stu-id="f23e7-211">Remember user credentials.</span></span>|
|<span data-ttu-id="f23e7-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="f23e7-212">enableConditionalAccess</span></span>|<span data-ttu-id="f23e7-213">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-213">Boolean</span></span>|<span data-ttu-id="f23e7-214">条件付きのアクセスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-214">Enable conditional access.</span></span>|
|<span data-ttu-id="f23e7-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="f23e7-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="f23e7-216">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-216">Boolean</span></span>|<span data-ttu-id="f23e7-217">シングル サインオン (SSO) 代替の証明書を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="f23e7-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="f23e7-218">singleSignOnEku</span></span>|[<span data-ttu-id="f23e7-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="f23e7-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="f23e7-220">シングル サインオンの拡張キー使用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="f23e7-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="f23e7-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="f23e7-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="f23e7-222">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-222">String</span></span>|<span data-ttu-id="f23e7-223">シングル サインオンが発行元のハッシュです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="f23e7-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="f23e7-224">eapXml</span></span>|<span data-ttu-id="f23e7-225">バイナリ</span><span class="sxs-lookup"><span data-stu-id="f23e7-225">Binary</span></span>|<span data-ttu-id="f23e7-226">プロトコル (EAP) の XML を拡張可能な認証です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="f23e7-227">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="f23e7-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="f23e7-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f23e7-228">proxyServer</span></span>|[<span data-ttu-id="f23e7-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f23e7-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="f23e7-230">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-230">Proxy Server.</span></span>|
|<span data-ttu-id="f23e7-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="f23e7-231">associatedApps</span></span>|<span data-ttu-id="f23e7-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="f23e7-233">関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-233">Associated Apps.</span></span> <span data-ttu-id="f23e7-234">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f23e7-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="f23e7-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="f23e7-236">ブール値</span><span class="sxs-lookup"><span data-stu-id="f23e7-236">Boolean</span></span>|<span data-ttu-id="f23e7-237">関連付けられているアプリケーションだけでは、接続 (アプリケーションごとの VPN) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="f23e7-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="f23e7-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="f23e7-239">String</span><span class="sxs-lookup"><span data-stu-id="f23e7-239">String</span></span>|<span data-ttu-id="f23e7-240">この接続に関連付けるには Windows の情報の保護 (WIP) のドメインです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="f23e7-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="f23e7-241">trafficRules</span></span>|<span data-ttu-id="f23e7-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="f23e7-243">トラフィックの規則。</span><span class="sxs-lookup"><span data-stu-id="f23e7-243">Traffic rules.</span></span> <span data-ttu-id="f23e7-244">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f23e7-245">ルート</span><span class="sxs-lookup"><span data-stu-id="f23e7-245">routes</span></span>|<span data-ttu-id="f23e7-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="f23e7-247">(サード パーティのプロバイダーでは省略可能) にルーティングします。</span><span class="sxs-lookup"><span data-stu-id="f23e7-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="f23e7-248">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f23e7-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="f23e7-249">dnsRules</span></span>|<span data-ttu-id="f23e7-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f23e7-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="f23e7-251">DNS の規則。</span><span class="sxs-lookup"><span data-stu-id="f23e7-251">DNS rules.</span></span> <span data-ttu-id="f23e7-252">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-252">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f23e7-253">応答</span><span class="sxs-lookup"><span data-stu-id="f23e7-253">Response</span></span>
<span data-ttu-id="f23e7-254">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f23e7-254">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23e7-255">例</span><span class="sxs-lookup"><span data-stu-id="f23e7-255">Example</span></span>
### <a name="request"></a><span data-ttu-id="f23e7-256">要求</span><span class="sxs-lookup"><span data-stu-id="f23e7-256">Request</span></span>
<span data-ttu-id="f23e7-257">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f23e7-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3259

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f23e7-258">応答</span><span class="sxs-lookup"><span data-stu-id="f23e7-258">Response</span></span>
<span data-ttu-id="f23e7-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f23e7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3431

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```





