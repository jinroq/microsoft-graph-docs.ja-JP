---
title: managedIOSStoreApp の更新
description: managedIOSStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75ee18a47c693c9099ccd18fb0b5434353c85397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923370"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="d8031-103">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="d8031-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="d8031-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8031-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8031-105">[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d8031-105">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8031-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8031-106">Prerequisites</span></span>
<span data-ttu-id="d8031-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8031-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8031-109">Permission type</span></span>|<span data-ttu-id="d8031-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8031-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8031-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8031-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8031-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8031-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8031-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8031-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8031-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8031-114">Not supported.</span></span>|
|<span data-ttu-id="d8031-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8031-115">Application</span></span>|<span data-ttu-id="d8031-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8031-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8031-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8031-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d8031-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8031-118">Request headers</span></span>
|<span data-ttu-id="d8031-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8031-119">Header</span></span>|<span data-ttu-id="d8031-120">値</span><span class="sxs-lookup"><span data-stu-id="d8031-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8031-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8031-121">Authorization</span></span>|<span data-ttu-id="d8031-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d8031-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8031-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d8031-123">Accept</span></span>|<span data-ttu-id="d8031-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8031-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8031-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8031-125">Request body</span></span>
<span data-ttu-id="d8031-126">要求本文で、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8031-126">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="d8031-127">次の表に、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8031-127">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="d8031-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8031-128">Property</span></span>|<span data-ttu-id="d8031-129">型</span><span class="sxs-lookup"><span data-stu-id="d8031-129">Type</span></span>|<span data-ttu-id="d8031-130">説明</span><span class="sxs-lookup"><span data-stu-id="d8031-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8031-131">id</span><span class="sxs-lookup"><span data-stu-id="d8031-131">id</span></span>|<span data-ttu-id="d8031-132">String</span><span class="sxs-lookup"><span data-stu-id="d8031-132">String</span></span>|<span data-ttu-id="d8031-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d8031-133">Key of the entity.</span></span> <span data-ttu-id="d8031-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d8031-135">displayName</span></span>|<span data-ttu-id="d8031-136">String</span><span class="sxs-lookup"><span data-stu-id="d8031-136">String</span></span>|<span data-ttu-id="d8031-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d8031-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d8031-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-139">説明</span><span class="sxs-lookup"><span data-stu-id="d8031-139">description</span></span>|<span data-ttu-id="d8031-140">String</span><span class="sxs-lookup"><span data-stu-id="d8031-140">String</span></span>|<span data-ttu-id="d8031-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d8031-141">The description of the app.</span></span> <span data-ttu-id="d8031-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d8031-143">publisher</span></span>|<span data-ttu-id="d8031-144">String</span><span class="sxs-lookup"><span data-stu-id="d8031-144">String</span></span>|<span data-ttu-id="d8031-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d8031-145">The publisher of the app.</span></span> <span data-ttu-id="d8031-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d8031-147">largeIcon</span></span>|[<span data-ttu-id="d8031-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d8031-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d8031-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="d8031-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d8031-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8031-151">createdDateTime</span></span>|<span data-ttu-id="d8031-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8031-152">DateTimeOffset</span></span>|<span data-ttu-id="d8031-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d8031-153">The date and time the app was created.</span></span> <span data-ttu-id="d8031-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8031-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d8031-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8031-156">DateTimeOffset</span></span>|<span data-ttu-id="d8031-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d8031-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d8031-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d8031-159">isFeatured</span></span>|<span data-ttu-id="d8031-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8031-160">Boolean</span></span>|<span data-ttu-id="d8031-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d8031-162">privacyInformationUrl</span></span>|<span data-ttu-id="d8031-163">String</span><span class="sxs-lookup"><span data-stu-id="d8031-163">String</span></span>|<span data-ttu-id="d8031-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d8031-164">The privacy statement Url.</span></span> <span data-ttu-id="d8031-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d8031-166">informationUrl</span></span>|<span data-ttu-id="d8031-167">String</span><span class="sxs-lookup"><span data-stu-id="d8031-167">String</span></span>|<span data-ttu-id="d8031-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d8031-168">The more information Url.</span></span> <span data-ttu-id="d8031-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-170">owner</span><span class="sxs-lookup"><span data-stu-id="d8031-170">owner</span></span>|<span data-ttu-id="d8031-171">String</span><span class="sxs-lookup"><span data-stu-id="d8031-171">String</span></span>|<span data-ttu-id="d8031-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d8031-172">The owner of the app.</span></span> <span data-ttu-id="d8031-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-174">developer</span><span class="sxs-lookup"><span data-stu-id="d8031-174">developer</span></span>|<span data-ttu-id="d8031-175">String</span><span class="sxs-lookup"><span data-stu-id="d8031-175">String</span></span>|<span data-ttu-id="d8031-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d8031-176">The developer of the app.</span></span> <span data-ttu-id="d8031-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-178">notes</span><span class="sxs-lookup"><span data-stu-id="d8031-178">notes</span></span>|<span data-ttu-id="d8031-179">String</span><span class="sxs-lookup"><span data-stu-id="d8031-179">String</span></span>|<span data-ttu-id="d8031-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d8031-180">Notes for the app.</span></span> <span data-ttu-id="d8031-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8031-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d8031-182">publishingState</span></span>|[<span data-ttu-id="d8031-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d8031-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d8031-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d8031-184">The publishing state for the app.</span></span> <span data-ttu-id="d8031-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d8031-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d8031-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d8031-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d8031-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d8031-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d8031-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d8031-188">appAvailability</span></span>|[<span data-ttu-id="d8031-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d8031-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d8031-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="d8031-190">The Application's availability.</span></span> <span data-ttu-id="d8031-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d8031-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d8031-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="d8031-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d8031-193">version</span><span class="sxs-lookup"><span data-stu-id="d8031-193">version</span></span>|<span data-ttu-id="d8031-194">String</span><span class="sxs-lookup"><span data-stu-id="d8031-194">String</span></span>|<span data-ttu-id="d8031-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d8031-195">The Application's version.</span></span> <span data-ttu-id="d8031-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d8031-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d8031-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="d8031-197">bundleId</span></span>|<span data-ttu-id="d8031-198">String</span><span class="sxs-lookup"><span data-stu-id="d8031-198">String</span></span>|<span data-ttu-id="d8031-199">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="d8031-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="d8031-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d8031-200">appStoreUrl</span></span>|<span data-ttu-id="d8031-201">String</span><span class="sxs-lookup"><span data-stu-id="d8031-201">String</span></span>|<span data-ttu-id="d8031-202">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="d8031-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="d8031-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d8031-203">applicableDeviceType</span></span>|[<span data-ttu-id="d8031-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d8031-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d8031-205">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="d8031-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d8031-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8031-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d8031-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8031-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d8031-208">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="d8031-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="d8031-209">応答</span><span class="sxs-lookup"><span data-stu-id="d8031-209">Response</span></span>
<span data-ttu-id="d8031-210">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d8031-210">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8031-211">例</span><span class="sxs-lookup"><span data-stu-id="d8031-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8031-212">要求</span><span class="sxs-lookup"><span data-stu-id="d8031-212">Request</span></span>
<span data-ttu-id="d8031-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8031-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="d8031-214">応答</span><span class="sxs-lookup"><span data-stu-id="d8031-214">Response</span></span>
<span data-ttu-id="d8031-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8031-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



