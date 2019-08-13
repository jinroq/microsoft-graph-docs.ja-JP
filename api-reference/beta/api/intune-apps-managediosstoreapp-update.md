---
title: managedIOSStoreApp の更新
description: managedIOSStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 823ec6074012d85831de2e745720a0ed4a40518e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329517"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="22c47-103">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="22c47-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="22c47-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22c47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22c47-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22c47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22c47-106">[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22c47-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22c47-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="22c47-107">Prerequisites</span></span>
<span data-ttu-id="22c47-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c47-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22c47-110">Permission type</span></span>|<span data-ttu-id="22c47-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22c47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22c47-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22c47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22c47-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22c47-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22c47-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22c47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22c47-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22c47-115">Not supported.</span></span>|
|<span data-ttu-id="22c47-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22c47-116">Application</span></span>|<span data-ttu-id="22c47-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22c47-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22c47-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22c47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="22c47-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22c47-119">Request headers</span></span>
|<span data-ttu-id="22c47-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22c47-120">Header</span></span>|<span data-ttu-id="22c47-121">値</span><span class="sxs-lookup"><span data-stu-id="22c47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22c47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22c47-122">Authorization</span></span>|<span data-ttu-id="22c47-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="22c47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22c47-124">承諾</span><span class="sxs-lookup"><span data-stu-id="22c47-124">Accept</span></span>|<span data-ttu-id="22c47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22c47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22c47-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="22c47-126">Request body</span></span>
<span data-ttu-id="22c47-127">要求本文で、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22c47-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="22c47-128">次の表に、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22c47-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="22c47-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22c47-129">Property</span></span>|<span data-ttu-id="22c47-130">型</span><span class="sxs-lookup"><span data-stu-id="22c47-130">Type</span></span>|<span data-ttu-id="22c47-131">説明</span><span class="sxs-lookup"><span data-stu-id="22c47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22c47-132">id</span><span class="sxs-lookup"><span data-stu-id="22c47-132">id</span></span>|<span data-ttu-id="22c47-133">文字列</span><span class="sxs-lookup"><span data-stu-id="22c47-133">String</span></span>|<span data-ttu-id="22c47-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22c47-134">Key of the entity.</span></span> <span data-ttu-id="22c47-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-136">displayName</span><span class="sxs-lookup"><span data-stu-id="22c47-136">displayName</span></span>|<span data-ttu-id="22c47-137">文字列</span><span class="sxs-lookup"><span data-stu-id="22c47-137">String</span></span>|<span data-ttu-id="22c47-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="22c47-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="22c47-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-140">description</span><span class="sxs-lookup"><span data-stu-id="22c47-140">description</span></span>|<span data-ttu-id="22c47-141">String</span><span class="sxs-lookup"><span data-stu-id="22c47-141">String</span></span>|<span data-ttu-id="22c47-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="22c47-142">The description of the app.</span></span> <span data-ttu-id="22c47-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-144">publisher</span><span class="sxs-lookup"><span data-stu-id="22c47-144">publisher</span></span>|<span data-ttu-id="22c47-145">String</span><span class="sxs-lookup"><span data-stu-id="22c47-145">String</span></span>|<span data-ttu-id="22c47-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="22c47-146">The publisher of the app.</span></span> <span data-ttu-id="22c47-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22c47-148">largeIcon</span></span>|[<span data-ttu-id="22c47-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22c47-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="22c47-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="22c47-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="22c47-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22c47-152">createdDateTime</span></span>|<span data-ttu-id="22c47-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c47-153">DateTimeOffset</span></span>|<span data-ttu-id="22c47-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="22c47-154">The date and time the app was created.</span></span> <span data-ttu-id="22c47-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22c47-156">lastModifiedDateTime</span></span>|<span data-ttu-id="22c47-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c47-157">DateTimeOffset</span></span>|<span data-ttu-id="22c47-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="22c47-158">The date and time the app was last modified.</span></span> <span data-ttu-id="22c47-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22c47-160">isFeatured</span></span>|<span data-ttu-id="22c47-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="22c47-161">Boolean</span></span>|<span data-ttu-id="22c47-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22c47-163">privacyInformationUrl</span></span>|<span data-ttu-id="22c47-164">String</span><span class="sxs-lookup"><span data-stu-id="22c47-164">String</span></span>|<span data-ttu-id="22c47-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="22c47-165">The privacy statement Url.</span></span> <span data-ttu-id="22c47-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22c47-167">informationUrl</span></span>|<span data-ttu-id="22c47-168">String</span><span class="sxs-lookup"><span data-stu-id="22c47-168">String</span></span>|<span data-ttu-id="22c47-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="22c47-169">The more information Url.</span></span> <span data-ttu-id="22c47-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-171">owner</span><span class="sxs-lookup"><span data-stu-id="22c47-171">owner</span></span>|<span data-ttu-id="22c47-172">String</span><span class="sxs-lookup"><span data-stu-id="22c47-172">String</span></span>|<span data-ttu-id="22c47-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="22c47-173">The owner of the app.</span></span> <span data-ttu-id="22c47-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-175">developer</span><span class="sxs-lookup"><span data-stu-id="22c47-175">developer</span></span>|<span data-ttu-id="22c47-176">String</span><span class="sxs-lookup"><span data-stu-id="22c47-176">String</span></span>|<span data-ttu-id="22c47-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="22c47-177">The developer of the app.</span></span> <span data-ttu-id="22c47-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-179">notes</span><span class="sxs-lookup"><span data-stu-id="22c47-179">notes</span></span>|<span data-ttu-id="22c47-180">String</span><span class="sxs-lookup"><span data-stu-id="22c47-180">String</span></span>|<span data-ttu-id="22c47-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="22c47-181">Notes for the app.</span></span> <span data-ttu-id="22c47-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="22c47-183">uploadState</span></span>|<span data-ttu-id="22c47-184">Int32</span><span class="sxs-lookup"><span data-stu-id="22c47-184">Int32</span></span>|<span data-ttu-id="22c47-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="22c47-185">The upload state.</span></span> <span data-ttu-id="22c47-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="22c47-187">publishingState</span></span>|[<span data-ttu-id="22c47-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="22c47-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="22c47-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="22c47-189">The publishing state for the app.</span></span> <span data-ttu-id="22c47-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="22c47-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22c47-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="22c47-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="22c47-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="22c47-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="22c47-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="22c47-193">isAssigned</span></span>|<span data-ttu-id="22c47-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="22c47-194">Boolean</span></span>|<span data-ttu-id="22c47-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="22c47-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="22c47-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22c47-197">roleScopeTagIds</span></span>|<span data-ttu-id="22c47-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="22c47-198">String collection</span></span>|<span data-ttu-id="22c47-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="22c47-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="22c47-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="22c47-201">dependentAppCount</span></span>|<span data-ttu-id="22c47-202">Int32</span><span class="sxs-lookup"><span data-stu-id="22c47-202">Int32</span></span>|<span data-ttu-id="22c47-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="22c47-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="22c47-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="22c47-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="22c47-205">appAvailability</span></span>|[<span data-ttu-id="22c47-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="22c47-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="22c47-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="22c47-207">The Application's availability.</span></span> <span data-ttu-id="22c47-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="22c47-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="22c47-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="22c47-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="22c47-210">version</span><span class="sxs-lookup"><span data-stu-id="22c47-210">version</span></span>|<span data-ttu-id="22c47-211">String</span><span class="sxs-lookup"><span data-stu-id="22c47-211">String</span></span>|<span data-ttu-id="22c47-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="22c47-212">The Application's version.</span></span> <span data-ttu-id="22c47-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="22c47-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="22c47-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="22c47-214">bundleId</span></span>|<span data-ttu-id="22c47-215">String</span><span class="sxs-lookup"><span data-stu-id="22c47-215">String</span></span>|<span data-ttu-id="22c47-216">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="22c47-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="22c47-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="22c47-217">appStoreUrl</span></span>|<span data-ttu-id="22c47-218">String</span><span class="sxs-lookup"><span data-stu-id="22c47-218">String</span></span>|<span data-ttu-id="22c47-219">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="22c47-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="22c47-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="22c47-220">applicableDeviceType</span></span>|[<span data-ttu-id="22c47-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="22c47-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="22c47-222">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="22c47-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="22c47-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22c47-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="22c47-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22c47-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="22c47-225">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="22c47-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="22c47-226">応答</span><span class="sxs-lookup"><span data-stu-id="22c47-226">Response</span></span>
<span data-ttu-id="22c47-227">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="22c47-227">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22c47-228">例</span><span class="sxs-lookup"><span data-stu-id="22c47-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="22c47-229">要求</span><span class="sxs-lookup"><span data-stu-id="22c47-229">Request</span></span>
<span data-ttu-id="22c47-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22c47-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1218

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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

### <a name="response"></a><span data-ttu-id="22c47-231">応答</span><span class="sxs-lookup"><span data-stu-id="22c47-231">Response</span></span>
<span data-ttu-id="22c47-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22c47-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1390

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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






