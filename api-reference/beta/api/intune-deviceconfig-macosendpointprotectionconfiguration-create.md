---
title: MacOSEndpointProtectionConfiguration を作成します。
description: 新しい macOSEndpointProtectionConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 31163931fd8f905b2ece59a51ba185211c70c474
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415958"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="56371-103">MacOSEndpointProtectionConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="56371-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="56371-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56371-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56371-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56371-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56371-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56371-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56371-107">新しい[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="56371-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56371-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="56371-108">Prerequisites</span></span>
<span data-ttu-id="56371-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56371-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56371-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56371-111">Permission type</span></span>|<span data-ttu-id="56371-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56371-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56371-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56371-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56371-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56371-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56371-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56371-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56371-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56371-116">Not supported.</span></span>|
|<span data-ttu-id="56371-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56371-117">Application</span></span>|<span data-ttu-id="56371-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56371-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56371-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56371-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56371-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56371-120">Request headers</span></span>
|<span data-ttu-id="56371-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56371-121">Header</span></span>|<span data-ttu-id="56371-122">値</span><span class="sxs-lookup"><span data-stu-id="56371-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56371-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56371-123">Authorization</span></span>|<span data-ttu-id="56371-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56371-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56371-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56371-125">Accept</span></span>|<span data-ttu-id="56371-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56371-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56371-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="56371-127">Request body</span></span>
<span data-ttu-id="56371-128">要求の本文に macOSEndpointProtectionConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="56371-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="56371-129">次の表は、macOSEndpointProtectionConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="56371-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="56371-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56371-130">Property</span></span>|<span data-ttu-id="56371-131">型</span><span class="sxs-lookup"><span data-stu-id="56371-131">Type</span></span>|<span data-ttu-id="56371-132">説明</span><span class="sxs-lookup"><span data-stu-id="56371-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56371-133">id</span><span class="sxs-lookup"><span data-stu-id="56371-133">id</span></span>|<span data-ttu-id="56371-134">String</span><span class="sxs-lookup"><span data-stu-id="56371-134">String</span></span>|<span data-ttu-id="56371-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="56371-135">Key of the entity.</span></span> <span data-ttu-id="56371-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56371-137">lastModifiedDateTime</span></span>|<span data-ttu-id="56371-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56371-138">DateTimeOffset</span></span>|<span data-ttu-id="56371-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="56371-139">DateTime the object was last modified.</span></span> <span data-ttu-id="56371-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56371-141">roleScopeTagIds</span></span>|<span data-ttu-id="56371-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="56371-142">String collection</span></span>|<span data-ttu-id="56371-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="56371-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56371-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="56371-145">supportsScopeTags</span></span>|<span data-ttu-id="56371-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="56371-146">Boolean</span></span>|<span data-ttu-id="56371-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56371-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="56371-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="56371-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="56371-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="56371-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="56371-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="56371-150">This property is read-only.</span></span> <span data-ttu-id="56371-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56371-152">createdDateTime</span></span>|<span data-ttu-id="56371-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56371-153">DateTimeOffset</span></span>|<span data-ttu-id="56371-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="56371-154">DateTime the object was created.</span></span> <span data-ttu-id="56371-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-156">説明</span><span class="sxs-lookup"><span data-stu-id="56371-156">description</span></span>|<span data-ttu-id="56371-157">String</span><span class="sxs-lookup"><span data-stu-id="56371-157">String</span></span>|<span data-ttu-id="56371-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="56371-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56371-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-160">displayName</span><span class="sxs-lookup"><span data-stu-id="56371-160">displayName</span></span>|<span data-ttu-id="56371-161">String</span><span class="sxs-lookup"><span data-stu-id="56371-161">String</span></span>|<span data-ttu-id="56371-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="56371-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56371-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-164">version</span><span class="sxs-lookup"><span data-stu-id="56371-164">version</span></span>|<span data-ttu-id="56371-165">Int32</span><span class="sxs-lookup"><span data-stu-id="56371-165">Int32</span></span>|<span data-ttu-id="56371-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="56371-166">Version of the device configuration.</span></span> <span data-ttu-id="56371-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56371-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56371-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="56371-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="56371-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="56371-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="56371-170">システムは、macOS のデバイスでどのダウンロード場所のアプリケーションから実行できるかを決定するプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="56371-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="56371-171">可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="56371-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="56371-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="56371-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="56371-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="56371-173">Boolean</span></span>|<span data-ttu-id="56371-174">場合は true、ユーザーには、ゲートキーパーは無効になってをオーバーライドします。</span><span class="sxs-lookup"><span data-stu-id="56371-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="56371-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="56371-175">firewallEnabled</span></span>|<span data-ttu-id="56371-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="56371-176">Boolean</span></span>|<span data-ttu-id="56371-177">かどうか、か、これらのファイアウォールは有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="56371-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="56371-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="56371-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="56371-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="56371-179">Boolean</span></span>|<span data-ttu-id="56371-180">「すべての着信接続をブロックする] オプションに対応します。</span><span class="sxs-lookup"><span data-stu-id="56371-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="56371-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="56371-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="56371-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="56371-182">Boolean</span></span>|<span data-ttu-id="56371-183">「有効にするステルス モード」に対応</span><span class="sxs-lookup"><span data-stu-id="56371-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="56371-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="56371-184">firewallApplications</span></span>|<span data-ttu-id="56371-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="56371-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="56371-186">ファイアウォールの設定を使用してアプリケーションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="56371-186">List of applications with firewall settings.</span></span> <span data-ttu-id="56371-187">この一覧にないアプリケーションのファイアウォールの設定は、ユーザーによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="56371-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="56371-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="56371-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="56371-189">応答</span><span class="sxs-lookup"><span data-stu-id="56371-189">Response</span></span>
<span data-ttu-id="56371-190">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="56371-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56371-191">例</span><span class="sxs-lookup"><span data-stu-id="56371-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="56371-192">要求</span><span class="sxs-lookup"><span data-stu-id="56371-192">Request</span></span>
<span data-ttu-id="56371-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56371-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="56371-194">応答</span><span class="sxs-lookup"><span data-stu-id="56371-194">Response</span></span>
<span data-ttu-id="56371-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56371-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 819

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```




