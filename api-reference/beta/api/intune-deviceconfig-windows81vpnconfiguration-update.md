---
title: Windows81VpnConfiguration の更新
description: Windows81VpnConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c47ad1be0cff68afddf11d5cac24ef8910df13dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344613"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="b3dcd-103">Windows81VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="b3dcd-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="b3dcd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3dcd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3dcd-106">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3dcd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3dcd-107">Prerequisites</span></span>
<span data-ttu-id="b3dcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3dcd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3dcd-110">Permission type</span></span>|<span data-ttu-id="b3dcd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3dcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3dcd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3dcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3dcd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3dcd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3dcd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3dcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3dcd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-115">Not supported.</span></span>|
|<span data-ttu-id="b3dcd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3dcd-116">Application</span></span>|<span data-ttu-id="b3dcd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3dcd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3dcd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3dcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3dcd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3dcd-119">Request headers</span></span>
|<span data-ttu-id="b3dcd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3dcd-120">Header</span></span>|<span data-ttu-id="b3dcd-121">値</span><span class="sxs-lookup"><span data-stu-id="b3dcd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3dcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3dcd-122">Authorization</span></span>|<span data-ttu-id="b3dcd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3dcd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b3dcd-124">Accept</span></span>|<span data-ttu-id="b3dcd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3dcd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3dcd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3dcd-126">Request body</span></span>
<span data-ttu-id="b3dcd-127">要求本文で、 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="b3dcd-128">次の表に、 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="b3dcd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dcd-129">Property</span></span>|<span data-ttu-id="b3dcd-130">型</span><span class="sxs-lookup"><span data-stu-id="b3dcd-130">Type</span></span>|<span data-ttu-id="b3dcd-131">説明</span><span class="sxs-lookup"><span data-stu-id="b3dcd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3dcd-132">id</span><span class="sxs-lookup"><span data-stu-id="b3dcd-132">id</span></span>|<span data-ttu-id="b3dcd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dcd-133">String</span></span>|<span data-ttu-id="b3dcd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-134">Key of the entity.</span></span> <span data-ttu-id="b3dcd-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3dcd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b3dcd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3dcd-137">DateTimeOffset</span></span>|<span data-ttu-id="b3dcd-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b3dcd-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3dcd-140">roleScopeTagIds</span></span>|<span data-ttu-id="b3dcd-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dcd-141">String collection</span></span>|<span data-ttu-id="b3dcd-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3dcd-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3dcd-144">supportsScopeTags</span></span>|<span data-ttu-id="b3dcd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3dcd-145">Boolean</span></span>|<span data-ttu-id="b3dcd-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3dcd-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3dcd-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3dcd-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-149">This property is read-only.</span></span> <span data-ttu-id="b3dcd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3dcd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3dcd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3dcd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3dcd-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3dcd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3dcd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3dcd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3dcd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3dcd-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3dcd-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b3dcd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3dcd-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b3dcd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3dcd-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3dcd-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3dcd-163">createdDateTime</span></span>|<span data-ttu-id="b3dcd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3dcd-164">DateTimeOffset</span></span>|<span data-ttu-id="b3dcd-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-165">DateTime the object was created.</span></span> <span data-ttu-id="b3dcd-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-167">description</span><span class="sxs-lookup"><span data-stu-id="b3dcd-167">description</span></span>|<span data-ttu-id="b3dcd-168">String</span><span class="sxs-lookup"><span data-stu-id="b3dcd-168">String</span></span>|<span data-ttu-id="b3dcd-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3dcd-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b3dcd-171">displayName</span></span>|<span data-ttu-id="b3dcd-172">String</span><span class="sxs-lookup"><span data-stu-id="b3dcd-172">String</span></span>|<span data-ttu-id="b3dcd-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3dcd-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-175">version</span><span class="sxs-lookup"><span data-stu-id="b3dcd-175">version</span></span>|<span data-ttu-id="b3dcd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b3dcd-176">Int32</span></span>|<span data-ttu-id="b3dcd-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-177">Version of the device configuration.</span></span> <span data-ttu-id="b3dcd-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="b3dcd-179">connectionName</span></span>|<span data-ttu-id="b3dcd-180">String</span><span class="sxs-lookup"><span data-stu-id="b3dcd-180">String</span></span>|<span data-ttu-id="b3dcd-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-181">Connection name displayed to the user.</span></span> <span data-ttu-id="b3dcd-182">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-183">サーバ</span><span class="sxs-lookup"><span data-stu-id="b3dcd-183">servers</span></span>|<span data-ttu-id="b3dcd-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dcd-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b3dcd-185">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="b3dcd-186">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b3dcd-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b3dcd-188">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-189">customXml</span><span class="sxs-lookup"><span data-stu-id="b3dcd-189">customXml</span></span>|<span data-ttu-id="b3dcd-190">Binary</span><span class="sxs-lookup"><span data-stu-id="b3dcd-190">Binary</span></span>|<span data-ttu-id="b3dcd-191">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b3dcd-192">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b3dcd-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3dcd-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b3dcd-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="b3dcd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3dcd-194">Boolean</span></span>|<span data-ttu-id="b3dcd-195">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b3dcd-196">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-196">This property is read-only.</span></span>|
|<span data-ttu-id="b3dcd-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="b3dcd-197">connectionType</span></span>|[<span data-ttu-id="b3dcd-198">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b3dcd-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="b3dcd-199">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-199">Connection type.</span></span> <span data-ttu-id="b3dcd-200">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="b3dcd-201">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b3dcd-201">loginGroupOrDomain</span></span>|<span data-ttu-id="b3dcd-202">String</span><span class="sxs-lookup"><span data-stu-id="b3dcd-202">String</span></span>|<span data-ttu-id="b3dcd-203">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="b3dcd-204">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b3dcd-204">enableSplitTunneling</span></span>|<span data-ttu-id="b3dcd-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3dcd-205">Boolean</span></span>|<span data-ttu-id="b3dcd-206">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="b3dcd-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b3dcd-207">proxyServer</span></span>|[<span data-ttu-id="b3dcd-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b3dcd-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="b3dcd-209">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="b3dcd-210">応答</span><span class="sxs-lookup"><span data-stu-id="b3dcd-210">Response</span></span>
<span data-ttu-id="b3dcd-211">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-211">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3dcd-212">例</span><span class="sxs-lookup"><span data-stu-id="b3dcd-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3dcd-213">要求</span><span class="sxs-lookup"><span data-stu-id="b3dcd-213">Request</span></span>
<span data-ttu-id="b3dcd-214">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b3dcd-215">応答</span><span class="sxs-lookup"><span data-stu-id="b3dcd-215">Response</span></span>
<span data-ttu-id="b3dcd-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3dcd-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```






