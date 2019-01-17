---
title: iosStoreApp の作成
description: 新しい iosStoreApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0eecf7db834c13894f21a47edb095801a9ed5b47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980553"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="c8960-103">iosStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="c8960-103">Create iosStoreApp</span></span>

> <span data-ttu-id="c8960-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8960-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8960-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8960-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8960-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8960-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8960-107">新しい [iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8960-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8960-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8960-108">Prerequisites</span></span>
<span data-ttu-id="c8960-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8960-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8960-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8960-111">Permission type</span></span>|<span data-ttu-id="c8960-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8960-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8960-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8960-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8960-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8960-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8960-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8960-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8960-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8960-116">Not supported.</span></span>|
|<span data-ttu-id="c8960-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8960-117">Application</span></span>|<span data-ttu-id="c8960-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8960-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8960-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8960-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c8960-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8960-120">Request headers</span></span>
|<span data-ttu-id="c8960-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8960-121">Header</span></span>|<span data-ttu-id="c8960-122">値</span><span class="sxs-lookup"><span data-stu-id="c8960-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8960-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8960-123">Authorization</span></span>|<span data-ttu-id="c8960-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8960-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8960-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8960-125">Accept</span></span>|<span data-ttu-id="c8960-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8960-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8960-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8960-127">Request body</span></span>
<span data-ttu-id="c8960-128">要求本文で、iosStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8960-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="c8960-129">次の表に、iosStoreApp 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8960-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="c8960-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8960-130">Property</span></span>|<span data-ttu-id="c8960-131">型</span><span class="sxs-lookup"><span data-stu-id="c8960-131">Type</span></span>|<span data-ttu-id="c8960-132">説明</span><span class="sxs-lookup"><span data-stu-id="c8960-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8960-133">id</span><span class="sxs-lookup"><span data-stu-id="c8960-133">id</span></span>|<span data-ttu-id="c8960-134">String</span><span class="sxs-lookup"><span data-stu-id="c8960-134">String</span></span>|<span data-ttu-id="c8960-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8960-135">Key of the entity.</span></span> <span data-ttu-id="c8960-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c8960-137">displayName</span></span>|<span data-ttu-id="c8960-138">String</span><span class="sxs-lookup"><span data-stu-id="c8960-138">String</span></span>|<span data-ttu-id="c8960-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c8960-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c8960-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-141">説明</span><span class="sxs-lookup"><span data-stu-id="c8960-141">description</span></span>|<span data-ttu-id="c8960-142">String</span><span class="sxs-lookup"><span data-stu-id="c8960-142">String</span></span>|<span data-ttu-id="c8960-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c8960-143">The description of the app.</span></span> <span data-ttu-id="c8960-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c8960-145">publisher</span></span>|<span data-ttu-id="c8960-146">String</span><span class="sxs-lookup"><span data-stu-id="c8960-146">String</span></span>|<span data-ttu-id="c8960-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c8960-147">The publisher of the app.</span></span> <span data-ttu-id="c8960-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c8960-149">largeIcon</span></span>|[<span data-ttu-id="c8960-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c8960-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c8960-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="c8960-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c8960-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8960-153">createdDateTime</span></span>|<span data-ttu-id="c8960-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8960-154">DateTimeOffset</span></span>|<span data-ttu-id="c8960-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c8960-155">The date and time the app was created.</span></span> <span data-ttu-id="c8960-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8960-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c8960-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8960-158">DateTimeOffset</span></span>|<span data-ttu-id="c8960-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c8960-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c8960-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c8960-161">isFeatured</span></span>|<span data-ttu-id="c8960-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8960-162">Boolean</span></span>|<span data-ttu-id="c8960-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c8960-164">privacyInformationUrl</span></span>|<span data-ttu-id="c8960-165">String</span><span class="sxs-lookup"><span data-stu-id="c8960-165">String</span></span>|<span data-ttu-id="c8960-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c8960-166">The privacy statement Url.</span></span> <span data-ttu-id="c8960-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c8960-168">informationUrl</span></span>|<span data-ttu-id="c8960-169">String</span><span class="sxs-lookup"><span data-stu-id="c8960-169">String</span></span>|<span data-ttu-id="c8960-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c8960-170">The more information Url.</span></span> <span data-ttu-id="c8960-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-172">owner</span><span class="sxs-lookup"><span data-stu-id="c8960-172">owner</span></span>|<span data-ttu-id="c8960-173">String</span><span class="sxs-lookup"><span data-stu-id="c8960-173">String</span></span>|<span data-ttu-id="c8960-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c8960-174">The owner of the app.</span></span> <span data-ttu-id="c8960-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-176">developer</span><span class="sxs-lookup"><span data-stu-id="c8960-176">developer</span></span>|<span data-ttu-id="c8960-177">String</span><span class="sxs-lookup"><span data-stu-id="c8960-177">String</span></span>|<span data-ttu-id="c8960-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c8960-178">The developer of the app.</span></span> <span data-ttu-id="c8960-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-180">notes</span><span class="sxs-lookup"><span data-stu-id="c8960-180">notes</span></span>|<span data-ttu-id="c8960-181">String</span><span class="sxs-lookup"><span data-stu-id="c8960-181">String</span></span>|<span data-ttu-id="c8960-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c8960-182">Notes for the app.</span></span> <span data-ttu-id="c8960-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c8960-184">uploadState</span></span>|<span data-ttu-id="c8960-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c8960-185">Int32</span></span>|<span data-ttu-id="c8960-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="c8960-186">The upload state.</span></span> <span data-ttu-id="c8960-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8960-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8960-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c8960-188">publishingState</span></span>|[<span data-ttu-id="c8960-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c8960-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c8960-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c8960-190">The publishing state for the app.</span></span> <span data-ttu-id="c8960-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c8960-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c8960-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c8960-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c8960-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c8960-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c8960-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="c8960-194">bundleId</span></span>|<span data-ttu-id="c8960-195">String</span><span class="sxs-lookup"><span data-stu-id="c8960-195">String</span></span>|<span data-ttu-id="c8960-196">ID 名。</span><span class="sxs-lookup"><span data-stu-id="c8960-196">The Identity Name.</span></span>|
|<span data-ttu-id="c8960-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c8960-197">appStoreUrl</span></span>|<span data-ttu-id="c8960-198">String</span><span class="sxs-lookup"><span data-stu-id="c8960-198">String</span></span>|<span data-ttu-id="c8960-199">Apple App Store の URL。</span><span class="sxs-lookup"><span data-stu-id="c8960-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="c8960-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c8960-200">applicableDeviceType</span></span>|[<span data-ttu-id="c8960-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c8960-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c8960-202">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="c8960-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c8960-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c8960-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c8960-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c8960-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c8960-205">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="c8960-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c8960-206">応答</span><span class="sxs-lookup"><span data-stu-id="c8960-206">Response</span></span>
<span data-ttu-id="c8960-207">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8960-207">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8960-208">例</span><span class="sxs-lookup"><span data-stu-id="c8960-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8960-209">要求</span><span class="sxs-lookup"><span data-stu-id="c8960-209">Request</span></span>
<span data-ttu-id="c8960-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8960-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1092

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
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

### <a name="response"></a><span data-ttu-id="c8960-211">応答</span><span class="sxs-lookup"><span data-stu-id="c8960-211">Response</span></span>
<span data-ttu-id="c8960-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8960-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1200

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
  "uploadState": 11,
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





