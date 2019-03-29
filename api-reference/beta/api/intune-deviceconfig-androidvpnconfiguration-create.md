---
title: androidvpnconfiguration の作成
description: 新しい androidvpnconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4611191cf4a8703f3a35f6b7b483d3a474b6c9a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968113"
---
# <a name="create-androidvpnconfiguration"></a><span data-ttu-id="cb193-103">androidvpnconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="cb193-103">Create androidVpnConfiguration</span></span>

> <span data-ttu-id="cb193-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb193-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb193-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb193-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb193-106">新しい[androidvpnconfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cb193-106">Create a new [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb193-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cb193-107">Prerequisites</span></span>
<span data-ttu-id="cb193-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb193-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb193-110">Permission type</span></span>|<span data-ttu-id="cb193-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb193-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb193-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb193-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb193-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb193-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb193-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb193-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb193-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb193-115">Not supported.</span></span>|
|<span data-ttu-id="cb193-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb193-116">Application</span></span>|<span data-ttu-id="cb193-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb193-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb193-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb193-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cb193-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb193-119">Request headers</span></span>
|<span data-ttu-id="cb193-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb193-120">Header</span></span>|<span data-ttu-id="cb193-121">値</span><span class="sxs-lookup"><span data-stu-id="cb193-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb193-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb193-122">Authorization</span></span>|<span data-ttu-id="cb193-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb193-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb193-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cb193-124">Accept</span></span>|<span data-ttu-id="cb193-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb193-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb193-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb193-126">Request body</span></span>
<span data-ttu-id="cb193-127">要求本文で、androidvpnconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb193-127">In the request body, supply a JSON representation for the androidVpnConfiguration object.</span></span>

<span data-ttu-id="cb193-128">次の表に、androidvpnconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cb193-128">The following table shows the properties that are required when you create the androidVpnConfiguration.</span></span>

|<span data-ttu-id="cb193-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb193-129">Property</span></span>|<span data-ttu-id="cb193-130">型</span><span class="sxs-lookup"><span data-stu-id="cb193-130">Type</span></span>|<span data-ttu-id="cb193-131">説明</span><span class="sxs-lookup"><span data-stu-id="cb193-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb193-132">id</span><span class="sxs-lookup"><span data-stu-id="cb193-132">id</span></span>|<span data-ttu-id="cb193-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cb193-133">String</span></span>|<span data-ttu-id="cb193-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb193-134">Key of the entity.</span></span> <span data-ttu-id="cb193-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb193-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cb193-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb193-137">DateTimeOffset</span></span>|<span data-ttu-id="cb193-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb193-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cb193-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb193-140">roleScopeTagIds</span></span>|<span data-ttu-id="cb193-141">String collection</span><span class="sxs-lookup"><span data-stu-id="cb193-141">String collection</span></span>|<span data-ttu-id="cb193-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="cb193-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb193-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cb193-144">supportsScopeTags</span></span>|<span data-ttu-id="cb193-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb193-145">Boolean</span></span>|<span data-ttu-id="cb193-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cb193-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb193-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="cb193-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb193-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="cb193-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb193-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="cb193-149">This property is read-only.</span></span> <span data-ttu-id="cb193-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb193-151">createdDateTime</span></span>|<span data-ttu-id="cb193-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb193-152">DateTimeOffset</span></span>|<span data-ttu-id="cb193-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cb193-153">DateTime the object was created.</span></span> <span data-ttu-id="cb193-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-155">description</span><span class="sxs-lookup"><span data-stu-id="cb193-155">description</span></span>|<span data-ttu-id="cb193-156">String</span><span class="sxs-lookup"><span data-stu-id="cb193-156">String</span></span>|<span data-ttu-id="cb193-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="cb193-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb193-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cb193-159">displayName</span></span>|<span data-ttu-id="cb193-160">String</span><span class="sxs-lookup"><span data-stu-id="cb193-160">String</span></span>|<span data-ttu-id="cb193-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="cb193-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb193-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-163">version</span><span class="sxs-lookup"><span data-stu-id="cb193-163">version</span></span>|<span data-ttu-id="cb193-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cb193-164">Int32</span></span>|<span data-ttu-id="cb193-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cb193-165">Version of the device configuration.</span></span> <span data-ttu-id="cb193-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cb193-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb193-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="cb193-167">connectionName</span></span>|<span data-ttu-id="cb193-168">String</span><span class="sxs-lookup"><span data-stu-id="cb193-168">String</span></span>|<span data-ttu-id="cb193-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="cb193-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="cb193-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="cb193-170">connectionType</span></span>|[<span data-ttu-id="cb193-171">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="cb193-171">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="cb193-172">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="cb193-172">Connection type.</span></span> <span data-ttu-id="cb193-173">可能な値は `ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix` です。</span><span class="sxs-lookup"><span data-stu-id="cb193-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="cb193-174">role</span><span class="sxs-lookup"><span data-stu-id="cb193-174">role</span></span>|<span data-ttu-id="cb193-175">String</span><span class="sxs-lookup"><span data-stu-id="cb193-175">String</span></span>|<span data-ttu-id="cb193-176">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="cb193-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="cb193-177">領域</span><span class="sxs-lookup"><span data-stu-id="cb193-177">realm</span></span>|<span data-ttu-id="cb193-178">String</span><span class="sxs-lookup"><span data-stu-id="cb193-178">String</span></span>|<span data-ttu-id="cb193-179">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="cb193-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="cb193-180">サーバ</span><span class="sxs-lookup"><span data-stu-id="cb193-180">servers</span></span>|<span data-ttu-id="cb193-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cb193-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="cb193-182">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="cb193-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="cb193-183">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="cb193-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="cb193-184">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb193-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb193-185">デジタル</span><span class="sxs-lookup"><span data-stu-id="cb193-185">fingerprint</span></span>|<span data-ttu-id="cb193-186">String</span><span class="sxs-lookup"><span data-stu-id="cb193-186">String</span></span>|<span data-ttu-id="cb193-187">フィンガープリントは、vpn サーバーが信頼できることを確認するために使用される文字列です。これは、接続の種類が [チェックポイントカプセル VPN] の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cb193-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="cb193-188">customData</span><span class="sxs-lookup"><span data-stu-id="cb193-188">customData</span></span>|<span data-ttu-id="cb193-189">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb193-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="cb193-190">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="cb193-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="cb193-191">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb193-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="cb193-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="cb193-192">customKeyValueData</span></span>|<span data-ttu-id="cb193-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb193-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cb193-194">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="cb193-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="cb193-195">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cb193-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="cb193-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb193-196">authenticationMethod</span></span>|[<span data-ttu-id="cb193-197">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="cb193-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="cb193-198">認証方法。</span><span class="sxs-lookup"><span data-stu-id="cb193-198">Authentication method.</span></span> <span data-ttu-id="cb193-199">可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="cb193-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="cb193-200">応答</span><span class="sxs-lookup"><span data-stu-id="cb193-200">Response</span></span>
<span data-ttu-id="cb193-201">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidvpnconfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb193-201">If successful, this method returns a `201 Created` response code and a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb193-202">例</span><span class="sxs-lookup"><span data-stu-id="cb193-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb193-203">要求</span><span class="sxs-lookup"><span data-stu-id="cb193-203">Request</span></span>
<span data-ttu-id="cb193-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb193-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 978

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="cb193-205">応答</span><span class="sxs-lookup"><span data-stu-id="cb193-205">Response</span></span>
<span data-ttu-id="cb193-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb193-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




