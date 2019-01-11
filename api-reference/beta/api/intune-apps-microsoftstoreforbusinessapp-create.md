---
title: Create microsoftStoreForBusinessApp
description: 新しい microsoftStoreForBusinessApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eb5b8bb6b07cff06291aa2cff5a188a54f950574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825047"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="d0abc-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="d0abc-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="d0abc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0abc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0abc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0abc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0abc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0abc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0abc-107">新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d0abc-107">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0abc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0abc-108">Prerequisites</span></span>
<span data-ttu-id="d0abc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0abc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0abc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0abc-111">Permission type</span></span>|<span data-ttu-id="d0abc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0abc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0abc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0abc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0abc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0abc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d0abc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0abc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0abc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0abc-116">Not supported.</span></span>|
|<span data-ttu-id="d0abc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0abc-117">Application</span></span>|<span data-ttu-id="d0abc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0abc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0abc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0abc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d0abc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0abc-120">Request headers</span></span>
|<span data-ttu-id="d0abc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0abc-121">Header</span></span>|<span data-ttu-id="d0abc-122">値</span><span class="sxs-lookup"><span data-stu-id="d0abc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0abc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0abc-123">Authorization</span></span>|<span data-ttu-id="d0abc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d0abc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0abc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0abc-125">Accept</span></span>|<span data-ttu-id="d0abc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0abc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0abc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0abc-127">Request body</span></span>
<span data-ttu-id="d0abc-128">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0abc-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="d0abc-129">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d0abc-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="d0abc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0abc-130">Property</span></span>|<span data-ttu-id="d0abc-131">種類</span><span class="sxs-lookup"><span data-stu-id="d0abc-131">Type</span></span>|<span data-ttu-id="d0abc-132">説明</span><span class="sxs-lookup"><span data-stu-id="d0abc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0abc-133">ID</span><span class="sxs-lookup"><span data-stu-id="d0abc-133">id</span></span>|<span data-ttu-id="d0abc-134">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-134">String</span></span>|<span data-ttu-id="d0abc-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d0abc-135">Key of the entity.</span></span> <span data-ttu-id="d0abc-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d0abc-137">displayName</span></span>|<span data-ttu-id="d0abc-138">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-138">String</span></span>|<span data-ttu-id="d0abc-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d0abc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d0abc-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-141">説明</span><span class="sxs-lookup"><span data-stu-id="d0abc-141">description</span></span>|<span data-ttu-id="d0abc-142">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-142">String</span></span>|<span data-ttu-id="d0abc-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d0abc-143">The description of the app.</span></span> <span data-ttu-id="d0abc-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d0abc-145">publisher</span></span>|<span data-ttu-id="d0abc-146">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-146">String</span></span>|<span data-ttu-id="d0abc-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d0abc-147">The publisher of the app.</span></span> <span data-ttu-id="d0abc-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d0abc-149">largeIcon</span></span>|[<span data-ttu-id="d0abc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d0abc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d0abc-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="d0abc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d0abc-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0abc-153">createdDateTime</span></span>|<span data-ttu-id="d0abc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0abc-154">DateTimeOffset</span></span>|<span data-ttu-id="d0abc-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d0abc-155">The date and time the app was created.</span></span> <span data-ttu-id="d0abc-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0abc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d0abc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0abc-158">DateTimeOffset</span></span>|<span data-ttu-id="d0abc-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d0abc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d0abc-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d0abc-161">isFeatured</span></span>|<span data-ttu-id="d0abc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0abc-162">Boolean</span></span>|<span data-ttu-id="d0abc-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d0abc-164">privacyInformationUrl</span></span>|<span data-ttu-id="d0abc-165">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-165">String</span></span>|<span data-ttu-id="d0abc-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d0abc-166">The privacy statement Url.</span></span> <span data-ttu-id="d0abc-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d0abc-168">informationUrl</span></span>|<span data-ttu-id="d0abc-169">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-169">String</span></span>|<span data-ttu-id="d0abc-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d0abc-170">The more information Url.</span></span> <span data-ttu-id="d0abc-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-172">owner</span><span class="sxs-lookup"><span data-stu-id="d0abc-172">owner</span></span>|<span data-ttu-id="d0abc-173">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-173">String</span></span>|<span data-ttu-id="d0abc-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d0abc-174">The owner of the app.</span></span> <span data-ttu-id="d0abc-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-176">developer</span><span class="sxs-lookup"><span data-stu-id="d0abc-176">developer</span></span>|<span data-ttu-id="d0abc-177">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-177">String</span></span>|<span data-ttu-id="d0abc-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d0abc-178">The developer of the app.</span></span> <span data-ttu-id="d0abc-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-180">notes</span><span class="sxs-lookup"><span data-stu-id="d0abc-180">notes</span></span>|<span data-ttu-id="d0abc-181">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-181">String</span></span>|<span data-ttu-id="d0abc-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d0abc-182">Notes for the app.</span></span> <span data-ttu-id="d0abc-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d0abc-184">uploadState</span></span>|<span data-ttu-id="d0abc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d0abc-185">Int32</span></span>|<span data-ttu-id="d0abc-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="d0abc-186">The upload state.</span></span> <span data-ttu-id="d0abc-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d0abc-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0abc-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d0abc-188">publishingState</span></span>|[<span data-ttu-id="d0abc-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d0abc-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d0abc-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d0abc-190">The publishing state for the app.</span></span> <span data-ttu-id="d0abc-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d0abc-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d0abc-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d0abc-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d0abc-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d0abc-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d0abc-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d0abc-194">usedLicenseCount</span></span>|<span data-ttu-id="d0abc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="d0abc-195">Int32</span></span>|<span data-ttu-id="d0abc-196">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="d0abc-196">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="d0abc-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d0abc-197">totalLicenseCount</span></span>|<span data-ttu-id="d0abc-198">Int32</span><span class="sxs-lookup"><span data-stu-id="d0abc-198">Int32</span></span>|<span data-ttu-id="d0abc-199">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="d0abc-199">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="d0abc-200">productKey</span><span class="sxs-lookup"><span data-stu-id="d0abc-200">productKey</span></span>|<span data-ttu-id="d0abc-201">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-201">String</span></span>|<span data-ttu-id="d0abc-202">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="d0abc-202">The app product key</span></span>|
|<span data-ttu-id="d0abc-203">licenseType</span><span class="sxs-lookup"><span data-stu-id="d0abc-203">licenseType</span></span>|[<span data-ttu-id="d0abc-204">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="d0abc-204">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="d0abc-205">アプリケーション ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="d0abc-205">The app license type.</span></span> <span data-ttu-id="d0abc-206">使用可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="d0abc-206">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="d0abc-207">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="d0abc-207">packageIdentityName</span></span>|<span data-ttu-id="d0abc-208">String</span><span class="sxs-lookup"><span data-stu-id="d0abc-208">String</span></span>|<span data-ttu-id="d0abc-209">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="d0abc-209">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="d0abc-210">応答</span><span class="sxs-lookup"><span data-stu-id="d0abc-210">Response</span></span>
<span data-ttu-id="d0abc-211">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d0abc-211">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0abc-212">例</span><span class="sxs-lookup"><span data-stu-id="d0abc-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0abc-213">要求</span><span class="sxs-lookup"><span data-stu-id="d0abc-213">Request</span></span>
<span data-ttu-id="d0abc-214">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0abc-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="d0abc-215">応答</span><span class="sxs-lookup"><span data-stu-id="d0abc-215">Response</span></span>
<span data-ttu-id="d0abc-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0abc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 963

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
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```





