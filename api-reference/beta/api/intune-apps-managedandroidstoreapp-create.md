---
title: managedAndroidStoreApp の作成
description: 新しい managedAndroidStoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f70421792c76b9cbfdd08caf74a5cc63016c1949
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961820"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="93861-103">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="93861-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="93861-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93861-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="93861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93861-106">新しい [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="93861-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93861-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="93861-107">Prerequisites</span></span>
<span data-ttu-id="93861-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93861-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93861-110">Permission type</span></span>|<span data-ttu-id="93861-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="93861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93861-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93861-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93861-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93861-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93861-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93861-115">Not supported.</span></span>|
|<span data-ttu-id="93861-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93861-116">Application</span></span>|<span data-ttu-id="93861-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93861-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93861-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="93861-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93861-119">Request headers</span></span>
|<span data-ttu-id="93861-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93861-120">Header</span></span>|<span data-ttu-id="93861-121">値</span><span class="sxs-lookup"><span data-stu-id="93861-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93861-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93861-122">Authorization</span></span>|<span data-ttu-id="93861-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="93861-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93861-124">承諾</span><span class="sxs-lookup"><span data-stu-id="93861-124">Accept</span></span>|<span data-ttu-id="93861-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93861-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93861-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="93861-126">Request body</span></span>
<span data-ttu-id="93861-127">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="93861-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="93861-128">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="93861-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="93861-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93861-129">Property</span></span>|<span data-ttu-id="93861-130">型</span><span class="sxs-lookup"><span data-stu-id="93861-130">Type</span></span>|<span data-ttu-id="93861-131">説明</span><span class="sxs-lookup"><span data-stu-id="93861-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93861-132">id</span><span class="sxs-lookup"><span data-stu-id="93861-132">id</span></span>|<span data-ttu-id="93861-133">文字列</span><span class="sxs-lookup"><span data-stu-id="93861-133">String</span></span>|<span data-ttu-id="93861-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="93861-134">Key of the entity.</span></span> <span data-ttu-id="93861-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93861-136">displayName</span></span>|<span data-ttu-id="93861-137">文字列</span><span class="sxs-lookup"><span data-stu-id="93861-137">String</span></span>|<span data-ttu-id="93861-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="93861-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="93861-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-140">description</span><span class="sxs-lookup"><span data-stu-id="93861-140">description</span></span>|<span data-ttu-id="93861-141">String</span><span class="sxs-lookup"><span data-stu-id="93861-141">String</span></span>|<span data-ttu-id="93861-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="93861-142">The description of the app.</span></span> <span data-ttu-id="93861-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-144">publisher</span><span class="sxs-lookup"><span data-stu-id="93861-144">publisher</span></span>|<span data-ttu-id="93861-145">String</span><span class="sxs-lookup"><span data-stu-id="93861-145">String</span></span>|<span data-ttu-id="93861-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="93861-146">The publisher of the app.</span></span> <span data-ttu-id="93861-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="93861-148">largeIcon</span></span>|[<span data-ttu-id="93861-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93861-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="93861-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="93861-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="93861-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93861-152">createdDateTime</span></span>|<span data-ttu-id="93861-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93861-153">DateTimeOffset</span></span>|<span data-ttu-id="93861-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="93861-154">The date and time the app was created.</span></span> <span data-ttu-id="93861-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93861-156">lastModifiedDateTime</span></span>|<span data-ttu-id="93861-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93861-157">DateTimeOffset</span></span>|<span data-ttu-id="93861-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="93861-158">The date and time the app was last modified.</span></span> <span data-ttu-id="93861-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="93861-160">isFeatured</span></span>|<span data-ttu-id="93861-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="93861-161">Boolean</span></span>|<span data-ttu-id="93861-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="93861-163">privacyInformationUrl</span></span>|<span data-ttu-id="93861-164">String</span><span class="sxs-lookup"><span data-stu-id="93861-164">String</span></span>|<span data-ttu-id="93861-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="93861-165">The privacy statement Url.</span></span> <span data-ttu-id="93861-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="93861-167">informationUrl</span></span>|<span data-ttu-id="93861-168">String</span><span class="sxs-lookup"><span data-stu-id="93861-168">String</span></span>|<span data-ttu-id="93861-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="93861-169">The more information Url.</span></span> <span data-ttu-id="93861-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-171">owner</span><span class="sxs-lookup"><span data-stu-id="93861-171">owner</span></span>|<span data-ttu-id="93861-172">String</span><span class="sxs-lookup"><span data-stu-id="93861-172">String</span></span>|<span data-ttu-id="93861-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="93861-173">The owner of the app.</span></span> <span data-ttu-id="93861-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-175">developer</span><span class="sxs-lookup"><span data-stu-id="93861-175">developer</span></span>|<span data-ttu-id="93861-176">String</span><span class="sxs-lookup"><span data-stu-id="93861-176">String</span></span>|<span data-ttu-id="93861-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="93861-177">The developer of the app.</span></span> <span data-ttu-id="93861-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-179">notes</span><span class="sxs-lookup"><span data-stu-id="93861-179">notes</span></span>|<span data-ttu-id="93861-180">String</span><span class="sxs-lookup"><span data-stu-id="93861-180">String</span></span>|<span data-ttu-id="93861-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="93861-181">Notes for the app.</span></span> <span data-ttu-id="93861-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="93861-183">uploadState</span></span>|<span data-ttu-id="93861-184">Int32</span><span class="sxs-lookup"><span data-stu-id="93861-184">Int32</span></span>|<span data-ttu-id="93861-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="93861-185">The upload state.</span></span> <span data-ttu-id="93861-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="93861-187">publishingState</span></span>|[<span data-ttu-id="93861-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="93861-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="93861-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="93861-189">The publishing state for the app.</span></span> <span data-ttu-id="93861-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="93861-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="93861-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="93861-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="93861-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="93861-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="93861-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="93861-193">isAssigned</span></span>|<span data-ttu-id="93861-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="93861-194">Boolean</span></span>|<span data-ttu-id="93861-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="93861-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="93861-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93861-197">roleScopeTagIds</span></span>|<span data-ttu-id="93861-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="93861-198">String collection</span></span>|<span data-ttu-id="93861-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="93861-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="93861-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="93861-201">dependentAppCount</span></span>|<span data-ttu-id="93861-202">Int32</span><span class="sxs-lookup"><span data-stu-id="93861-202">Int32</span></span>|<span data-ttu-id="93861-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="93861-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="93861-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93861-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="93861-205">appAvailability</span></span>|[<span data-ttu-id="93861-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="93861-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="93861-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="93861-207">The Application's availability.</span></span> <span data-ttu-id="93861-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="93861-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="93861-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="93861-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="93861-210">version</span><span class="sxs-lookup"><span data-stu-id="93861-210">version</span></span>|<span data-ttu-id="93861-211">String</span><span class="sxs-lookup"><span data-stu-id="93861-211">String</span></span>|<span data-ttu-id="93861-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="93861-212">The Application's version.</span></span> <span data-ttu-id="93861-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="93861-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="93861-214">packageId</span><span class="sxs-lookup"><span data-stu-id="93861-214">packageId</span></span>|<span data-ttu-id="93861-215">String</span><span class="sxs-lookup"><span data-stu-id="93861-215">String</span></span>|<span data-ttu-id="93861-216">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="93861-216">The app's package ID.</span></span>|
|<span data-ttu-id="93861-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="93861-217">appStoreUrl</span></span>|<span data-ttu-id="93861-218">String</span><span class="sxs-lookup"><span data-stu-id="93861-218">String</span></span>|<span data-ttu-id="93861-219">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="93861-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="93861-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93861-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="93861-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93861-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="93861-222">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="93861-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="93861-223">応答</span><span class="sxs-lookup"><span data-stu-id="93861-223">Response</span></span>
<span data-ttu-id="93861-224">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="93861-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93861-225">例</span><span class="sxs-lookup"><span data-stu-id="93861-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="93861-226">要求</span><span class="sxs-lookup"><span data-stu-id="93861-226">Request</span></span>
<span data-ttu-id="93861-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="93861-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="93861-228">応答</span><span class="sxs-lookup"><span data-stu-id="93861-228">Response</span></span>
<span data-ttu-id="93861-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="93861-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





