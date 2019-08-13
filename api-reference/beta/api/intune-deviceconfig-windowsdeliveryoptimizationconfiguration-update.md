---
title: WindowsDeliveryOptimizationConfiguration の更新
description: WindowsDeliveryOptimizationConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2573233d0db47bffcfcbf80a0a74d4acfcbfab62
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344547"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="8d509-103">WindowsDeliveryOptimizationConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="8d509-103">Update windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="8d509-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d509-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d509-106">[WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d509-106">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d509-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d509-107">Prerequisites</span></span>
<span data-ttu-id="8d509-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d509-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d509-110">Permission type</span></span>|<span data-ttu-id="8d509-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d509-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d509-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d509-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d509-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d509-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d509-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d509-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d509-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d509-115">Not supported.</span></span>|
|<span data-ttu-id="8d509-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d509-116">Application</span></span>|<span data-ttu-id="8d509-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d509-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d509-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d509-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8d509-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d509-119">Request headers</span></span>
|<span data-ttu-id="8d509-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d509-120">Header</span></span>|<span data-ttu-id="8d509-121">値</span><span class="sxs-lookup"><span data-stu-id="8d509-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d509-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d509-122">Authorization</span></span>|<span data-ttu-id="8d509-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d509-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d509-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8d509-124">Accept</span></span>|<span data-ttu-id="8d509-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d509-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d509-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d509-126">Request body</span></span>
<span data-ttu-id="8d509-127">要求本文で、 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-127">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="8d509-128">次の表に、 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8d509-128">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="8d509-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d509-129">Property</span></span>|<span data-ttu-id="8d509-130">型</span><span class="sxs-lookup"><span data-stu-id="8d509-130">Type</span></span>|<span data-ttu-id="8d509-131">説明</span><span class="sxs-lookup"><span data-stu-id="8d509-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d509-132">id</span><span class="sxs-lookup"><span data-stu-id="8d509-132">id</span></span>|<span data-ttu-id="8d509-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8d509-133">String</span></span>|<span data-ttu-id="8d509-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8d509-134">Key of the entity.</span></span> <span data-ttu-id="8d509-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d509-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d509-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d509-137">DateTimeOffset</span></span>|<span data-ttu-id="8d509-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8d509-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8d509-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d509-140">roleScopeTagIds</span></span>|<span data-ttu-id="8d509-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d509-141">String collection</span></span>|<span data-ttu-id="8d509-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8d509-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d509-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8d509-144">supportsScopeTags</span></span>|<span data-ttu-id="8d509-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d509-145">Boolean</span></span>|<span data-ttu-id="8d509-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d509-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d509-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8d509-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d509-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8d509-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d509-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8d509-149">This property is read-only.</span></span> <span data-ttu-id="8d509-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8d509-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8d509-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8d509-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8d509-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="8d509-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8d509-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d509-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8d509-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d509-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8d509-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8d509-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8d509-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8d509-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8d509-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="8d509-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8d509-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="8d509-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8d509-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d509-163">createdDateTime</span></span>|<span data-ttu-id="8d509-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d509-164">DateTimeOffset</span></span>|<span data-ttu-id="8d509-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8d509-165">DateTime the object was created.</span></span> <span data-ttu-id="8d509-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-167">description</span><span class="sxs-lookup"><span data-stu-id="8d509-167">description</span></span>|<span data-ttu-id="8d509-168">String</span><span class="sxs-lookup"><span data-stu-id="8d509-168">String</span></span>|<span data-ttu-id="8d509-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8d509-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d509-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8d509-171">displayName</span></span>|<span data-ttu-id="8d509-172">String</span><span class="sxs-lookup"><span data-stu-id="8d509-172">String</span></span>|<span data-ttu-id="8d509-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8d509-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d509-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-175">version</span><span class="sxs-lookup"><span data-stu-id="8d509-175">version</span></span>|<span data-ttu-id="8d509-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-176">Int32</span></span>|<span data-ttu-id="8d509-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8d509-177">Version of the device configuration.</span></span> <span data-ttu-id="8d509-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d509-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d509-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="8d509-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="8d509-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="8d509-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="8d509-181">大規模なコンテンツ配信シナリオのネットワーク帯域幅の消費を管理するために、配信の最適化で使用できるダウンロード方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="8d509-182">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="8d509-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="8d509-183">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="8d509-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="8d509-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="8d509-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="8d509-185">選択したオプションを使用してピアの選択を制限するように指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="8d509-186">オプション 1 (サブネットマスク) は、配信最適化モードのダウンロードモード LAN (1) とグループ (2) にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="8d509-187">可能な値は、`notConfigured`、`subnetMask` です。</span><span class="sxs-lookup"><span data-stu-id="8d509-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="8d509-188">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="8d509-188">groupIdSource</span></span>|[<span data-ttu-id="8d509-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="8d509-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="8d509-190">ピア選択を固有ソースに制限するように指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="8d509-191">このポリシーで設定されたオプションは、配信最適化モードグループ (2) ダウンロードモードにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="8d509-192">グループ (2) がダウンロードモードに設定されていない場合、このポリシーは無視されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="8d509-193">オプション 3-DHCP オプション ID の場合、クライアントは DHCP オプション ID 234 に対してクエリを実行し、返された GUID 値をグループ ID として使用します。</span><span class="sxs-lookup"><span data-stu-id="8d509-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="8d509-194">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="8d509-194">bandwidthMode</span></span>|[<span data-ttu-id="8d509-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="8d509-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="8d509-196">パーセント、absolutes、または時間を使用して、フォアグラウンドおよびバックグラウンドの帯域幅の使用を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="8d509-197">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8d509-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="8d509-198">Int64</span><span class="sxs-lookup"><span data-stu-id="8d509-198">Int64</span></span>|<span data-ttu-id="8d509-199">ピアツーピアの使用が許可されているバックグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="8d509-200">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="8d509-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="8d509-201">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8d509-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="8d509-202">Int64</span><span class="sxs-lookup"><span data-stu-id="8d509-202">Int64</span></span>|<span data-ttu-id="8d509-203">ピアツーピア (0-86400) の使用が許可されているフォアグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="8d509-204">有効な値は 0 ~ 86400</span><span class="sxs-lookup"><span data-stu-id="8d509-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="8d509-205">0を指定すると、クラウドサービスを使用してこの設定を管理するための配信の最適化が設定されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="8d509-206">有効な値は 0 ~ 86400</span><span class="sxs-lookup"><span data-stu-id="8d509-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="8d509-207">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="8d509-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="8d509-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-208">Int32</span></span>|<span data-ttu-id="8d509-209">ピアキャッシュを使用するための最小 RAM サイズを GB 単位で指定します (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="8d509-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="8d509-210">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="8d509-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="8d509-211">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="8d509-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="8d509-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-212">Int32</span></span>|<span data-ttu-id="8d509-213">ピアキャッシュ (1-100000) を使用するための最小ディスクサイズを GB 単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="8d509-214">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="8d509-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="8d509-215">推奨値:64 GB から 256 GB。</span><span class="sxs-lookup"><span data-stu-id="8d509-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="8d509-216">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="8d509-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="8d509-217">minimumFileSizeToCacheInMegabytes バイト</span><span class="sxs-lookup"><span data-stu-id="8d509-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="8d509-218">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-218">Int32</span></span>|<span data-ttu-id="8d509-219">ピアキャッシュを使用するために有効にするコンテンツファイルの最小サイズを MB 単位で指定します (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="8d509-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="8d509-220">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="8d509-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="8d509-221">推奨値: 1 MB ~ 10万 MB。</span><span class="sxs-lookup"><span data-stu-id="8d509-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="8d509-222">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="8d509-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="8d509-223">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="8d509-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="8d509-224">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-224">Int32</span></span>|<span data-ttu-id="8d509-225">デバイスがデータをアップロードできるように、最小バッテリの割合 (0-100) を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="8d509-226">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d509-226">Valid values 0 to 100</span></span>
<span data-ttu-id="8d509-227">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="8d509-227">The default value is 0.</span></span> <span data-ttu-id="8d509-228">値 0 (ゼロ) は "制限なし" を意味し、クラウドサービスの既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="8d509-229">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="8d509-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8d509-230">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="8d509-230">modifyCacheLocation</span></span>|<span data-ttu-id="8d509-231">String</span><span class="sxs-lookup"><span data-stu-id="8d509-231">String</span></span>|<span data-ttu-id="8d509-232">配信の最適化でキャッシュに使用するドライブを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="8d509-233">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="8d509-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="8d509-234">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-234">Int32</span></span>|<span data-ttu-id="8d509-235">正常にダウンロードされた後に、各ファイルが配信最適化キャッシュに保持される最大時間 (0-3650) を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="8d509-236">有効な値は 0 ~ 3650</span><span class="sxs-lookup"><span data-stu-id="8d509-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="8d509-237">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="8d509-237">maximumCacheSize</span></span>|[<span data-ttu-id="8d509-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="8d509-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="8d509-239">配信最適化の最大キャッシュサイズをパーセンテージまたは GB で指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="8d509-240">vpnPeerCaching キャッシュ</span><span class="sxs-lookup"><span data-stu-id="8d509-240">vpnPeerCaching</span></span>|[<span data-ttu-id="8d509-241">購入</span><span class="sxs-lookup"><span data-stu-id="8d509-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8d509-242">ドメインネットワークに VPN 経由で接続している間、デバイスがピアキャッシュへの参加を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="8d509-243">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8d509-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8d509-244">cacheServerHostNames 名</span><span class="sxs-lookup"><span data-stu-id="8d509-244">cacheServerHostNames</span></span>|<span data-ttu-id="8d509-245">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d509-245">String collection</span></span>|<span data-ttu-id="8d509-246">キャッシュサーバーのホスト名を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-246">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="8d509-247">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8d509-247">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="8d509-248">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-248">Int32</span></span>|<span data-ttu-id="8d509-249">フォアグラウンドダウンロードのためにキャッシュサーバーから HTTP ソースへのフォールバックを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-249">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="8d509-250">有効な値は0から2592000です。</span><span class="sxs-lookup"><span data-stu-id="8d509-250">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="8d509-251">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8d509-251">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="8d509-252">Int32</span><span class="sxs-lookup"><span data-stu-id="8d509-252">Int32</span></span>|<span data-ttu-id="8d509-253">バックグラウンドをダウンロードするためにキャッシュサーバーから HTTP ソースへのフォールバックを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d509-253">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="8d509-254">有効な値は0から2592000です。</span><span class="sxs-lookup"><span data-stu-id="8d509-254">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="8d509-255">応答</span><span class="sxs-lookup"><span data-stu-id="8d509-255">Response</span></span>
<span data-ttu-id="8d509-256">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d509-256">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d509-257">例</span><span class="sxs-lookup"><span data-stu-id="8d509-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d509-258">要求</span><span class="sxs-lookup"><span data-stu-id="8d509-258">Request</span></span>
<span data-ttu-id="8d509-259">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d509-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2039

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```

### <a name="response"></a><span data-ttu-id="8d509-260">応答</span><span class="sxs-lookup"><span data-stu-id="8d509-260">Response</span></span>
<span data-ttu-id="8d509-p130">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d509-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2211

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```






