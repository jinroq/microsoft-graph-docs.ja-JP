---
title: androidStoreApp の更新
description: androidStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15bfdeba3ed97c50dd49f510a73ba0a34a92f956
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259403"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="b8202-103">androidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="b8202-103">Update androidStoreApp</span></span>

> <span data-ttu-id="b8202-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8202-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8202-105">[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8202-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8202-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b8202-106">Prerequisites</span></span>
<span data-ttu-id="b8202-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8202-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b8202-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8202-109">Permission type</span></span>|<span data-ttu-id="b8202-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8202-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8202-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8202-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8202-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8202-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8202-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8202-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8202-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8202-114">Not supported.</span></span>|
|<span data-ttu-id="b8202-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8202-115">Application</span></span>|<span data-ttu-id="b8202-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8202-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8202-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8202-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b8202-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8202-118">Request headers</span></span>
|<span data-ttu-id="b8202-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8202-119">Header</span></span>|<span data-ttu-id="b8202-120">値</span><span class="sxs-lookup"><span data-stu-id="b8202-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8202-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8202-121">Authorization</span></span>|<span data-ttu-id="b8202-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b8202-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8202-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b8202-123">Accept</span></span>|<span data-ttu-id="b8202-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8202-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8202-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8202-125">Request body</span></span>
<span data-ttu-id="b8202-126">要求本文で、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8202-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="b8202-127">次の表に、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b8202-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="b8202-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8202-128">Property</span></span>|<span data-ttu-id="b8202-129">型</span><span class="sxs-lookup"><span data-stu-id="b8202-129">Type</span></span>|<span data-ttu-id="b8202-130">説明</span><span class="sxs-lookup"><span data-stu-id="b8202-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8202-131">id</span><span class="sxs-lookup"><span data-stu-id="b8202-131">id</span></span>|<span data-ttu-id="b8202-132">文字列</span><span class="sxs-lookup"><span data-stu-id="b8202-132">String</span></span>|<span data-ttu-id="b8202-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b8202-133">Key of the entity.</span></span> <span data-ttu-id="b8202-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b8202-135">displayName</span></span>|<span data-ttu-id="b8202-136">String</span><span class="sxs-lookup"><span data-stu-id="b8202-136">String</span></span>|<span data-ttu-id="b8202-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b8202-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b8202-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-139">説明</span><span class="sxs-lookup"><span data-stu-id="b8202-139">description</span></span>|<span data-ttu-id="b8202-140">文字列</span><span class="sxs-lookup"><span data-stu-id="b8202-140">String</span></span>|<span data-ttu-id="b8202-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b8202-141">The description of the app.</span></span> <span data-ttu-id="b8202-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b8202-143">publisher</span></span>|<span data-ttu-id="b8202-144">String</span><span class="sxs-lookup"><span data-stu-id="b8202-144">String</span></span>|<span data-ttu-id="b8202-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b8202-145">The publisher of the app.</span></span> <span data-ttu-id="b8202-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b8202-147">largeIcon</span></span>|[<span data-ttu-id="b8202-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b8202-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b8202-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="b8202-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b8202-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8202-151">createdDateTime</span></span>|<span data-ttu-id="b8202-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8202-152">DateTimeOffset</span></span>|<span data-ttu-id="b8202-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b8202-153">The date and time the app was created.</span></span> <span data-ttu-id="b8202-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8202-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b8202-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8202-156">DateTimeOffset</span></span>|<span data-ttu-id="b8202-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b8202-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b8202-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b8202-159">isFeatured</span></span>|<span data-ttu-id="b8202-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8202-160">Boolean</span></span>|<span data-ttu-id="b8202-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b8202-162">privacyInformationUrl</span></span>|<span data-ttu-id="b8202-163">String</span><span class="sxs-lookup"><span data-stu-id="b8202-163">String</span></span>|<span data-ttu-id="b8202-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b8202-164">The privacy statement Url.</span></span> <span data-ttu-id="b8202-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b8202-166">informationUrl</span></span>|<span data-ttu-id="b8202-167">String</span><span class="sxs-lookup"><span data-stu-id="b8202-167">String</span></span>|<span data-ttu-id="b8202-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b8202-168">The more information Url.</span></span> <span data-ttu-id="b8202-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-170">owner</span><span class="sxs-lookup"><span data-stu-id="b8202-170">owner</span></span>|<span data-ttu-id="b8202-171">String</span><span class="sxs-lookup"><span data-stu-id="b8202-171">String</span></span>|<span data-ttu-id="b8202-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b8202-172">The owner of the app.</span></span> <span data-ttu-id="b8202-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-174">developer</span><span class="sxs-lookup"><span data-stu-id="b8202-174">developer</span></span>|<span data-ttu-id="b8202-175">String</span><span class="sxs-lookup"><span data-stu-id="b8202-175">String</span></span>|<span data-ttu-id="b8202-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b8202-176">The developer of the app.</span></span> <span data-ttu-id="b8202-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-178">notes</span><span class="sxs-lookup"><span data-stu-id="b8202-178">notes</span></span>|<span data-ttu-id="b8202-179">String</span><span class="sxs-lookup"><span data-stu-id="b8202-179">String</span></span>|<span data-ttu-id="b8202-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b8202-180">Notes for the app.</span></span> <span data-ttu-id="b8202-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8202-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8202-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b8202-182">publishingState</span></span>|[<span data-ttu-id="b8202-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b8202-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b8202-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b8202-184">The publishing state for the app.</span></span> <span data-ttu-id="b8202-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b8202-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b8202-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b8202-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b8202-187">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b8202-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b8202-188">packageId</span><span class="sxs-lookup"><span data-stu-id="b8202-188">packageId</span></span>|<span data-ttu-id="b8202-189">String</span><span class="sxs-lookup"><span data-stu-id="b8202-189">String</span></span>|<span data-ttu-id="b8202-190">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="b8202-190">The package identifier.</span></span>|
|<span data-ttu-id="b8202-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b8202-191">appStoreUrl</span></span>|<span data-ttu-id="b8202-192">String</span><span class="sxs-lookup"><span data-stu-id="b8202-192">String</span></span>|<span data-ttu-id="b8202-193">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="b8202-193">The Android app store URL.</span></span>|
|<span data-ttu-id="b8202-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8202-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b8202-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8202-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b8202-196">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="b8202-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b8202-197">応答</span><span class="sxs-lookup"><span data-stu-id="b8202-197">Response</span></span>
<span data-ttu-id="b8202-198">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b8202-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8202-199">例</span><span class="sxs-lookup"><span data-stu-id="b8202-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8202-200">要求</span><span class="sxs-lookup"><span data-stu-id="b8202-200">Request</span></span>
<span data-ttu-id="b8202-201">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8202-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b8202-202">応答</span><span class="sxs-lookup"><span data-stu-id="b8202-202">Response</span></span>
<span data-ttu-id="b8202-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b8202-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```



