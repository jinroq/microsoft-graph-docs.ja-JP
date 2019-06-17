---
title: managedAndroidStoreApp の更新
description: managedAndroidStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e635cac001a7c4283da931845e314fcb5ff1406
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974938"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="22ddd-103">managedAndroidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="22ddd-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="22ddd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ddd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ddd-106">[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22ddd-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22ddd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="22ddd-107">Prerequisites</span></span>
<span data-ttu-id="22ddd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ddd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22ddd-110">Permission type</span></span>|<span data-ttu-id="22ddd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22ddd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ddd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22ddd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22ddd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ddd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22ddd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22ddd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ddd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ddd-115">Not supported.</span></span>|
|<span data-ttu-id="22ddd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22ddd-116">Application</span></span>|<span data-ttu-id="22ddd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ddd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22ddd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22ddd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="22ddd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22ddd-119">Request headers</span></span>
|<span data-ttu-id="22ddd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22ddd-120">Header</span></span>|<span data-ttu-id="22ddd-121">値</span><span class="sxs-lookup"><span data-stu-id="22ddd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22ddd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22ddd-122">Authorization</span></span>|<span data-ttu-id="22ddd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="22ddd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22ddd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="22ddd-124">Accept</span></span>|<span data-ttu-id="22ddd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22ddd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ddd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="22ddd-126">Request body</span></span>
<span data-ttu-id="22ddd-127">要求本文で、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22ddd-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="22ddd-128">次の表に、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22ddd-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="22ddd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ddd-129">Property</span></span>|<span data-ttu-id="22ddd-130">型</span><span class="sxs-lookup"><span data-stu-id="22ddd-130">Type</span></span>|<span data-ttu-id="22ddd-131">説明</span><span class="sxs-lookup"><span data-stu-id="22ddd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ddd-132">id</span><span class="sxs-lookup"><span data-stu-id="22ddd-132">id</span></span>|<span data-ttu-id="22ddd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="22ddd-133">String</span></span>|<span data-ttu-id="22ddd-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22ddd-134">Key of the entity.</span></span> <span data-ttu-id="22ddd-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="22ddd-136">displayName</span></span>|<span data-ttu-id="22ddd-137">文字列</span><span class="sxs-lookup"><span data-stu-id="22ddd-137">String</span></span>|<span data-ttu-id="22ddd-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="22ddd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="22ddd-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-140">description</span><span class="sxs-lookup"><span data-stu-id="22ddd-140">description</span></span>|<span data-ttu-id="22ddd-141">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-141">String</span></span>|<span data-ttu-id="22ddd-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="22ddd-142">The description of the app.</span></span> <span data-ttu-id="22ddd-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="22ddd-144">publisher</span></span>|<span data-ttu-id="22ddd-145">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-145">String</span></span>|<span data-ttu-id="22ddd-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="22ddd-146">The publisher of the app.</span></span> <span data-ttu-id="22ddd-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22ddd-148">largeIcon</span></span>|[<span data-ttu-id="22ddd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22ddd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="22ddd-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="22ddd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="22ddd-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22ddd-152">createdDateTime</span></span>|<span data-ttu-id="22ddd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ddd-153">DateTimeOffset</span></span>|<span data-ttu-id="22ddd-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="22ddd-154">The date and time the app was created.</span></span> <span data-ttu-id="22ddd-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22ddd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="22ddd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ddd-157">DateTimeOffset</span></span>|<span data-ttu-id="22ddd-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="22ddd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="22ddd-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22ddd-160">isFeatured</span></span>|<span data-ttu-id="22ddd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="22ddd-161">Boolean</span></span>|<span data-ttu-id="22ddd-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22ddd-163">privacyInformationUrl</span></span>|<span data-ttu-id="22ddd-164">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-164">String</span></span>|<span data-ttu-id="22ddd-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="22ddd-165">The privacy statement Url.</span></span> <span data-ttu-id="22ddd-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22ddd-167">informationUrl</span></span>|<span data-ttu-id="22ddd-168">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-168">String</span></span>|<span data-ttu-id="22ddd-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="22ddd-169">The more information Url.</span></span> <span data-ttu-id="22ddd-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-171">owner</span><span class="sxs-lookup"><span data-stu-id="22ddd-171">owner</span></span>|<span data-ttu-id="22ddd-172">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-172">String</span></span>|<span data-ttu-id="22ddd-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="22ddd-173">The owner of the app.</span></span> <span data-ttu-id="22ddd-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-175">developer</span><span class="sxs-lookup"><span data-stu-id="22ddd-175">developer</span></span>|<span data-ttu-id="22ddd-176">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-176">String</span></span>|<span data-ttu-id="22ddd-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="22ddd-177">The developer of the app.</span></span> <span data-ttu-id="22ddd-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-179">notes</span><span class="sxs-lookup"><span data-stu-id="22ddd-179">notes</span></span>|<span data-ttu-id="22ddd-180">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-180">String</span></span>|<span data-ttu-id="22ddd-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="22ddd-181">Notes for the app.</span></span> <span data-ttu-id="22ddd-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="22ddd-183">uploadState</span></span>|<span data-ttu-id="22ddd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="22ddd-184">Int32</span></span>|<span data-ttu-id="22ddd-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="22ddd-185">The upload state.</span></span> <span data-ttu-id="22ddd-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="22ddd-187">publishingState</span></span>|[<span data-ttu-id="22ddd-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="22ddd-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="22ddd-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="22ddd-189">The publishing state for the app.</span></span> <span data-ttu-id="22ddd-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="22ddd-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22ddd-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="22ddd-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="22ddd-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="22ddd-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="22ddd-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="22ddd-193">isAssigned</span></span>|<span data-ttu-id="22ddd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="22ddd-194">Boolean</span></span>|<span data-ttu-id="22ddd-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="22ddd-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="22ddd-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22ddd-197">roleScopeTagIds</span></span>|<span data-ttu-id="22ddd-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="22ddd-198">String collection</span></span>|<span data-ttu-id="22ddd-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="22ddd-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="22ddd-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="22ddd-201">dependentAppCount</span></span>|<span data-ttu-id="22ddd-202">Int32</span><span class="sxs-lookup"><span data-stu-id="22ddd-202">Int32</span></span>|<span data-ttu-id="22ddd-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="22ddd-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="22ddd-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22ddd-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="22ddd-205">appAvailability</span></span>|[<span data-ttu-id="22ddd-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="22ddd-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="22ddd-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="22ddd-207">The Application's availability.</span></span> <span data-ttu-id="22ddd-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="22ddd-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="22ddd-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="22ddd-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="22ddd-210">version</span><span class="sxs-lookup"><span data-stu-id="22ddd-210">version</span></span>|<span data-ttu-id="22ddd-211">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-211">String</span></span>|<span data-ttu-id="22ddd-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="22ddd-212">The Application's version.</span></span> <span data-ttu-id="22ddd-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22ddd-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="22ddd-214">packageId</span><span class="sxs-lookup"><span data-stu-id="22ddd-214">packageId</span></span>|<span data-ttu-id="22ddd-215">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-215">String</span></span>|<span data-ttu-id="22ddd-216">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="22ddd-216">The app's package ID.</span></span>|
|<span data-ttu-id="22ddd-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="22ddd-217">appStoreUrl</span></span>|<span data-ttu-id="22ddd-218">String</span><span class="sxs-lookup"><span data-stu-id="22ddd-218">String</span></span>|<span data-ttu-id="22ddd-219">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="22ddd-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="22ddd-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22ddd-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="22ddd-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22ddd-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="22ddd-222">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="22ddd-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="22ddd-223">応答</span><span class="sxs-lookup"><span data-stu-id="22ddd-223">Response</span></span>
<span data-ttu-id="22ddd-224">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="22ddd-224">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ddd-225">例</span><span class="sxs-lookup"><span data-stu-id="22ddd-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="22ddd-226">要求</span><span class="sxs-lookup"><span data-stu-id="22ddd-226">Request</span></span>
<span data-ttu-id="22ddd-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22ddd-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "dependentAppCount": 1,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="22ddd-228">応答</span><span class="sxs-lookup"><span data-stu-id="22ddd-228">Response</span></span>
<span data-ttu-id="22ddd-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22ddd-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "dependentAppCount": 1,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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





