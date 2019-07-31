---
title: WindowsPhone81VpnConfiguration の更新
description: WindowsPhone81VpnConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae5d5583c7d87ad9c5f9495300ad7debcb39d977
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986450"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="d5563-103">WindowsPhone81VpnConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d5563-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="d5563-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5563-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5563-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5563-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5563-106">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5563-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5563-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5563-107">Prerequisites</span></span>
<span data-ttu-id="d5563-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5563-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5563-110">Permission type</span></span>|<span data-ttu-id="d5563-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5563-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5563-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5563-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5563-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5563-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5563-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5563-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5563-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5563-115">Not supported.</span></span>|
|<span data-ttu-id="d5563-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5563-116">Application</span></span>|<span data-ttu-id="d5563-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5563-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5563-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5563-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d5563-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5563-119">Request headers</span></span>
|<span data-ttu-id="d5563-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5563-120">Header</span></span>|<span data-ttu-id="d5563-121">値</span><span class="sxs-lookup"><span data-stu-id="d5563-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5563-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5563-122">Authorization</span></span>|<span data-ttu-id="d5563-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5563-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5563-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d5563-124">Accept</span></span>|<span data-ttu-id="d5563-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5563-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5563-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5563-126">Request body</span></span>
<span data-ttu-id="d5563-127">要求本文で、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5563-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="d5563-128">次の表に、 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d5563-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="d5563-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5563-129">Property</span></span>|<span data-ttu-id="d5563-130">型</span><span class="sxs-lookup"><span data-stu-id="d5563-130">Type</span></span>|<span data-ttu-id="d5563-131">説明</span><span class="sxs-lookup"><span data-stu-id="d5563-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5563-132">id</span><span class="sxs-lookup"><span data-stu-id="d5563-132">id</span></span>|<span data-ttu-id="d5563-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d5563-133">String</span></span>|<span data-ttu-id="d5563-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d5563-134">Key of the entity.</span></span> <span data-ttu-id="d5563-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5563-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d5563-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5563-137">DateTimeOffset</span></span>|<span data-ttu-id="d5563-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5563-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d5563-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5563-140">roleScopeTagIds</span></span>|<span data-ttu-id="d5563-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d5563-141">String collection</span></span>|<span data-ttu-id="d5563-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d5563-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5563-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5563-144">supportsScopeTags</span></span>|<span data-ttu-id="d5563-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-145">Boolean</span></span>|<span data-ttu-id="d5563-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d5563-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5563-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d5563-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5563-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d5563-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5563-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d5563-149">This property is read-only.</span></span> <span data-ttu-id="d5563-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d5563-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d5563-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d5563-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d5563-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="d5563-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d5563-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d5563-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d5563-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d5563-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d5563-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d5563-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d5563-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d5563-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d5563-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d5563-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d5563-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d5563-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d5563-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5563-163">createdDateTime</span></span>|<span data-ttu-id="d5563-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5563-164">DateTimeOffset</span></span>|<span data-ttu-id="d5563-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5563-165">DateTime the object was created.</span></span> <span data-ttu-id="d5563-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-167">description</span><span class="sxs-lookup"><span data-stu-id="d5563-167">description</span></span>|<span data-ttu-id="d5563-168">String</span><span class="sxs-lookup"><span data-stu-id="d5563-168">String</span></span>|<span data-ttu-id="d5563-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d5563-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5563-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d5563-171">displayName</span></span>|<span data-ttu-id="d5563-172">String</span><span class="sxs-lookup"><span data-stu-id="d5563-172">String</span></span>|<span data-ttu-id="d5563-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d5563-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5563-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-175">version</span><span class="sxs-lookup"><span data-stu-id="d5563-175">version</span></span>|<span data-ttu-id="d5563-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d5563-176">Int32</span></span>|<span data-ttu-id="d5563-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d5563-177">Version of the device configuration.</span></span> <span data-ttu-id="d5563-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="d5563-179">connectionName</span></span>|<span data-ttu-id="d5563-180">String</span><span class="sxs-lookup"><span data-stu-id="d5563-180">String</span></span>|<span data-ttu-id="d5563-181">ユーザーに表示される接続名。</span><span class="sxs-lookup"><span data-stu-id="d5563-181">Connection name displayed to the user.</span></span> <span data-ttu-id="d5563-182">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-183">サーバ</span><span class="sxs-lookup"><span data-stu-id="d5563-183">servers</span></span>|<span data-ttu-id="d5563-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d5563-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d5563-185">ネットワーク上の VPN サーバーの一覧。</span><span class="sxs-lookup"><span data-stu-id="d5563-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="d5563-186">エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d5563-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d5563-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d5563-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d5563-188">[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-189">customXml</span><span class="sxs-lookup"><span data-stu-id="d5563-189">customXml</span></span>|<span data-ttu-id="d5563-190">Binary</span><span class="sxs-lookup"><span data-stu-id="d5563-190">Binary</span></span>|<span data-ttu-id="d5563-191">VPN 接続を構成するカスタム XML コマンド。</span><span class="sxs-lookup"><span data-stu-id="d5563-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="d5563-192">(UTF8 でエンコードされたバイト配列)[Windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d5563-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="d5563-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="d5563-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-194">Boolean</span></span>|<span data-ttu-id="d5563-195">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d5563-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d5563-196">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5563-196">This property is read-only.</span></span> <span data-ttu-id="d5563-197">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d5563-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="d5563-198">connectionType</span></span>|[<span data-ttu-id="d5563-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d5563-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="d5563-200">接続の種類。</span><span class="sxs-lookup"><span data-stu-id="d5563-200">Connection type.</span></span> <span data-ttu-id="d5563-201">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d5563-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="d5563-202">使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。</span><span class="sxs-lookup"><span data-stu-id="d5563-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="d5563-203">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="d5563-203">loginGroupOrDomain</span></span>|<span data-ttu-id="d5563-204">String</span><span class="sxs-lookup"><span data-stu-id="d5563-204">String</span></span>|<span data-ttu-id="d5563-205">接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。</span><span class="sxs-lookup"><span data-stu-id="d5563-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d5563-206">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d5563-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-207">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d5563-207">enableSplitTunneling</span></span>|<span data-ttu-id="d5563-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-208">Boolean</span></span>|<span data-ttu-id="d5563-209">VPN の分割トンネリングを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d5563-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="d5563-210">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d5563-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d5563-211">proxyServer</span></span>|[<span data-ttu-id="d5563-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d5563-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="d5563-213">プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="d5563-213">Proxy Server.</span></span> <span data-ttu-id="d5563-214">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d5563-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5563-215">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="d5563-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="d5563-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-216">Boolean</span></span>|<span data-ttu-id="d5563-217">会社の Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="d5563-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="d5563-218">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="d5563-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="d5563-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-219">Boolean</span></span>|<span data-ttu-id="d5563-220">自宅 Wi-fi で VPN をバイパスします。</span><span class="sxs-lookup"><span data-stu-id="d5563-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="d5563-221">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d5563-221">authenticationMethod</span></span>|[<span data-ttu-id="d5563-222">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d5563-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d5563-223">認証方法。</span><span class="sxs-lookup"><span data-stu-id="d5563-223">Authentication method.</span></span> <span data-ttu-id="d5563-224">使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="d5563-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d5563-225">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="d5563-225">rememberUserCredentials</span></span>|<span data-ttu-id="d5563-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5563-226">Boolean</span></span>|<span data-ttu-id="d5563-227">ユーザーの資格情報を記憶します。</span><span class="sxs-lookup"><span data-stu-id="d5563-227">Remember user credentials.</span></span>|
|<span data-ttu-id="d5563-228">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="d5563-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="d5563-229">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d5563-229">String collection</span></span>|<span data-ttu-id="d5563-230">DNS サフィックス検索一覧。</span><span class="sxs-lookup"><span data-stu-id="d5563-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="d5563-231">応答</span><span class="sxs-lookup"><span data-stu-id="d5563-231">Response</span></span>
<span data-ttu-id="d5563-232">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d5563-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5563-233">例</span><span class="sxs-lookup"><span data-stu-id="d5563-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5563-234">要求</span><span class="sxs-lookup"><span data-stu-id="d5563-234">Request</span></span>
<span data-ttu-id="d5563-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5563-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5563-236">応答</span><span class="sxs-lookup"><span data-stu-id="d5563-236">Response</span></span>
<span data-ttu-id="d5563-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5563-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





