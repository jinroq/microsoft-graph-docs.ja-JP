---
title: Update iosDeviceFeaturesConfiguration
description: iosDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34d95e925ebc1e60bb05b183744ae97e8a23f141
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923645"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="a4fc4-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4fc4-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a4fc4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4fc4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4fc4-106">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4fc4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4fc4-107">Prerequisites</span></span>
<span data-ttu-id="a4fc4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4fc4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4fc4-110">Permission type</span></span>|<span data-ttu-id="a4fc4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4fc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4fc4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4fc4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4fc4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4fc4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4fc4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-115">Not supported.</span></span>|
|<span data-ttu-id="a4fc4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4fc4-116">Application</span></span>|<span data-ttu-id="a4fc4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4fc4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4fc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a4fc4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fc4-119">Request headers</span></span>
|<span data-ttu-id="a4fc4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fc4-120">Header</span></span>|<span data-ttu-id="a4fc4-121">値</span><span class="sxs-lookup"><span data-stu-id="a4fc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4fc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4fc4-122">Authorization</span></span>|<span data-ttu-id="a4fc4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4fc4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a4fc4-124">Accept</span></span>|<span data-ttu-id="a4fc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4fc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4fc4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4fc4-126">Request body</span></span>
<span data-ttu-id="a4fc4-127">要求本文で、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="a4fc4-128">次の表に、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="a4fc4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4fc4-129">Property</span></span>|<span data-ttu-id="a4fc4-130">型</span><span class="sxs-lookup"><span data-stu-id="a4fc4-130">Type</span></span>|<span data-ttu-id="a4fc4-131">説明</span><span class="sxs-lookup"><span data-stu-id="a4fc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4fc4-132">id</span><span class="sxs-lookup"><span data-stu-id="a4fc4-132">id</span></span>|<span data-ttu-id="a4fc4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a4fc4-133">String</span></span>|<span data-ttu-id="a4fc4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-134">Key of the entity.</span></span> <span data-ttu-id="a4fc4-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4fc4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a4fc4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4fc4-137">DateTimeOffset</span></span>|<span data-ttu-id="a4fc4-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a4fc4-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4fc4-140">roleScopeTagIds</span></span>|<span data-ttu-id="a4fc4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a4fc4-141">String collection</span></span>|<span data-ttu-id="a4fc4-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4fc4-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a4fc4-144">supportsScopeTags</span></span>|<span data-ttu-id="a4fc4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4fc4-145">Boolean</span></span>|<span data-ttu-id="a4fc4-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a4fc4-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a4fc4-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a4fc4-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-149">This property is read-only.</span></span> <span data-ttu-id="a4fc4-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4fc4-151">createdDateTime</span></span>|<span data-ttu-id="a4fc4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4fc4-152">DateTimeOffset</span></span>|<span data-ttu-id="a4fc4-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-153">DateTime the object was created.</span></span> <span data-ttu-id="a4fc4-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-155">description</span><span class="sxs-lookup"><span data-stu-id="a4fc4-155">description</span></span>|<span data-ttu-id="a4fc4-156">String</span><span class="sxs-lookup"><span data-stu-id="a4fc4-156">String</span></span>|<span data-ttu-id="a4fc4-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4fc4-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a4fc4-159">displayName</span></span>|<span data-ttu-id="a4fc4-160">String</span><span class="sxs-lookup"><span data-stu-id="a4fc4-160">String</span></span>|<span data-ttu-id="a4fc4-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4fc4-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-163">version</span><span class="sxs-lookup"><span data-stu-id="a4fc4-163">version</span></span>|<span data-ttu-id="a4fc4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fc4-164">Int32</span></span>|<span data-ttu-id="a4fc4-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-165">Version of the device configuration.</span></span> <span data-ttu-id="a4fc4-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4fc4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4fc4-167">放映した Print行先</span><span class="sxs-lookup"><span data-stu-id="a4fc4-167">airPrintDestinations</span></span>|<span data-ttu-id="a4fc4-168">[放映 Printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4fc4-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="a4fc4-169">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="a4fc4-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a4fc4-171">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="a4fc4-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="a4fc4-172">assetTagTemplate</span></span>|<span data-ttu-id="a4fc4-173">String</span><span class="sxs-lookup"><span data-stu-id="a4fc4-173">String</span></span>|<span data-ttu-id="a4fc4-174">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="a4fc4-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="a4fc4-175">contentFilterSettings</span></span>|[<span data-ttu-id="a4fc4-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="a4fc4-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="a4fc4-177">IOS Web コンテンツフィルターの設定、監視モードのみを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="a4fc4-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="a4fc4-178">lockScreenFootnote</span></span>|<span data-ttu-id="a4fc4-179">String</span><span class="sxs-lookup"><span data-stu-id="a4fc4-179">String</span></span>|<span data-ttu-id="a4fc4-180">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="a4fc4-181">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="a4fc4-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="a4fc4-182">homeScreenDockIcons</span></span>|<span data-ttu-id="a4fc4-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4fc4-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a4fc4-184">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="a4fc4-185">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4fc4-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="a4fc4-186">homeScreenPages</span></span>|<span data-ttu-id="a4fc4-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4fc4-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="a4fc4-188">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="a4fc4-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4fc4-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="a4fc4-190">notificationSettings</span></span>|<span data-ttu-id="a4fc4-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4fc4-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="a4fc4-192">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="a4fc4-193">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a4fc4-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a4fc4-194">singleSignOnSettings</span></span>|[<span data-ttu-id="a4fc4-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a4fc4-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="a4fc4-196">受信デバイス上のアプリをスムーズに認証できるようにする Kerberos ログイン設定。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="a4fc4-197">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="a4fc4-197">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="a4fc4-198">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="a4fc4-198">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="a4fc4-199">壁紙の表示場所の指定子。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-199">A wallpaper display location specifier.</span></span> <span data-ttu-id="a4fc4-200">使用可能な値は、`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens` です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-200">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="a4fc4-201">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="a4fc4-201">wallpaperImage</span></span>|[<span data-ttu-id="a4fc4-202">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4fc4-202">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4fc4-203">壁紙の画像は、PNG または JPEG 形式のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-203">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="a4fc4-204">IOS 8 以降のバージョンの監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-204">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="a4fc4-205">応答</span><span class="sxs-lookup"><span data-stu-id="a4fc4-205">Response</span></span>
<span data-ttu-id="a4fc4-206">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-206">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4fc4-207">例</span><span class="sxs-lookup"><span data-stu-id="a4fc4-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4fc4-208">要求</span><span class="sxs-lookup"><span data-stu-id="a4fc4-208">Request</span></span>
<span data-ttu-id="a4fc4-209">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3656

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="a4fc4-210">応答</span><span class="sxs-lookup"><span data-stu-id="a4fc4-210">Response</span></span>
<span data-ttu-id="a4fc4-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4fc4-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3828

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




