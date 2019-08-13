---
title: Androidwork Profilevpnconfiguration の更新
description: Androidwork Profilevpnconfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c01d0573aca4b8616fc189f897b4652a28c56e6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311005"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="e056e-103">Androidwork Profilevpnconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e056e-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="e056e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e056e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e056e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e056e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e056e-106">[Androidwork Profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e056e-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e056e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e056e-107">Prerequisites</span></span>
<span data-ttu-id="e056e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e056e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e056e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e056e-110">Permission type</span></span>|<span data-ttu-id="e056e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e056e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e056e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e056e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e056e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e056e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e056e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e056e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e056e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e056e-115">Not supported.</span></span>|
|<span data-ttu-id="e056e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e056e-116">Application</span></span>|<span data-ttu-id="e056e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e056e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e056e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e056e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e056e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e056e-119">Request headers</span></span>
|<span data-ttu-id="e056e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e056e-120">Header</span></span>|<span data-ttu-id="e056e-121">値</span><span class="sxs-lookup"><span data-stu-id="e056e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e056e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e056e-122">Authorization</span></span>|<span data-ttu-id="e056e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e056e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e056e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e056e-124">Accept</span></span>|<span data-ttu-id="e056e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e056e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e056e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e056e-126">Request body</span></span>
<span data-ttu-id="e056e-127">要求本文で、 [Androidwork Profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e056e-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="e056e-128">次の表に、 [Androidwork Profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e056e-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="e056e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e056e-129">Property</span></span>|<span data-ttu-id="e056e-130">型</span><span class="sxs-lookup"><span data-stu-id="e056e-130">Type</span></span>|<span data-ttu-id="e056e-131">説明</span><span class="sxs-lookup"><span data-stu-id="e056e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e056e-132">id</span><span class="sxs-lookup"><span data-stu-id="e056e-132">id</span></span>|<span data-ttu-id="e056e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e056e-133">String</span></span>|<span data-ttu-id="e056e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e056e-134">Key of the entity.</span></span> <span data-ttu-id="e056e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e056e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e056e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e056e-137">DateTimeOffset</span></span>|<span data-ttu-id="e056e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e056e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e056e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e056e-140">roleScopeTagIds</span></span>|<span data-ttu-id="e056e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e056e-141">String collection</span></span>|<span data-ttu-id="e056e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e056e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e056e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e056e-144">supportsScopeTags</span></span>|<span data-ttu-id="e056e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e056e-145">Boolean</span></span>|<span data-ttu-id="e056e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e056e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e056e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e056e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e056e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e056e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e056e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e056e-149">This property is read-only.</span></span> <span data-ttu-id="e056e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e056e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e056e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e056e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e056e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="e056e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e056e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e056e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e056e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e056e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e056e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e056e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e056e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e056e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e056e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="e056e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e056e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="e056e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e056e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e056e-163">createdDateTime</span></span>|<span data-ttu-id="e056e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e056e-164">DateTimeOffset</span></span>|<span data-ttu-id="e056e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e056e-165">DateTime the object was created.</span></span> <span data-ttu-id="e056e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-167">description</span><span class="sxs-lookup"><span data-stu-id="e056e-167">description</span></span>|<span data-ttu-id="e056e-168">String</span><span class="sxs-lookup"><span data-stu-id="e056e-168">String</span></span>|<span data-ttu-id="e056e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e056e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e056e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e056e-171">displayName</span></span>|<span data-ttu-id="e056e-172">String</span><span class="sxs-lookup"><span data-stu-id="e056e-172">String</span></span>|<span data-ttu-id="e056e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e056e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e056e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-175">version</span><span class="sxs-lookup"><span data-stu-id="e056e-175">version</span></span>|<span data-ttu-id="e056e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e056e-176">Int32</span></span>|<span data-ttu-id="e056e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e056e-177">Version of the device configuration.</span></span> <span data-ttu-id="e056e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e056e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e056e-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="e056e-179">connectionName</span></span>|<span data-ttu-id="e056e-180">String</span><span class="sxs-lookup"><span data-stu-id="e056e-180">String</span></span>|<span data-ttu-id="e056e-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="e056e-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="e056e-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="e056e-182">connectionType</span></span>|[<span data-ttu-id="e056e-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="e056e-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="e056e-184">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="e056e-184">Connection type.</span></span> <span data-ttu-id="e056e-185">可能な値は、`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect` です。</span><span class="sxs-lookup"><span data-stu-id="e056e-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="e056e-186">role</span><span class="sxs-lookup"><span data-stu-id="e056e-186">role</span></span>|<span data-ttu-id="e056e-187">String</span><span class="sxs-lookup"><span data-stu-id="e056e-187">String</span></span>|<span data-ttu-id="e056e-188">接続の種類がパルス Secure に設定されている場合の役割。</span><span class="sxs-lookup"><span data-stu-id="e056e-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="e056e-189">領域</span><span class="sxs-lookup"><span data-stu-id="e056e-189">realm</span></span>|<span data-ttu-id="e056e-190">String</span><span class="sxs-lookup"><span data-stu-id="e056e-190">String</span></span>|<span data-ttu-id="e056e-191">接続の種類がパルス Secure に設定されている場合の領域。</span><span class="sxs-lookup"><span data-stu-id="e056e-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="e056e-192">サーバ</span><span class="sxs-lookup"><span data-stu-id="e056e-192">servers</span></span>|<span data-ttu-id="e056e-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e056e-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="e056e-194">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="e056e-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="e056e-195">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e056e-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="e056e-196">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e056e-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e056e-197">デジタル</span><span class="sxs-lookup"><span data-stu-id="e056e-197">fingerprint</span></span>|<span data-ttu-id="e056e-198">String</span><span class="sxs-lookup"><span data-stu-id="e056e-198">String</span></span>|<span data-ttu-id="e056e-199">フィンガープリントは、VPN サーバーが信頼できることを確認するために使用される文字列です。これは、接続の種類が [チェックポイントカプセル VPN] の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="e056e-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="e056e-200">customData</span><span class="sxs-lookup"><span data-stu-id="e056e-200">customData</span></span>|<span data-ttu-id="e056e-201">[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e056e-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e056e-202">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="e056e-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="e056e-203">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e056e-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="e056e-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e056e-204">customKeyValueData</span></span>|<span data-ttu-id="e056e-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e056e-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e056e-206">接続の種類が Citrix に設定されている場合のカスタムデータ。</span><span class="sxs-lookup"><span data-stu-id="e056e-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="e056e-207">このコレクションには、最大25個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e056e-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="e056e-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e056e-208">authenticationMethod</span></span>|[<span data-ttu-id="e056e-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e056e-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e056e-210">認証方法。</span><span class="sxs-lookup"><span data-stu-id="e056e-210">Authentication method.</span></span> <span data-ttu-id="e056e-211">可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="e056e-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="e056e-212">応答</span><span class="sxs-lookup"><span data-stu-id="e056e-212">Response</span></span>
<span data-ttu-id="e056e-213">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androidwork Profilevpnconfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e056e-213">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e056e-214">例</span><span class="sxs-lookup"><span data-stu-id="e056e-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="e056e-215">要求</span><span class="sxs-lookup"><span data-stu-id="e056e-215">Request</span></span>
<span data-ttu-id="e056e-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e056e-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1762

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="e056e-217">応答</span><span class="sxs-lookup"><span data-stu-id="e056e-217">Response</span></span>
<span data-ttu-id="e056e-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e056e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1934

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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






