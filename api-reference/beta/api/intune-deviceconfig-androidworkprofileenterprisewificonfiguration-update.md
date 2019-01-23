---
title: AndroidWorkProfileEnterpriseWiFiConfiguration を更新します。
description: AndroidWorkProfileEnterpriseWiFiConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05dd752507a402fb54d27dad40a4264617395b50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406760"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="6fb5b-103">AndroidWorkProfileEnterpriseWiFiConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="6fb5b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fb5b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fb5b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fb5b-107">[AndroidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-107">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fb5b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6fb5b-108">Prerequisites</span></span>
<span data-ttu-id="6fb5b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6fb5b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fb5b-111">Permission type</span></span>|<span data-ttu-id="6fb5b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fb5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fb5b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fb5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fb5b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb5b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fb5b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fb5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fb5b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-116">Not supported.</span></span>|
|<span data-ttu-id="6fb5b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fb5b-117">Application</span></span>|<span data-ttu-id="6fb5b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fb5b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fb5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6fb5b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fb5b-120">Request headers</span></span>
|<span data-ttu-id="6fb5b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fb5b-121">Header</span></span>|<span data-ttu-id="6fb5b-122">値</span><span class="sxs-lookup"><span data-stu-id="6fb5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fb5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb5b-123">Authorization</span></span>|<span data-ttu-id="6fb5b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fb5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fb5b-125">Accept</span></span>|<span data-ttu-id="6fb5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fb5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb5b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fb5b-127">Request body</span></span>
<span data-ttu-id="6fb5b-128">要求の本文に[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-128">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="6fb5b-129">[AndroidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-129">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="6fb5b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb5b-130">Property</span></span>|<span data-ttu-id="6fb5b-131">型</span><span class="sxs-lookup"><span data-stu-id="6fb5b-131">Type</span></span>|<span data-ttu-id="6fb5b-132">説明</span><span class="sxs-lookup"><span data-stu-id="6fb5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb5b-133">id</span><span class="sxs-lookup"><span data-stu-id="6fb5b-133">id</span></span>|<span data-ttu-id="6fb5b-134">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-134">String</span></span>|<span data-ttu-id="6fb5b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-135">Key of the entity.</span></span> <span data-ttu-id="6fb5b-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb5b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6fb5b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb5b-138">DateTimeOffset</span></span>|<span data-ttu-id="6fb5b-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6fb5b-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fb5b-141">roleScopeTagIds</span></span>|<span data-ttu-id="6fb5b-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6fb5b-142">String collection</span></span>|<span data-ttu-id="6fb5b-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6fb5b-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6fb5b-145">supportsScopeTags</span></span>|<span data-ttu-id="6fb5b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb5b-146">Boolean</span></span>|<span data-ttu-id="6fb5b-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6fb5b-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6fb5b-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6fb5b-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-150">This property is read-only.</span></span> <span data-ttu-id="6fb5b-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb5b-152">createdDateTime</span></span>|<span data-ttu-id="6fb5b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb5b-153">DateTimeOffset</span></span>|<span data-ttu-id="6fb5b-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-154">DateTime the object was created.</span></span> <span data-ttu-id="6fb5b-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-156">説明</span><span class="sxs-lookup"><span data-stu-id="6fb5b-156">description</span></span>|<span data-ttu-id="6fb5b-157">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-157">String</span></span>|<span data-ttu-id="6fb5b-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fb5b-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6fb5b-160">displayName</span></span>|<span data-ttu-id="6fb5b-161">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-161">String</span></span>|<span data-ttu-id="6fb5b-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fb5b-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-164">version</span><span class="sxs-lookup"><span data-stu-id="6fb5b-164">version</span></span>|<span data-ttu-id="6fb5b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb5b-165">Int32</span></span>|<span data-ttu-id="6fb5b-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-166">Version of the device configuration.</span></span> <span data-ttu-id="6fb5b-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fb5b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-168">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="6fb5b-168">networkName</span></span>|<span data-ttu-id="6fb5b-169">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-169">String</span></span>|<span data-ttu-id="6fb5b-170">ネットワーク名は、 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-170">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-171">ssid</span><span class="sxs-lookup"><span data-stu-id="6fb5b-171">ssid</span></span>|<span data-ttu-id="6fb5b-172">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-172">String</span></span>|<span data-ttu-id="6fb5b-173">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6fb5b-174">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-174">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6fb5b-175">connectAutomatically</span></span>|<span data-ttu-id="6fb5b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb5b-176">Boolean</span></span>|<span data-ttu-id="6fb5b-177">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6fb5b-178">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6fb5b-179">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-179">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6fb5b-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6fb5b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb5b-181">Boolean</span></span>|<span data-ttu-id="6fb5b-182">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6fb5b-183">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-183">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fb5b-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6fb5b-184">wiFiSecurityType</span></span>|[<span data-ttu-id="6fb5b-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6fb5b-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="6fb5b-186">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6fb5b-187">[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-187">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="6fb5b-188">使用可能な値は、`open`、`wpaEnterprise` です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="6fb5b-189">eapType</span><span class="sxs-lookup"><span data-stu-id="6fb5b-189">eapType</span></span>|[<span data-ttu-id="6fb5b-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="6fb5b-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="6fb5b-191">[EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6fb5b-192">可能な値は、`eapTls`、`eapTtls`、`peap` です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="6fb5b-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fb5b-193">authenticationMethod</span></span>|[<span data-ttu-id="6fb5b-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fb5b-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6fb5b-195">PEAP や EAP TTLS、EAP の種類が構成されているときに使用する必要があるクライアント (デバイス) の認証方法を示します。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6fb5b-196">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6fb5b-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="6fb5b-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6fb5b-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6fb5b-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6fb5b-199">(内部) するときのユーザーは EAP TTLS、EAP の種類の認証と Authenticationmethod の非 EAP メソッドは、ユーザー名とパスワードです。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6fb5b-200">可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6fb5b-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="6fb5b-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="6fb5b-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="6fb5b-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="6fb5b-203">(内部) するときのユーザー [EAP の種類は、PEAP を認証し、Authenticationmethod の非 EAP メソッドは、ユーザー名とパスワードです。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6fb5b-204">使用可能な値は、`none`、`microsoftChapVersionTwo` です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6fb5b-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6fb5b-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6fb5b-206">String</span><span class="sxs-lookup"><span data-stu-id="6fb5b-206">String</span></span>|<span data-ttu-id="6fb5b-207">EAP TTLS または PEAP に EAP の種類が構成されている場合は、(外部ユーザー) の [id プライバシーを有効にします。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="6fb5b-208">ここで指定した文字列を使用して、Wi-fi ネットワークに接続しようとするときは、個々 のユーザーのユーザー名をマスクします。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="6fb5b-209">応答</span><span class="sxs-lookup"><span data-stu-id="6fb5b-209">Response</span></span>
<span data-ttu-id="6fb5b-210">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-210">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fb5b-211">例</span><span class="sxs-lookup"><span data-stu-id="6fb5b-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fb5b-212">要求</span><span class="sxs-lookup"><span data-stu-id="6fb5b-212">Request</span></span>
<span data-ttu-id="6fb5b-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fb5b-214">応答</span><span class="sxs-lookup"><span data-stu-id="6fb5b-214">Response</span></span>
<span data-ttu-id="6fb5b-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6fb5b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




