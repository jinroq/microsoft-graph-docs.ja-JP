---
title: WindowsWifiEnterpriseEAPConfiguration を作成する
description: 新しい windowsWifiEnterpriseEAPConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b53438ab717e28688dbf9c80ce643efd5d8a6fa
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961169"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="e7ee9-103">WindowsWifiEnterpriseEAPConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="e7ee9-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="e7ee9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ee9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ee9-106">新しい[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ee9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7ee9-107">Prerequisites</span></span>
<span data-ttu-id="e7ee9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ee9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7ee9-110">Permission type</span></span>|<span data-ttu-id="e7ee9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7ee9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ee9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7ee9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ee9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ee9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7ee9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7ee9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ee9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-115">Not supported.</span></span>|
|<span data-ttu-id="e7ee9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7ee9-116">Application</span></span>|<span data-ttu-id="e7ee9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ee9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7ee9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7ee9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7ee9-119">Request headers</span></span>
|<span data-ttu-id="e7ee9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7ee9-120">Header</span></span>|<span data-ttu-id="e7ee9-121">値</span><span class="sxs-lookup"><span data-stu-id="e7ee9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ee9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7ee9-122">Authorization</span></span>|<span data-ttu-id="e7ee9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ee9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e7ee9-124">Accept</span></span>|<span data-ttu-id="e7ee9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ee9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ee9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7ee9-126">Request body</span></span>
<span data-ttu-id="e7ee9-127">要求本文で、windowsWifiEnterpriseEAPConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="e7ee9-128">次の表に、windowsWifiEnterpriseEAPConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="e7ee9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7ee9-129">Property</span></span>|<span data-ttu-id="e7ee9-130">型</span><span class="sxs-lookup"><span data-stu-id="e7ee9-130">Type</span></span>|<span data-ttu-id="e7ee9-131">説明</span><span class="sxs-lookup"><span data-stu-id="e7ee9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ee9-132">id</span><span class="sxs-lookup"><span data-stu-id="e7ee9-132">id</span></span>|<span data-ttu-id="e7ee9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e7ee9-133">String</span></span>|<span data-ttu-id="e7ee9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-134">Key of the entity.</span></span> <span data-ttu-id="e7ee9-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ee9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7ee9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ee9-137">DateTimeOffset</span></span>|<span data-ttu-id="e7ee9-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7ee9-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7ee9-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7ee9-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e7ee9-141">String collection</span></span>|<span data-ttu-id="e7ee9-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7ee9-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7ee9-144">supportsScopeTags</span></span>|<span data-ttu-id="e7ee9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-145">Boolean</span></span>|<span data-ttu-id="e7ee9-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7ee9-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7ee9-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7ee9-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-149">This property is read-only.</span></span> <span data-ttu-id="e7ee9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7ee9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7ee9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7ee9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7ee9-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7ee9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7ee9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7ee9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7ee9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7ee9-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7ee9-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e7ee9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7ee9-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e7ee9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7ee9-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7ee9-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ee9-163">createdDateTime</span></span>|<span data-ttu-id="e7ee9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ee9-164">DateTimeOffset</span></span>|<span data-ttu-id="e7ee9-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-165">DateTime the object was created.</span></span> <span data-ttu-id="e7ee9-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-167">description</span><span class="sxs-lookup"><span data-stu-id="e7ee9-167">description</span></span>|<span data-ttu-id="e7ee9-168">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-168">String</span></span>|<span data-ttu-id="e7ee9-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7ee9-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e7ee9-171">displayName</span></span>|<span data-ttu-id="e7ee9-172">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-172">String</span></span>|<span data-ttu-id="e7ee9-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7ee9-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-175">version</span><span class="sxs-lookup"><span data-stu-id="e7ee9-175">version</span></span>|<span data-ttu-id="e7ee9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-176">Int32</span></span>|<span data-ttu-id="e7ee9-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-177">Version of the device configuration.</span></span> <span data-ttu-id="e7ee9-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7ee9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e7ee9-179">preSharedKey</span></span>|<span data-ttu-id="e7ee9-180">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-180">String</span></span>|<span data-ttu-id="e7ee9-181">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="e7ee9-182">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-183">wifiSecurityType</span></span>|[<span data-ttu-id="e7ee9-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e7ee9-185">Wifi セキュリティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="e7ee9-186">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e7ee9-187">使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e7ee9-188">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="e7ee9-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="e7ee9-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="e7ee9-190">Wifi 接続の従量制課金接続制限の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="e7ee9-191">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e7ee9-192">可能な値は、`unrestricted`、`fixed`、`variable` です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="e7ee9-193">ssid</span><span class="sxs-lookup"><span data-stu-id="e7ee9-193">ssid</span></span>|<span data-ttu-id="e7ee9-194">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-194">String</span></span>|<span data-ttu-id="e7ee9-195">Wifi 接続の SSID を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="e7ee9-196">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-197">networkName</span><span class="sxs-lookup"><span data-stu-id="e7ee9-197">networkName</span></span>|<span data-ttu-id="e7ee9-198">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-198">String</span></span>|<span data-ttu-id="e7ee9-199">ネットワーク構成名を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-199">Specify the network configuration name.</span></span> <span data-ttu-id="e7ee9-200">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-201">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="e7ee9-201">connectAutomatically</span></span>|<span data-ttu-id="e7ee9-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-202">Boolean</span></span>|<span data-ttu-id="e7ee9-203">範囲内で wifi 接続を自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="e7ee9-204">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-205">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="e7ee9-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="e7ee9-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-206">Boolean</span></span>|<span data-ttu-id="e7ee9-207">この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="e7ee9-208">ConnectAutomatically 自動的に true になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="e7ee9-209">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-210">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e7ee9-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e7ee9-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-211">Boolean</span></span>|<span data-ttu-id="e7ee9-212">SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="e7ee9-213">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-214">proxySetting</span><span class="sxs-lookup"><span data-stu-id="e7ee9-214">proxySetting</span></span>|[<span data-ttu-id="e7ee9-215">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e7ee9-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e7ee9-216">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承した wi-fi 構成のプロキシ設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e7ee9-217">可能な値は、`none`、`manual`、`automatic` です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e7ee9-218">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e7ee9-218">proxyManualAddress</span></span>|<span data-ttu-id="e7ee9-219">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-219">String</span></span>|<span data-ttu-id="e7ee9-220">プロキシサーバーの IP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="e7ee9-221">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-222">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e7ee9-222">proxyManualPort</span></span>|<span data-ttu-id="e7ee9-223">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-223">Int32</span></span>|<span data-ttu-id="e7ee9-224">プロキシサーバーのポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="e7ee9-225">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-226">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e7ee9-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e7ee9-227">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-227">String</span></span>|<span data-ttu-id="e7ee9-228">プロキシサーバー構成スクリプトの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="e7ee9-229">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-230">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="e7ee9-230">forceFIPSCompliance</span></span>|<span data-ttu-id="e7ee9-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-231">Boolean</span></span>|<span data-ttu-id="e7ee9-232">FIPS 準拠を強制するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="e7ee9-233">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e7ee9-234">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="e7ee9-234">networkSingleSignOn</span></span>|[<span data-ttu-id="e7ee9-235">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="e7ee9-236">ネットワークのシングルサインオンの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-236">Specify the network single sign on type.</span></span> <span data-ttu-id="e7ee9-237">可能な値は、`disabled`、`prelogon`、`postlogon` です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="e7ee9-238">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="e7ee9-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="e7ee9-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-239">Int32</span></span>|<span data-ttu-id="e7ee9-240">[最大認証タイムアウト (秒)] を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="e7ee9-241">有効な範囲: 1-120</span><span class="sxs-lookup"><span data-stu-id="e7ee9-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="e7ee9-242">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="e7ee9-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="e7ee9-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-243">Boolean</span></span>|<span data-ttu-id="e7ee9-244">Wifi 接続で追加の認証資格情報を求めるメッセージを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="e7ee9-245">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="e7ee9-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="e7ee9-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-246">Boolean</span></span>|<span data-ttu-id="e7ee9-247">Wifi 接続で、ペアワイズマスターキーのキャッシュを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="e7ee9-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="e7ee9-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="e7ee9-249">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-249">Int32</span></span>|<span data-ttu-id="e7ee9-250">最大ペアワイズマスターキーキャッシュ時間を指定します (分単位)。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="e7ee9-251">有効な範囲: 5-1440</span><span class="sxs-lookup"><span data-stu-id="e7ee9-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="e7ee9-252">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="e7ee9-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="e7ee9-253">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-253">Int32</span></span>|<span data-ttu-id="e7ee9-254">キャッシュ内のペアワイズマスターキーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="e7ee9-255">有効な範囲: 1-255</span><span class="sxs-lookup"><span data-stu-id="e7ee9-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="e7ee9-256">enablePreAuthentication 認証</span><span class="sxs-lookup"><span data-stu-id="e7ee9-256">enablePreAuthentication</span></span>|<span data-ttu-id="e7ee9-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee9-257">Boolean</span></span>|<span data-ttu-id="e7ee9-258">事前認証を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="e7ee9-259">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="e7ee9-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="e7ee9-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ee9-260">Int32</span></span>|<span data-ttu-id="e7ee9-261">事前認証の最大試行回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="e7ee9-262">有効な範囲: 1-16</span><span class="sxs-lookup"><span data-stu-id="e7ee9-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="e7ee9-263">eapType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-263">eapType</span></span>|[<span data-ttu-id="e7ee9-264">eapType</span><span class="sxs-lookup"><span data-stu-id="e7ee9-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="e7ee9-265">拡張認証プロトコル (EAP)。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="e7ee9-266">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="e7ee9-267">使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="e7ee9-268">Trustedserverの形式</span><span class="sxs-lookup"><span data-stu-id="e7ee9-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="e7ee9-269">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e7ee9-269">String collection</span></span>|<span data-ttu-id="e7ee9-270">信頼されたサーバー証明書の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="e7ee9-271">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7ee9-271">authenticationMethod</span></span>|[<span data-ttu-id="e7ee9-272">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7ee9-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="e7ee9-273">認証方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-273">Specify the authentication method.</span></span> <span data-ttu-id="e7ee9-274">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7ee9-275">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="e7ee9-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="e7ee9-276">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="e7ee9-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="e7ee9-277">EAP TTLS の内部認証プロトコルを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="e7ee9-278">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="e7ee9-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="e7ee9-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="e7ee9-280">String</span><span class="sxs-lookup"><span data-stu-id="e7ee9-280">String</span></span>|<span data-ttu-id="e7ee9-281">EAP TTLS または PEAP を使用している場合は、プライバシー保護のために、ユーザー名を置換する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="e7ee9-282">応答</span><span class="sxs-lookup"><span data-stu-id="e7ee9-282">Response</span></span>
<span data-ttu-id="e7ee9-283">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-283">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ee9-284">例</span><span class="sxs-lookup"><span data-stu-id="e7ee9-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ee9-285">要求</span><span class="sxs-lookup"><span data-stu-id="e7ee9-285">Request</span></span>
<span data-ttu-id="e7ee9-286">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2277

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="e7ee9-287">応答</span><span class="sxs-lookup"><span data-stu-id="e7ee9-287">Response</span></span>
<span data-ttu-id="e7ee9-p134">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7ee9-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2449

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





