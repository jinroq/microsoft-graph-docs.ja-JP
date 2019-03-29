---
title: androidStoreApp の更新
description: androidStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e895082061cac0c572ac9fd240d7eff18f096202
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972453"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="50775-103">androidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="50775-103">Update androidStoreApp</span></span>

> <span data-ttu-id="50775-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50775-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50775-106">[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50775-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50775-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="50775-107">Prerequisites</span></span>
<span data-ttu-id="50775-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50775-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50775-110">Permission type</span></span>|<span data-ttu-id="50775-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50775-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50775-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50775-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50775-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50775-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50775-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50775-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50775-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50775-115">Not supported.</span></span>|
|<span data-ttu-id="50775-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50775-116">Application</span></span>|<span data-ttu-id="50775-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50775-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50775-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50775-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="50775-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50775-119">Request headers</span></span>
|<span data-ttu-id="50775-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50775-120">Header</span></span>|<span data-ttu-id="50775-121">値</span><span class="sxs-lookup"><span data-stu-id="50775-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50775-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50775-122">Authorization</span></span>|<span data-ttu-id="50775-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="50775-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50775-124">承諾</span><span class="sxs-lookup"><span data-stu-id="50775-124">Accept</span></span>|<span data-ttu-id="50775-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50775-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50775-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50775-126">Request body</span></span>
<span data-ttu-id="50775-127">要求本文で、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50775-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="50775-128">次の表に、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="50775-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="50775-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50775-129">Property</span></span>|<span data-ttu-id="50775-130">型</span><span class="sxs-lookup"><span data-stu-id="50775-130">Type</span></span>|<span data-ttu-id="50775-131">説明</span><span class="sxs-lookup"><span data-stu-id="50775-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50775-132">id</span><span class="sxs-lookup"><span data-stu-id="50775-132">id</span></span>|<span data-ttu-id="50775-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50775-133">String</span></span>|<span data-ttu-id="50775-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50775-134">Key of the entity.</span></span> <span data-ttu-id="50775-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50775-136">displayName</span></span>|<span data-ttu-id="50775-137">String</span><span class="sxs-lookup"><span data-stu-id="50775-137">String</span></span>|<span data-ttu-id="50775-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="50775-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="50775-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-140">description</span><span class="sxs-lookup"><span data-stu-id="50775-140">description</span></span>|<span data-ttu-id="50775-141">String</span><span class="sxs-lookup"><span data-stu-id="50775-141">String</span></span>|<span data-ttu-id="50775-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="50775-142">The description of the app.</span></span> <span data-ttu-id="50775-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-144">publisher</span><span class="sxs-lookup"><span data-stu-id="50775-144">publisher</span></span>|<span data-ttu-id="50775-145">String</span><span class="sxs-lookup"><span data-stu-id="50775-145">String</span></span>|<span data-ttu-id="50775-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="50775-146">The publisher of the app.</span></span> <span data-ttu-id="50775-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="50775-148">largeIcon</span></span>|[<span data-ttu-id="50775-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50775-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50775-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="50775-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="50775-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50775-152">createdDateTime</span></span>|<span data-ttu-id="50775-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50775-153">DateTimeOffset</span></span>|<span data-ttu-id="50775-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="50775-154">The date and time the app was created.</span></span> <span data-ttu-id="50775-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50775-156">lastModifiedDateTime</span></span>|<span data-ttu-id="50775-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50775-157">DateTimeOffset</span></span>|<span data-ttu-id="50775-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="50775-158">The date and time the app was last modified.</span></span> <span data-ttu-id="50775-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="50775-160">isFeatured</span></span>|<span data-ttu-id="50775-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="50775-161">Boolean</span></span>|<span data-ttu-id="50775-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="50775-163">privacyInformationUrl</span></span>|<span data-ttu-id="50775-164">String</span><span class="sxs-lookup"><span data-stu-id="50775-164">String</span></span>|<span data-ttu-id="50775-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="50775-165">The privacy statement Url.</span></span> <span data-ttu-id="50775-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="50775-167">informationUrl</span></span>|<span data-ttu-id="50775-168">String</span><span class="sxs-lookup"><span data-stu-id="50775-168">String</span></span>|<span data-ttu-id="50775-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="50775-169">The more information Url.</span></span> <span data-ttu-id="50775-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-171">owner</span><span class="sxs-lookup"><span data-stu-id="50775-171">owner</span></span>|<span data-ttu-id="50775-172">String</span><span class="sxs-lookup"><span data-stu-id="50775-172">String</span></span>|<span data-ttu-id="50775-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="50775-173">The owner of the app.</span></span> <span data-ttu-id="50775-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-175">developer</span><span class="sxs-lookup"><span data-stu-id="50775-175">developer</span></span>|<span data-ttu-id="50775-176">String</span><span class="sxs-lookup"><span data-stu-id="50775-176">String</span></span>|<span data-ttu-id="50775-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="50775-177">The developer of the app.</span></span> <span data-ttu-id="50775-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-179">notes</span><span class="sxs-lookup"><span data-stu-id="50775-179">notes</span></span>|<span data-ttu-id="50775-180">String</span><span class="sxs-lookup"><span data-stu-id="50775-180">String</span></span>|<span data-ttu-id="50775-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="50775-181">Notes for the app.</span></span> <span data-ttu-id="50775-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="50775-183">uploadState</span></span>|<span data-ttu-id="50775-184">Int32</span><span class="sxs-lookup"><span data-stu-id="50775-184">Int32</span></span>|<span data-ttu-id="50775-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="50775-185">The upload state.</span></span> <span data-ttu-id="50775-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="50775-187">publishingState</span></span>|[<span data-ttu-id="50775-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="50775-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="50775-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="50775-189">The publishing state for the app.</span></span> <span data-ttu-id="50775-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="50775-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="50775-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="50775-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="50775-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="50775-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="50775-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="50775-193">isAssigned</span></span>|<span data-ttu-id="50775-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="50775-194">Boolean</span></span>|<span data-ttu-id="50775-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="50775-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="50775-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50775-197">roleScopeTagIds</span></span>|<span data-ttu-id="50775-198">String collection</span><span class="sxs-lookup"><span data-stu-id="50775-198">String collection</span></span>|<span data-ttu-id="50775-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="50775-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="50775-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50775-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50775-201">packageId</span><span class="sxs-lookup"><span data-stu-id="50775-201">packageId</span></span>|<span data-ttu-id="50775-202">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50775-202">String</span></span>|<span data-ttu-id="50775-203">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="50775-203">The package identifier.</span></span>|
|<span data-ttu-id="50775-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="50775-204">appIdentifier</span></span>|<span data-ttu-id="50775-205">String</span><span class="sxs-lookup"><span data-stu-id="50775-205">String</span></span>|<span data-ttu-id="50775-206">ID 名。</span><span class="sxs-lookup"><span data-stu-id="50775-206">The Identity Name.</span></span>|
|<span data-ttu-id="50775-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="50775-207">appStoreUrl</span></span>|<span data-ttu-id="50775-208">String</span><span class="sxs-lookup"><span data-stu-id="50775-208">String</span></span>|<span data-ttu-id="50775-209">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="50775-209">The Android app store URL.</span></span>|
|<span data-ttu-id="50775-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50775-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="50775-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50775-211">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="50775-212">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="50775-212">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="50775-213">応答</span><span class="sxs-lookup"><span data-stu-id="50775-213">Response</span></span>
<span data-ttu-id="50775-214">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="50775-214">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50775-215">例</span><span class="sxs-lookup"><span data-stu-id="50775-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="50775-216">要求</span><span class="sxs-lookup"><span data-stu-id="50775-216">Request</span></span>
<span data-ttu-id="50775-217">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50775-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1203

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="50775-218">応答</span><span class="sxs-lookup"><span data-stu-id="50775-218">Response</span></span>
<span data-ttu-id="50775-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50775-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1375

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




