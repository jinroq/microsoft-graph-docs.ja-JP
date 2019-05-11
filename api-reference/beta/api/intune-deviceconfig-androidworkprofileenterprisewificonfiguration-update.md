---
title: AndroidWorkProfileEnterpriseWiFiConfiguration の更新
description: AndroidWorkProfileEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28f818ab7723ed03ccccec75883e095f90e2bbff
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928576"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="583e6-103">AndroidWorkProfileEnterpriseWiFiConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="583e6-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="583e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="583e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="583e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="583e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="583e6-106">[AndroidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="583e6-106">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="583e6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="583e6-107">Prerequisites</span></span>
<span data-ttu-id="583e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="583e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="583e6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="583e6-110">Permission type</span></span>|<span data-ttu-id="583e6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="583e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="583e6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="583e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="583e6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="583e6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="583e6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="583e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="583e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="583e6-115">Not supported.</span></span>|
|<span data-ttu-id="583e6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="583e6-116">Application</span></span>|<span data-ttu-id="583e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="583e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="583e6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="583e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="583e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="583e6-119">Request headers</span></span>
|<span data-ttu-id="583e6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="583e6-120">Header</span></span>|<span data-ttu-id="583e6-121">値</span><span class="sxs-lookup"><span data-stu-id="583e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="583e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="583e6-122">Authorization</span></span>|<span data-ttu-id="583e6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="583e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="583e6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="583e6-124">Accept</span></span>|<span data-ttu-id="583e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="583e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="583e6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="583e6-126">Request body</span></span>
<span data-ttu-id="583e6-127">要求本文で、 [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="583e6-127">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="583e6-128">次の表に、 [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="583e6-128">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="583e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="583e6-129">Property</span></span>|<span data-ttu-id="583e6-130">型</span><span class="sxs-lookup"><span data-stu-id="583e6-130">Type</span></span>|<span data-ttu-id="583e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="583e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="583e6-132">id</span><span class="sxs-lookup"><span data-stu-id="583e6-132">id</span></span>|<span data-ttu-id="583e6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="583e6-133">String</span></span>|<span data-ttu-id="583e6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="583e6-134">Key of the entity.</span></span> <span data-ttu-id="583e6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="583e6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="583e6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="583e6-137">DateTimeOffset</span></span>|<span data-ttu-id="583e6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="583e6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="583e6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="583e6-140">roleScopeTagIds</span></span>|<span data-ttu-id="583e6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="583e6-141">String collection</span></span>|<span data-ttu-id="583e6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="583e6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="583e6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="583e6-144">supportsScopeTags</span></span>|<span data-ttu-id="583e6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="583e6-145">Boolean</span></span>|<span data-ttu-id="583e6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="583e6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="583e6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="583e6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="583e6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="583e6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="583e6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="583e6-149">This property is read-only.</span></span> <span data-ttu-id="583e6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="583e6-151">createdDateTime</span></span>|<span data-ttu-id="583e6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="583e6-152">DateTimeOffset</span></span>|<span data-ttu-id="583e6-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="583e6-153">DateTime the object was created.</span></span> <span data-ttu-id="583e6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-155">description</span><span class="sxs-lookup"><span data-stu-id="583e6-155">description</span></span>|<span data-ttu-id="583e6-156">String</span><span class="sxs-lookup"><span data-stu-id="583e6-156">String</span></span>|<span data-ttu-id="583e6-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="583e6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="583e6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="583e6-159">displayName</span></span>|<span data-ttu-id="583e6-160">String</span><span class="sxs-lookup"><span data-stu-id="583e6-160">String</span></span>|<span data-ttu-id="583e6-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="583e6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="583e6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-163">version</span><span class="sxs-lookup"><span data-stu-id="583e6-163">version</span></span>|<span data-ttu-id="583e6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="583e6-164">Int32</span></span>|<span data-ttu-id="583e6-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="583e6-165">Version of the device configuration.</span></span> <span data-ttu-id="583e6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="583e6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="583e6-167">networkName</span><span class="sxs-lookup"><span data-stu-id="583e6-167">networkName</span></span>|<span data-ttu-id="583e6-168">String</span><span class="sxs-lookup"><span data-stu-id="583e6-168">String</span></span>|<span data-ttu-id="583e6-169">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されたネットワーク名</span><span class="sxs-lookup"><span data-stu-id="583e6-169">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="583e6-170">ssid</span><span class="sxs-lookup"><span data-stu-id="583e6-170">ssid</span></span>|<span data-ttu-id="583e6-171">String</span><span class="sxs-lookup"><span data-stu-id="583e6-171">String</span></span>|<span data-ttu-id="583e6-172">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="583e6-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="583e6-173">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="583e6-173">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="583e6-174">connectAutomatically に</span><span class="sxs-lookup"><span data-stu-id="583e6-174">connectAutomatically</span></span>|<span data-ttu-id="583e6-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="583e6-175">Boolean</span></span>|<span data-ttu-id="583e6-176">このネットワークが範囲内にあるときに自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="583e6-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="583e6-177">この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが Wi-fi ネットワークに自動的に接続されます。</span><span class="sxs-lookup"><span data-stu-id="583e6-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="583e6-178">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="583e6-178">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="583e6-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="583e6-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="583e6-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="583e6-180">Boolean</span></span>|<span data-ttu-id="583e6-181">このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。</span><span class="sxs-lookup"><span data-stu-id="583e6-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="583e6-182">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="583e6-182">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="583e6-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="583e6-183">wiFiSecurityType</span></span>|[<span data-ttu-id="583e6-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="583e6-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="583e6-185">Wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="583e6-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="583e6-186">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="583e6-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="583e6-187">可能な値は、`open`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="583e6-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="583e6-188">eapType</span><span class="sxs-lookup"><span data-stu-id="583e6-188">eapType</span></span>|[<span data-ttu-id="583e6-189">Androide Aptype</span><span class="sxs-lookup"><span data-stu-id="583e6-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="583e6-190">Wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="583e6-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="583e6-191">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="583e6-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="583e6-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="583e6-192">authenticationMethod</span></span>|[<span data-ttu-id="583e6-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="583e6-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="583e6-194">EAP の種類が PEAP または EAP-TLS に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="583e6-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="583e6-195">可能な値は、`certificate`、`usernameAndPassword`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="583e6-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="583e6-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="583e6-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="583e6-197">None Apauthenticationmethod_ Apttlstype</span><span class="sxs-lookup"><span data-stu-id="583e6-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="583e6-198">Eap タイプが EAP-TLS で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="583e6-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="583e6-199">使用可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="583e6-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="583e6-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="583e6-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="583e6-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="583e6-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="583e6-202">Eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 EAP メソッド (内部 Id)。</span><span class="sxs-lookup"><span data-stu-id="583e6-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="583e6-203">可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="583e6-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="583e6-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="583e6-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="583e6-205">String</span><span class="sxs-lookup"><span data-stu-id="583e6-205">String</span></span>|<span data-ttu-id="583e6-206">Eap の種類が EAP-TLS または PEAP に構成されている場合は、id プライバシー (外部 Id) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="583e6-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="583e6-207">ここに示す文字列を使用して、Wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="583e6-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="583e6-208">応答</span><span class="sxs-lookup"><span data-stu-id="583e6-208">Response</span></span>
<span data-ttu-id="583e6-209">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="583e6-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="583e6-210">例</span><span class="sxs-lookup"><span data-stu-id="583e6-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="583e6-211">要求</span><span class="sxs-lookup"><span data-stu-id="583e6-211">Request</span></span>
<span data-ttu-id="583e6-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="583e6-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="583e6-213">応答</span><span class="sxs-lookup"><span data-stu-id="583e6-213">Response</span></span>
<span data-ttu-id="583e6-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="583e6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 948

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




