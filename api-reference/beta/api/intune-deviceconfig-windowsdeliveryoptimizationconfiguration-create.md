---
title: WindowsDeliveryOptimizationConfiguration を作成する
description: 新しい windowsDeliveryOptimizationConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b504d7a403aec15fad14ae370bf4d76fb7bf7f6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977619"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="4cb7f-103">WindowsDeliveryOptimizationConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="4cb7f-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="4cb7f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cb7f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cb7f-106">新しい[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-106">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cb7f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4cb7f-107">Prerequisites</span></span>
<span data-ttu-id="4cb7f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb7f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4cb7f-110">Permission type</span></span>|<span data-ttu-id="4cb7f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4cb7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cb7f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4cb7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cb7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cb7f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4cb7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cb7f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-115">Not supported.</span></span>|
|<span data-ttu-id="4cb7f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4cb7f-116">Application</span></span>|<span data-ttu-id="4cb7f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cb7f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4cb7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4cb7f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cb7f-119">Request headers</span></span>
|<span data-ttu-id="4cb7f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cb7f-120">Header</span></span>|<span data-ttu-id="4cb7f-121">値</span><span class="sxs-lookup"><span data-stu-id="4cb7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cb7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb7f-122">Authorization</span></span>|<span data-ttu-id="4cb7f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cb7f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4cb7f-124">Accept</span></span>|<span data-ttu-id="4cb7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cb7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb7f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4cb7f-126">Request body</span></span>
<span data-ttu-id="4cb7f-127">要求本文で、windowsDeliveryOptimizationConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-127">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="4cb7f-128">次の表に、windowsDeliveryOptimizationConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-128">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="4cb7f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb7f-129">Property</span></span>|<span data-ttu-id="4cb7f-130">型</span><span class="sxs-lookup"><span data-stu-id="4cb7f-130">Type</span></span>|<span data-ttu-id="4cb7f-131">説明</span><span class="sxs-lookup"><span data-stu-id="4cb7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb7f-132">id</span><span class="sxs-lookup"><span data-stu-id="4cb7f-132">id</span></span>|<span data-ttu-id="4cb7f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4cb7f-133">String</span></span>|<span data-ttu-id="4cb7f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-134">Key of the entity.</span></span> <span data-ttu-id="4cb7f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb7f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4cb7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb7f-137">DateTimeOffset</span></span>|<span data-ttu-id="4cb7f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4cb7f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4cb7f-140">roleScopeTagIds</span></span>|<span data-ttu-id="4cb7f-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="4cb7f-141">String collection</span></span>|<span data-ttu-id="4cb7f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4cb7f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4cb7f-144">supportsScopeTags</span></span>|<span data-ttu-id="4cb7f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb7f-145">Boolean</span></span>|<span data-ttu-id="4cb7f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4cb7f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4cb7f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4cb7f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-149">This property is read-only.</span></span> <span data-ttu-id="4cb7f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4cb7f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4cb7f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4cb7f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4cb7f-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4cb7f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4cb7f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4cb7f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4cb7f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4cb7f-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4cb7f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4cb7f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4cb7f-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4cb7f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4cb7f-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4cb7f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb7f-163">createdDateTime</span></span>|<span data-ttu-id="4cb7f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb7f-164">DateTimeOffset</span></span>|<span data-ttu-id="4cb7f-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-165">DateTime the object was created.</span></span> <span data-ttu-id="4cb7f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-167">description</span><span class="sxs-lookup"><span data-stu-id="4cb7f-167">description</span></span>|<span data-ttu-id="4cb7f-168">String</span><span class="sxs-lookup"><span data-stu-id="4cb7f-168">String</span></span>|<span data-ttu-id="4cb7f-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4cb7f-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4cb7f-171">displayName</span></span>|<span data-ttu-id="4cb7f-172">String</span><span class="sxs-lookup"><span data-stu-id="4cb7f-172">String</span></span>|<span data-ttu-id="4cb7f-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4cb7f-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-175">version</span><span class="sxs-lookup"><span data-stu-id="4cb7f-175">version</span></span>|<span data-ttu-id="4cb7f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-176">Int32</span></span>|<span data-ttu-id="4cb7f-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-177">Version of the device configuration.</span></span> <span data-ttu-id="4cb7f-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4cb7f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cb7f-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4cb7f-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="4cb7f-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4cb7f-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="4cb7f-181">大規模なコンテンツ配信シナリオのネットワーク帯域幅の消費を管理するために、配信の最適化で使用できるダウンロード方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="4cb7f-182">可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="4cb7f-183">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="4cb7f-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="4cb7f-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="4cb7f-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="4cb7f-185">選択したオプションを使用してピアの選択を制限するように指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="4cb7f-186">オプション 1 (サブネットマスク) は、配信最適化モードのダウンロードモード LAN (1) とグループ (2) にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="4cb7f-187">可能な値は、`notConfigured`、`subnetMask` です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="4cb7f-188">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="4cb7f-188">groupIdSource</span></span>|[<span data-ttu-id="4cb7f-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="4cb7f-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="4cb7f-190">ピア選択を固有ソースに制限するように指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="4cb7f-191">このポリシーで設定されたオプションは、配信最適化モードグループ (2) ダウンロードモードにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="4cb7f-192">グループ (2) がダウンロードモードに設定されていない場合、このポリシーは無視されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="4cb7f-193">オプション 3-DHCP オプション ID の場合、クライアントは DHCP オプション ID 234 に対してクエリを実行し、返された GUID 値をグループ ID として使用します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="4cb7f-194">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="4cb7f-194">bandwidthMode</span></span>|[<span data-ttu-id="4cb7f-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="4cb7f-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="4cb7f-196">パーセント、absolutes、または時間を使用して、フォアグラウンドおよびバックグラウンドの帯域幅の使用を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="4cb7f-197">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4cb7f-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4cb7f-198">Int64</span><span class="sxs-lookup"><span data-stu-id="4cb7f-198">Int64</span></span>|<span data-ttu-id="4cb7f-199">ピアツーピアの使用が許可されているバックグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="4cb7f-200">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="4cb7f-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="4cb7f-201">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4cb7f-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4cb7f-202">Int64</span><span class="sxs-lookup"><span data-stu-id="4cb7f-202">Int64</span></span>|<span data-ttu-id="4cb7f-203">ピアツーピア (0-86400) の使用が許可されているフォアグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="4cb7f-204">有効な値は 0 ~ 86400</span><span class="sxs-lookup"><span data-stu-id="4cb7f-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="4cb7f-205">0を指定すると、クラウドサービスを使用してこの設定を管理するための配信の最適化が設定されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="4cb7f-206">有効な値は 0 ~ 86400</span><span class="sxs-lookup"><span data-stu-id="4cb7f-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="4cb7f-207">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="4cb7f-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4cb7f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-208">Int32</span></span>|<span data-ttu-id="4cb7f-209">ピアキャッシュを使用するための最小 RAM サイズを GB 単位で指定します (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4cb7f-210">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="4cb7f-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4cb7f-211">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="4cb7f-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4cb7f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-212">Int32</span></span>|<span data-ttu-id="4cb7f-213">ピアキャッシュ (1-100000) を使用するための最小ディスクサイズを GB 単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4cb7f-214">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="4cb7f-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="4cb7f-215">推奨値:64 GB から 256 GB。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="4cb7f-216">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="4cb7f-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4cb7f-217">minimumFileSizeToCacheInMegabytes バイト</span><span class="sxs-lookup"><span data-stu-id="4cb7f-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="4cb7f-218">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-218">Int32</span></span>|<span data-ttu-id="4cb7f-219">ピアキャッシュを使用するために有効にするコンテンツファイルの最小サイズを MB 単位で指定します (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4cb7f-220">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="4cb7f-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="4cb7f-221">推奨値: 1 MB ~ 10万 MB。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="4cb7f-222">有効な値は 1 ~ 10万</span><span class="sxs-lookup"><span data-stu-id="4cb7f-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4cb7f-223">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="4cb7f-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="4cb7f-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-224">Int32</span></span>|<span data-ttu-id="4cb7f-225">デバイスがデータをアップロードできるように、最小バッテリの割合 (0-100) を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="4cb7f-226">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="4cb7f-226">Valid values 0 to 100</span></span>
<span data-ttu-id="4cb7f-227">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-227">The default value is 0.</span></span> <span data-ttu-id="4cb7f-228">値 0 (ゼロ) は "制限なし" を意味し、クラウドサービスの既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="4cb7f-229">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="4cb7f-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4cb7f-230">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="4cb7f-230">modifyCacheLocation</span></span>|<span data-ttu-id="4cb7f-231">String</span><span class="sxs-lookup"><span data-stu-id="4cb7f-231">String</span></span>|<span data-ttu-id="4cb7f-232">配信の最適化でキャッシュに使用するドライブを指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="4cb7f-233">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="4cb7f-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="4cb7f-234">Int32</span><span class="sxs-lookup"><span data-stu-id="4cb7f-234">Int32</span></span>|<span data-ttu-id="4cb7f-235">正常にダウンロードされた後に、各ファイルが配信最適化キャッシュに保持される最大時間 (0-3650) を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="4cb7f-236">有効な値は 0 ~ 3650</span><span class="sxs-lookup"><span data-stu-id="4cb7f-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="4cb7f-237">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="4cb7f-237">maximumCacheSize</span></span>|[<span data-ttu-id="4cb7f-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="4cb7f-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="4cb7f-239">配信最適化の最大キャッシュサイズをパーセンテージまたは GB で指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="4cb7f-240">vpnPeerCaching キャッシュ</span><span class="sxs-lookup"><span data-stu-id="4cb7f-240">vpnPeerCaching</span></span>|[<span data-ttu-id="4cb7f-241">購入</span><span class="sxs-lookup"><span data-stu-id="4cb7f-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4cb7f-242">ドメインネットワークに VPN 経由で接続している間、デバイスがピアキャッシュへの参加を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="4cb7f-243">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="4cb7f-244">応答</span><span class="sxs-lookup"><span data-stu-id="4cb7f-244">Response</span></span>
<span data-ttu-id="4cb7f-245">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-245">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cb7f-246">例</span><span class="sxs-lookup"><span data-stu-id="4cb7f-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cb7f-247">要求</span><span class="sxs-lookup"><span data-stu-id="4cb7f-247">Request</span></span>
<span data-ttu-id="4cb7f-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1833

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
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="4cb7f-249">応答</span><span class="sxs-lookup"><span data-stu-id="4cb7f-249">Response</span></span>
<span data-ttu-id="4cb7f-p128">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4cb7f-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2005

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
  "vpnPeerCaching": "enabled"
}
```





