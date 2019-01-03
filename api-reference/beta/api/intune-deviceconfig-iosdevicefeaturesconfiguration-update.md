---
title: Update iosDeviceFeaturesConfiguration
description: iosDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: f76aebf3d88083c88318befd32c2654630fdecba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347720"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="39327-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="39327-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="39327-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39327-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39327-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39327-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39327-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39327-107">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="39327-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39327-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="39327-108">Prerequisites</span></span>
<span data-ttu-id="39327-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39327-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39327-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="39327-111">Permission type</span></span>|<span data-ttu-id="39327-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="39327-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39327-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="39327-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39327-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39327-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39327-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="39327-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39327-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39327-116">Not supported.</span></span>|
|<span data-ttu-id="39327-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="39327-117">Application</span></span>|<span data-ttu-id="39327-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39327-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39327-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="39327-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="39327-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39327-120">Request headers</span></span>
|<span data-ttu-id="39327-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39327-121">Header</span></span>|<span data-ttu-id="39327-122">値</span><span class="sxs-lookup"><span data-stu-id="39327-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39327-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39327-123">Authorization</span></span>|<span data-ttu-id="39327-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="39327-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39327-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39327-125">Accept</span></span>|<span data-ttu-id="39327-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39327-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39327-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="39327-127">Request body</span></span>
<span data-ttu-id="39327-128">要求本文で、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="39327-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="39327-129">次の表に、[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="39327-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="39327-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39327-130">Property</span></span>|<span data-ttu-id="39327-131">種類</span><span class="sxs-lookup"><span data-stu-id="39327-131">Type</span></span>|<span data-ttu-id="39327-132">説明</span><span class="sxs-lookup"><span data-stu-id="39327-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39327-133">ID</span><span class="sxs-lookup"><span data-stu-id="39327-133">id</span></span>|<span data-ttu-id="39327-134">String</span><span class="sxs-lookup"><span data-stu-id="39327-134">String</span></span>|<span data-ttu-id="39327-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="39327-135">Key of the entity.</span></span> <span data-ttu-id="39327-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39327-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39327-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39327-138">DateTimeOffset</span></span>|<span data-ttu-id="39327-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="39327-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39327-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39327-141">roleScopeTagIds</span></span>|<span data-ttu-id="39327-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="39327-142">String collection</span></span>|<span data-ttu-id="39327-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="39327-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39327-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39327-145">supportsScopeTags</span></span>|<span data-ttu-id="39327-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="39327-146">Boolean</span></span>|<span data-ttu-id="39327-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="39327-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39327-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="39327-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39327-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="39327-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39327-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="39327-150">This property is read-only.</span></span> <span data-ttu-id="39327-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39327-152">createdDateTime</span></span>|<span data-ttu-id="39327-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39327-153">DateTimeOffset</span></span>|<span data-ttu-id="39327-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="39327-154">DateTime the object was created.</span></span> <span data-ttu-id="39327-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-156">説明</span><span class="sxs-lookup"><span data-stu-id="39327-156">description</span></span>|<span data-ttu-id="39327-157">String</span><span class="sxs-lookup"><span data-stu-id="39327-157">String</span></span>|<span data-ttu-id="39327-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="39327-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39327-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-160">displayName</span><span class="sxs-lookup"><span data-stu-id="39327-160">displayName</span></span>|<span data-ttu-id="39327-161">String</span><span class="sxs-lookup"><span data-stu-id="39327-161">String</span></span>|<span data-ttu-id="39327-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="39327-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39327-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-164">version</span><span class="sxs-lookup"><span data-stu-id="39327-164">version</span></span>|<span data-ttu-id="39327-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39327-165">Int32</span></span>|<span data-ttu-id="39327-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="39327-166">Version of the device configuration.</span></span> <span data-ttu-id="39327-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="39327-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39327-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="39327-168">airPrintDestinations</span></span>|<span data-ttu-id="39327-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="39327-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="39327-170">常に表示されている必要があります AirPrint プリンターの配列。</span><span class="sxs-lookup"><span data-stu-id="39327-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="39327-171">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39327-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="39327-172">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="39327-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="39327-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="39327-173">assetTagTemplate</span></span>|<span data-ttu-id="39327-174">String</span><span class="sxs-lookup"><span data-stu-id="39327-174">String</span></span>|<span data-ttu-id="39327-175">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="39327-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="39327-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="39327-176">contentFilterSettings</span></span>|[<span data-ttu-id="39327-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="39327-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="39327-178">Web コンテンツ フィルター設定、コールを管理モードでのみを設定するには、iOS を取得または</span><span class="sxs-lookup"><span data-stu-id="39327-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="39327-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="39327-179">lockScreenFootnote</span></span>|<span data-ttu-id="39327-180">String</span><span class="sxs-lookup"><span data-stu-id="39327-180">String</span></span>|<span data-ttu-id="39327-181">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="39327-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="39327-182">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="39327-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="39327-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="39327-183">homeScreenDockIcons</span></span>|<span data-ttu-id="39327-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39327-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="39327-185">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="39327-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="39327-186">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39327-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39327-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="39327-187">homeScreenPages</span></span>|<span data-ttu-id="39327-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39327-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="39327-189">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="39327-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="39327-190">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39327-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39327-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="39327-191">notificationSettings</span></span>|<span data-ttu-id="39327-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39327-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="39327-193">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="39327-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="39327-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39327-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39327-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="39327-195">singleSignOnSettings</span></span>|[<span data-ttu-id="39327-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="39327-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="39327-197">受信認証をスムーズにするためにデバイス上のアプリを有効にする Kerberos ログインの設定です。</span><span class="sxs-lookup"><span data-stu-id="39327-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="39327-198">応答</span><span class="sxs-lookup"><span data-stu-id="39327-198">Response</span></span>
<span data-ttu-id="39327-199">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="39327-199">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39327-200">例</span><span class="sxs-lookup"><span data-stu-id="39327-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="39327-201">要求</span><span class="sxs-lookup"><span data-stu-id="39327-201">Request</span></span>
<span data-ttu-id="39327-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="39327-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3474

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="39327-203">応答</span><span class="sxs-lookup"><span data-stu-id="39327-203">Response</span></span>
<span data-ttu-id="39327-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="39327-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3651

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
  }
}
```




