---
title: Update iosDeviceFeaturesConfiguration
description: iosDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78f8a620d57e9d16f61fe9884c1cfd5486f39343
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339429"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="78011-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="78011-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="78011-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78011-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78011-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78011-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78011-106">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78011-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78011-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="78011-107">Prerequisites</span></span>
<span data-ttu-id="78011-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78011-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78011-110">Permission type</span></span>|<span data-ttu-id="78011-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78011-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78011-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78011-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78011-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78011-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78011-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78011-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78011-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78011-115">Not supported.</span></span>|
|<span data-ttu-id="78011-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78011-116">Application</span></span>|<span data-ttu-id="78011-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78011-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78011-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78011-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="78011-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78011-119">Request headers</span></span>
|<span data-ttu-id="78011-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78011-120">Header</span></span>|<span data-ttu-id="78011-121">値</span><span class="sxs-lookup"><span data-stu-id="78011-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78011-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78011-122">Authorization</span></span>|<span data-ttu-id="78011-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="78011-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78011-124">承諾</span><span class="sxs-lookup"><span data-stu-id="78011-124">Accept</span></span>|<span data-ttu-id="78011-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78011-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78011-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="78011-126">Request body</span></span>
<span data-ttu-id="78011-127">要求本文で、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78011-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="78011-128">次の表に、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78011-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="78011-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78011-129">Property</span></span>|<span data-ttu-id="78011-130">型</span><span class="sxs-lookup"><span data-stu-id="78011-130">Type</span></span>|<span data-ttu-id="78011-131">説明</span><span class="sxs-lookup"><span data-stu-id="78011-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78011-132">id</span><span class="sxs-lookup"><span data-stu-id="78011-132">id</span></span>|<span data-ttu-id="78011-133">文字列</span><span class="sxs-lookup"><span data-stu-id="78011-133">String</span></span>|<span data-ttu-id="78011-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78011-134">Key of the entity.</span></span> <span data-ttu-id="78011-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78011-136">lastModifiedDateTime</span></span>|<span data-ttu-id="78011-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78011-137">DateTimeOffset</span></span>|<span data-ttu-id="78011-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="78011-138">DateTime the object was last modified.</span></span> <span data-ttu-id="78011-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78011-140">roleScopeTagIds</span></span>|<span data-ttu-id="78011-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="78011-141">String collection</span></span>|<span data-ttu-id="78011-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="78011-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="78011-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="78011-144">supportsScopeTags</span></span>|<span data-ttu-id="78011-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="78011-145">Boolean</span></span>|<span data-ttu-id="78011-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78011-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="78011-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="78011-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="78011-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="78011-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="78011-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="78011-149">This property is read-only.</span></span> <span data-ttu-id="78011-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="78011-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="78011-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="78011-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="78011-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="78011-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="78011-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="78011-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="78011-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="78011-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="78011-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="78011-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="78011-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="78011-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="78011-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="78011-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="78011-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="78011-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="78011-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78011-163">createdDateTime</span></span>|<span data-ttu-id="78011-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78011-164">DateTimeOffset</span></span>|<span data-ttu-id="78011-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="78011-165">DateTime the object was created.</span></span> <span data-ttu-id="78011-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-167">description</span><span class="sxs-lookup"><span data-stu-id="78011-167">description</span></span>|<span data-ttu-id="78011-168">String</span><span class="sxs-lookup"><span data-stu-id="78011-168">String</span></span>|<span data-ttu-id="78011-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="78011-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="78011-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-171">displayName</span><span class="sxs-lookup"><span data-stu-id="78011-171">displayName</span></span>|<span data-ttu-id="78011-172">String</span><span class="sxs-lookup"><span data-stu-id="78011-172">String</span></span>|<span data-ttu-id="78011-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="78011-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="78011-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-175">version</span><span class="sxs-lookup"><span data-stu-id="78011-175">version</span></span>|<span data-ttu-id="78011-176">Int32</span><span class="sxs-lookup"><span data-stu-id="78011-176">Int32</span></span>|<span data-ttu-id="78011-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="78011-177">Version of the device configuration.</span></span> <span data-ttu-id="78011-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78011-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78011-179">放映した Print行先</span><span class="sxs-lookup"><span data-stu-id="78011-179">airPrintDestinations</span></span>|<span data-ttu-id="78011-180">[放映 Printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78011-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="78011-181">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="78011-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="78011-182">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="78011-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="78011-183">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78011-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="78011-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="78011-184">assetTagTemplate</span></span>|<span data-ttu-id="78011-185">String</span><span class="sxs-lookup"><span data-stu-id="78011-185">String</span></span>|<span data-ttu-id="78011-186">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="78011-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="78011-187">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="78011-187">contentFilterSettings</span></span>|[<span data-ttu-id="78011-188">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="78011-188">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="78011-189">IOS Web コンテンツフィルターの設定、監視モードのみを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="78011-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="78011-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="78011-190">lockScreenFootnote</span></span>|<span data-ttu-id="78011-191">String</span><span class="sxs-lookup"><span data-stu-id="78011-191">String</span></span>|<span data-ttu-id="78011-192">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="78011-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="78011-193">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="78011-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="78011-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="78011-194">homeScreenDockIcons</span></span>|<span data-ttu-id="78011-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78011-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="78011-196">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="78011-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="78011-197">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="78011-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="78011-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="78011-198">homeScreenPages</span></span>|<span data-ttu-id="78011-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78011-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="78011-200">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="78011-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="78011-201">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="78011-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="78011-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="78011-202">notificationSettings</span></span>|<span data-ttu-id="78011-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78011-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="78011-204">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="78011-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="78011-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="78011-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="78011-206">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="78011-206">singleSignOnSettings</span></span>|[<span data-ttu-id="78011-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="78011-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="78011-208">受信デバイス上のアプリをスムーズに認証できるようにする Kerberos ログイン設定。</span><span class="sxs-lookup"><span data-stu-id="78011-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="78011-209">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="78011-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="78011-210">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="78011-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="78011-211">壁紙の表示場所の指定子。</span><span class="sxs-lookup"><span data-stu-id="78011-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="78011-212">使用可能な値は、`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens` です。</span><span class="sxs-lookup"><span data-stu-id="78011-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="78011-213">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="78011-213">wallpaperImage</span></span>|[<span data-ttu-id="78011-214">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78011-214">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="78011-215">壁紙の画像は、PNG または JPEG 形式のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="78011-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="78011-216">IOS 8 以降のバージョンの監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="78011-216">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="78011-217">応答</span><span class="sxs-lookup"><span data-stu-id="78011-217">Response</span></span>
<span data-ttu-id="78011-218">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="78011-218">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78011-219">例</span><span class="sxs-lookup"><span data-stu-id="78011-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="78011-220">要求</span><span class="sxs-lookup"><span data-stu-id="78011-220">Request</span></span>
<span data-ttu-id="78011-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78011-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4429

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="78011-222">応答</span><span class="sxs-lookup"><span data-stu-id="78011-222">Response</span></span>
<span data-ttu-id="78011-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78011-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```






