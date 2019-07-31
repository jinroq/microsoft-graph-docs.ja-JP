---
title: AndroidEnterpriseWiFiConfiguration を作成する
description: 新しい androidEnterpriseWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5061155a7a3e4d8eac37116b39ada81c74fbfc32
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957956"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="24fbd-103">AndroidEnterpriseWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="24fbd-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="24fbd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24fbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24fbd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24fbd-106">新しい[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24fbd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="24fbd-107">Prerequisites</span></span>
<span data-ttu-id="24fbd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24fbd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24fbd-110">Permission type</span></span>|<span data-ttu-id="24fbd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24fbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24fbd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24fbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24fbd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fbd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24fbd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24fbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24fbd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24fbd-115">Not supported.</span></span>|
|<span data-ttu-id="24fbd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24fbd-116">Application</span></span>|<span data-ttu-id="24fbd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24fbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24fbd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24fbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="24fbd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24fbd-119">Request headers</span></span>
|<span data-ttu-id="24fbd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24fbd-120">Header</span></span>|<span data-ttu-id="24fbd-121">値</span><span class="sxs-lookup"><span data-stu-id="24fbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24fbd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24fbd-122">Authorization</span></span>|<span data-ttu-id="24fbd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24fbd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="24fbd-124">Accept</span></span>|<span data-ttu-id="24fbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24fbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24fbd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="24fbd-126">Request body</span></span>
<span data-ttu-id="24fbd-127">要求本文で、androidEnterpriseWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="24fbd-128">次の表に、androidEnterpriseWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="24fbd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24fbd-129">Property</span></span>|<span data-ttu-id="24fbd-130">型</span><span class="sxs-lookup"><span data-stu-id="24fbd-130">Type</span></span>|<span data-ttu-id="24fbd-131">説明</span><span class="sxs-lookup"><span data-stu-id="24fbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24fbd-132">id</span><span class="sxs-lookup"><span data-stu-id="24fbd-132">id</span></span>|<span data-ttu-id="24fbd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="24fbd-133">String</span></span>|<span data-ttu-id="24fbd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="24fbd-134">Key of the entity.</span></span> <span data-ttu-id="24fbd-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24fbd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="24fbd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24fbd-137">DateTimeOffset</span></span>|<span data-ttu-id="24fbd-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="24fbd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="24fbd-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24fbd-140">roleScopeTagIds</span></span>|<span data-ttu-id="24fbd-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="24fbd-141">String collection</span></span>|<span data-ttu-id="24fbd-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="24fbd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="24fbd-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="24fbd-144">supportsScopeTags</span></span>|<span data-ttu-id="24fbd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="24fbd-145">Boolean</span></span>|<span data-ttu-id="24fbd-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="24fbd-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="24fbd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="24fbd-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="24fbd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="24fbd-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-149">This property is read-only.</span></span> <span data-ttu-id="24fbd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24fbd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="24fbd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24fbd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="24fbd-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="24fbd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="24fbd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24fbd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="24fbd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24fbd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="24fbd-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="24fbd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="24fbd-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="24fbd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="24fbd-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="24fbd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="24fbd-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="24fbd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="24fbd-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24fbd-163">createdDateTime</span></span>|<span data-ttu-id="24fbd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24fbd-164">DateTimeOffset</span></span>|<span data-ttu-id="24fbd-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="24fbd-165">DateTime the object was created.</span></span> <span data-ttu-id="24fbd-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-167">description</span><span class="sxs-lookup"><span data-stu-id="24fbd-167">description</span></span>|<span data-ttu-id="24fbd-168">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-168">String</span></span>|<span data-ttu-id="24fbd-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="24fbd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24fbd-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="24fbd-171">displayName</span></span>|<span data-ttu-id="24fbd-172">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-172">String</span></span>|<span data-ttu-id="24fbd-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="24fbd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24fbd-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-175">version</span><span class="sxs-lookup"><span data-stu-id="24fbd-175">version</span></span>|<span data-ttu-id="24fbd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="24fbd-176">Int32</span></span>|<span data-ttu-id="24fbd-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="24fbd-177">Version of the device configuration.</span></span> <span data-ttu-id="24fbd-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24fbd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-179">networkName</span><span class="sxs-lookup"><span data-stu-id="24fbd-179">networkName</span></span>|<span data-ttu-id="24fbd-180">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-180">String</span></span>|<span data-ttu-id="24fbd-181">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="24fbd-181">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-182">ssid</span><span class="sxs-lookup"><span data-stu-id="24fbd-182">ssid</span></span>|<span data-ttu-id="24fbd-183">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-183">String</span></span>|<span data-ttu-id="24fbd-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="24fbd-185">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-185">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-186">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="24fbd-186">connectAutomatically</span></span>|<span data-ttu-id="24fbd-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="24fbd-187">Boolean</span></span>|<span data-ttu-id="24fbd-188">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="24fbd-189">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="24fbd-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="24fbd-190">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-190">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="24fbd-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="24fbd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="24fbd-192">Boolean</span></span>|<span data-ttu-id="24fbd-193">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="24fbd-194">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-194">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="24fbd-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="24fbd-195">wiFiSecurityType</span></span>|[<span data-ttu-id="24fbd-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="24fbd-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="24fbd-197">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="24fbd-198">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="24fbd-198">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="24fbd-199">可能な値は、`open`、`wpaEnterprise`、`wpa2Enterprise` です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="24fbd-200">eapType</span><span class="sxs-lookup"><span data-stu-id="24fbd-200">eapType</span></span>|[<span data-ttu-id="24fbd-201">Androide Aptype</span><span class="sxs-lookup"><span data-stu-id="24fbd-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="24fbd-202">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="24fbd-203">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="24fbd-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="24fbd-204">authenticationMethod</span></span>|[<span data-ttu-id="24fbd-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="24fbd-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="24fbd-206">EAP の種類が PEAP または EAP-TLS に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="24fbd-207">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="24fbd-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="24fbd-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="24fbd-209">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="24fbd-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="24fbd-210">Eap タイプが EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="24fbd-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="24fbd-211">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="24fbd-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="24fbd-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="24fbd-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="24fbd-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="24fbd-214">Eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="24fbd-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="24fbd-215">可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="24fbd-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="24fbd-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="24fbd-217">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-217">String</span></span>|<span data-ttu-id="24fbd-218">Eap の種類が EAP-TLS または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="24fbd-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="24fbd-219">ここに示す文字列を使用して、Wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="24fbd-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="24fbd-220">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="24fbd-220">usernameFormatString</span></span>|<span data-ttu-id="24fbd-221">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-221">String</span></span>|<span data-ttu-id="24fbd-222">Wifi に接続するためのユーザー名を作成するために使用されるユーザー名の形式文字列</span><span class="sxs-lookup"><span data-stu-id="24fbd-222">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="24fbd-223">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="24fbd-223">passwordFormatString</span></span>|<span data-ttu-id="24fbd-224">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-224">String</span></span>|<span data-ttu-id="24fbd-225">Wifi に接続するためのパスワードを作成するために使用されるパスワード形式の文字列</span><span class="sxs-lookup"><span data-stu-id="24fbd-225">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="24fbd-226">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="24fbd-226">preSharedKey</span></span>|<span data-ttu-id="24fbd-227">String</span><span class="sxs-lookup"><span data-stu-id="24fbd-227">String</span></span>|<span data-ttu-id="24fbd-228">Wi-fi に接続するためにパスワードを作成するために使用される PreSharedKey</span><span class="sxs-lookup"><span data-stu-id="24fbd-228">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="24fbd-229">応答</span><span class="sxs-lookup"><span data-stu-id="24fbd-229">Response</span></span>
<span data-ttu-id="24fbd-230">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24fbd-230">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fbd-231">例</span><span class="sxs-lookup"><span data-stu-id="24fbd-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="24fbd-232">要求</span><span class="sxs-lookup"><span data-stu-id="24fbd-232">Request</span></span>
<span data-ttu-id="24fbd-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24fbd-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1699

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="24fbd-234">応答</span><span class="sxs-lookup"><span data-stu-id="24fbd-234">Response</span></span>
<span data-ttu-id="24fbd-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24fbd-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1871

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```





