---
title: WindowsPhone81VpnConfiguration の更新
description: WindowsPhone81VpnConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7608a653f09679077719291bb997a49459fc335c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313818"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="49905-103">WindowsPhone81VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="49905-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="49905-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49905-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49905-106">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="49905-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49905-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="49905-107">Prerequisites</span></span>
<span data-ttu-id="49905-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49905-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49905-110">Permission type</span></span>|<span data-ttu-id="49905-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="49905-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49905-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49905-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49905-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49905-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49905-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49905-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49905-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49905-115">Not supported.</span></span>|
|<span data-ttu-id="49905-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49905-116">Application</span></span>|<span data-ttu-id="49905-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49905-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49905-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49905-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="49905-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49905-119">Request headers</span></span>
|<span data-ttu-id="49905-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49905-120">Header</span></span>|<span data-ttu-id="49905-121">値</span><span class="sxs-lookup"><span data-stu-id="49905-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49905-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49905-122">Authorization</span></span>|<span data-ttu-id="49905-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="49905-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49905-124">承諾</span><span class="sxs-lookup"><span data-stu-id="49905-124">Accept</span></span>|<span data-ttu-id="49905-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49905-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49905-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="49905-126">Request body</span></span>
<span data-ttu-id="49905-127">要求本文で、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="49905-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="49905-128">次の表に、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="49905-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="49905-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49905-129">Property</span></span>|<span data-ttu-id="49905-130">型</span><span class="sxs-lookup"><span data-stu-id="49905-130">Type</span></span>|<span data-ttu-id="49905-131">説明</span><span class="sxs-lookup"><span data-stu-id="49905-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49905-132">id</span><span class="sxs-lookup"><span data-stu-id="49905-132">id</span></span>|<span data-ttu-id="49905-133">文字列</span><span class="sxs-lookup"><span data-stu-id="49905-133">String</span></span>|<span data-ttu-id="49905-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="49905-134">Key of the entity.</span></span> <span data-ttu-id="49905-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49905-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49905-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49905-137">DateTimeOffset</span></span>|<span data-ttu-id="49905-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="49905-138">DateTime the object was last modified.</span></span> <span data-ttu-id="49905-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49905-140">roleScopeTagIds</span></span>|<span data-ttu-id="49905-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="49905-141">String collection</span></span>|<span data-ttu-id="49905-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="49905-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49905-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="49905-144">supportsScopeTags</span></span>|<span data-ttu-id="49905-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-145">Boolean</span></span>|<span data-ttu-id="49905-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="49905-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49905-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="49905-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49905-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="49905-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49905-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="49905-149">This property is read-only.</span></span> <span data-ttu-id="49905-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="49905-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="49905-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="49905-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="49905-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="49905-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="49905-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="49905-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="49905-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="49905-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="49905-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="49905-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="49905-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="49905-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="49905-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="49905-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="49905-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="49905-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="49905-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49905-163">createdDateTime</span></span>|<span data-ttu-id="49905-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49905-164">DateTimeOffset</span></span>|<span data-ttu-id="49905-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="49905-165">DateTime the object was created.</span></span> <span data-ttu-id="49905-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-167">description</span><span class="sxs-lookup"><span data-stu-id="49905-167">description</span></span>|<span data-ttu-id="49905-168">String</span><span class="sxs-lookup"><span data-stu-id="49905-168">String</span></span>|<span data-ttu-id="49905-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="49905-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49905-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-171">displayName</span><span class="sxs-lookup"><span data-stu-id="49905-171">displayName</span></span>|<span data-ttu-id="49905-172">String</span><span class="sxs-lookup"><span data-stu-id="49905-172">String</span></span>|<span data-ttu-id="49905-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="49905-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49905-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-175">version</span><span class="sxs-lookup"><span data-stu-id="49905-175">version</span></span>|<span data-ttu-id="49905-176">Int32</span><span class="sxs-lookup"><span data-stu-id="49905-176">Int32</span></span>|<span data-ttu-id="49905-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="49905-177">Version of the device configuration.</span></span> <span data-ttu-id="49905-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49905-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="49905-179">connectionName</span></span>|<span data-ttu-id="49905-180">String</span><span class="sxs-lookup"><span data-stu-id="49905-180">String</span></span>|<span data-ttu-id="49905-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="49905-181">Connection name displayed to the user.</span></span> <span data-ttu-id="49905-182">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-183">サーバ</span><span class="sxs-lookup"><span data-stu-id="49905-183">servers</span></span>|<span data-ttu-id="49905-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49905-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="49905-185">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="49905-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="49905-186">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="49905-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="49905-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="49905-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="49905-188">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-189">customXml</span><span class="sxs-lookup"><span data-stu-id="49905-189">customXml</span></span>|<span data-ttu-id="49905-190">Binary</span><span class="sxs-lookup"><span data-stu-id="49905-190">Binary</span></span>|<span data-ttu-id="49905-191">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="49905-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="49905-192">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="49905-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="49905-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="49905-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-194">Boolean</span></span>|<span data-ttu-id="49905-195">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="49905-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="49905-196">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49905-196">This property is read-only.</span></span> <span data-ttu-id="49905-197">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49905-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="49905-198">connectionType</span></span>|[<span data-ttu-id="49905-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="49905-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="49905-200">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="49905-200">Connection type.</span></span> <span data-ttu-id="49905-201">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="49905-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="49905-202">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="49905-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="49905-203">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="49905-203">loginGroupOrDomain</span></span>|<span data-ttu-id="49905-204">String</span><span class="sxs-lookup"><span data-stu-id="49905-204">String</span></span>|<span data-ttu-id="49905-205">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="49905-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="49905-206">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49905-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-207">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="49905-207">enableSplitTunneling</span></span>|<span data-ttu-id="49905-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-208">Boolean</span></span>|<span data-ttu-id="49905-209">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="49905-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="49905-210">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49905-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="49905-211">proxyServer</span></span>|[<span data-ttu-id="49905-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="49905-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="49905-213">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="49905-213">Proxy Server.</span></span> <span data-ttu-id="49905-214">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="49905-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="49905-215">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="49905-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="49905-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-216">Boolean</span></span>|<span data-ttu-id="49905-217">会社の Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="49905-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="49905-218">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="49905-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="49905-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-219">Boolean</span></span>|<span data-ttu-id="49905-220">自宅 Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="49905-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="49905-221">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="49905-221">authenticationMethod</span></span>|[<span data-ttu-id="49905-222">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="49905-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="49905-223">認証方法。</span><span class="sxs-lookup"><span data-stu-id="49905-223">Authentication method.</span></span> <span data-ttu-id="49905-224">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="49905-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="49905-225">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="49905-225">rememberUserCredentials</span></span>|<span data-ttu-id="49905-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="49905-226">Boolean</span></span>|<span data-ttu-id="49905-227">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="49905-227">Remember user credentials.</span></span>|
|<span data-ttu-id="49905-228">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="49905-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="49905-229">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="49905-229">String collection</span></span>|<span data-ttu-id="49905-230">DNS サフィックス検索一覧。</span><span class="sxs-lookup"><span data-stu-id="49905-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="49905-231">応答</span><span class="sxs-lookup"><span data-stu-id="49905-231">Response</span></span>
<span data-ttu-id="49905-232">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="49905-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49905-233">例</span><span class="sxs-lookup"><span data-stu-id="49905-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="49905-234">要求</span><span class="sxs-lookup"><span data-stu-id="49905-234">Request</span></span>
<span data-ttu-id="49905-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49905-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="49905-236">応答</span><span class="sxs-lookup"><span data-stu-id="49905-236">Response</span></span>
<span data-ttu-id="49905-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49905-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```






