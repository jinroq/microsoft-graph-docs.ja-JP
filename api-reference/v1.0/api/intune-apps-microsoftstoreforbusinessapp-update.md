---
title: microsoftStoreForBusinessApp の更新
description: microsoftStoreForBusinessApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 053721e2bc58258e4f6d4d28478ce1bbd736e520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002112"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="cbd28-103">microsoftStoreForBusinessApp の更新</span><span class="sxs-lookup"><span data-stu-id="cbd28-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="cbd28-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbd28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbd28-105">[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbd28-105">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbd28-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cbd28-106">Prerequisites</span></span>
<span data-ttu-id="cbd28-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbd28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd28-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbd28-109">Permission type</span></span>|<span data-ttu-id="cbd28-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbd28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbd28-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbd28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbd28-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd28-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbd28-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbd28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbd28-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd28-114">Not supported.</span></span>|
|<span data-ttu-id="cbd28-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbd28-115">Application</span></span>|<span data-ttu-id="cbd28-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbd28-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbd28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cbd28-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbd28-118">Request headers</span></span>
|<span data-ttu-id="cbd28-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbd28-119">Header</span></span>|<span data-ttu-id="cbd28-120">値</span><span class="sxs-lookup"><span data-stu-id="cbd28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbd28-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd28-121">Authorization</span></span>|<span data-ttu-id="cbd28-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbd28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbd28-123">承諾</span><span class="sxs-lookup"><span data-stu-id="cbd28-123">Accept</span></span>|<span data-ttu-id="cbd28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbd28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbd28-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbd28-125">Request body</span></span>
<span data-ttu-id="cbd28-126">要求本文で、[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cbd28-126">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="cbd28-127">次の表に、[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cbd28-127">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="cbd28-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd28-128">Property</span></span>|<span data-ttu-id="cbd28-129">型</span><span class="sxs-lookup"><span data-stu-id="cbd28-129">Type</span></span>|<span data-ttu-id="cbd28-130">説明</span><span class="sxs-lookup"><span data-stu-id="cbd28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd28-131">id</span><span class="sxs-lookup"><span data-stu-id="cbd28-131">id</span></span>|<span data-ttu-id="cbd28-132">文字列</span><span class="sxs-lookup"><span data-stu-id="cbd28-132">String</span></span>|<span data-ttu-id="cbd28-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cbd28-133">Key of the entity.</span></span> <span data-ttu-id="cbd28-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cbd28-135">displayName</span></span>|<span data-ttu-id="cbd28-136">文字列</span><span class="sxs-lookup"><span data-stu-id="cbd28-136">String</span></span>|<span data-ttu-id="cbd28-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="cbd28-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cbd28-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-139">description</span><span class="sxs-lookup"><span data-stu-id="cbd28-139">description</span></span>|<span data-ttu-id="cbd28-140">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-140">String</span></span>|<span data-ttu-id="cbd28-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="cbd28-141">The description of the app.</span></span> <span data-ttu-id="cbd28-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-143">publisher</span><span class="sxs-lookup"><span data-stu-id="cbd28-143">publisher</span></span>|<span data-ttu-id="cbd28-144">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-144">String</span></span>|<span data-ttu-id="cbd28-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="cbd28-145">The publisher of the app.</span></span> <span data-ttu-id="cbd28-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cbd28-147">largeIcon</span></span>|[<span data-ttu-id="cbd28-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cbd28-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cbd28-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="cbd28-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cbd28-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbd28-151">createdDateTime</span></span>|<span data-ttu-id="cbd28-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbd28-152">DateTimeOffset</span></span>|<span data-ttu-id="cbd28-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cbd28-153">The date and time the app was created.</span></span> <span data-ttu-id="cbd28-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbd28-155">lastModifiedDateTime</span></span>|<span data-ttu-id="cbd28-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbd28-156">DateTimeOffset</span></span>|<span data-ttu-id="cbd28-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="cbd28-157">The date and time the app was last modified.</span></span> <span data-ttu-id="cbd28-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cbd28-159">isFeatured</span></span>|<span data-ttu-id="cbd28-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd28-160">Boolean</span></span>|<span data-ttu-id="cbd28-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cbd28-162">privacyInformationUrl</span></span>|<span data-ttu-id="cbd28-163">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-163">String</span></span>|<span data-ttu-id="cbd28-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="cbd28-164">The privacy statement Url.</span></span> <span data-ttu-id="cbd28-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cbd28-166">informationUrl</span></span>|<span data-ttu-id="cbd28-167">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-167">String</span></span>|<span data-ttu-id="cbd28-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="cbd28-168">The more information Url.</span></span> <span data-ttu-id="cbd28-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-170">owner</span><span class="sxs-lookup"><span data-stu-id="cbd28-170">owner</span></span>|<span data-ttu-id="cbd28-171">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-171">String</span></span>|<span data-ttu-id="cbd28-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="cbd28-172">The owner of the app.</span></span> <span data-ttu-id="cbd28-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-174">developer</span><span class="sxs-lookup"><span data-stu-id="cbd28-174">developer</span></span>|<span data-ttu-id="cbd28-175">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-175">String</span></span>|<span data-ttu-id="cbd28-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="cbd28-176">The developer of the app.</span></span> <span data-ttu-id="cbd28-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-178">notes</span><span class="sxs-lookup"><span data-stu-id="cbd28-178">notes</span></span>|<span data-ttu-id="cbd28-179">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-179">String</span></span>|<span data-ttu-id="cbd28-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="cbd28-180">Notes for the app.</span></span> <span data-ttu-id="cbd28-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cbd28-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cbd28-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="cbd28-182">publishingState</span></span>|[<span data-ttu-id="cbd28-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cbd28-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cbd28-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="cbd28-184">The publishing state for the app.</span></span> <span data-ttu-id="cbd28-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="cbd28-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cbd28-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="cbd28-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cbd28-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="cbd28-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cbd28-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cbd28-188">usedLicenseCount</span></span>|<span data-ttu-id="cbd28-189">Int32</span><span class="sxs-lookup"><span data-stu-id="cbd28-189">Int32</span></span>|<span data-ttu-id="cbd28-190">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="cbd28-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="cbd28-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cbd28-191">totalLicenseCount</span></span>|<span data-ttu-id="cbd28-192">Int32</span><span class="sxs-lookup"><span data-stu-id="cbd28-192">Int32</span></span>|<span data-ttu-id="cbd28-193">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="cbd28-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="cbd28-194">productKey</span><span class="sxs-lookup"><span data-stu-id="cbd28-194">productKey</span></span>|<span data-ttu-id="cbd28-195">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-195">String</span></span>|<span data-ttu-id="cbd28-196">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="cbd28-196">The app product key</span></span>|
|<span data-ttu-id="cbd28-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="cbd28-197">licenseType</span></span>|[<span data-ttu-id="cbd28-198">Microsoft Storeforbusinesslicensetype</span><span class="sxs-lookup"><span data-stu-id="cbd28-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="cbd28-199">アプリライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="cbd28-199">The app license type.</span></span> <span data-ttu-id="cbd28-200">可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="cbd28-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="cbd28-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="cbd28-201">packageIdentityName</span></span>|<span data-ttu-id="cbd28-202">String</span><span class="sxs-lookup"><span data-stu-id="cbd28-202">String</span></span>|<span data-ttu-id="cbd28-203">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="cbd28-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="cbd28-204">応答</span><span class="sxs-lookup"><span data-stu-id="cbd28-204">Response</span></span>
<span data-ttu-id="cbd28-205">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="cbd28-205">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbd28-206">例</span><span class="sxs-lookup"><span data-stu-id="cbd28-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbd28-207">要求</span><span class="sxs-lookup"><span data-stu-id="cbd28-207">Request</span></span>
<span data-ttu-id="cbd28-208">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbd28-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="cbd28-209">応答</span><span class="sxs-lookup"><span data-stu-id="cbd28-209">Response</span></span>
<span data-ttu-id="cbd28-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cbd28-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



