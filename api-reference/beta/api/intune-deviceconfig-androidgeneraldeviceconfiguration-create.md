---
title: Create androidGeneralDeviceConfiguration
description: 新しい androidGeneralDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f00283f4a416c09930ab99862355647dd038eab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341165"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="47375-103">Create androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="47375-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="47375-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47375-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47375-106">新しい [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="47375-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47375-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="47375-107">Prerequisites</span></span>
<span data-ttu-id="47375-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47375-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47375-110">Permission type</span></span>|<span data-ttu-id="47375-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47375-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47375-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47375-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47375-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47375-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47375-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47375-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47375-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47375-115">Not supported.</span></span>|
|<span data-ttu-id="47375-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47375-116">Application</span></span>|<span data-ttu-id="47375-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47375-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47375-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47375-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47375-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47375-119">Request headers</span></span>
|<span data-ttu-id="47375-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47375-120">Header</span></span>|<span data-ttu-id="47375-121">値</span><span class="sxs-lookup"><span data-stu-id="47375-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47375-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47375-122">Authorization</span></span>|<span data-ttu-id="47375-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="47375-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47375-124">承諾</span><span class="sxs-lookup"><span data-stu-id="47375-124">Accept</span></span>|<span data-ttu-id="47375-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47375-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47375-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="47375-126">Request body</span></span>
<span data-ttu-id="47375-127">要求本文で、androidGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="47375-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="47375-128">次の表に、androidGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="47375-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47375-129">Property</span></span>|<span data-ttu-id="47375-130">型</span><span class="sxs-lookup"><span data-stu-id="47375-130">Type</span></span>|<span data-ttu-id="47375-131">説明</span><span class="sxs-lookup"><span data-stu-id="47375-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47375-132">id</span><span class="sxs-lookup"><span data-stu-id="47375-132">id</span></span>|<span data-ttu-id="47375-133">文字列</span><span class="sxs-lookup"><span data-stu-id="47375-133">String</span></span>|<span data-ttu-id="47375-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47375-134">Key of the entity.</span></span> <span data-ttu-id="47375-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47375-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47375-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47375-137">DateTimeOffset</span></span>|<span data-ttu-id="47375-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="47375-138">DateTime the object was last modified.</span></span> <span data-ttu-id="47375-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47375-140">roleScopeTagIds</span></span>|<span data-ttu-id="47375-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-141">String collection</span></span>|<span data-ttu-id="47375-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="47375-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47375-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47375-144">supportsScopeTags</span></span>|<span data-ttu-id="47375-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-145">Boolean</span></span>|<span data-ttu-id="47375-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47375-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="47375-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47375-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="47375-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47375-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="47375-149">This property is read-only.</span></span> <span data-ttu-id="47375-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47375-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47375-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47375-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47375-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="47375-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47375-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47375-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47375-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47375-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47375-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="47375-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47375-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="47375-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47375-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="47375-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47375-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="47375-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47375-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47375-163">createdDateTime</span></span>|<span data-ttu-id="47375-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47375-164">DateTimeOffset</span></span>|<span data-ttu-id="47375-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="47375-165">DateTime the object was created.</span></span> <span data-ttu-id="47375-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-167">description</span><span class="sxs-lookup"><span data-stu-id="47375-167">description</span></span>|<span data-ttu-id="47375-168">String</span><span class="sxs-lookup"><span data-stu-id="47375-168">String</span></span>|<span data-ttu-id="47375-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="47375-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47375-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-171">displayName</span><span class="sxs-lookup"><span data-stu-id="47375-171">displayName</span></span>|<span data-ttu-id="47375-172">String</span><span class="sxs-lookup"><span data-stu-id="47375-172">String</span></span>|<span data-ttu-id="47375-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="47375-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47375-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-175">version</span><span class="sxs-lookup"><span data-stu-id="47375-175">version</span></span>|<span data-ttu-id="47375-176">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-176">Int32</span></span>|<span data-ttu-id="47375-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="47375-177">Version of the device configuration.</span></span> <span data-ttu-id="47375-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="47375-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47375-179">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="47375-179">appsBlockClipboardSharing</span></span>|<span data-ttu-id="47375-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-180">Boolean</span></span>|<span data-ttu-id="47375-181">アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-181">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="47375-182">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="47375-182">appsBlockCopyPaste</span></span>|<span data-ttu-id="47375-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-183">Boolean</span></span>|<span data-ttu-id="47375-184">アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-184">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="47375-185">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="47375-185">appsBlockYouTube</span></span>|<span data-ttu-id="47375-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-186">Boolean</span></span>|<span data-ttu-id="47375-187">YouTube アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-187">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="47375-188">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-188">bluetoothBlocked</span></span>|<span data-ttu-id="47375-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-189">Boolean</span></span>|<span data-ttu-id="47375-190">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-190">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="47375-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-191">cameraBlocked</span></span>|<span data-ttu-id="47375-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-192">Boolean</span></span>|<span data-ttu-id="47375-193">カメラの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-193">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="47375-194">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="47375-194">cellularBlockDataRoaming</span></span>|<span data-ttu-id="47375-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-195">Boolean</span></span>|<span data-ttu-id="47375-196">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-196">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="47375-197">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="47375-197">cellularBlockMessaging</span></span>|<span data-ttu-id="47375-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-198">Boolean</span></span>|<span data-ttu-id="47375-199">SMS/MMS メッセージングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-199">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="47375-200">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="47375-200">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="47375-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-201">Boolean</span></span>|<span data-ttu-id="47375-202">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-202">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="47375-203">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="47375-203">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="47375-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-204">Boolean</span></span>|<span data-ttu-id="47375-205">Wi-Fi テザリングの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-205">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="47375-206">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="47375-206">compliantAppsList</span></span>|<span data-ttu-id="47375-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="47375-208">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="47375-208">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="47375-209">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="47375-209">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="47375-210">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="47375-210">compliantAppListType</span></span>|[<span data-ttu-id="47375-211">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="47375-211">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="47375-212">CompliantAppsList 内にあるリストの種類。</span><span class="sxs-lookup"><span data-stu-id="47375-212">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="47375-213">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="47375-213">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="47375-214">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="47375-214">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="47375-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-215">Boolean</span></span>|<span data-ttu-id="47375-216">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-216">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="47375-217">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-217">locationServicesBlocked</span></span>|<span data-ttu-id="47375-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-218">Boolean</span></span>|<span data-ttu-id="47375-219">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-219">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="47375-220">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="47375-220">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="47375-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-221">Boolean</span></span>|<span data-ttu-id="47375-222">Google アカウントの自動同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-222">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="47375-223">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-223">googlePlayStoreBlocked</span></span>|<span data-ttu-id="47375-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-224">Boolean</span></span>|<span data-ttu-id="47375-225">Google Play ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-225">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="47375-226">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="47375-226">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="47375-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-227">Boolean</span></span>|<span data-ttu-id="47375-228">キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-228">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="47375-229">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="47375-229">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="47375-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-230">Boolean</span></span>|<span data-ttu-id="47375-231">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-231">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="47375-232">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="47375-232">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="47375-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-233">Boolean</span></span>|<span data-ttu-id="47375-234">KNOX モードの間に日付と時刻の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-234">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="47375-235">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="47375-235">kioskModeApps</span></span>|<span data-ttu-id="47375-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="47375-237">デバイスがキオスク モードのときに実行できるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="47375-237">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="47375-238">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="47375-238">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47375-239">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-239">nfcBlocked</span></span>|<span data-ttu-id="47375-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-240">Boolean</span></span>|<span data-ttu-id="47375-241">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-241">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="47375-242">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="47375-242">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="47375-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-243">Boolean</span></span>|<span data-ttu-id="47375-244">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-244">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="47375-245">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="47375-245">passwordBlockTrustAgents</span></span>|<span data-ttu-id="47375-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-246">Boolean</span></span>|<span data-ttu-id="47375-247">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-247">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="47375-248">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="47375-248">passwordExpirationDays</span></span>|<span data-ttu-id="47375-249">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-249">Int32</span></span>|<span data-ttu-id="47375-250">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="47375-250">Number of days before the password expires.</span></span> <span data-ttu-id="47375-251">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="47375-251">Valid values 1 to 365</span></span>|
|<span data-ttu-id="47375-252">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="47375-252">passwordMinimumLength</span></span>|<span data-ttu-id="47375-253">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-253">Int32</span></span>|<span data-ttu-id="47375-254">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="47375-254">Minimum length of passwords.</span></span> <span data-ttu-id="47375-255">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="47375-255">Valid values 4 to 16</span></span>|
|<span data-ttu-id="47375-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="47375-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="47375-257">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-257">Int32</span></span>|<span data-ttu-id="47375-258">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="47375-258">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="47375-259">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="47375-259">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="47375-260">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-260">Int32</span></span>|<span data-ttu-id="47375-261">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="47375-261">Number of previous passwords to block.</span></span> <span data-ttu-id="47375-262">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="47375-262">Valid values 0 to 24</span></span>|
|<span data-ttu-id="47375-263">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="47375-263">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="47375-264">Int32</span><span class="sxs-lookup"><span data-stu-id="47375-264">Int32</span></span>|<span data-ttu-id="47375-265">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="47375-265">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="47375-266">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="47375-266">Valid values 1 to 16</span></span>|
|<span data-ttu-id="47375-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="47375-267">passwordRequiredType</span></span>|[<span data-ttu-id="47375-268">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="47375-268">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="47375-269">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="47375-269">Type of password that is required.</span></span> <span data-ttu-id="47375-270">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="47375-270">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="47375-271">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="47375-271">passwordRequired</span></span>|<span data-ttu-id="47375-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-272">Boolean</span></span>|<span data-ttu-id="47375-273">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="47375-273">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="47375-274">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-274">powerOffBlocked</span></span>|<span data-ttu-id="47375-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-275">Boolean</span></span>|<span data-ttu-id="47375-276">デバイスの電源オフをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-276">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="47375-277">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-277">factoryResetBlocked</span></span>|<span data-ttu-id="47375-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-278">Boolean</span></span>|<span data-ttu-id="47375-279">ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-279">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="47375-280">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-280">screenCaptureBlocked</span></span>|<span data-ttu-id="47375-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-281">Boolean</span></span>|<span data-ttu-id="47375-282">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-282">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="47375-283">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="47375-283">deviceSharingAllowed</span></span>|<span data-ttu-id="47375-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-284">Boolean</span></span>|<span data-ttu-id="47375-285">デバイスの共有モードを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-285">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="47375-286">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="47375-286">storageBlockGoogleBackup</span></span>|<span data-ttu-id="47375-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-287">Boolean</span></span>|<span data-ttu-id="47375-288">Google バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-288">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="47375-289">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="47375-289">storageBlockRemovableStorage</span></span>|<span data-ttu-id="47375-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-290">Boolean</span></span>|<span data-ttu-id="47375-291">リムーバブル記憶域の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-291">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="47375-292">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="47375-292">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="47375-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-293">Boolean</span></span>|<span data-ttu-id="47375-294">デバイスの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-294">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="47375-295">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="47375-295">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="47375-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-296">Boolean</span></span>|<span data-ttu-id="47375-297">リムーバブル記憶域の暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-297">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="47375-298">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-298">voiceAssistantBlocked</span></span>|<span data-ttu-id="47375-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-299">Boolean</span></span>|<span data-ttu-id="47375-300">音声アシスタントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-300">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="47375-301">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-301">voiceDialingBlocked</span></span>|<span data-ttu-id="47375-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-302">Boolean</span></span>|<span data-ttu-id="47375-303">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-303">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="47375-304">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="47375-304">webBrowserBlockPopups</span></span>|<span data-ttu-id="47375-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-305">Boolean</span></span>|<span data-ttu-id="47375-306">Web ブラウザー内のポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-306">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="47375-307">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="47375-307">webBrowserBlockAutofill</span></span>|<span data-ttu-id="47375-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-308">Boolean</span></span>|<span data-ttu-id="47375-309">Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-309">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="47375-310">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="47375-310">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="47375-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-311">Boolean</span></span>|<span data-ttu-id="47375-312">Web ブラウザー内の JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-312">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="47375-313">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-313">webBrowserBlocked</span></span>|<span data-ttu-id="47375-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-314">Boolean</span></span>|<span data-ttu-id="47375-315">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-315">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="47375-316">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="47375-316">webBrowserCookieSettings</span></span>|[<span data-ttu-id="47375-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="47375-317">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="47375-318">Web ブラウザー内の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="47375-318">Cookie settings within the web browser.</span></span> <span data-ttu-id="47375-319">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="47375-319">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="47375-320">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="47375-320">wiFiBlocked</span></span>|<span data-ttu-id="47375-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-321">Boolean</span></span>|<span data-ttu-id="47375-322">Wi-Fi の同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="47375-322">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="47375-323">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="47375-323">appsInstallAllowList</span></span>|<span data-ttu-id="47375-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="47375-325">KNOX デバイス上にインストールできるアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="47375-325">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="47375-326">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="47375-326">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47375-327">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="47375-327">appsLaunchBlockList</span></span>|<span data-ttu-id="47375-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="47375-329">KNOX デバイス上での起動がブロックされているアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="47375-329">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="47375-330">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="47375-330">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47375-331">appsHideList</span><span class="sxs-lookup"><span data-stu-id="47375-331">appsHideList</span></span>|<span data-ttu-id="47375-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47375-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="47375-333">KNOX デバイス上で非表示にするアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="47375-333">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="47375-334">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="47375-334">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47375-335">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="47375-335">securityRequireVerifyApps</span></span>|<span data-ttu-id="47375-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="47375-336">Boolean</span></span>|<span data-ttu-id="47375-337">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="47375-337">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="47375-338">応答</span><span class="sxs-lookup"><span data-stu-id="47375-338">Response</span></span>
<span data-ttu-id="47375-339">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="47375-339">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47375-340">例</span><span class="sxs-lookup"><span data-stu-id="47375-340">Example</span></span>

### <a name="request"></a><span data-ttu-id="47375-341">要求</span><span class="sxs-lookup"><span data-stu-id="47375-341">Request</span></span>
<span data-ttu-id="47375-342">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47375-342">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3934

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="47375-343">応答</span><span class="sxs-lookup"><span data-stu-id="47375-343">Response</span></span>
<span data-ttu-id="47375-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47375-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4106

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```






