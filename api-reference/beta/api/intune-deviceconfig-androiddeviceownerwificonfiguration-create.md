---
title: AndroidDeviceOwnerWiFiConfiguration を作成する
description: 新しい androidDeviceOwnerWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73c0ec47f811270479cb4b86df169a3cd867ff7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958096"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="8ae94-103">AndroidDeviceOwnerWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="8ae94-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="8ae94-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ae94-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ae94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae94-106">新しい[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ae94-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ae94-107">Prerequisites</span></span>
<span data-ttu-id="8ae94-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ae94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ae94-110">Permission type</span></span>|<span data-ttu-id="8ae94-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ae94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ae94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ae94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae94-115">Not supported.</span></span>|
|<span data-ttu-id="8ae94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ae94-116">Application</span></span>|<span data-ttu-id="8ae94-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ae94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ae94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae94-119">Request headers</span></span>
|<span data-ttu-id="8ae94-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae94-120">Header</span></span>|<span data-ttu-id="8ae94-121">値</span><span class="sxs-lookup"><span data-stu-id="8ae94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae94-122">Authorization</span></span>|<span data-ttu-id="8ae94-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ae94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae94-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8ae94-124">Accept</span></span>|<span data-ttu-id="8ae94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae94-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ae94-126">Request body</span></span>
<span data-ttu-id="8ae94-127">要求本文で、androidDeviceOwnerWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="8ae94-128">次の表に、androidDeviceOwnerWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="8ae94-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ae94-129">Property</span></span>|<span data-ttu-id="8ae94-130">型</span><span class="sxs-lookup"><span data-stu-id="8ae94-130">Type</span></span>|<span data-ttu-id="8ae94-131">説明</span><span class="sxs-lookup"><span data-stu-id="8ae94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae94-132">id</span><span class="sxs-lookup"><span data-stu-id="8ae94-132">id</span></span>|<span data-ttu-id="8ae94-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8ae94-133">String</span></span>|<span data-ttu-id="8ae94-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8ae94-134">Key of the entity.</span></span> <span data-ttu-id="8ae94-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8ae94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae94-137">DateTimeOffset</span></span>|<span data-ttu-id="8ae94-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8ae94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8ae94-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ae94-140">roleScopeTagIds</span></span>|<span data-ttu-id="8ae94-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8ae94-141">String collection</span></span>|<span data-ttu-id="8ae94-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8ae94-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ae94-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ae94-144">supportsScopeTags</span></span>|<span data-ttu-id="8ae94-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae94-145">Boolean</span></span>|<span data-ttu-id="8ae94-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ae94-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8ae94-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ae94-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8ae94-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ae94-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-149">This property is read-only.</span></span> <span data-ttu-id="8ae94-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ae94-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ae94-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ae94-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ae94-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="8ae94-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ae94-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ae94-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ae94-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ae94-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ae94-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8ae94-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ae94-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8ae94-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ae94-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8ae94-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ae94-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8ae94-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ae94-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae94-163">createdDateTime</span></span>|<span data-ttu-id="8ae94-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae94-164">DateTimeOffset</span></span>|<span data-ttu-id="8ae94-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8ae94-165">DateTime the object was created.</span></span> <span data-ttu-id="8ae94-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-167">description</span><span class="sxs-lookup"><span data-stu-id="8ae94-167">description</span></span>|<span data-ttu-id="8ae94-168">String</span><span class="sxs-lookup"><span data-stu-id="8ae94-168">String</span></span>|<span data-ttu-id="8ae94-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8ae94-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ae94-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8ae94-171">displayName</span></span>|<span data-ttu-id="8ae94-172">String</span><span class="sxs-lookup"><span data-stu-id="8ae94-172">String</span></span>|<span data-ttu-id="8ae94-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8ae94-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ae94-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-175">version</span><span class="sxs-lookup"><span data-stu-id="8ae94-175">version</span></span>|<span data-ttu-id="8ae94-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae94-176">Int32</span></span>|<span data-ttu-id="8ae94-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8ae94-177">Version of the device configuration.</span></span> <span data-ttu-id="8ae94-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ae94-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae94-179">networkName</span><span class="sxs-lookup"><span data-stu-id="8ae94-179">networkName</span></span>|<span data-ttu-id="8ae94-180">String</span><span class="sxs-lookup"><span data-stu-id="8ae94-180">String</span></span>|<span data-ttu-id="8ae94-181">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="8ae94-181">Network Name</span></span>|
|<span data-ttu-id="8ae94-182">ssid</span><span class="sxs-lookup"><span data-stu-id="8ae94-182">ssid</span></span>|<span data-ttu-id="8ae94-183">String</span><span class="sxs-lookup"><span data-stu-id="8ae94-183">String</span></span>|<span data-ttu-id="8ae94-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="8ae94-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="8ae94-185">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="8ae94-185">connectAutomatically</span></span>|<span data-ttu-id="8ae94-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae94-186">Boolean</span></span>|<span data-ttu-id="8ae94-187">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8ae94-188">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="8ae94-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="8ae94-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="8ae94-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8ae94-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae94-190">Boolean</span></span>|<span data-ttu-id="8ae94-191">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="8ae94-192">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8ae94-192">wiFiSecurityType</span></span>|[<span data-ttu-id="8ae94-193">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8ae94-193">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="8ae94-194">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8ae94-195">使用可能な値は、`open`、`wep`、`wpaPersonal`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="8ae94-195">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="8ae94-196">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="8ae94-196">preSharedKey</span></span>|<span data-ttu-id="8ae94-197">String</span><span class="sxs-lookup"><span data-stu-id="8ae94-197">String</span></span>|<span data-ttu-id="8ae94-198">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="8ae94-198">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="8ae94-199">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="8ae94-199">preSharedKeyIsSet</span></span>|<span data-ttu-id="8ae94-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae94-200">Boolean</span></span>|<span data-ttu-id="8ae94-201">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="8ae94-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="8ae94-202">応答</span><span class="sxs-lookup"><span data-stu-id="8ae94-202">Response</span></span>
<span data-ttu-id="8ae94-203">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ae94-203">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae94-204">例</span><span class="sxs-lookup"><span data-stu-id="8ae94-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ae94-205">要求</span><span class="sxs-lookup"><span data-stu-id="8ae94-205">Request</span></span>
<span data-ttu-id="8ae94-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ae94-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1282

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="8ae94-207">応答</span><span class="sxs-lookup"><span data-stu-id="8ae94-207">Response</span></span>
<span data-ttu-id="8ae94-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ae94-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1454

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





