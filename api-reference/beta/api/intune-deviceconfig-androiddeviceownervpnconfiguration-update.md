---
title: AndroidDeviceOwnerVpnConfiguration の更新
description: AndroidDeviceOwnerVpnConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8146d3813c94c3ef3c6a481d7dbc80c6c03598c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316983"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="7f84f-103">AndroidDeviceOwnerVpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="7f84f-103">Update androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="7f84f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f84f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f84f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f84f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f84f-106">[Androiddeviceownervpnconfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-106">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f84f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f84f-107">Prerequisites</span></span>
<span data-ttu-id="7f84f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f84f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f84f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f84f-110">Permission type</span></span>|<span data-ttu-id="7f84f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f84f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f84f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f84f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f84f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f84f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f84f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f84f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f84f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f84f-115">Not supported.</span></span>|
|<span data-ttu-id="7f84f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f84f-116">Application</span></span>|<span data-ttu-id="7f84f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f84f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f84f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f84f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7f84f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f84f-119">Request headers</span></span>
|<span data-ttu-id="7f84f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f84f-120">Header</span></span>|<span data-ttu-id="7f84f-121">値</span><span class="sxs-lookup"><span data-stu-id="7f84f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f84f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f84f-122">Authorization</span></span>|<span data-ttu-id="7f84f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f84f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f84f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f84f-124">Accept</span></span>|<span data-ttu-id="7f84f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f84f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f84f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f84f-126">Request body</span></span>
<span data-ttu-id="7f84f-127">要求本文で、 [Androiddeviceownervpnconfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-127">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="7f84f-128">次の表に、 [Androiddeviceownervpnconfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-128">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="7f84f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f84f-129">Property</span></span>|<span data-ttu-id="7f84f-130">型</span><span class="sxs-lookup"><span data-stu-id="7f84f-130">Type</span></span>|<span data-ttu-id="7f84f-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f84f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f84f-132">id</span><span class="sxs-lookup"><span data-stu-id="7f84f-132">id</span></span>|<span data-ttu-id="7f84f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7f84f-133">String</span></span>|<span data-ttu-id="7f84f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f84f-134">Key of the entity.</span></span> <span data-ttu-id="7f84f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f84f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7f84f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f84f-137">DateTimeOffset</span></span>|<span data-ttu-id="7f84f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f84f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7f84f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f84f-140">roleScopeTagIds</span></span>|<span data-ttu-id="7f84f-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f84f-141">String collection</span></span>|<span data-ttu-id="7f84f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7f84f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7f84f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7f84f-144">supportsScopeTags</span></span>|<span data-ttu-id="7f84f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f84f-145">Boolean</span></span>|<span data-ttu-id="7f84f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7f84f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7f84f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7f84f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7f84f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7f84f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-149">This property is read-only.</span></span> <span data-ttu-id="7f84f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7f84f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7f84f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7f84f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7f84f-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="7f84f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7f84f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f84f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7f84f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f84f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7f84f-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7f84f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7f84f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7f84f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7f84f-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7f84f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7f84f-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7f84f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7f84f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f84f-163">createdDateTime</span></span>|<span data-ttu-id="7f84f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f84f-164">DateTimeOffset</span></span>|<span data-ttu-id="7f84f-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f84f-165">DateTime the object was created.</span></span> <span data-ttu-id="7f84f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-167">description</span><span class="sxs-lookup"><span data-stu-id="7f84f-167">description</span></span>|<span data-ttu-id="7f84f-168">String</span><span class="sxs-lookup"><span data-stu-id="7f84f-168">String</span></span>|<span data-ttu-id="7f84f-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7f84f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f84f-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7f84f-171">displayName</span></span>|<span data-ttu-id="7f84f-172">String</span><span class="sxs-lookup"><span data-stu-id="7f84f-172">String</span></span>|<span data-ttu-id="7f84f-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7f84f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f84f-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-175">version</span><span class="sxs-lookup"><span data-stu-id="7f84f-175">version</span></span>|<span data-ttu-id="7f84f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7f84f-176">Int32</span></span>|<span data-ttu-id="7f84f-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7f84f-177">Version of the device configuration.</span></span> <span data-ttu-id="7f84f-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f84f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7f84f-179">authenticationMethod</span></span>|[<span data-ttu-id="7f84f-180">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7f84f-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7f84f-181">認証方法。</span><span class="sxs-lookup"><span data-stu-id="7f84f-181">Authentication method.</span></span> <span data-ttu-id="7f84f-182">[Vpnconfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="7f84f-183">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="7f84f-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7f84f-184">connectionName</span><span class="sxs-lookup"><span data-stu-id="7f84f-184">connectionName</span></span>|<span data-ttu-id="7f84f-185">String</span><span class="sxs-lookup"><span data-stu-id="7f84f-185">String</span></span>|<span data-ttu-id="7f84f-186">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="7f84f-186">Connection name displayed to the user.</span></span> <span data-ttu-id="7f84f-187">[Vpnconfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7f84f-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-188">role</span><span class="sxs-lookup"><span data-stu-id="7f84f-188">role</span></span>|<span data-ttu-id="7f84f-189">String</span><span class="sxs-lookup"><span data-stu-id="7f84f-189">String</span></span>|<span data-ttu-id="7f84f-190">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="7f84f-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7f84f-191">[Vpnconfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7f84f-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-192">領域</span><span class="sxs-lookup"><span data-stu-id="7f84f-192">realm</span></span>|<span data-ttu-id="7f84f-193">String</span><span class="sxs-lookup"><span data-stu-id="7f84f-193">String</span></span>|<span data-ttu-id="7f84f-194">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="7f84f-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7f84f-195">[Vpnconfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7f84f-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-196">サーバ</span><span class="sxs-lookup"><span data-stu-id="7f84f-196">servers</span></span>|<span data-ttu-id="7f84f-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7f84f-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="7f84f-198">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="7f84f-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="7f84f-199">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="7f84f-200">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7f84f-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7f84f-201">[Vpnconfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="7f84f-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7f84f-202">connectionType</span><span class="sxs-lookup"><span data-stu-id="7f84f-202">connectionType</span></span>|[<span data-ttu-id="7f84f-203">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7f84f-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="7f84f-204">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="7f84f-204">Connection type.</span></span> <span data-ttu-id="7f84f-205">使用可能な値: `ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="7f84f-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f84f-206">応答</span><span class="sxs-lookup"><span data-stu-id="7f84f-206">Response</span></span>
<span data-ttu-id="7f84f-207">成功した場合、このメソッド`200 OK`は応答コードと、更新された[Androiddeviceownervpnconfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7f84f-207">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f84f-208">例</span><span class="sxs-lookup"><span data-stu-id="7f84f-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f84f-209">要求</span><span class="sxs-lookup"><span data-stu-id="7f84f-209">Request</span></span>
<span data-ttu-id="7f84f-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f84f-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1417

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```

### <a name="response"></a><span data-ttu-id="7f84f-211">応答</span><span class="sxs-lookup"><span data-stu-id="7f84f-211">Response</span></span>
<span data-ttu-id="7f84f-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f84f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1589

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
  "id": "972962e3-62e3-9729-e362-2997e3622997",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```






