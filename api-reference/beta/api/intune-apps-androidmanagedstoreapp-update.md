---
title: AndroidManagedStoreApp の更新
description: AndroidManagedStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72917bc015f2ca6729bc0efe8156462d001f1eed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331932"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="3efef-103">AndroidManagedStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="3efef-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="3efef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3efef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3efef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3efef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3efef-106">[Androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3efef-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3efef-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3efef-107">Prerequisites</span></span>
<span data-ttu-id="3efef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3efef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3efef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3efef-110">Permission type</span></span>|<span data-ttu-id="3efef-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3efef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3efef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3efef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3efef-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3efef-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3efef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3efef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3efef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3efef-115">Not supported.</span></span>|
|<span data-ttu-id="3efef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3efef-116">Application</span></span>|<span data-ttu-id="3efef-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3efef-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3efef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3efef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3efef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3efef-119">Request headers</span></span>
|<span data-ttu-id="3efef-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3efef-120">Header</span></span>|<span data-ttu-id="3efef-121">値</span><span class="sxs-lookup"><span data-stu-id="3efef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3efef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3efef-122">Authorization</span></span>|<span data-ttu-id="3efef-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3efef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3efef-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3efef-124">Accept</span></span>|<span data-ttu-id="3efef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3efef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3efef-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3efef-126">Request body</span></span>
<span data-ttu-id="3efef-127">要求本文で、 [Androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3efef-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="3efef-128">次の表に、 [Androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3efef-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="3efef-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3efef-129">Property</span></span>|<span data-ttu-id="3efef-130">型</span><span class="sxs-lookup"><span data-stu-id="3efef-130">Type</span></span>|<span data-ttu-id="3efef-131">説明</span><span class="sxs-lookup"><span data-stu-id="3efef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efef-132">id</span><span class="sxs-lookup"><span data-stu-id="3efef-132">id</span></span>|<span data-ttu-id="3efef-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3efef-133">String</span></span>|<span data-ttu-id="3efef-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3efef-134">Key of the entity.</span></span> <span data-ttu-id="3efef-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3efef-136">displayName</span></span>|<span data-ttu-id="3efef-137">文字列</span><span class="sxs-lookup"><span data-stu-id="3efef-137">String</span></span>|<span data-ttu-id="3efef-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="3efef-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3efef-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-140">description</span><span class="sxs-lookup"><span data-stu-id="3efef-140">description</span></span>|<span data-ttu-id="3efef-141">String</span><span class="sxs-lookup"><span data-stu-id="3efef-141">String</span></span>|<span data-ttu-id="3efef-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="3efef-142">The description of the app.</span></span> <span data-ttu-id="3efef-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3efef-144">publisher</span></span>|<span data-ttu-id="3efef-145">String</span><span class="sxs-lookup"><span data-stu-id="3efef-145">String</span></span>|<span data-ttu-id="3efef-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="3efef-146">The publisher of the app.</span></span> <span data-ttu-id="3efef-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3efef-148">largeIcon</span></span>|[<span data-ttu-id="3efef-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3efef-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3efef-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="3efef-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3efef-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3efef-152">createdDateTime</span></span>|<span data-ttu-id="3efef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efef-153">DateTimeOffset</span></span>|<span data-ttu-id="3efef-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="3efef-154">The date and time the app was created.</span></span> <span data-ttu-id="3efef-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3efef-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3efef-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efef-157">DateTimeOffset</span></span>|<span data-ttu-id="3efef-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="3efef-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3efef-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3efef-160">isFeatured</span></span>|<span data-ttu-id="3efef-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3efef-161">Boolean</span></span>|<span data-ttu-id="3efef-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3efef-163">privacyInformationUrl</span></span>|<span data-ttu-id="3efef-164">String</span><span class="sxs-lookup"><span data-stu-id="3efef-164">String</span></span>|<span data-ttu-id="3efef-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="3efef-165">The privacy statement Url.</span></span> <span data-ttu-id="3efef-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3efef-167">informationUrl</span></span>|<span data-ttu-id="3efef-168">String</span><span class="sxs-lookup"><span data-stu-id="3efef-168">String</span></span>|<span data-ttu-id="3efef-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="3efef-169">The more information Url.</span></span> <span data-ttu-id="3efef-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-171">owner</span><span class="sxs-lookup"><span data-stu-id="3efef-171">owner</span></span>|<span data-ttu-id="3efef-172">String</span><span class="sxs-lookup"><span data-stu-id="3efef-172">String</span></span>|<span data-ttu-id="3efef-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="3efef-173">The owner of the app.</span></span> <span data-ttu-id="3efef-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-175">developer</span><span class="sxs-lookup"><span data-stu-id="3efef-175">developer</span></span>|<span data-ttu-id="3efef-176">String</span><span class="sxs-lookup"><span data-stu-id="3efef-176">String</span></span>|<span data-ttu-id="3efef-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="3efef-177">The developer of the app.</span></span> <span data-ttu-id="3efef-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-179">notes</span><span class="sxs-lookup"><span data-stu-id="3efef-179">notes</span></span>|<span data-ttu-id="3efef-180">String</span><span class="sxs-lookup"><span data-stu-id="3efef-180">String</span></span>|<span data-ttu-id="3efef-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="3efef-181">Notes for the app.</span></span> <span data-ttu-id="3efef-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3efef-183">uploadState</span></span>|<span data-ttu-id="3efef-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3efef-184">Int32</span></span>|<span data-ttu-id="3efef-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="3efef-185">The upload state.</span></span> <span data-ttu-id="3efef-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3efef-187">publishingState</span></span>|[<span data-ttu-id="3efef-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3efef-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3efef-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="3efef-189">The publishing state for the app.</span></span> <span data-ttu-id="3efef-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="3efef-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3efef-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3efef-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3efef-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="3efef-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3efef-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3efef-193">isAssigned</span></span>|<span data-ttu-id="3efef-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3efef-194">Boolean</span></span>|<span data-ttu-id="3efef-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="3efef-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3efef-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3efef-197">roleScopeTagIds</span></span>|<span data-ttu-id="3efef-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3efef-198">String collection</span></span>|<span data-ttu-id="3efef-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="3efef-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3efef-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="3efef-201">dependentAppCount</span></span>|<span data-ttu-id="3efef-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3efef-202">Int32</span></span>|<span data-ttu-id="3efef-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="3efef-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3efef-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3efef-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3efef-205">packageId</span><span class="sxs-lookup"><span data-stu-id="3efef-205">packageId</span></span>|<span data-ttu-id="3efef-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3efef-206">String</span></span>|<span data-ttu-id="3efef-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="3efef-207">The package identifier.</span></span>|
|<span data-ttu-id="3efef-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3efef-208">appIdentifier</span></span>|<span data-ttu-id="3efef-209">String</span><span class="sxs-lookup"><span data-stu-id="3efef-209">String</span></span>|<span data-ttu-id="3efef-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="3efef-210">The Identity Name.</span></span>|
|<span data-ttu-id="3efef-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3efef-211">usedLicenseCount</span></span>|<span data-ttu-id="3efef-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3efef-212">Int32</span></span>|<span data-ttu-id="3efef-213">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="3efef-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="3efef-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3efef-214">totalLicenseCount</span></span>|<span data-ttu-id="3efef-215">Int32</span><span class="sxs-lookup"><span data-stu-id="3efef-215">Int32</span></span>|<span data-ttu-id="3efef-216">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="3efef-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="3efef-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3efef-217">appStoreUrl</span></span>|<span data-ttu-id="3efef-218">String</span><span class="sxs-lookup"><span data-stu-id="3efef-218">String</span></span>|<span data-ttu-id="3efef-219">ワークストアアプリの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="3efef-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="3efef-220">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="3efef-220">supportsOemConfig</span></span>|<span data-ttu-id="3efef-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3efef-221">Boolean</span></span>|<span data-ttu-id="3efef-222">このアプリが OEMConfig ポリシーをサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="3efef-222">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3efef-223">応答</span><span class="sxs-lookup"><span data-stu-id="3efef-223">Response</span></span>
<span data-ttu-id="3efef-224">成功した場合、このメソッド`200 OK`は応答コードと、更新された[Androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3efef-224">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3efef-225">例</span><span class="sxs-lookup"><span data-stu-id="3efef-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="3efef-226">要求</span><span class="sxs-lookup"><span data-stu-id="3efef-226">Request</span></span>
<span data-ttu-id="3efef-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3efef-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="3efef-228">応答</span><span class="sxs-lookup"><span data-stu-id="3efef-228">Response</span></span>
<span data-ttu-id="3efef-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3efef-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```






