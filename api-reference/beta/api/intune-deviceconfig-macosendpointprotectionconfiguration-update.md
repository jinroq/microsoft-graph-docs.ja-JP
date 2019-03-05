---
title: macosendpointprotectionconfiguration の更新
description: macosendpointprotectionconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd50715b1a50079dd971c528185de71240c3fcce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140188"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="1f8d0-103">macosendpointprotectionconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1f8d0-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="1f8d0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f8d0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f8d0-106">[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-106">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f8d0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f8d0-107">Prerequisites</span></span>
<span data-ttu-id="1f8d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f8d0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f8d0-110">Permission type</span></span>|<span data-ttu-id="1f8d0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f8d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f8d0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f8d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f8d0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f8d0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f8d0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f8d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f8d0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-115">Not supported.</span></span>|
|<span data-ttu-id="1f8d0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f8d0-116">Application</span></span>|<span data-ttu-id="1f8d0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f8d0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f8d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f8d0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f8d0-119">Request headers</span></span>
|<span data-ttu-id="1f8d0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f8d0-120">Header</span></span>|<span data-ttu-id="1f8d0-121">値</span><span class="sxs-lookup"><span data-stu-id="1f8d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f8d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f8d0-122">Authorization</span></span>|<span data-ttu-id="1f8d0-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f8d0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1f8d0-124">Accept</span></span>|<span data-ttu-id="1f8d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f8d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f8d0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f8d0-126">Request body</span></span>
<span data-ttu-id="1f8d0-127">要求本文で、 [macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-127">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="1f8d0-128">次の表に、 [macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-128">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="1f8d0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f8d0-129">Property</span></span>|<span data-ttu-id="1f8d0-130">型</span><span class="sxs-lookup"><span data-stu-id="1f8d0-130">Type</span></span>|<span data-ttu-id="1f8d0-131">説明</span><span class="sxs-lookup"><span data-stu-id="1f8d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f8d0-132">id</span><span class="sxs-lookup"><span data-stu-id="1f8d0-132">id</span></span>|<span data-ttu-id="1f8d0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1f8d0-133">String</span></span>|<span data-ttu-id="1f8d0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-134">Key of the entity.</span></span> <span data-ttu-id="1f8d0-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8d0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1f8d0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8d0-137">DateTimeOffset</span></span>|<span data-ttu-id="1f8d0-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1f8d0-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f8d0-140">roleScopeTagIds</span></span>|<span data-ttu-id="1f8d0-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1f8d0-141">String collection</span></span>|<span data-ttu-id="1f8d0-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f8d0-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1f8d0-144">supportsScopeTags</span></span>|<span data-ttu-id="1f8d0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8d0-145">Boolean</span></span>|<span data-ttu-id="1f8d0-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1f8d0-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1f8d0-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1f8d0-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-149">This property is read-only.</span></span> <span data-ttu-id="1f8d0-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8d0-151">createdDateTime</span></span>|<span data-ttu-id="1f8d0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8d0-152">DateTimeOffset</span></span>|<span data-ttu-id="1f8d0-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-153">DateTime the object was created.</span></span> <span data-ttu-id="1f8d0-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-155">説明</span><span class="sxs-lookup"><span data-stu-id="1f8d0-155">description</span></span>|<span data-ttu-id="1f8d0-156">String</span><span class="sxs-lookup"><span data-stu-id="1f8d0-156">String</span></span>|<span data-ttu-id="1f8d0-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f8d0-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1f8d0-159">displayName</span></span>|<span data-ttu-id="1f8d0-160">String</span><span class="sxs-lookup"><span data-stu-id="1f8d0-160">String</span></span>|<span data-ttu-id="1f8d0-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f8d0-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-163">version</span><span class="sxs-lookup"><span data-stu-id="1f8d0-163">version</span></span>|<span data-ttu-id="1f8d0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1f8d0-164">Int32</span></span>|<span data-ttu-id="1f8d0-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-165">Version of the device configuration.</span></span> <span data-ttu-id="1f8d0-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1f8d0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f8d0-167">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="1f8d0-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="1f8d0-168">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="1f8d0-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="1f8d0-169">macOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="1f8d0-170">使用可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="1f8d0-171">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="1f8d0-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="1f8d0-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8d0-172">Boolean</span></span>|<span data-ttu-id="1f8d0-173">true に設定されている場合、ゲートキーパーのユーザーオーバーライドは無効になります。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="1f8d0-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="1f8d0-174">firewallEnabled</span></span>|<span data-ttu-id="1f8d0-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8d0-175">Boolean</span></span>|<span data-ttu-id="1f8d0-176">ファイアウォールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="1f8d0-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="1f8d0-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="1f8d0-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8d0-178">Boolean</span></span>|<span data-ttu-id="1f8d0-179">[着信接続をすべてブロックする] オプションに対応しています。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="1f8d0-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="1f8d0-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="1f8d0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f8d0-181">Boolean</span></span>|<span data-ttu-id="1f8d0-182">[ステルスモードを有効にする] に相当します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="1f8d0-183">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="1f8d0-183">firewallApplications</span></span>|<span data-ttu-id="1f8d0-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f8d0-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="1f8d0-185">ファイアウォール設定のあるアプリケーションの一覧。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-185">List of applications with firewall settings.</span></span> <span data-ttu-id="1f8d0-186">この一覧にないアプリケーションのファイアウォール設定は、ユーザーによって決まります。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="1f8d0-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1f8d0-188">応答</span><span class="sxs-lookup"><span data-stu-id="1f8d0-188">Response</span></span>
<span data-ttu-id="1f8d0-189">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-189">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f8d0-190">例</span><span class="sxs-lookup"><span data-stu-id="1f8d0-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f8d0-191">要求</span><span class="sxs-lookup"><span data-stu-id="1f8d0-191">Request</span></span>
<span data-ttu-id="1f8d0-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="1f8d0-193">応答</span><span class="sxs-lookup"><span data-stu-id="1f8d0-193">Response</span></span>
<span data-ttu-id="1f8d0-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f8d0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




