---
title: AndroidDeviceOwnerEnterpriseWiFiConfiguration を作成する
description: 新しい androidDeviceOwnerEnterpriseWiFiConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8feef3038fd397ce3dfd51cab45226dbdb3dce1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317011"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="78d55-103">AndroidDeviceOwnerEnterpriseWiFiConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="78d55-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="78d55-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78d55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78d55-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78d55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78d55-106">新しい[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="78d55-106">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78d55-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="78d55-107">Prerequisites</span></span>
<span data-ttu-id="78d55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78d55-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78d55-110">Permission type</span></span>|<span data-ttu-id="78d55-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78d55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78d55-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78d55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78d55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78d55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78d55-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78d55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78d55-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78d55-115">Not supported.</span></span>|
|<span data-ttu-id="78d55-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78d55-116">Application</span></span>|<span data-ttu-id="78d55-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78d55-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78d55-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78d55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="78d55-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78d55-119">Request headers</span></span>
|<span data-ttu-id="78d55-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78d55-120">Header</span></span>|<span data-ttu-id="78d55-121">値</span><span class="sxs-lookup"><span data-stu-id="78d55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78d55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78d55-122">Authorization</span></span>|<span data-ttu-id="78d55-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="78d55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78d55-124">承諾</span><span class="sxs-lookup"><span data-stu-id="78d55-124">Accept</span></span>|<span data-ttu-id="78d55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78d55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78d55-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="78d55-126">Request body</span></span>
<span data-ttu-id="78d55-127">要求本文で、androidDeviceOwnerEnterpriseWiFiConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78d55-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="78d55-128">次の表に、androidDeviceOwnerEnterpriseWiFiConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78d55-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="78d55-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78d55-129">Property</span></span>|<span data-ttu-id="78d55-130">型</span><span class="sxs-lookup"><span data-stu-id="78d55-130">Type</span></span>|<span data-ttu-id="78d55-131">説明</span><span class="sxs-lookup"><span data-stu-id="78d55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d55-132">id</span><span class="sxs-lookup"><span data-stu-id="78d55-132">id</span></span>|<span data-ttu-id="78d55-133">文字列</span><span class="sxs-lookup"><span data-stu-id="78d55-133">String</span></span>|<span data-ttu-id="78d55-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78d55-134">Key of the entity.</span></span> <span data-ttu-id="78d55-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78d55-136">lastModifiedDateTime</span></span>|<span data-ttu-id="78d55-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d55-137">DateTimeOffset</span></span>|<span data-ttu-id="78d55-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="78d55-138">DateTime the object was last modified.</span></span> <span data-ttu-id="78d55-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78d55-140">roleScopeTagIds</span></span>|<span data-ttu-id="78d55-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="78d55-141">String collection</span></span>|<span data-ttu-id="78d55-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="78d55-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="78d55-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="78d55-144">supportsScopeTags</span></span>|<span data-ttu-id="78d55-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d55-145">Boolean</span></span>|<span data-ttu-id="78d55-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78d55-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="78d55-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="78d55-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="78d55-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="78d55-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="78d55-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="78d55-149">This property is read-only.</span></span> <span data-ttu-id="78d55-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="78d55-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="78d55-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="78d55-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="78d55-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="78d55-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="78d55-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="78d55-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="78d55-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="78d55-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="78d55-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="78d55-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="78d55-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="78d55-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="78d55-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="78d55-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="78d55-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="78d55-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="78d55-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78d55-163">createdDateTime</span></span>|<span data-ttu-id="78d55-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d55-164">DateTimeOffset</span></span>|<span data-ttu-id="78d55-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="78d55-165">DateTime the object was created.</span></span> <span data-ttu-id="78d55-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-167">description</span><span class="sxs-lookup"><span data-stu-id="78d55-167">description</span></span>|<span data-ttu-id="78d55-168">String</span><span class="sxs-lookup"><span data-stu-id="78d55-168">String</span></span>|<span data-ttu-id="78d55-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="78d55-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="78d55-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-171">displayName</span><span class="sxs-lookup"><span data-stu-id="78d55-171">displayName</span></span>|<span data-ttu-id="78d55-172">String</span><span class="sxs-lookup"><span data-stu-id="78d55-172">String</span></span>|<span data-ttu-id="78d55-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="78d55-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="78d55-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-175">version</span><span class="sxs-lookup"><span data-stu-id="78d55-175">version</span></span>|<span data-ttu-id="78d55-176">Int32</span><span class="sxs-lookup"><span data-stu-id="78d55-176">Int32</span></span>|<span data-ttu-id="78d55-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="78d55-177">Version of the device configuration.</span></span> <span data-ttu-id="78d55-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78d55-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78d55-179">networkName</span><span class="sxs-lookup"><span data-stu-id="78d55-179">networkName</span></span>|<span data-ttu-id="78d55-180">String</span><span class="sxs-lookup"><span data-stu-id="78d55-180">String</span></span>|<span data-ttu-id="78d55-181">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="78d55-181">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-182">ssid</span><span class="sxs-lookup"><span data-stu-id="78d55-182">ssid</span></span>|<span data-ttu-id="78d55-183">String</span><span class="sxs-lookup"><span data-stu-id="78d55-183">String</span></span>|<span data-ttu-id="78d55-184">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="78d55-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="78d55-185">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78d55-185">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-186">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="78d55-186">connectAutomatically</span></span>|<span data-ttu-id="78d55-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d55-187">Boolean</span></span>|<span data-ttu-id="78d55-188">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="78d55-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="78d55-189">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="78d55-190">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78d55-190">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="78d55-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="78d55-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d55-192">Boolean</span></span>|<span data-ttu-id="78d55-193">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="78d55-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="78d55-194">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78d55-194">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="78d55-195">wiFiSecurityType</span></span>|[<span data-ttu-id="78d55-196">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="78d55-196">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="78d55-197">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78d55-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="78d55-198">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-198">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="78d55-199">使用可能な値は、`open`、`wep`、`wpaPersonal`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="78d55-199">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="78d55-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="78d55-200">preSharedKey</span></span>|<span data-ttu-id="78d55-201">String</span><span class="sxs-lookup"><span data-stu-id="78d55-201">String</span></span>|<span data-ttu-id="78d55-202">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="78d55-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="78d55-203">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78d55-203">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-204">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="78d55-204">preSharedKeyIsSet</span></span>|<span data-ttu-id="78d55-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d55-205">Boolean</span></span>|<span data-ttu-id="78d55-206">これは、WPA 個人用 Wi-fi ネットワークの事前共有キーです。</span><span class="sxs-lookup"><span data-stu-id="78d55-206">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="78d55-207">[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78d55-207">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="78d55-208">eapType</span><span class="sxs-lookup"><span data-stu-id="78d55-208">eapType</span></span>|[<span data-ttu-id="78d55-209">Androide Aptype</span><span class="sxs-lookup"><span data-stu-id="78d55-209">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="78d55-210">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="78d55-210">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="78d55-211">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="78d55-211">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="78d55-212">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78d55-212">authenticationMethod</span></span>|[<span data-ttu-id="78d55-213">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78d55-213">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="78d55-214">EAP の種類が PEAP または EAP-TLS に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="78d55-214">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="78d55-215">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="78d55-215">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="78d55-216">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="78d55-216">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="78d55-217">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="78d55-217">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="78d55-218">Eap タイプが EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="78d55-218">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="78d55-219">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="78d55-219">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="78d55-220">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="78d55-220">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="78d55-221">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="78d55-221">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="78d55-222">Eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="78d55-222">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="78d55-223">可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="78d55-223">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="78d55-224">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="78d55-224">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="78d55-225">String</span><span class="sxs-lookup"><span data-stu-id="78d55-225">String</span></span>|<span data-ttu-id="78d55-226">Eap の種類が EAP-TLS または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="78d55-226">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="78d55-227">ここに示す文字列を使用して、Wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="78d55-227">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="78d55-228">応答</span><span class="sxs-lookup"><span data-stu-id="78d55-228">Response</span></span>
<span data-ttu-id="78d55-229">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78d55-229">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78d55-230">例</span><span class="sxs-lookup"><span data-stu-id="78d55-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="78d55-231">要求</span><span class="sxs-lookup"><span data-stu-id="78d55-231">Request</span></span>
<span data-ttu-id="78d55-232">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78d55-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1612

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="78d55-233">応答</span><span class="sxs-lookup"><span data-stu-id="78d55-233">Response</span></span>
<span data-ttu-id="78d55-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1784

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
  "id": "7ef0d9c3-d9c3-7ef0-c3d9-f07ec3d9f07e",
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
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```






