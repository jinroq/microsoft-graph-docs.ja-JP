---
title: AndroidForWorkEnterpriseWiFiConfiguration の更新
description: AndroidForWorkEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6706c637a625e07f69fd5db5cc4846af3cf7e03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963676"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="73994-103">AndroidForWorkEnterpriseWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="73994-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="73994-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73994-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73994-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73994-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73994-106">[AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="73994-106">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73994-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="73994-107">Prerequisites</span></span>
<span data-ttu-id="73994-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73994-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73994-110">Permission type</span></span>|<span data-ttu-id="73994-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="73994-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73994-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73994-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73994-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73994-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73994-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73994-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73994-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73994-115">Not supported.</span></span>|
|<span data-ttu-id="73994-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73994-116">Application</span></span>|<span data-ttu-id="73994-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73994-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73994-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73994-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="73994-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73994-119">Request headers</span></span>
|<span data-ttu-id="73994-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73994-120">Header</span></span>|<span data-ttu-id="73994-121">値</span><span class="sxs-lookup"><span data-stu-id="73994-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73994-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73994-122">Authorization</span></span>|<span data-ttu-id="73994-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="73994-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73994-124">承諾</span><span class="sxs-lookup"><span data-stu-id="73994-124">Accept</span></span>|<span data-ttu-id="73994-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73994-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73994-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="73994-126">Request body</span></span>
<span data-ttu-id="73994-127">要求本文で、 [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="73994-127">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="73994-128">次の表に、 [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="73994-128">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="73994-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73994-129">Property</span></span>|<span data-ttu-id="73994-130">型</span><span class="sxs-lookup"><span data-stu-id="73994-130">Type</span></span>|<span data-ttu-id="73994-131">説明</span><span class="sxs-lookup"><span data-stu-id="73994-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73994-132">id</span><span class="sxs-lookup"><span data-stu-id="73994-132">id</span></span>|<span data-ttu-id="73994-133">文字列</span><span class="sxs-lookup"><span data-stu-id="73994-133">String</span></span>|<span data-ttu-id="73994-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="73994-134">Key of the entity.</span></span> <span data-ttu-id="73994-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73994-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73994-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73994-137">DateTimeOffset</span></span>|<span data-ttu-id="73994-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="73994-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73994-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73994-140">roleScopeTagIds</span></span>|<span data-ttu-id="73994-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="73994-141">String collection</span></span>|<span data-ttu-id="73994-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="73994-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73994-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73994-144">supportsScopeTags</span></span>|<span data-ttu-id="73994-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="73994-145">Boolean</span></span>|<span data-ttu-id="73994-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="73994-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73994-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="73994-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73994-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="73994-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73994-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="73994-149">This property is read-only.</span></span> <span data-ttu-id="73994-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73994-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="73994-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73994-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="73994-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="73994-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="73994-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73994-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="73994-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73994-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="73994-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="73994-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="73994-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="73994-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="73994-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="73994-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="73994-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="73994-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="73994-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73994-163">createdDateTime</span></span>|<span data-ttu-id="73994-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73994-164">DateTimeOffset</span></span>|<span data-ttu-id="73994-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="73994-165">DateTime the object was created.</span></span> <span data-ttu-id="73994-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-167">description</span><span class="sxs-lookup"><span data-stu-id="73994-167">description</span></span>|<span data-ttu-id="73994-168">String</span><span class="sxs-lookup"><span data-stu-id="73994-168">String</span></span>|<span data-ttu-id="73994-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="73994-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73994-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-171">displayName</span><span class="sxs-lookup"><span data-stu-id="73994-171">displayName</span></span>|<span data-ttu-id="73994-172">String</span><span class="sxs-lookup"><span data-stu-id="73994-172">String</span></span>|<span data-ttu-id="73994-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="73994-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73994-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-175">version</span><span class="sxs-lookup"><span data-stu-id="73994-175">version</span></span>|<span data-ttu-id="73994-176">Int32</span><span class="sxs-lookup"><span data-stu-id="73994-176">Int32</span></span>|<span data-ttu-id="73994-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="73994-177">Version of the device configuration.</span></span> <span data-ttu-id="73994-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73994-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73994-179">networkName</span><span class="sxs-lookup"><span data-stu-id="73994-179">networkName</span></span>|<span data-ttu-id="73994-180">String</span><span class="sxs-lookup"><span data-stu-id="73994-180">String</span></span>|<span data-ttu-id="73994-181">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="73994-181">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="73994-182">ssid</span><span class="sxs-lookup"><span data-stu-id="73994-182">ssid</span></span>|<span data-ttu-id="73994-183">String</span><span class="sxs-lookup"><span data-stu-id="73994-183">String</span></span>|<span data-ttu-id="73994-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="73994-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="73994-185">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="73994-185">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="73994-186">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="73994-186">connectAutomatically</span></span>|<span data-ttu-id="73994-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="73994-187">Boolean</span></span>|<span data-ttu-id="73994-188">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="73994-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="73994-189">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="73994-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="73994-190">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="73994-190">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="73994-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="73994-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="73994-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="73994-192">Boolean</span></span>|<span data-ttu-id="73994-193">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="73994-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="73994-194">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="73994-194">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="73994-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="73994-195">wiFiSecurityType</span></span>|[<span data-ttu-id="73994-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="73994-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="73994-197">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="73994-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="73994-198">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="73994-198">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="73994-199">可能な値は、`open`、`wpaEnterprise`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="73994-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="73994-200">eapType</span><span class="sxs-lookup"><span data-stu-id="73994-200">eapType</span></span>|[<span data-ttu-id="73994-201">Androide Aptype</span><span class="sxs-lookup"><span data-stu-id="73994-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="73994-202">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="73994-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="73994-203">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="73994-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="73994-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73994-204">authenticationMethod</span></span>|[<span data-ttu-id="73994-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73994-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="73994-206">EAP の種類が PEAP または EAP-TLS に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="73994-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="73994-207">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="73994-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="73994-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="73994-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="73994-209">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="73994-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="73994-210">Eap タイプが EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="73994-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="73994-211">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="73994-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="73994-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="73994-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="73994-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="73994-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="73994-214">Eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="73994-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="73994-215">可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="73994-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="73994-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="73994-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="73994-217">String</span><span class="sxs-lookup"><span data-stu-id="73994-217">String</span></span>|<span data-ttu-id="73994-218">Eap の種類が EAP-TLS または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="73994-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="73994-219">ここに示す文字列を使用して、Wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="73994-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="73994-220">応答</span><span class="sxs-lookup"><span data-stu-id="73994-220">Response</span></span>
<span data-ttu-id="73994-221">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73994-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73994-222">例</span><span class="sxs-lookup"><span data-stu-id="73994-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="73994-223">要求</span><span class="sxs-lookup"><span data-stu-id="73994-223">Request</span></span>
<span data-ttu-id="73994-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73994-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="73994-225">応答</span><span class="sxs-lookup"><span data-stu-id="73994-225">Response</span></span>
<span data-ttu-id="73994-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73994-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





