---
title: MacOSEndpointProtectionConfiguration を作成します。
description: 新しい macOSEndpointProtectionConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 160a98e2d05bc362f69741d0459b37aef0c260cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823038"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="fab38-103">MacOSEndpointProtectionConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="fab38-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="fab38-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fab38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fab38-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fab38-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fab38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fab38-107">新しい[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fab38-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fab38-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fab38-108">Prerequisites</span></span>
<span data-ttu-id="fab38-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fab38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab38-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fab38-111">Permission type</span></span>|<span data-ttu-id="fab38-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fab38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fab38-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fab38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fab38-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fab38-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fab38-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fab38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fab38-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab38-116">Not supported.</span></span>|
|<span data-ttu-id="fab38-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fab38-117">Application</span></span>|<span data-ttu-id="fab38-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fab38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fab38-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fab38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fab38-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fab38-120">Request headers</span></span>
|<span data-ttu-id="fab38-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fab38-121">Header</span></span>|<span data-ttu-id="fab38-122">値</span><span class="sxs-lookup"><span data-stu-id="fab38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fab38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fab38-123">Authorization</span></span>|<span data-ttu-id="fab38-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fab38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fab38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fab38-125">Accept</span></span>|<span data-ttu-id="fab38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fab38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fab38-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fab38-127">Request body</span></span>
<span data-ttu-id="fab38-128">要求の本文に macOSEndpointProtectionConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fab38-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="fab38-129">次の表は、macOSEndpointProtectionConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fab38-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="fab38-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fab38-130">Property</span></span>|<span data-ttu-id="fab38-131">種類</span><span class="sxs-lookup"><span data-stu-id="fab38-131">Type</span></span>|<span data-ttu-id="fab38-132">説明</span><span class="sxs-lookup"><span data-stu-id="fab38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab38-133">ID</span><span class="sxs-lookup"><span data-stu-id="fab38-133">id</span></span>|<span data-ttu-id="fab38-134">String</span><span class="sxs-lookup"><span data-stu-id="fab38-134">String</span></span>|<span data-ttu-id="fab38-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fab38-135">Key of the entity.</span></span> <span data-ttu-id="fab38-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fab38-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fab38-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab38-138">DateTimeOffset</span></span>|<span data-ttu-id="fab38-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fab38-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fab38-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fab38-141">roleScopeTagIds</span></span>|<span data-ttu-id="fab38-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fab38-142">String collection</span></span>|<span data-ttu-id="fab38-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="fab38-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fab38-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fab38-145">supportsScopeTags</span></span>|<span data-ttu-id="fab38-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="fab38-146">Boolean</span></span>|<span data-ttu-id="fab38-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fab38-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fab38-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="fab38-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fab38-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="fab38-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fab38-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fab38-150">This property is read-only.</span></span> <span data-ttu-id="fab38-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fab38-152">createdDateTime</span></span>|<span data-ttu-id="fab38-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab38-153">DateTimeOffset</span></span>|<span data-ttu-id="fab38-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fab38-154">DateTime the object was created.</span></span> <span data-ttu-id="fab38-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-156">説明</span><span class="sxs-lookup"><span data-stu-id="fab38-156">description</span></span>|<span data-ttu-id="fab38-157">String</span><span class="sxs-lookup"><span data-stu-id="fab38-157">String</span></span>|<span data-ttu-id="fab38-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fab38-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fab38-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fab38-160">displayName</span></span>|<span data-ttu-id="fab38-161">String</span><span class="sxs-lookup"><span data-stu-id="fab38-161">String</span></span>|<span data-ttu-id="fab38-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fab38-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fab38-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-164">version</span><span class="sxs-lookup"><span data-stu-id="fab38-164">version</span></span>|<span data-ttu-id="fab38-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fab38-165">Int32</span></span>|<span data-ttu-id="fab38-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fab38-166">Version of the device configuration.</span></span> <span data-ttu-id="fab38-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fab38-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fab38-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="fab38-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="fab38-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="fab38-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="fab38-170">システムは、macOS のデバイスでどのダウンロード場所のアプリケーションから実行できるかを決定するプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="fab38-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="fab38-171">可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="fab38-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="fab38-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="fab38-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="fab38-173">ブール型</span><span class="sxs-lookup"><span data-stu-id="fab38-173">Boolean</span></span>|<span data-ttu-id="fab38-174">場合は true、ユーザーには、ゲートキーパーは無効になってをオーバーライドします。</span><span class="sxs-lookup"><span data-stu-id="fab38-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="fab38-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="fab38-175">firewallEnabled</span></span>|<span data-ttu-id="fab38-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="fab38-176">Boolean</span></span>|<span data-ttu-id="fab38-177">かどうか、か、これらのファイアウォールは有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fab38-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="fab38-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="fab38-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="fab38-179">ブール型</span><span class="sxs-lookup"><span data-stu-id="fab38-179">Boolean</span></span>|<span data-ttu-id="fab38-180">「すべての着信接続をブロックする] オプションに対応します。</span><span class="sxs-lookup"><span data-stu-id="fab38-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="fab38-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="fab38-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="fab38-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="fab38-182">Boolean</span></span>|<span data-ttu-id="fab38-183">「有効にするステルス モード」に対応</span><span class="sxs-lookup"><span data-stu-id="fab38-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="fab38-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="fab38-184">firewallApplications</span></span>|<span data-ttu-id="fab38-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fab38-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="fab38-186">ファイアウォールの設定を使用してアプリケーションの一覧です。</span><span class="sxs-lookup"><span data-stu-id="fab38-186">List of applications with firewall settings.</span></span> <span data-ttu-id="fab38-187">この一覧にないアプリケーションのファイアウォールの設定は、ユーザーによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="fab38-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="fab38-188">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fab38-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fab38-189">応答</span><span class="sxs-lookup"><span data-stu-id="fab38-189">Response</span></span>
<span data-ttu-id="fab38-190">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fab38-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab38-191">例</span><span class="sxs-lookup"><span data-stu-id="fab38-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="fab38-192">要求</span><span class="sxs-lookup"><span data-stu-id="fab38-192">Request</span></span>
<span data-ttu-id="fab38-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fab38-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 711

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="fab38-194">応答</span><span class="sxs-lookup"><span data-stu-id="fab38-194">Response</span></span>
<span data-ttu-id="fab38-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fab38-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





