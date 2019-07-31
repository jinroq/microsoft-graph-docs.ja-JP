---
title: Windows10NetworkBoundaryConfiguration を作成する
description: 新しい windows10NetworkBoundaryConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a06010b80c8cc45598c2e2b0131bb4fa8395af57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977322"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="ecca3-103">Windows10NetworkBoundaryConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="ecca3-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="ecca3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecca3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecca3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecca3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecca3-106">新しい[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-106">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecca3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ecca3-107">Prerequisites</span></span>
<span data-ttu-id="ecca3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecca3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecca3-110">Permission type</span></span>|<span data-ttu-id="ecca3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecca3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecca3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecca3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecca3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecca3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ecca3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecca3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecca3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecca3-115">Not supported.</span></span>|
|<span data-ttu-id="ecca3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecca3-116">Application</span></span>|<span data-ttu-id="ecca3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecca3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecca3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecca3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecca3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecca3-119">Request headers</span></span>
|<span data-ttu-id="ecca3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecca3-120">Header</span></span>|<span data-ttu-id="ecca3-121">値</span><span class="sxs-lookup"><span data-stu-id="ecca3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecca3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecca3-122">Authorization</span></span>|<span data-ttu-id="ecca3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecca3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecca3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ecca3-124">Accept</span></span>|<span data-ttu-id="ecca3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecca3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecca3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecca3-126">Request body</span></span>
<span data-ttu-id="ecca3-127">要求本文で、windows10NetworkBoundaryConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-127">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="ecca3-128">次の表に、windows10NetworkBoundaryConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-128">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="ecca3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecca3-129">Property</span></span>|<span data-ttu-id="ecca3-130">型</span><span class="sxs-lookup"><span data-stu-id="ecca3-130">Type</span></span>|<span data-ttu-id="ecca3-131">説明</span><span class="sxs-lookup"><span data-stu-id="ecca3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecca3-132">id</span><span class="sxs-lookup"><span data-stu-id="ecca3-132">id</span></span>|<span data-ttu-id="ecca3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ecca3-133">String</span></span>|<span data-ttu-id="ecca3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ecca3-134">Key of the entity.</span></span> <span data-ttu-id="ecca3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecca3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ecca3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecca3-137">DateTimeOffset</span></span>|<span data-ttu-id="ecca3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ecca3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ecca3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecca3-140">roleScopeTagIds</span></span>|<span data-ttu-id="ecca3-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ecca3-141">String collection</span></span>|<span data-ttu-id="ecca3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ecca3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ecca3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ecca3-144">supportsScopeTags</span></span>|<span data-ttu-id="ecca3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecca3-145">Boolean</span></span>|<span data-ttu-id="ecca3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ecca3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ecca3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ecca3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ecca3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ecca3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-149">This property is read-only.</span></span> <span data-ttu-id="ecca3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ecca3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ecca3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ecca3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ecca3-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ecca3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ecca3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ecca3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ecca3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ecca3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ecca3-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ecca3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ecca3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ecca3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ecca3-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ecca3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ecca3-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ecca3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ecca3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecca3-163">createdDateTime</span></span>|<span data-ttu-id="ecca3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecca3-164">DateTimeOffset</span></span>|<span data-ttu-id="ecca3-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ecca3-165">DateTime the object was created.</span></span> <span data-ttu-id="ecca3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-167">description</span><span class="sxs-lookup"><span data-stu-id="ecca3-167">description</span></span>|<span data-ttu-id="ecca3-168">String</span><span class="sxs-lookup"><span data-stu-id="ecca3-168">String</span></span>|<span data-ttu-id="ecca3-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ecca3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ecca3-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ecca3-171">displayName</span></span>|<span data-ttu-id="ecca3-172">String</span><span class="sxs-lookup"><span data-stu-id="ecca3-172">String</span></span>|<span data-ttu-id="ecca3-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ecca3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ecca3-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-175">version</span><span class="sxs-lookup"><span data-stu-id="ecca3-175">version</span></span>|<span data-ttu-id="ecca3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ecca3-176">Int32</span></span>|<span data-ttu-id="ecca3-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ecca3-177">Version of the device configuration.</span></span> <span data-ttu-id="ecca3-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ecca3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecca3-179">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ecca3-179">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="ecca3-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ecca3-180">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="ecca3-181">Windows ネットワーク分離ポリシー</span><span class="sxs-lookup"><span data-stu-id="ecca3-181">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="ecca3-182">応答</span><span class="sxs-lookup"><span data-stu-id="ecca3-182">Response</span></span>
<span data-ttu-id="ecca3-183">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ecca3-183">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecca3-184">例</span><span class="sxs-lookup"><span data-stu-id="ecca3-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecca3-185">要求</span><span class="sxs-lookup"><span data-stu-id="ecca3-185">Request</span></span>
<span data-ttu-id="ecca3-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecca3-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="ecca3-187">応答</span><span class="sxs-lookup"><span data-stu-id="ecca3-187">Response</span></span>
<span data-ttu-id="ecca3-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ecca3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```





