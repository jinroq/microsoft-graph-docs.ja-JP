---
title: AndroidWorkProfileVpnConfiguration を作成します。
description: 新しい androidWorkProfileVpnConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: bc00b1b06c28385412a84cdfd7f37d6a8ab7f560
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358199"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="9a72d-103">AndroidWorkProfileVpnConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="9a72d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a72d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a72d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a72d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a72d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a72d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a72d-107">新しい[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a72d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a72d-108">Prerequisites</span></span>
<span data-ttu-id="9a72d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a72d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a72d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a72d-111">Permission type</span></span>|<span data-ttu-id="9a72d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a72d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a72d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a72d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a72d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a72d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a72d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a72d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a72d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a72d-116">Not supported.</span></span>|
|<span data-ttu-id="9a72d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a72d-117">Application</span></span>|<span data-ttu-id="9a72d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a72d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a72d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a72d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9a72d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a72d-120">Request headers</span></span>
|<span data-ttu-id="9a72d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a72d-121">Header</span></span>|<span data-ttu-id="9a72d-122">値</span><span class="sxs-lookup"><span data-stu-id="9a72d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a72d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a72d-123">Authorization</span></span>|<span data-ttu-id="9a72d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9a72d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a72d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a72d-125">Accept</span></span>|<span data-ttu-id="9a72d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a72d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a72d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a72d-127">Request body</span></span>
<span data-ttu-id="9a72d-128">要求の本文に androidWorkProfileVpnConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="9a72d-129">次の表は、androidWorkProfileVpnConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="9a72d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a72d-130">Property</span></span>|<span data-ttu-id="9a72d-131">種類</span><span class="sxs-lookup"><span data-stu-id="9a72d-131">Type</span></span>|<span data-ttu-id="9a72d-132">説明</span><span class="sxs-lookup"><span data-stu-id="9a72d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a72d-133">ID</span><span class="sxs-lookup"><span data-stu-id="9a72d-133">id</span></span>|<span data-ttu-id="9a72d-134">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-134">String</span></span>|<span data-ttu-id="9a72d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9a72d-135">Key of the entity.</span></span> <span data-ttu-id="9a72d-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a72d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9a72d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a72d-138">DateTimeOffset</span></span>|<span data-ttu-id="9a72d-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a72d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9a72d-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a72d-141">roleScopeTagIds</span></span>|<span data-ttu-id="9a72d-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9a72d-142">String collection</span></span>|<span data-ttu-id="9a72d-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9a72d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a72d-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a72d-145">supportsScopeTags</span></span>|<span data-ttu-id="9a72d-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="9a72d-146">Boolean</span></span>|<span data-ttu-id="9a72d-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a72d-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9a72d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a72d-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a72d-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-150">This property is read-only.</span></span> <span data-ttu-id="9a72d-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a72d-152">createdDateTime</span></span>|<span data-ttu-id="9a72d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a72d-153">DateTimeOffset</span></span>|<span data-ttu-id="9a72d-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a72d-154">DateTime the object was created.</span></span> <span data-ttu-id="9a72d-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-156">説明</span><span class="sxs-lookup"><span data-stu-id="9a72d-156">description</span></span>|<span data-ttu-id="9a72d-157">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-157">String</span></span>|<span data-ttu-id="9a72d-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9a72d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a72d-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9a72d-160">displayName</span></span>|<span data-ttu-id="9a72d-161">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-161">String</span></span>|<span data-ttu-id="9a72d-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9a72d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a72d-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-164">version</span><span class="sxs-lookup"><span data-stu-id="9a72d-164">version</span></span>|<span data-ttu-id="9a72d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9a72d-165">Int32</span></span>|<span data-ttu-id="9a72d-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9a72d-166">Version of the device configuration.</span></span> <span data-ttu-id="9a72d-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a72d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a72d-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="9a72d-168">connectionName</span></span>|<span data-ttu-id="9a72d-169">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-169">String</span></span>|<span data-ttu-id="9a72d-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="9a72d-171">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="9a72d-171">connectionType</span></span>|[<span data-ttu-id="9a72d-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9a72d-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="9a72d-173">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-173">Connection type.</span></span> <span data-ttu-id="9a72d-174">可能な値は、`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="9a72d-175">role</span><span class="sxs-lookup"><span data-stu-id="9a72d-175">role</span></span>|<span data-ttu-id="9a72d-176">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-176">String</span></span>|<span data-ttu-id="9a72d-177">パルスをセキュリティで保護する接続の種類が設定されている場合の役割です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9a72d-178">領域</span><span class="sxs-lookup"><span data-stu-id="9a72d-178">realm</span></span>|<span data-ttu-id="9a72d-179">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-179">String</span></span>|<span data-ttu-id="9a72d-180">領域のパルスをセキュリティで保護する接続の種類が設定されている場合です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9a72d-181">サーバー</span><span class="sxs-lookup"><span data-stu-id="9a72d-181">servers</span></span>|<span data-ttu-id="9a72d-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a72d-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9a72d-183">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="9a72d-184">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9a72d-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9a72d-185">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9a72d-186">指紋</span><span class="sxs-lookup"><span data-stu-id="9a72d-186">fingerprint</span></span>|<span data-ttu-id="9a72d-187">String</span><span class="sxs-lookup"><span data-stu-id="9a72d-187">String</span></span>|<span data-ttu-id="9a72d-188">指紋は、VPN サーバーの確認に使用される文字列は、信頼できるチェック ポイントのカプセルの VPN 接続の種類の場合は該当する場合のみです。</span><span class="sxs-lookup"><span data-stu-id="9a72d-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9a72d-189">customData</span><span class="sxs-lookup"><span data-stu-id="9a72d-189">customData</span></span>|<span data-ttu-id="9a72d-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a72d-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="9a72d-191">カスタム データ接続の種類は、Citrix に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="9a72d-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9a72d-192">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9a72d-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="9a72d-193">customKeyValueData</span></span>|<span data-ttu-id="9a72d-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a72d-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9a72d-195">カスタム データ接続の種類は、Citrix に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="9a72d-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9a72d-196">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9a72d-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9a72d-197">authenticationMethod</span></span>|[<span data-ttu-id="9a72d-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9a72d-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9a72d-199">認証方法です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-199">Authentication method.</span></span> <span data-ttu-id="9a72d-200">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="9a72d-201">応答</span><span class="sxs-lookup"><span data-stu-id="9a72d-201">Response</span></span>
<span data-ttu-id="9a72d-202">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9a72d-202">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a72d-203">例</span><span class="sxs-lookup"><span data-stu-id="9a72d-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a72d-204">要求</span><span class="sxs-lookup"><span data-stu-id="9a72d-204">Request</span></span>
<span data-ttu-id="9a72d-205">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a72d-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1053

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="9a72d-206">応答</span><span class="sxs-lookup"><span data-stu-id="9a72d-206">Response</span></span>
<span data-ttu-id="9a72d-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a72d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```





