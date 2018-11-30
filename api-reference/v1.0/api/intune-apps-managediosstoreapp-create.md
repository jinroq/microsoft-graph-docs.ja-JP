---
title: managedIOSStoreApp の作成
description: 新しい managedIOSStoreApp オブジェクトを作成します。
ms.openlocfilehash: 7cdbcf6e3690a16fe0a6754d89bdb0ebd45e3cdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023902"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="bbdee-103">managedIOSStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="bbdee-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="bbdee-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bbdee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbdee-105">新しい [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bbdee-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbdee-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bbdee-106">Prerequisites</span></span>
<span data-ttu-id="bbdee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbdee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbdee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbdee-109">Permission type</span></span>|<span data-ttu-id="bbdee-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbdee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbdee-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbdee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bbdee-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdee-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbdee-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbdee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbdee-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbdee-114">Not supported.</span></span>|
|<span data-ttu-id="bbdee-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbdee-115">Application</span></span>|<span data-ttu-id="bbdee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbdee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbdee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbdee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bbdee-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbdee-118">Request headers</span></span>
|<span data-ttu-id="bbdee-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbdee-119">Header</span></span>|<span data-ttu-id="bbdee-120">値</span><span class="sxs-lookup"><span data-stu-id="bbdee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbdee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbdee-121">Authorization</span></span>|<span data-ttu-id="bbdee-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bbdee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbdee-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bbdee-123">Accept</span></span>|<span data-ttu-id="bbdee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bbdee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbdee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbdee-125">Request body</span></span>
<span data-ttu-id="bbdee-126">要求本文で、managedIOSStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bbdee-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="bbdee-127">次の表に、managedIOSStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bbdee-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="bbdee-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbdee-128">Property</span></span>|<span data-ttu-id="bbdee-129">型</span><span class="sxs-lookup"><span data-stu-id="bbdee-129">Type</span></span>|<span data-ttu-id="bbdee-130">説明</span><span class="sxs-lookup"><span data-stu-id="bbdee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbdee-131">id</span><span class="sxs-lookup"><span data-stu-id="bbdee-131">id</span></span>|<span data-ttu-id="bbdee-132">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-132">String</span></span>|<span data-ttu-id="bbdee-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bbdee-133">Key of the entity.</span></span> <span data-ttu-id="bbdee-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bbdee-135">displayName</span></span>|<span data-ttu-id="bbdee-136">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-136">String</span></span>|<span data-ttu-id="bbdee-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="bbdee-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bbdee-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-139">説明</span><span class="sxs-lookup"><span data-stu-id="bbdee-139">description</span></span>|<span data-ttu-id="bbdee-140">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-140">String</span></span>|<span data-ttu-id="bbdee-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="bbdee-141">The description of the app.</span></span> <span data-ttu-id="bbdee-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bbdee-143">publisher</span></span>|<span data-ttu-id="bbdee-144">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-144">String</span></span>|<span data-ttu-id="bbdee-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="bbdee-145">The publisher of the app.</span></span> <span data-ttu-id="bbdee-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bbdee-147">largeIcon</span></span>|[<span data-ttu-id="bbdee-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bbdee-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bbdee-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="bbdee-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bbdee-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbdee-151">createdDateTime</span></span>|<span data-ttu-id="bbdee-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbdee-152">DateTimeOffset</span></span>|<span data-ttu-id="bbdee-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="bbdee-153">The date and time the app was created.</span></span> <span data-ttu-id="bbdee-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbdee-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bbdee-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbdee-156">DateTimeOffset</span></span>|<span data-ttu-id="bbdee-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="bbdee-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bbdee-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bbdee-159">isFeatured</span></span>|<span data-ttu-id="bbdee-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbdee-160">Boolean</span></span>|<span data-ttu-id="bbdee-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bbdee-162">privacyInformationUrl</span></span>|<span data-ttu-id="bbdee-163">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-163">String</span></span>|<span data-ttu-id="bbdee-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="bbdee-164">The privacy statement Url.</span></span> <span data-ttu-id="bbdee-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bbdee-166">informationUrl</span></span>|<span data-ttu-id="bbdee-167">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-167">String</span></span>|<span data-ttu-id="bbdee-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="bbdee-168">The more information Url.</span></span> <span data-ttu-id="bbdee-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-170">owner</span><span class="sxs-lookup"><span data-stu-id="bbdee-170">owner</span></span>|<span data-ttu-id="bbdee-171">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-171">String</span></span>|<span data-ttu-id="bbdee-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="bbdee-172">The owner of the app.</span></span> <span data-ttu-id="bbdee-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-174">developer</span><span class="sxs-lookup"><span data-stu-id="bbdee-174">developer</span></span>|<span data-ttu-id="bbdee-175">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-175">String</span></span>|<span data-ttu-id="bbdee-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="bbdee-176">The developer of the app.</span></span> <span data-ttu-id="bbdee-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-178">notes</span><span class="sxs-lookup"><span data-stu-id="bbdee-178">notes</span></span>|<span data-ttu-id="bbdee-179">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-179">String</span></span>|<span data-ttu-id="bbdee-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="bbdee-180">Notes for the app.</span></span> <span data-ttu-id="bbdee-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bbdee-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bbdee-182">publishingState</span></span>|[<span data-ttu-id="bbdee-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bbdee-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bbdee-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="bbdee-184">The publishing state for the app.</span></span> <span data-ttu-id="bbdee-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="bbdee-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bbdee-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="bbdee-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bbdee-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="bbdee-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bbdee-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bbdee-188">appAvailability</span></span>|[<span data-ttu-id="bbdee-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bbdee-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bbdee-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="bbdee-190">The Application's availability.</span></span> <span data-ttu-id="bbdee-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="bbdee-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bbdee-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="bbdee-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bbdee-193">version</span><span class="sxs-lookup"><span data-stu-id="bbdee-193">version</span></span>|<span data-ttu-id="bbdee-194">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-194">String</span></span>|<span data-ttu-id="bbdee-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="bbdee-195">The Application's version.</span></span> <span data-ttu-id="bbdee-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bbdee-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bbdee-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="bbdee-197">bundleId</span></span>|<span data-ttu-id="bbdee-198">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-198">String</span></span>|<span data-ttu-id="bbdee-199">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="bbdee-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="bbdee-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bbdee-200">appStoreUrl</span></span>|<span data-ttu-id="bbdee-201">String</span><span class="sxs-lookup"><span data-stu-id="bbdee-201">String</span></span>|<span data-ttu-id="bbdee-202">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="bbdee-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="bbdee-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bbdee-203">applicableDeviceType</span></span>|[<span data-ttu-id="bbdee-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bbdee-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="bbdee-205">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="bbdee-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bbdee-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bbdee-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bbdee-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bbdee-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="bbdee-208">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="bbdee-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="bbdee-209">応答</span><span class="sxs-lookup"><span data-stu-id="bbdee-209">Response</span></span>
<span data-ttu-id="bbdee-210">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bbdee-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbdee-211">例</span><span class="sxs-lookup"><span data-stu-id="bbdee-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbdee-212">要求</span><span class="sxs-lookup"><span data-stu-id="bbdee-212">Request</span></span>
<span data-ttu-id="bbdee-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bbdee-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="bbdee-214">応答</span><span class="sxs-lookup"><span data-stu-id="bbdee-214">Response</span></span>
<span data-ttu-id="bbdee-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bbdee-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```


