---
title: AndroidManagedStoreApp を更新します。
description: AndroidManagedStoreApp オブジェクトのプロパティを更新します。
ms.openlocfilehash: c3c2edde22e1b6538b08930507136e15d470e221
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072446"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="452df-103">AndroidManagedStoreApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="452df-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="452df-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="452df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="452df-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="452df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="452df-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="452df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="452df-107">[AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="452df-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="452df-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="452df-108">Prerequisites</span></span>
<span data-ttu-id="452df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="452df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="452df-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="452df-111">Permission type</span></span>|<span data-ttu-id="452df-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="452df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="452df-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="452df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="452df-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452df-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="452df-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="452df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="452df-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="452df-116">Not supported.</span></span>|
|<span data-ttu-id="452df-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="452df-117">Application</span></span>|<span data-ttu-id="452df-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="452df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="452df-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="452df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="452df-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="452df-120">Request headers</span></span>
|<span data-ttu-id="452df-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="452df-121">Header</span></span>|<span data-ttu-id="452df-122">値</span><span class="sxs-lookup"><span data-stu-id="452df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="452df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="452df-123">Authorization</span></span>|<span data-ttu-id="452df-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="452df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="452df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="452df-125">Accept</span></span>|<span data-ttu-id="452df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="452df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="452df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="452df-127">Request body</span></span>
<span data-ttu-id="452df-128">要求の本文に[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="452df-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="452df-129">[AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="452df-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="452df-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="452df-130">Property</span></span>|<span data-ttu-id="452df-131">型</span><span class="sxs-lookup"><span data-stu-id="452df-131">Type</span></span>|<span data-ttu-id="452df-132">説明</span><span class="sxs-lookup"><span data-stu-id="452df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="452df-133">id</span><span class="sxs-lookup"><span data-stu-id="452df-133">id</span></span>|<span data-ttu-id="452df-134">String</span><span class="sxs-lookup"><span data-stu-id="452df-134">String</span></span>|<span data-ttu-id="452df-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="452df-135">Key of the entity.</span></span> <span data-ttu-id="452df-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-137">displayName</span><span class="sxs-lookup"><span data-stu-id="452df-137">displayName</span></span>|<span data-ttu-id="452df-138">String</span><span class="sxs-lookup"><span data-stu-id="452df-138">String</span></span>|<span data-ttu-id="452df-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="452df-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="452df-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-141">説明</span><span class="sxs-lookup"><span data-stu-id="452df-141">description</span></span>|<span data-ttu-id="452df-142">String</span><span class="sxs-lookup"><span data-stu-id="452df-142">String</span></span>|<span data-ttu-id="452df-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="452df-143">The description of the app.</span></span> <span data-ttu-id="452df-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-145">publisher</span><span class="sxs-lookup"><span data-stu-id="452df-145">publisher</span></span>|<span data-ttu-id="452df-146">String</span><span class="sxs-lookup"><span data-stu-id="452df-146">String</span></span>|<span data-ttu-id="452df-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="452df-147">The publisher of the app.</span></span> <span data-ttu-id="452df-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="452df-149">largeIcon</span></span>|[<span data-ttu-id="452df-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="452df-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="452df-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="452df-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="452df-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="452df-153">createdDateTime</span></span>|<span data-ttu-id="452df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="452df-154">DateTimeOffset</span></span>|<span data-ttu-id="452df-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="452df-155">The date and time the app was created.</span></span> <span data-ttu-id="452df-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="452df-157">lastModifiedDateTime</span></span>|<span data-ttu-id="452df-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="452df-158">DateTimeOffset</span></span>|<span data-ttu-id="452df-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="452df-159">The date and time the app was last modified.</span></span> <span data-ttu-id="452df-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="452df-161">isFeatured</span></span>|<span data-ttu-id="452df-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="452df-162">Boolean</span></span>|<span data-ttu-id="452df-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="452df-164">privacyInformationUrl</span></span>|<span data-ttu-id="452df-165">String</span><span class="sxs-lookup"><span data-stu-id="452df-165">String</span></span>|<span data-ttu-id="452df-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="452df-166">The privacy statement Url.</span></span> <span data-ttu-id="452df-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="452df-168">informationUrl</span></span>|<span data-ttu-id="452df-169">String</span><span class="sxs-lookup"><span data-stu-id="452df-169">String</span></span>|<span data-ttu-id="452df-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="452df-170">The more information Url.</span></span> <span data-ttu-id="452df-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-172">owner</span><span class="sxs-lookup"><span data-stu-id="452df-172">owner</span></span>|<span data-ttu-id="452df-173">String</span><span class="sxs-lookup"><span data-stu-id="452df-173">String</span></span>|<span data-ttu-id="452df-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="452df-174">The owner of the app.</span></span> <span data-ttu-id="452df-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-176">developer</span><span class="sxs-lookup"><span data-stu-id="452df-176">developer</span></span>|<span data-ttu-id="452df-177">String</span><span class="sxs-lookup"><span data-stu-id="452df-177">String</span></span>|<span data-ttu-id="452df-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="452df-178">The developer of the app.</span></span> <span data-ttu-id="452df-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-180">notes</span><span class="sxs-lookup"><span data-stu-id="452df-180">notes</span></span>|<span data-ttu-id="452df-181">String</span><span class="sxs-lookup"><span data-stu-id="452df-181">String</span></span>|<span data-ttu-id="452df-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="452df-182">Notes for the app.</span></span> <span data-ttu-id="452df-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="452df-184">uploadState</span></span>|<span data-ttu-id="452df-185">Int32</span><span class="sxs-lookup"><span data-stu-id="452df-185">Int32</span></span>|<span data-ttu-id="452df-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="452df-186">The upload state.</span></span> <span data-ttu-id="452df-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="452df-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="452df-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="452df-188">publishingState</span></span>|[<span data-ttu-id="452df-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="452df-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="452df-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="452df-190">The publishing state for the app.</span></span> <span data-ttu-id="452df-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="452df-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="452df-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="452df-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="452df-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="452df-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="452df-194">packageId</span><span class="sxs-lookup"><span data-stu-id="452df-194">packageId</span></span>|<span data-ttu-id="452df-195">String</span><span class="sxs-lookup"><span data-stu-id="452df-195">String</span></span>|<span data-ttu-id="452df-196">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="452df-196">The package identifier.</span></span>|
|<span data-ttu-id="452df-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="452df-197">appIdentifier</span></span>|<span data-ttu-id="452df-198">String</span><span class="sxs-lookup"><span data-stu-id="452df-198">String</span></span>|<span data-ttu-id="452df-199">ID 名。</span><span class="sxs-lookup"><span data-stu-id="452df-199">The Identity Name.</span></span>|
|<span data-ttu-id="452df-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="452df-200">usedLicenseCount</span></span>|<span data-ttu-id="452df-201">Int32</span><span class="sxs-lookup"><span data-stu-id="452df-201">Int32</span></span>|<span data-ttu-id="452df-202">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="452df-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="452df-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="452df-203">totalLicenseCount</span></span>|<span data-ttu-id="452df-204">Int32</span><span class="sxs-lookup"><span data-stu-id="452df-204">Int32</span></span>|<span data-ttu-id="452df-205">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="452df-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="452df-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="452df-206">appStoreUrl</span></span>|<span data-ttu-id="452df-207">String</span><span class="sxs-lookup"><span data-stu-id="452df-207">String</span></span>|<span data-ttu-id="452df-208">作業ストア アプリケーションの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="452df-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="452df-209">応答</span><span class="sxs-lookup"><span data-stu-id="452df-209">Response</span></span>
<span data-ttu-id="452df-210">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="452df-210">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="452df-211">例</span><span class="sxs-lookup"><span data-stu-id="452df-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="452df-212">要求</span><span class="sxs-lookup"><span data-stu-id="452df-212">Request</span></span>
<span data-ttu-id="452df-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="452df-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 799

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="452df-214">応答</span><span class="sxs-lookup"><span data-stu-id="452df-214">Response</span></span>
<span data-ttu-id="452df-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="452df-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





