---
title: MacOSVpnConfiguration を作成します。
description: 新しい macOSVpnConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: bc5f01ef506564165252c16336f157d14af7f1ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319664"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="b84f1-103">MacOSVpnConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="b84f1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b84f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b84f1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b84f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b84f1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b84f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b84f1-107">新しい[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b84f1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b84f1-108">Prerequisites</span></span>
<span data-ttu-id="b84f1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b84f1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b84f1-111">Permission type</span></span>|<span data-ttu-id="b84f1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b84f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b84f1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b84f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b84f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b84f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b84f1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b84f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b84f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b84f1-116">Not supported.</span></span>|
|<span data-ttu-id="b84f1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b84f1-117">Application</span></span>|<span data-ttu-id="b84f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b84f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b84f1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b84f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b84f1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b84f1-120">Request headers</span></span>
|<span data-ttu-id="b84f1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b84f1-121">Header</span></span>|<span data-ttu-id="b84f1-122">値</span><span class="sxs-lookup"><span data-stu-id="b84f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b84f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84f1-123">Authorization</span></span>|<span data-ttu-id="b84f1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b84f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b84f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b84f1-125">Accept</span></span>|<span data-ttu-id="b84f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b84f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b84f1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b84f1-127">Request body</span></span>
<span data-ttu-id="b84f1-128">要求の本文に macOSVpnConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="b84f1-129">次の表は、macOSVpnConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="b84f1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b84f1-130">Property</span></span>|<span data-ttu-id="b84f1-131">種類</span><span class="sxs-lookup"><span data-stu-id="b84f1-131">Type</span></span>|<span data-ttu-id="b84f1-132">説明</span><span class="sxs-lookup"><span data-stu-id="b84f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b84f1-133">ID</span><span class="sxs-lookup"><span data-stu-id="b84f1-133">id</span></span>|<span data-ttu-id="b84f1-134">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-134">String</span></span>|<span data-ttu-id="b84f1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b84f1-135">Key of the entity.</span></span> <span data-ttu-id="b84f1-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b84f1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b84f1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84f1-138">DateTimeOffset</span></span>|<span data-ttu-id="b84f1-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b84f1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b84f1-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b84f1-141">roleScopeTagIds</span></span>|<span data-ttu-id="b84f1-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b84f1-142">String collection</span></span>|<span data-ttu-id="b84f1-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="b84f1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b84f1-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b84f1-145">supportsScopeTags</span></span>|<span data-ttu-id="b84f1-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="b84f1-146">Boolean</span></span>|<span data-ttu-id="b84f1-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b84f1-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="b84f1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b84f1-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b84f1-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-150">This property is read-only.</span></span> <span data-ttu-id="b84f1-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b84f1-152">createdDateTime</span></span>|<span data-ttu-id="b84f1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84f1-153">DateTimeOffset</span></span>|<span data-ttu-id="b84f1-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b84f1-154">DateTime the object was created.</span></span> <span data-ttu-id="b84f1-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-156">説明</span><span class="sxs-lookup"><span data-stu-id="b84f1-156">description</span></span>|<span data-ttu-id="b84f1-157">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-157">String</span></span>|<span data-ttu-id="b84f1-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="b84f1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b84f1-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b84f1-160">displayName</span></span>|<span data-ttu-id="b84f1-161">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-161">String</span></span>|<span data-ttu-id="b84f1-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="b84f1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b84f1-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-164">version</span><span class="sxs-lookup"><span data-stu-id="b84f1-164">version</span></span>|<span data-ttu-id="b84f1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b84f1-165">Int32</span></span>|<span data-ttu-id="b84f1-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b84f1-166">Version of the device configuration.</span></span> <span data-ttu-id="b84f1-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b84f1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="b84f1-168">connectionName</span></span>|<span data-ttu-id="b84f1-169">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-169">String</span></span>|<span data-ttu-id="b84f1-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-170">Connection name displayed to the user.</span></span> <span data-ttu-id="b84f1-171">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-172">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="b84f1-172">connectionType</span></span>|[<span data-ttu-id="b84f1-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b84f1-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b84f1-174">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-174">Connection type.</span></span> <span data-ttu-id="b84f1-175">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b84f1-176">使用可能な値: `ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect`、 `checkPointCapsuleVpn`、 `customVpn`、 `ciscoIPSec`、 `citrix`、 `ciscoAnyConnectV2`、 `paloAltoGlobalProtect`、 `zscalerPrivateAccess`、 `f5Access2018`、 `citrixSso`、 `paloAltoGlobalProtectV2`。</span><span class="sxs-lookup"><span data-stu-id="b84f1-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="b84f1-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b84f1-177">loginGroupOrDomain</span></span>|<span data-ttu-id="b84f1-178">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-178">String</span></span>|<span data-ttu-id="b84f1-179">ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。</span><span class="sxs-lookup"><span data-stu-id="b84f1-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b84f1-180">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-181">role</span><span class="sxs-lookup"><span data-stu-id="b84f1-181">role</span></span>|<span data-ttu-id="b84f1-182">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-182">String</span></span>|<span data-ttu-id="b84f1-183">パルスをセキュリティで保護する接続の種類が設定されている場合の役割です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b84f1-184">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-185">領域</span><span class="sxs-lookup"><span data-stu-id="b84f1-185">realm</span></span>|<span data-ttu-id="b84f1-186">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-186">String</span></span>|<span data-ttu-id="b84f1-187">領域のパルスをセキュリティで保護する接続の種類が設定されている場合です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b84f1-188">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-189">サーバー</span><span class="sxs-lookup"><span data-stu-id="b84f1-189">server</span></span>|[<span data-ttu-id="b84f1-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="b84f1-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b84f1-191">ネットワーク上の VPN サーバーです。</span><span class="sxs-lookup"><span data-stu-id="b84f1-191">VPN Server on the network.</span></span> <span data-ttu-id="b84f1-192">エンド ・ ユーザーがこのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="b84f1-193">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-194">識別子</span><span class="sxs-lookup"><span data-stu-id="b84f1-194">identifier</span></span>|<span data-ttu-id="b84f1-195">String</span><span class="sxs-lookup"><span data-stu-id="b84f1-195">String</span></span>|<span data-ttu-id="b84f1-196">カスタム VPN への接続の種類が設定されている場合に、VPN ベンダーによって提供される識別子です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b84f1-197">例: Cisco AnyConnect は[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からのフォーム com.cisco.anyconnect.applevpn.plugin 継承の識別子を使用して</span><span class="sxs-lookup"><span data-stu-id="b84f1-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-198">customData</span><span class="sxs-lookup"><span data-stu-id="b84f1-198">customData</span></span>|<span data-ttu-id="b84f1-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b84f1-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b84f1-200">カスタム VPN への接続の種類が設定されている場合のカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="b84f1-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b84f1-201">VPN ソリューションで使用可能なのですが、Intune でサポートされていない機能を有効にするのにには、このフィールドを使用します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b84f1-202">これらのキーと値のペアを追加する方法については、VPN のベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="b84f1-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b84f1-203">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b84f1-204">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b84f1-205">customKeyValueData</span></span>|<span data-ttu-id="b84f1-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b84f1-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b84f1-207">カスタム VPN への接続の種類が設定されている場合のカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="b84f1-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b84f1-208">VPN ソリューションで使用可能なのですが、Intune でサポートされていない機能を有効にするのにには、このフィールドを使用します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b84f1-209">これらのキーと値のペアを追加する方法については、VPN のベンダーに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="b84f1-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b84f1-210">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b84f1-211">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b84f1-212">enableSplitTunneling</span></span>|<span data-ttu-id="b84f1-213">ブール型</span><span class="sxs-lookup"><span data-stu-id="b84f1-213">Boolean</span></span>|<span data-ttu-id="b84f1-214">VPN 経由のすべてのネットワーク トラフィックを送信します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="b84f1-215">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b84f1-216">authenticationMethod</span></span>|[<span data-ttu-id="b84f1-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b84f1-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b84f1-218">この VPN 接続の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b84f1-219">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b84f1-220">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b84f1-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="b84f1-221">enablePerApp</span></span>|<span data-ttu-id="b84f1-222">ブール型</span><span class="sxs-lookup"><span data-stu-id="b84f1-222">Boolean</span></span>|<span data-ttu-id="b84f1-223">これを true に設定する可能性がある後でエンド ・ ユーザーの iOS デバイスでは、この VPN 接続を開始するアプリケーションに関連付けられているアプリケーションごとの VPN のペイロードを作成します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b84f1-224">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="b84f1-225">safariDomains</span></span>|<span data-ttu-id="b84f1-226">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b84f1-226">String collection</span></span>|<span data-ttu-id="b84f1-227">Safari のドメインごとのアプリケーション設定には、この VPN を有効にするとします。</span><span class="sxs-lookup"><span data-stu-id="b84f1-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b84f1-228">この VPN に関連付けられているアプリケーションだけでなくは、Safari のドメインは、ここでもできるようになりますこの VPN 接続をトリガーを指定します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b84f1-229">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="b84f1-230">onDemandRules</span></span>|<span data-ttu-id="b84f1-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b84f1-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b84f1-232">オン ・ デマンドでのルール。</span><span class="sxs-lookup"><span data-stu-id="b84f1-232">On-Demand Rules.</span></span> <span data-ttu-id="b84f1-233">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b84f1-234">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b84f1-235">proxyServer</span></span>|[<span data-ttu-id="b84f1-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b84f1-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b84f1-237">プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="b84f1-237">Proxy Server.</span></span> <span data-ttu-id="b84f1-238">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b84f1-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="b84f1-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b84f1-240">ブール型</span><span class="sxs-lookup"><span data-stu-id="b84f1-240">Boolean</span></span>|<span data-ttu-id="b84f1-241">オプトインのネットワーク アクセス コントロールの検証中にサードパーティ製の vpn クライアントを使用するためにデバイスの Id を共有します。</span><span class="sxs-lookup"><span data-stu-id="b84f1-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b84f1-242">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b84f1-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b84f1-243">応答</span><span class="sxs-lookup"><span data-stu-id="b84f1-243">Response</span></span>
<span data-ttu-id="b84f1-244">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b84f1-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84f1-245">例</span><span class="sxs-lookup"><span data-stu-id="b84f1-245">Example</span></span>
### <a name="request"></a><span data-ttu-id="b84f1-246">要求</span><span class="sxs-lookup"><span data-stu-id="b84f1-246">Request</span></span>
<span data-ttu-id="b84f1-247">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b84f1-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1921

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="b84f1-248">応答</span><span class="sxs-lookup"><span data-stu-id="b84f1-248">Response</span></span>
<span data-ttu-id="b84f1-p127">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b84f1-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





