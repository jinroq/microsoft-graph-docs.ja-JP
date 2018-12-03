---
title: androidStoreApp の作成
description: 新しい androidStoreApp オブジェクトを作成します。
ms.openlocfilehash: cfb571610880a54f0b3b73e0d86841b8c1365db9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069499"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="acfc7-103">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="acfc7-103">Create androidStoreApp</span></span>

> <span data-ttu-id="acfc7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="acfc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acfc7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acfc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acfc7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="acfc7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acfc7-107">新しい [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="acfc7-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acfc7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="acfc7-108">Prerequisites</span></span>
<span data-ttu-id="acfc7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acfc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acfc7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acfc7-111">Permission type</span></span>|<span data-ttu-id="acfc7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="acfc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acfc7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acfc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acfc7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acfc7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="acfc7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acfc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acfc7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acfc7-116">Not supported.</span></span>|
|<span data-ttu-id="acfc7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acfc7-117">Application</span></span>|<span data-ttu-id="acfc7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acfc7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acfc7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acfc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="acfc7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acfc7-120">Request headers</span></span>
|<span data-ttu-id="acfc7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acfc7-121">Header</span></span>|<span data-ttu-id="acfc7-122">値</span><span class="sxs-lookup"><span data-stu-id="acfc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acfc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acfc7-123">Authorization</span></span>|<span data-ttu-id="acfc7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="acfc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acfc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acfc7-125">Accept</span></span>|<span data-ttu-id="acfc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acfc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acfc7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="acfc7-127">Request body</span></span>
<span data-ttu-id="acfc7-128">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="acfc7-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="acfc7-129">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="acfc7-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="acfc7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acfc7-130">Property</span></span>|<span data-ttu-id="acfc7-131">型</span><span class="sxs-lookup"><span data-stu-id="acfc7-131">Type</span></span>|<span data-ttu-id="acfc7-132">説明</span><span class="sxs-lookup"><span data-stu-id="acfc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acfc7-133">id</span><span class="sxs-lookup"><span data-stu-id="acfc7-133">id</span></span>|<span data-ttu-id="acfc7-134">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-134">String</span></span>|<span data-ttu-id="acfc7-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="acfc7-135">Key of the entity.</span></span> <span data-ttu-id="acfc7-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="acfc7-137">displayName</span></span>|<span data-ttu-id="acfc7-138">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-138">String</span></span>|<span data-ttu-id="acfc7-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="acfc7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="acfc7-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-141">説明</span><span class="sxs-lookup"><span data-stu-id="acfc7-141">description</span></span>|<span data-ttu-id="acfc7-142">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-142">String</span></span>|<span data-ttu-id="acfc7-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="acfc7-143">The description of the app.</span></span> <span data-ttu-id="acfc7-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="acfc7-145">publisher</span></span>|<span data-ttu-id="acfc7-146">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-146">String</span></span>|<span data-ttu-id="acfc7-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="acfc7-147">The publisher of the app.</span></span> <span data-ttu-id="acfc7-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="acfc7-149">largeIcon</span></span>|[<span data-ttu-id="acfc7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="acfc7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="acfc7-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="acfc7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="acfc7-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acfc7-153">createdDateTime</span></span>|<span data-ttu-id="acfc7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acfc7-154">DateTimeOffset</span></span>|<span data-ttu-id="acfc7-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="acfc7-155">The date and time the app was created.</span></span> <span data-ttu-id="acfc7-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acfc7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="acfc7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acfc7-158">DateTimeOffset</span></span>|<span data-ttu-id="acfc7-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="acfc7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="acfc7-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="acfc7-161">isFeatured</span></span>|<span data-ttu-id="acfc7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="acfc7-162">Boolean</span></span>|<span data-ttu-id="acfc7-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="acfc7-164">privacyInformationUrl</span></span>|<span data-ttu-id="acfc7-165">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-165">String</span></span>|<span data-ttu-id="acfc7-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="acfc7-166">The privacy statement Url.</span></span> <span data-ttu-id="acfc7-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="acfc7-168">informationUrl</span></span>|<span data-ttu-id="acfc7-169">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-169">String</span></span>|<span data-ttu-id="acfc7-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="acfc7-170">The more information Url.</span></span> <span data-ttu-id="acfc7-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-172">owner</span><span class="sxs-lookup"><span data-stu-id="acfc7-172">owner</span></span>|<span data-ttu-id="acfc7-173">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-173">String</span></span>|<span data-ttu-id="acfc7-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="acfc7-174">The owner of the app.</span></span> <span data-ttu-id="acfc7-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-176">developer</span><span class="sxs-lookup"><span data-stu-id="acfc7-176">developer</span></span>|<span data-ttu-id="acfc7-177">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-177">String</span></span>|<span data-ttu-id="acfc7-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="acfc7-178">The developer of the app.</span></span> <span data-ttu-id="acfc7-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-180">notes</span><span class="sxs-lookup"><span data-stu-id="acfc7-180">notes</span></span>|<span data-ttu-id="acfc7-181">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-181">String</span></span>|<span data-ttu-id="acfc7-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="acfc7-182">Notes for the app.</span></span> <span data-ttu-id="acfc7-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="acfc7-184">uploadState</span></span>|<span data-ttu-id="acfc7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="acfc7-185">Int32</span></span>|<span data-ttu-id="acfc7-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="acfc7-186">The upload state.</span></span> <span data-ttu-id="acfc7-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="acfc7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfc7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="acfc7-188">publishingState</span></span>|[<span data-ttu-id="acfc7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="acfc7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="acfc7-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="acfc7-190">The publishing state for the app.</span></span> <span data-ttu-id="acfc7-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="acfc7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="acfc7-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="acfc7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="acfc7-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="acfc7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="acfc7-194">packageId</span><span class="sxs-lookup"><span data-stu-id="acfc7-194">packageId</span></span>|<span data-ttu-id="acfc7-195">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-195">String</span></span>|<span data-ttu-id="acfc7-196">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="acfc7-196">The package identifier.</span></span>|
|<span data-ttu-id="acfc7-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="acfc7-197">appIdentifier</span></span>|<span data-ttu-id="acfc7-198">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-198">String</span></span>|<span data-ttu-id="acfc7-199">ID 名。</span><span class="sxs-lookup"><span data-stu-id="acfc7-199">The Identity Name.</span></span>|
|<span data-ttu-id="acfc7-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="acfc7-200">appStoreUrl</span></span>|<span data-ttu-id="acfc7-201">String</span><span class="sxs-lookup"><span data-stu-id="acfc7-201">String</span></span>|<span data-ttu-id="acfc7-202">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="acfc7-202">The Android app store URL.</span></span>|
|<span data-ttu-id="acfc7-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="acfc7-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="acfc7-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="acfc7-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="acfc7-205">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="acfc7-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="acfc7-206">応答</span><span class="sxs-lookup"><span data-stu-id="acfc7-206">Response</span></span>
<span data-ttu-id="acfc7-207">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="acfc7-207">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acfc7-208">例</span><span class="sxs-lookup"><span data-stu-id="acfc7-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="acfc7-209">要求</span><span class="sxs-lookup"><span data-stu-id="acfc7-209">Request</span></span>
<span data-ttu-id="acfc7-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="acfc7-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1182

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
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="acfc7-211">応答</span><span class="sxs-lookup"><span data-stu-id="acfc7-211">Response</span></span>
<span data-ttu-id="acfc7-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="acfc7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1290

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
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





