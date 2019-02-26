---
title: androidwork profilevpnconfiguration の更新
description: androidwork profilevpnconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61ea061f5e6a1d1e9f9900ceb5de5ec8cabfd6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164107"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="9a4a8-103">androidwork profilevpnconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9a4a8-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="9a4a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a4a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4a8-106">[androidwork profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a4a8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a4a8-107">Prerequisites</span></span>
<span data-ttu-id="9a4a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a4a8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a4a8-110">Permission type</span></span>|<span data-ttu-id="9a4a8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a4a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a4a8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a4a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a4a8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a4a8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a4a8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a4a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a4a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-115">Not supported.</span></span>|
|<span data-ttu-id="9a4a8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a4a8-116">Application</span></span>|<span data-ttu-id="9a4a8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a4a8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a4a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9a4a8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a4a8-119">Request headers</span></span>
|<span data-ttu-id="9a4a8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a4a8-120">Header</span></span>|<span data-ttu-id="9a4a8-121">値</span><span class="sxs-lookup"><span data-stu-id="9a4a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a4a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a4a8-122">Authorization</span></span>|<span data-ttu-id="9a4a8-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a4a8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9a4a8-124">Accept</span></span>|<span data-ttu-id="9a4a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a4a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a4a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a4a8-126">Request body</span></span>
<span data-ttu-id="9a4a8-127">要求本文で、 [androidwork profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="9a4a8-128">次の表に、 [androidwork profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="9a4a8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a4a8-129">Property</span></span>|<span data-ttu-id="9a4a8-130">型</span><span class="sxs-lookup"><span data-stu-id="9a4a8-130">Type</span></span>|<span data-ttu-id="9a4a8-131">説明</span><span class="sxs-lookup"><span data-stu-id="9a4a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a4a8-132">id</span><span class="sxs-lookup"><span data-stu-id="9a4a8-132">id</span></span>|<span data-ttu-id="9a4a8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9a4a8-133">String</span></span>|<span data-ttu-id="9a4a8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-134">Key of the entity.</span></span> <span data-ttu-id="9a4a8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a4a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9a4a8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a4a8-137">DateTimeOffset</span></span>|<span data-ttu-id="9a4a8-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9a4a8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a4a8-140">roleScopeTagIds</span></span>|<span data-ttu-id="9a4a8-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9a4a8-141">String collection</span></span>|<span data-ttu-id="9a4a8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a4a8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a4a8-144">supportsScopeTags</span></span>|<span data-ttu-id="9a4a8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a4a8-145">Boolean</span></span>|<span data-ttu-id="9a4a8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a4a8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a4a8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a4a8-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-149">This property is read-only.</span></span> <span data-ttu-id="9a4a8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a4a8-151">createdDateTime</span></span>|<span data-ttu-id="9a4a8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a4a8-152">DateTimeOffset</span></span>|<span data-ttu-id="9a4a8-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-153">DateTime the object was created.</span></span> <span data-ttu-id="9a4a8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-155">説明</span><span class="sxs-lookup"><span data-stu-id="9a4a8-155">description</span></span>|<span data-ttu-id="9a4a8-156">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-156">String</span></span>|<span data-ttu-id="9a4a8-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a4a8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9a4a8-159">displayName</span></span>|<span data-ttu-id="9a4a8-160">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-160">String</span></span>|<span data-ttu-id="9a4a8-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a4a8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-163">version</span><span class="sxs-lookup"><span data-stu-id="9a4a8-163">version</span></span>|<span data-ttu-id="9a4a8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9a4a8-164">Int32</span></span>|<span data-ttu-id="9a4a8-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-165">Version of the device configuration.</span></span> <span data-ttu-id="9a4a8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a4a8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a4a8-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="9a4a8-167">connectionName</span></span>|<span data-ttu-id="9a4a8-168">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-168">String</span></span>|<span data-ttu-id="9a4a8-169">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="9a4a8-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="9a4a8-170">connectionType</span></span>|[<span data-ttu-id="9a4a8-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9a4a8-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="9a4a8-172">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-172">Connection type.</span></span> <span data-ttu-id="9a4a8-173">可能な値は、`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="9a4a8-174">role</span><span class="sxs-lookup"><span data-stu-id="9a4a8-174">role</span></span>|<span data-ttu-id="9a4a8-175">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-175">String</span></span>|<span data-ttu-id="9a4a8-176">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9a4a8-177">領域</span><span class="sxs-lookup"><span data-stu-id="9a4a8-177">realm</span></span>|<span data-ttu-id="9a4a8-178">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-178">String</span></span>|<span data-ttu-id="9a4a8-179">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="9a4a8-180">サーバー</span><span class="sxs-lookup"><span data-stu-id="9a4a8-180">servers</span></span>|<span data-ttu-id="9a4a8-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a4a8-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9a4a8-182">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="9a4a8-183">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9a4a8-184">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9a4a8-185">デジタル</span><span class="sxs-lookup"><span data-stu-id="9a4a8-185">fingerprint</span></span>|<span data-ttu-id="9a4a8-186">String</span><span class="sxs-lookup"><span data-stu-id="9a4a8-186">String</span></span>|<span data-ttu-id="9a4a8-187">フィンガープリントは、vpn サーバーが信頼できることを確認するために使用される文字列です。これは、接続の種類が [チェックポイントカプセル VPN] の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9a4a8-188">customData</span><span class="sxs-lookup"><span data-stu-id="9a4a8-188">customData</span></span>|<span data-ttu-id="9a4a8-189">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a4a8-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="9a4a8-190">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9a4a8-191">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9a4a8-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="9a4a8-192">customKeyValueData</span></span>|<span data-ttu-id="9a4a8-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a4a8-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9a4a8-194">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="9a4a8-195">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="9a4a8-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9a4a8-196">authenticationMethod</span></span>|[<span data-ttu-id="9a4a8-197">vpnauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="9a4a8-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9a4a8-198">認証方法。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-198">Authentication method.</span></span> <span data-ttu-id="9a4a8-199">使用可能な値は、`certificate`、`usernameAndPassword` です。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="9a4a8-200">応答</span><span class="sxs-lookup"><span data-stu-id="9a4a8-200">Response</span></span>
<span data-ttu-id="9a4a8-201">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidwork profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-201">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a4a8-202">例</span><span class="sxs-lookup"><span data-stu-id="9a4a8-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a4a8-203">要求</span><span class="sxs-lookup"><span data-stu-id="9a4a8-203">Request</span></span>
<span data-ttu-id="9a4a8-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 989

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="9a4a8-205">応答</span><span class="sxs-lookup"><span data-stu-id="9a4a8-205">Response</span></span>
<span data-ttu-id="9a4a8-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a4a8-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```




