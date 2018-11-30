---
title: AndroidVpnConfiguration を更新します。
description: AndroidVpnConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 80d491a1a6a97b8bcbde1c2c5cb55cd58dfe629b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070307"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="09bba-103">AndroidVpnConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="09bba-103">Update androidVpnConfiguration</span></span>

> <span data-ttu-id="09bba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09bba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09bba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09bba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09bba-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09bba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09bba-107">[AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09bba-107">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09bba-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="09bba-108">Prerequisites</span></span>
<span data-ttu-id="09bba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09bba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09bba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09bba-111">Permission type</span></span>|<span data-ttu-id="09bba-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09bba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09bba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09bba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09bba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09bba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09bba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09bba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09bba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09bba-116">Not supported.</span></span>|
|<span data-ttu-id="09bba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09bba-117">Application</span></span>|<span data-ttu-id="09bba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09bba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09bba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09bba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="09bba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09bba-120">Request headers</span></span>
|<span data-ttu-id="09bba-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09bba-121">Header</span></span>|<span data-ttu-id="09bba-122">値</span><span class="sxs-lookup"><span data-stu-id="09bba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09bba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09bba-123">Authorization</span></span>|<span data-ttu-id="09bba-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="09bba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09bba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09bba-125">Accept</span></span>|<span data-ttu-id="09bba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09bba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09bba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="09bba-127">Request body</span></span>
<span data-ttu-id="09bba-128">要求の本文に[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="09bba-128">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="09bba-129">[AndroidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="09bba-129">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="09bba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09bba-130">Property</span></span>|<span data-ttu-id="09bba-131">型</span><span class="sxs-lookup"><span data-stu-id="09bba-131">Type</span></span>|<span data-ttu-id="09bba-132">説明</span><span class="sxs-lookup"><span data-stu-id="09bba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09bba-133">id</span><span class="sxs-lookup"><span data-stu-id="09bba-133">id</span></span>|<span data-ttu-id="09bba-134">String</span><span class="sxs-lookup"><span data-stu-id="09bba-134">String</span></span>|<span data-ttu-id="09bba-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09bba-135">Key of the entity.</span></span> <span data-ttu-id="09bba-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09bba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09bba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09bba-138">DateTimeOffset</span></span>|<span data-ttu-id="09bba-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="09bba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="09bba-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09bba-141">roleScopeTagIds</span></span>|<span data-ttu-id="09bba-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09bba-142">String collection</span></span>|<span data-ttu-id="09bba-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="09bba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09bba-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="09bba-145">supportsScopeTags</span></span>|<span data-ttu-id="09bba-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="09bba-146">Boolean</span></span>|<span data-ttu-id="09bba-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09bba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09bba-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="09bba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09bba-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="09bba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09bba-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="09bba-150">This property is read-only.</span></span> <span data-ttu-id="09bba-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09bba-152">createdDateTime</span></span>|<span data-ttu-id="09bba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09bba-153">DateTimeOffset</span></span>|<span data-ttu-id="09bba-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="09bba-154">DateTime the object was created.</span></span> <span data-ttu-id="09bba-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-156">説明</span><span class="sxs-lookup"><span data-stu-id="09bba-156">description</span></span>|<span data-ttu-id="09bba-157">String</span><span class="sxs-lookup"><span data-stu-id="09bba-157">String</span></span>|<span data-ttu-id="09bba-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="09bba-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09bba-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-160">displayName</span><span class="sxs-lookup"><span data-stu-id="09bba-160">displayName</span></span>|<span data-ttu-id="09bba-161">String</span><span class="sxs-lookup"><span data-stu-id="09bba-161">String</span></span>|<span data-ttu-id="09bba-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="09bba-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09bba-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-164">version</span><span class="sxs-lookup"><span data-stu-id="09bba-164">version</span></span>|<span data-ttu-id="09bba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="09bba-165">Int32</span></span>|<span data-ttu-id="09bba-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="09bba-166">Version of the device configuration.</span></span> <span data-ttu-id="09bba-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09bba-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09bba-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="09bba-168">connectionName</span></span>|<span data-ttu-id="09bba-169">String</span><span class="sxs-lookup"><span data-stu-id="09bba-169">String</span></span>|<span data-ttu-id="09bba-170">接続名がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="09bba-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="09bba-171">接続タイプ</span><span class="sxs-lookup"><span data-stu-id="09bba-171">connectionType</span></span>|[<span data-ttu-id="09bba-172">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="09bba-172">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="09bba-173">接続の種類です。</span><span class="sxs-lookup"><span data-stu-id="09bba-173">Connection type.</span></span> <span data-ttu-id="09bba-174">使用可能な値: `ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="09bba-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="09bba-175">role</span><span class="sxs-lookup"><span data-stu-id="09bba-175">role</span></span>|<span data-ttu-id="09bba-176">String</span><span class="sxs-lookup"><span data-stu-id="09bba-176">String</span></span>|<span data-ttu-id="09bba-177">パルスをセキュリティで保護する接続の種類が設定されている場合の役割です。</span><span class="sxs-lookup"><span data-stu-id="09bba-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="09bba-178">領域</span><span class="sxs-lookup"><span data-stu-id="09bba-178">realm</span></span>|<span data-ttu-id="09bba-179">String</span><span class="sxs-lookup"><span data-stu-id="09bba-179">String</span></span>|<span data-ttu-id="09bba-180">領域のパルスをセキュリティで保護する接続の種類が設定されている場合です。</span><span class="sxs-lookup"><span data-stu-id="09bba-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="09bba-181">サーバー</span><span class="sxs-lookup"><span data-stu-id="09bba-181">servers</span></span>|<span data-ttu-id="09bba-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09bba-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="09bba-183">ネットワーク上の VPN サーバーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="09bba-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="09bba-184">エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="09bba-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="09bba-185">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="09bba-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="09bba-186">指紋</span><span class="sxs-lookup"><span data-stu-id="09bba-186">fingerprint</span></span>|<span data-ttu-id="09bba-187">String</span><span class="sxs-lookup"><span data-stu-id="09bba-187">String</span></span>|<span data-ttu-id="09bba-188">指紋は、VPN サーバーの確認に使用される文字列は、信頼できるチェック ポイントのカプセルの VPN 接続の種類の場合は該当する場合のみです。</span><span class="sxs-lookup"><span data-stu-id="09bba-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="09bba-189">customData</span><span class="sxs-lookup"><span data-stu-id="09bba-189">customData</span></span>|<span data-ttu-id="09bba-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09bba-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="09bba-191">カスタム データ接続の種類は、Citrix に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="09bba-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="09bba-192">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="09bba-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="09bba-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="09bba-193">customKeyValueData</span></span>|<span data-ttu-id="09bba-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="09bba-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="09bba-195">カスタム データ接続の種類は、Citrix に設定されている場合。</span><span class="sxs-lookup"><span data-stu-id="09bba-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="09bba-196">このコレクションには、最大 25 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="09bba-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="09bba-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09bba-197">authenticationMethod</span></span>|[<span data-ttu-id="09bba-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09bba-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="09bba-199">認証方法です。</span><span class="sxs-lookup"><span data-stu-id="09bba-199">Authentication method.</span></span> <span data-ttu-id="09bba-200">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="09bba-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="09bba-201">応答</span><span class="sxs-lookup"><span data-stu-id="09bba-201">Response</span></span>
<span data-ttu-id="09bba-202">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="09bba-202">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09bba-203">例</span><span class="sxs-lookup"><span data-stu-id="09bba-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="09bba-204">要求</span><span class="sxs-lookup"><span data-stu-id="09bba-204">Request</span></span>
<span data-ttu-id="09bba-205">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09bba-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 980

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

### <a name="response"></a><span data-ttu-id="09bba-206">応答</span><span class="sxs-lookup"><span data-stu-id="09bba-206">Response</span></span>
<span data-ttu-id="09bba-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09bba-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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





