---
title: AndroidEnterpriseWiFiConfiguration の更新
description: AndroidEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: daa945b2f6919ea75e9730edc393b8fd57182c93
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33932914"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="767e1-103">AndroidEnterpriseWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="767e1-103">Update androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="767e1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="767e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767e1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="767e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767e1-106">[AndroidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="767e1-106">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="767e1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="767e1-107">Prerequisites</span></span>
<span data-ttu-id="767e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="767e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767e1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="767e1-110">Permission type</span></span>|<span data-ttu-id="767e1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="767e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767e1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="767e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="767e1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="767e1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="767e1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="767e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767e1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="767e1-115">Not supported.</span></span>|
|<span data-ttu-id="767e1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="767e1-116">Application</span></span>|<span data-ttu-id="767e1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="767e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767e1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="767e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="767e1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="767e1-119">Request headers</span></span>
|<span data-ttu-id="767e1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="767e1-120">Header</span></span>|<span data-ttu-id="767e1-121">値</span><span class="sxs-lookup"><span data-stu-id="767e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="767e1-122">Authorization</span></span>|<span data-ttu-id="767e1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="767e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767e1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="767e1-124">Accept</span></span>|<span data-ttu-id="767e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="767e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767e1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="767e1-126">Request body</span></span>
<span data-ttu-id="767e1-127">要求本文で、 [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="767e1-127">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="767e1-128">次の表に、 [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="767e1-128">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="767e1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="767e1-129">Property</span></span>|<span data-ttu-id="767e1-130">型</span><span class="sxs-lookup"><span data-stu-id="767e1-130">Type</span></span>|<span data-ttu-id="767e1-131">説明</span><span class="sxs-lookup"><span data-stu-id="767e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767e1-132">id</span><span class="sxs-lookup"><span data-stu-id="767e1-132">id</span></span>|<span data-ttu-id="767e1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="767e1-133">String</span></span>|<span data-ttu-id="767e1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="767e1-134">Key of the entity.</span></span> <span data-ttu-id="767e1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="767e1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="767e1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="767e1-137">DateTimeOffset</span></span>|<span data-ttu-id="767e1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="767e1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="767e1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="767e1-140">roleScopeTagIds</span></span>|<span data-ttu-id="767e1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="767e1-141">String collection</span></span>|<span data-ttu-id="767e1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="767e1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="767e1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="767e1-144">supportsScopeTags</span></span>|<span data-ttu-id="767e1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="767e1-145">Boolean</span></span>|<span data-ttu-id="767e1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="767e1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="767e1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="767e1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="767e1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="767e1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="767e1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="767e1-149">This property is read-only.</span></span> <span data-ttu-id="767e1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="767e1-151">createdDateTime</span></span>|<span data-ttu-id="767e1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="767e1-152">DateTimeOffset</span></span>|<span data-ttu-id="767e1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="767e1-153">DateTime the object was created.</span></span> <span data-ttu-id="767e1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-155">description</span><span class="sxs-lookup"><span data-stu-id="767e1-155">description</span></span>|<span data-ttu-id="767e1-156">String</span><span class="sxs-lookup"><span data-stu-id="767e1-156">String</span></span>|<span data-ttu-id="767e1-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="767e1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="767e1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="767e1-159">displayName</span></span>|<span data-ttu-id="767e1-160">String</span><span class="sxs-lookup"><span data-stu-id="767e1-160">String</span></span>|<span data-ttu-id="767e1-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="767e1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="767e1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-163">version</span><span class="sxs-lookup"><span data-stu-id="767e1-163">version</span></span>|<span data-ttu-id="767e1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="767e1-164">Int32</span></span>|<span data-ttu-id="767e1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="767e1-165">Version of the device configuration.</span></span> <span data-ttu-id="767e1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="767e1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="767e1-167">networkName</span><span class="sxs-lookup"><span data-stu-id="767e1-167">networkName</span></span>|<span data-ttu-id="767e1-168">String</span><span class="sxs-lookup"><span data-stu-id="767e1-168">String</span></span>|<span data-ttu-id="767e1-169">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="767e1-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="767e1-170">ssid</span><span class="sxs-lookup"><span data-stu-id="767e1-170">ssid</span></span>|<span data-ttu-id="767e1-171">String</span><span class="sxs-lookup"><span data-stu-id="767e1-171">String</span></span>|<span data-ttu-id="767e1-172">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="767e1-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="767e1-173">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="767e1-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="767e1-174">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="767e1-174">connectAutomatically</span></span>|<span data-ttu-id="767e1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="767e1-175">Boolean</span></span>|<span data-ttu-id="767e1-176">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="767e1-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="767e1-177">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="767e1-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="767e1-178">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="767e1-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="767e1-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="767e1-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="767e1-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="767e1-180">Boolean</span></span>|<span data-ttu-id="767e1-181">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="767e1-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="767e1-182">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="767e1-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="767e1-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="767e1-183">wiFiSecurityType</span></span>|[<span data-ttu-id="767e1-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="767e1-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="767e1-185">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="767e1-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="767e1-186">[AndroidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="767e1-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="767e1-187">可能な値は、`open`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="767e1-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="767e1-188">eapType</span><span class="sxs-lookup"><span data-stu-id="767e1-188">eapType</span></span>|[<span data-ttu-id="767e1-189">Androide Aptype</span><span class="sxs-lookup"><span data-stu-id="767e1-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="767e1-190">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="767e1-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="767e1-191">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="767e1-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="767e1-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="767e1-192">authenticationMethod</span></span>|[<span data-ttu-id="767e1-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="767e1-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="767e1-194">EAP の種類が PEAP または EAP-TLS に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="767e1-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="767e1-195">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="767e1-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="767e1-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="767e1-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="767e1-197">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="767e1-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="767e1-198">Eap タイプが EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="767e1-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="767e1-199">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="767e1-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="767e1-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="767e1-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="767e1-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="767e1-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="767e1-202">Eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="767e1-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="767e1-203">可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="767e1-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="767e1-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="767e1-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="767e1-205">String</span><span class="sxs-lookup"><span data-stu-id="767e1-205">String</span></span>|<span data-ttu-id="767e1-206">Eap の種類が EAP-TLS または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="767e1-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="767e1-207">ここに示す文字列を使用して、Wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="767e1-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="767e1-208">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="767e1-208">usernameFormatString</span></span>|<span data-ttu-id="767e1-209">String</span><span class="sxs-lookup"><span data-stu-id="767e1-209">String</span></span>|<span data-ttu-id="767e1-210">Wifi に接続するためのユーザー名を作成するために使用されるユーザー名の形式文字列</span><span class="sxs-lookup"><span data-stu-id="767e1-210">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="767e1-211">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="767e1-211">passwordFormatString</span></span>|<span data-ttu-id="767e1-212">String</span><span class="sxs-lookup"><span data-stu-id="767e1-212">String</span></span>|<span data-ttu-id="767e1-213">Wifi に接続するためのパスワードを作成するために使用されるパスワード形式の文字列</span><span class="sxs-lookup"><span data-stu-id="767e1-213">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="767e1-214">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="767e1-214">preSharedKey</span></span>|<span data-ttu-id="767e1-215">String</span><span class="sxs-lookup"><span data-stu-id="767e1-215">String</span></span>|<span data-ttu-id="767e1-216">Wi-fi に接続するためにパスワードを作成するために使用される PreSharedKey</span><span class="sxs-lookup"><span data-stu-id="767e1-216">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="767e1-217">応答</span><span class="sxs-lookup"><span data-stu-id="767e1-217">Response</span></span>
<span data-ttu-id="767e1-218">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="767e1-218">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767e1-219">例</span><span class="sxs-lookup"><span data-stu-id="767e1-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="767e1-220">要求</span><span class="sxs-lookup"><span data-stu-id="767e1-220">Request</span></span>
<span data-ttu-id="767e1-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="767e1-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="767e1-222">応答</span><span class="sxs-lookup"><span data-stu-id="767e1-222">Response</span></span>
<span data-ttu-id="767e1-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="767e1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1098

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




