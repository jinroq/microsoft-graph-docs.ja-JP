---
title: Create windowsPhone81GeneralConfiguration
description: 新しい windowsPhone81GeneralConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0485c2ca9618fd671b3855c59a8bb38cbb73a7b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982187"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="4ee60-103">Create windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ee60-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="4ee60-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ee60-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ee60-106">新しい [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ee60-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4ee60-107">Prerequisites</span></span>
<span data-ttu-id="4ee60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ee60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee60-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ee60-110">Permission type</span></span>|<span data-ttu-id="4ee60-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ee60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ee60-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ee60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ee60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ee60-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ee60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ee60-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-115">Not supported.</span></span>|
|<span data-ttu-id="4ee60-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ee60-116">Application</span></span>|<span data-ttu-id="4ee60-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ee60-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ee60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ee60-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ee60-119">Request headers</span></span>
|<span data-ttu-id="4ee60-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ee60-120">Header</span></span>|<span data-ttu-id="4ee60-121">値</span><span class="sxs-lookup"><span data-stu-id="4ee60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ee60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ee60-122">Authorization</span></span>|<span data-ttu-id="4ee60-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ee60-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4ee60-124">Accept</span></span>|<span data-ttu-id="4ee60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ee60-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ee60-126">Request body</span></span>
<span data-ttu-id="4ee60-127">要求本文で、windowsPhone81GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="4ee60-128">次の表に、windowsPhone81GeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="4ee60-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ee60-129">Property</span></span>|<span data-ttu-id="4ee60-130">型</span><span class="sxs-lookup"><span data-stu-id="4ee60-130">Type</span></span>|<span data-ttu-id="4ee60-131">説明</span><span class="sxs-lookup"><span data-stu-id="4ee60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ee60-132">id</span><span class="sxs-lookup"><span data-stu-id="4ee60-132">id</span></span>|<span data-ttu-id="4ee60-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4ee60-133">String</span></span>|<span data-ttu-id="4ee60-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4ee60-134">Key of the entity.</span></span> <span data-ttu-id="4ee60-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ee60-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ee60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ee60-137">DateTimeOffset</span></span>|<span data-ttu-id="4ee60-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4ee60-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ee60-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ee60-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ee60-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="4ee60-141">String collection</span></span>|<span data-ttu-id="4ee60-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4ee60-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ee60-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ee60-144">supportsScopeTags</span></span>|<span data-ttu-id="4ee60-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-145">Boolean</span></span>|<span data-ttu-id="4ee60-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ee60-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ee60-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4ee60-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ee60-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-149">This property is read-only.</span></span> <span data-ttu-id="4ee60-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ee60-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ee60-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ee60-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ee60-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="4ee60-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ee60-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ee60-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ee60-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ee60-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ee60-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4ee60-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ee60-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4ee60-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ee60-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4ee60-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ee60-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4ee60-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ee60-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ee60-163">createdDateTime</span></span>|<span data-ttu-id="4ee60-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ee60-164">DateTimeOffset</span></span>|<span data-ttu-id="4ee60-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4ee60-165">DateTime the object was created.</span></span> <span data-ttu-id="4ee60-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-167">description</span><span class="sxs-lookup"><span data-stu-id="4ee60-167">description</span></span>|<span data-ttu-id="4ee60-168">String</span><span class="sxs-lookup"><span data-stu-id="4ee60-168">String</span></span>|<span data-ttu-id="4ee60-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4ee60-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ee60-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4ee60-171">displayName</span></span>|<span data-ttu-id="4ee60-172">String</span><span class="sxs-lookup"><span data-stu-id="4ee60-172">String</span></span>|<span data-ttu-id="4ee60-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4ee60-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ee60-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-175">version</span><span class="sxs-lookup"><span data-stu-id="4ee60-175">version</span></span>|<span data-ttu-id="4ee60-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-176">Int32</span></span>|<span data-ttu-id="4ee60-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4ee60-177">Version of the device configuration.</span></span> <span data-ttu-id="4ee60-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4ee60-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ee60-179">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4ee60-179">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4ee60-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-180">Boolean</span></span>|<span data-ttu-id="4ee60-181">このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="4ee60-181">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4ee60-182">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-182">This property is read-only.</span></span>|
|<span data-ttu-id="4ee60-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4ee60-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="4ee60-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-184">Boolean</span></span>|<span data-ttu-id="4ee60-185">コピー/貼り付けを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-185">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4ee60-186">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-186">bluetoothBlocked</span></span>|<span data-ttu-id="4ee60-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-187">Boolean</span></span>|<span data-ttu-id="4ee60-188">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-188">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4ee60-189">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-189">cameraBlocked</span></span>|<span data-ttu-id="4ee60-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-190">Boolean</span></span>|<span data-ttu-id="4ee60-191">カメラをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-191">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4ee60-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4ee60-192">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4ee60-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-193">Boolean</span></span>|<span data-ttu-id="4ee60-194">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-194">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4ee60-195">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-195">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4ee60-196">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4ee60-196">compliantAppsList</span></span>|<span data-ttu-id="4ee60-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4ee60-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4ee60-198">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="4ee60-198">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4ee60-199">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4ee60-199">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4ee60-200">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4ee60-200">compliantAppListType</span></span>|[<span data-ttu-id="4ee60-201">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="4ee60-201">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4ee60-202">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="4ee60-202">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4ee60-203">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-203">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4ee60-204">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4ee60-204">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4ee60-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-205">Boolean</span></span>|<span data-ttu-id="4ee60-206">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-206">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4ee60-207">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4ee60-207">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4ee60-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-208">Boolean</span></span>|<span data-ttu-id="4ee60-209">カスタム電子メール アカウントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-209">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4ee60-210">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-210">locationServicesBlocked</span></span>|<span data-ttu-id="4ee60-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-211">Boolean</span></span>|<span data-ttu-id="4ee60-212">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-212">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4ee60-213">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-213">microsoftAccountBlocked</span></span>|<span data-ttu-id="4ee60-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-214">Boolean</span></span>|<span data-ttu-id="4ee60-215">Microsoft アカウントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-215">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4ee60-216">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-216">nfcBlocked</span></span>|<span data-ttu-id="4ee60-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-217">Boolean</span></span>|<span data-ttu-id="4ee60-218">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-218">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4ee60-219">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4ee60-219">passwordBlockSimple</span></span>|<span data-ttu-id="4ee60-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-220">Boolean</span></span>|<span data-ttu-id="4ee60-221">カレンダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-221">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4ee60-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4ee60-222">passwordExpirationDays</span></span>|<span data-ttu-id="4ee60-223">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-223">Int32</span></span>|<span data-ttu-id="4ee60-224">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="4ee60-224">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4ee60-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4ee60-225">passwordMinimumLength</span></span>|<span data-ttu-id="4ee60-226">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-226">Int32</span></span>|<span data-ttu-id="4ee60-227">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="4ee60-227">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4ee60-228">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4ee60-228">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4ee60-229">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-229">Int32</span></span>|<span data-ttu-id="4ee60-230">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4ee60-230">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4ee60-231">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4ee60-231">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4ee60-232">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-232">Int32</span></span>|<span data-ttu-id="4ee60-233">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="4ee60-233">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4ee60-234">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4ee60-234">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4ee60-235">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-235">Int32</span></span>|<span data-ttu-id="4ee60-236">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="4ee60-236">Number of previous passwords to block.</span></span> <span data-ttu-id="4ee60-237">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="4ee60-237">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4ee60-238">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4ee60-238">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4ee60-239">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee60-239">Int32</span></span>|<span data-ttu-id="4ee60-240">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="4ee60-240">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4ee60-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4ee60-241">passwordRequiredType</span></span>|[<span data-ttu-id="4ee60-242">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4ee60-242">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4ee60-243">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4ee60-243">Password type that is required.</span></span> <span data-ttu-id="4ee60-244">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-244">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4ee60-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4ee60-245">passwordRequired</span></span>|<span data-ttu-id="4ee60-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-246">Boolean</span></span>|<span data-ttu-id="4ee60-247">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4ee60-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-248">screenCaptureBlocked</span></span>|<span data-ttu-id="4ee60-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-249">Boolean</span></span>|<span data-ttu-id="4ee60-250">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-250">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4ee60-251">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4ee60-251">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4ee60-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-252">Boolean</span></span>|<span data-ttu-id="4ee60-253">リムーバブル記憶域をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-253">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4ee60-254">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4ee60-254">storageRequireEncryption</span></span>|<span data-ttu-id="4ee60-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-255">Boolean</span></span>|<span data-ttu-id="4ee60-256">暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-256">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4ee60-257">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-257">webBrowserBlocked</span></span>|<span data-ttu-id="4ee60-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-258">Boolean</span></span>|<span data-ttu-id="4ee60-259">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-259">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4ee60-260">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-260">wifiBlocked</span></span>|<span data-ttu-id="4ee60-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-261">Boolean</span></span>|<span data-ttu-id="4ee60-262">Wi-Fi をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-262">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4ee60-263">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4ee60-263">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4ee60-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-264">Boolean</span></span>|<span data-ttu-id="4ee60-265">Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-265">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4ee60-266">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-266">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4ee60-267">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4ee60-267">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4ee60-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-268">Boolean</span></span>|<span data-ttu-id="4ee60-269">Wi-Fi ホットスポット レポートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-269">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4ee60-270">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4ee60-270">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4ee60-271">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4ee60-271">windowsStoreBlocked</span></span>|<span data-ttu-id="4ee60-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee60-272">Boolean</span></span>|<span data-ttu-id="4ee60-273">Windows ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-273">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4ee60-274">応答</span><span class="sxs-lookup"><span data-stu-id="4ee60-274">Response</span></span>
<span data-ttu-id="4ee60-275">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ee60-275">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ee60-276">例</span><span class="sxs-lookup"><span data-stu-id="4ee60-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ee60-277">要求</span><span class="sxs-lookup"><span data-stu-id="4ee60-277">Request</span></span>
<span data-ttu-id="4ee60-278">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ee60-278">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2326

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="4ee60-279">応答</span><span class="sxs-lookup"><span data-stu-id="4ee60-279">Response</span></span>
<span data-ttu-id="4ee60-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ee60-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2498

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





