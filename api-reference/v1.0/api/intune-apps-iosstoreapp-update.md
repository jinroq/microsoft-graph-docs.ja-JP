---
title: Update iosStoreApp
description: iosStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4ad218975d5d4b6ac23e294a3321635ff415d69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979558"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="95b44-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="95b44-103">Update iosStoreApp</span></span>

> <span data-ttu-id="95b44-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95b44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b44-105">[iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95b44-105">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95b44-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="95b44-106">Prerequisites</span></span>
<span data-ttu-id="95b44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b44-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95b44-109">Permission type</span></span>|<span data-ttu-id="95b44-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95b44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b44-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95b44-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95b44-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b44-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95b44-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95b44-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b44-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95b44-114">Not supported.</span></span>|
|<span data-ttu-id="95b44-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95b44-115">Application</span></span>|<span data-ttu-id="95b44-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95b44-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b44-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95b44-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="95b44-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95b44-118">Request headers</span></span>
|<span data-ttu-id="95b44-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95b44-119">Header</span></span>|<span data-ttu-id="95b44-120">値</span><span class="sxs-lookup"><span data-stu-id="95b44-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95b44-121">Authorization</span></span>|<span data-ttu-id="95b44-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95b44-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b44-123">承諾</span><span class="sxs-lookup"><span data-stu-id="95b44-123">Accept</span></span>|<span data-ttu-id="95b44-124">application/json</span><span class="sxs-lookup"><span data-stu-id="95b44-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b44-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="95b44-125">Request body</span></span>
<span data-ttu-id="95b44-126">要求本文で、[iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95b44-126">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="95b44-127">次の表に、[iosStoreApp](../resources/intune-apps-iosstoreapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95b44-127">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="95b44-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95b44-128">Property</span></span>|<span data-ttu-id="95b44-129">型</span><span class="sxs-lookup"><span data-stu-id="95b44-129">Type</span></span>|<span data-ttu-id="95b44-130">説明</span><span class="sxs-lookup"><span data-stu-id="95b44-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b44-131">id</span><span class="sxs-lookup"><span data-stu-id="95b44-131">id</span></span>|<span data-ttu-id="95b44-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="95b44-132">String</span></span>|<span data-ttu-id="95b44-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95b44-133">Key of the entity.</span></span> <span data-ttu-id="95b44-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-135">displayName</span><span class="sxs-lookup"><span data-stu-id="95b44-135">displayName</span></span>|<span data-ttu-id="95b44-136">String</span><span class="sxs-lookup"><span data-stu-id="95b44-136">String</span></span>|<span data-ttu-id="95b44-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="95b44-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95b44-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-139">description</span><span class="sxs-lookup"><span data-stu-id="95b44-139">description</span></span>|<span data-ttu-id="95b44-140">String</span><span class="sxs-lookup"><span data-stu-id="95b44-140">String</span></span>|<span data-ttu-id="95b44-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="95b44-141">The description of the app.</span></span> <span data-ttu-id="95b44-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-143">publisher</span><span class="sxs-lookup"><span data-stu-id="95b44-143">publisher</span></span>|<span data-ttu-id="95b44-144">String</span><span class="sxs-lookup"><span data-stu-id="95b44-144">String</span></span>|<span data-ttu-id="95b44-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="95b44-145">The publisher of the app.</span></span> <span data-ttu-id="95b44-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95b44-147">largeIcon</span></span>|[<span data-ttu-id="95b44-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95b44-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="95b44-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="95b44-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95b44-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95b44-151">createdDateTime</span></span>|<span data-ttu-id="95b44-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b44-152">DateTimeOffset</span></span>|<span data-ttu-id="95b44-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="95b44-153">The date and time the app was created.</span></span> <span data-ttu-id="95b44-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95b44-155">lastModifiedDateTime</span></span>|<span data-ttu-id="95b44-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b44-156">DateTimeOffset</span></span>|<span data-ttu-id="95b44-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="95b44-157">The date and time the app was last modified.</span></span> <span data-ttu-id="95b44-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95b44-159">isFeatured</span></span>|<span data-ttu-id="95b44-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b44-160">Boolean</span></span>|<span data-ttu-id="95b44-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95b44-162">privacyInformationUrl</span></span>|<span data-ttu-id="95b44-163">String</span><span class="sxs-lookup"><span data-stu-id="95b44-163">String</span></span>|<span data-ttu-id="95b44-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="95b44-164">The privacy statement Url.</span></span> <span data-ttu-id="95b44-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95b44-166">informationUrl</span></span>|<span data-ttu-id="95b44-167">String</span><span class="sxs-lookup"><span data-stu-id="95b44-167">String</span></span>|<span data-ttu-id="95b44-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="95b44-168">The more information Url.</span></span> <span data-ttu-id="95b44-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-170">owner</span><span class="sxs-lookup"><span data-stu-id="95b44-170">owner</span></span>|<span data-ttu-id="95b44-171">String</span><span class="sxs-lookup"><span data-stu-id="95b44-171">String</span></span>|<span data-ttu-id="95b44-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="95b44-172">The owner of the app.</span></span> <span data-ttu-id="95b44-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-174">developer</span><span class="sxs-lookup"><span data-stu-id="95b44-174">developer</span></span>|<span data-ttu-id="95b44-175">String</span><span class="sxs-lookup"><span data-stu-id="95b44-175">String</span></span>|<span data-ttu-id="95b44-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="95b44-176">The developer of the app.</span></span> <span data-ttu-id="95b44-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-178">notes</span><span class="sxs-lookup"><span data-stu-id="95b44-178">notes</span></span>|<span data-ttu-id="95b44-179">String</span><span class="sxs-lookup"><span data-stu-id="95b44-179">String</span></span>|<span data-ttu-id="95b44-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="95b44-180">Notes for the app.</span></span> <span data-ttu-id="95b44-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95b44-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95b44-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="95b44-182">publishingState</span></span>|[<span data-ttu-id="95b44-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="95b44-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="95b44-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="95b44-184">The publishing state for the app.</span></span> <span data-ttu-id="95b44-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="95b44-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95b44-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95b44-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="95b44-187">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="95b44-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95b44-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="95b44-188">bundleId</span></span>|<span data-ttu-id="95b44-189">String</span><span class="sxs-lookup"><span data-stu-id="95b44-189">String</span></span>|<span data-ttu-id="95b44-190">ID 名。</span><span class="sxs-lookup"><span data-stu-id="95b44-190">The Identity Name.</span></span>|
|<span data-ttu-id="95b44-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="95b44-191">appStoreUrl</span></span>|<span data-ttu-id="95b44-192">String</span><span class="sxs-lookup"><span data-stu-id="95b44-192">String</span></span>|<span data-ttu-id="95b44-193">Apple App Store の URL。</span><span class="sxs-lookup"><span data-stu-id="95b44-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="95b44-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="95b44-194">applicableDeviceType</span></span>|[<span data-ttu-id="95b44-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="95b44-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="95b44-196">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="95b44-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="95b44-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95b44-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="95b44-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95b44-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="95b44-199">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="95b44-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="95b44-200">応答</span><span class="sxs-lookup"><span data-stu-id="95b44-200">Response</span></span>
<span data-ttu-id="95b44-201">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="95b44-201">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b44-202">例</span><span class="sxs-lookup"><span data-stu-id="95b44-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="95b44-203">要求</span><span class="sxs-lookup"><span data-stu-id="95b44-203">Request</span></span>
<span data-ttu-id="95b44-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95b44-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="95b44-205">応答</span><span class="sxs-lookup"><span data-stu-id="95b44-205">Response</span></span>
<span data-ttu-id="95b44-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95b44-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1178

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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



