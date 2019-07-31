---
title: iosDeviceFeaturesConfiguration の作成
description: 新しい iosDeviceFeaturesConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75244e069208c343fce10fc5d6d7a3617e2940f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948580"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="92d30-103">iosDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="92d30-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="92d30-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92d30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92d30-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92d30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92d30-106">新しい [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="92d30-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92d30-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="92d30-107">Prerequisites</span></span>
<span data-ttu-id="92d30-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d30-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92d30-110">Permission type</span></span>|<span data-ttu-id="92d30-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92d30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92d30-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92d30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92d30-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d30-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92d30-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92d30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92d30-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92d30-115">Not supported.</span></span>|
|<span data-ttu-id="92d30-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92d30-116">Application</span></span>|<span data-ttu-id="92d30-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92d30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92d30-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92d30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92d30-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92d30-119">Request headers</span></span>
|<span data-ttu-id="92d30-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92d30-120">Header</span></span>|<span data-ttu-id="92d30-121">値</span><span class="sxs-lookup"><span data-stu-id="92d30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92d30-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92d30-122">Authorization</span></span>|<span data-ttu-id="92d30-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="92d30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92d30-124">承諾</span><span class="sxs-lookup"><span data-stu-id="92d30-124">Accept</span></span>|<span data-ttu-id="92d30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92d30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92d30-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="92d30-126">Request body</span></span>
<span data-ttu-id="92d30-127">要求本文で、iosDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92d30-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="92d30-128">次の表に、iosDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="92d30-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="92d30-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92d30-129">Property</span></span>|<span data-ttu-id="92d30-130">型</span><span class="sxs-lookup"><span data-stu-id="92d30-130">Type</span></span>|<span data-ttu-id="92d30-131">説明</span><span class="sxs-lookup"><span data-stu-id="92d30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d30-132">id</span><span class="sxs-lookup"><span data-stu-id="92d30-132">id</span></span>|<span data-ttu-id="92d30-133">文字列</span><span class="sxs-lookup"><span data-stu-id="92d30-133">String</span></span>|<span data-ttu-id="92d30-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="92d30-134">Key of the entity.</span></span> <span data-ttu-id="92d30-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92d30-136">lastModifiedDateTime</span></span>|<span data-ttu-id="92d30-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d30-137">DateTimeOffset</span></span>|<span data-ttu-id="92d30-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="92d30-138">DateTime the object was last modified.</span></span> <span data-ttu-id="92d30-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92d30-140">roleScopeTagIds</span></span>|<span data-ttu-id="92d30-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="92d30-141">String collection</span></span>|<span data-ttu-id="92d30-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="92d30-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92d30-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92d30-144">supportsScopeTags</span></span>|<span data-ttu-id="92d30-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="92d30-145">Boolean</span></span>|<span data-ttu-id="92d30-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="92d30-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92d30-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="92d30-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92d30-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="92d30-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92d30-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="92d30-149">This property is read-only.</span></span> <span data-ttu-id="92d30-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92d30-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92d30-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92d30-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92d30-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="92d30-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92d30-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92d30-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92d30-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92d30-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92d30-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="92d30-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92d30-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="92d30-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92d30-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="92d30-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92d30-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="92d30-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92d30-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92d30-163">createdDateTime</span></span>|<span data-ttu-id="92d30-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d30-164">DateTimeOffset</span></span>|<span data-ttu-id="92d30-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="92d30-165">DateTime the object was created.</span></span> <span data-ttu-id="92d30-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-167">description</span><span class="sxs-lookup"><span data-stu-id="92d30-167">description</span></span>|<span data-ttu-id="92d30-168">String</span><span class="sxs-lookup"><span data-stu-id="92d30-168">String</span></span>|<span data-ttu-id="92d30-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="92d30-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92d30-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-171">displayName</span><span class="sxs-lookup"><span data-stu-id="92d30-171">displayName</span></span>|<span data-ttu-id="92d30-172">String</span><span class="sxs-lookup"><span data-stu-id="92d30-172">String</span></span>|<span data-ttu-id="92d30-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="92d30-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92d30-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-175">version</span><span class="sxs-lookup"><span data-stu-id="92d30-175">version</span></span>|<span data-ttu-id="92d30-176">Int32</span><span class="sxs-lookup"><span data-stu-id="92d30-176">Int32</span></span>|<span data-ttu-id="92d30-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="92d30-177">Version of the device configuration.</span></span> <span data-ttu-id="92d30-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92d30-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92d30-179">放映した Print行先</span><span class="sxs-lookup"><span data-stu-id="92d30-179">airPrintDestinations</span></span>|<span data-ttu-id="92d30-180">[放映 Printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92d30-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="92d30-181">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="92d30-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="92d30-182">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="92d30-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="92d30-183">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="92d30-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="92d30-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="92d30-184">assetTagTemplate</span></span>|<span data-ttu-id="92d30-185">String</span><span class="sxs-lookup"><span data-stu-id="92d30-185">String</span></span>|<span data-ttu-id="92d30-186">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="92d30-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="92d30-187">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="92d30-187">contentFilterSettings</span></span>|[<span data-ttu-id="92d30-188">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="92d30-188">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="92d30-189">IOS Web コンテンツフィルターの設定、監視モードのみを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="92d30-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="92d30-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="92d30-190">lockScreenFootnote</span></span>|<span data-ttu-id="92d30-191">String</span><span class="sxs-lookup"><span data-stu-id="92d30-191">String</span></span>|<span data-ttu-id="92d30-192">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="92d30-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="92d30-193">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="92d30-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="92d30-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="92d30-194">homeScreenDockIcons</span></span>|<span data-ttu-id="92d30-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92d30-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="92d30-196">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="92d30-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="92d30-197">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="92d30-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="92d30-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="92d30-198">homeScreenPages</span></span>|<span data-ttu-id="92d30-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92d30-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="92d30-200">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="92d30-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="92d30-201">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="92d30-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="92d30-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="92d30-202">notificationSettings</span></span>|<span data-ttu-id="92d30-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92d30-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="92d30-204">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="92d30-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="92d30-205">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="92d30-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="92d30-206">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="92d30-206">singleSignOnSettings</span></span>|[<span data-ttu-id="92d30-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="92d30-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="92d30-208">受信デバイス上のアプリをスムーズに認証できるようにする Kerberos ログイン設定。</span><span class="sxs-lookup"><span data-stu-id="92d30-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="92d30-209">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="92d30-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="92d30-210">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="92d30-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="92d30-211">壁紙の表示場所の指定子。</span><span class="sxs-lookup"><span data-stu-id="92d30-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="92d30-212">使用可能な値は、`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens` です。</span><span class="sxs-lookup"><span data-stu-id="92d30-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="92d30-213">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="92d30-213">wallpaperImage</span></span>|[<span data-ttu-id="92d30-214">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92d30-214">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="92d30-215">壁紙の画像は、PNG または JPEG 形式のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="92d30-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="92d30-216">IOS 8 以降のバージョンの監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="92d30-216">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="92d30-217">応答</span><span class="sxs-lookup"><span data-stu-id="92d30-217">Response</span></span>
<span data-ttu-id="92d30-218">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="92d30-218">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d30-219">例</span><span class="sxs-lookup"><span data-stu-id="92d30-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="92d30-220">要求</span><span class="sxs-lookup"><span data-stu-id="92d30-220">Request</span></span>
<span data-ttu-id="92d30-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92d30-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="92d30-222">応答</span><span class="sxs-lookup"><span data-stu-id="92d30-222">Response</span></span>
<span data-ttu-id="92d30-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92d30-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





