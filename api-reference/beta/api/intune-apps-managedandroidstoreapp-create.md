---
title: managedAndroidStoreApp の作成
description: 新しい managedAndroidStoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 566ceaa4818f335b2f98ba0b3c86a5895f5d96df
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935763"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="8a26a-103">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="8a26a-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="8a26a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a26a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a26a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a26a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a26a-106">新しい [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8a26a-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a26a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a26a-107">Prerequisites</span></span>
<span data-ttu-id="8a26a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a26a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a26a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a26a-110">Permission type</span></span>|<span data-ttu-id="8a26a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a26a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a26a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a26a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a26a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a26a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a26a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a26a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a26a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a26a-115">Not supported.</span></span>|
|<span data-ttu-id="8a26a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a26a-116">Application</span></span>|<span data-ttu-id="8a26a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a26a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a26a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a26a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8a26a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a26a-119">Request headers</span></span>
|<span data-ttu-id="8a26a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a26a-120">Header</span></span>|<span data-ttu-id="8a26a-121">値</span><span class="sxs-lookup"><span data-stu-id="8a26a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a26a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a26a-122">Authorization</span></span>|<span data-ttu-id="8a26a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a26a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a26a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8a26a-124">Accept</span></span>|<span data-ttu-id="8a26a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a26a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a26a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a26a-126">Request body</span></span>
<span data-ttu-id="8a26a-127">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a26a-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="8a26a-128">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8a26a-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="8a26a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a26a-129">Property</span></span>|<span data-ttu-id="8a26a-130">型</span><span class="sxs-lookup"><span data-stu-id="8a26a-130">Type</span></span>|<span data-ttu-id="8a26a-131">説明</span><span class="sxs-lookup"><span data-stu-id="8a26a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a26a-132">id</span><span class="sxs-lookup"><span data-stu-id="8a26a-132">id</span></span>|<span data-ttu-id="8a26a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8a26a-133">String</span></span>|<span data-ttu-id="8a26a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8a26a-134">Key of the entity.</span></span> <span data-ttu-id="8a26a-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8a26a-136">displayName</span></span>|<span data-ttu-id="8a26a-137">文字列</span><span class="sxs-lookup"><span data-stu-id="8a26a-137">String</span></span>|<span data-ttu-id="8a26a-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="8a26a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8a26a-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-140">description</span><span class="sxs-lookup"><span data-stu-id="8a26a-140">description</span></span>|<span data-ttu-id="8a26a-141">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-141">String</span></span>|<span data-ttu-id="8a26a-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8a26a-142">The description of the app.</span></span> <span data-ttu-id="8a26a-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8a26a-144">publisher</span></span>|<span data-ttu-id="8a26a-145">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-145">String</span></span>|<span data-ttu-id="8a26a-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="8a26a-146">The publisher of the app.</span></span> <span data-ttu-id="8a26a-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8a26a-148">largeIcon</span></span>|[<span data-ttu-id="8a26a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a26a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a26a-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="8a26a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8a26a-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a26a-152">createdDateTime</span></span>|<span data-ttu-id="8a26a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a26a-153">DateTimeOffset</span></span>|<span data-ttu-id="8a26a-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8a26a-154">The date and time the app was created.</span></span> <span data-ttu-id="8a26a-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a26a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8a26a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a26a-157">DateTimeOffset</span></span>|<span data-ttu-id="8a26a-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8a26a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8a26a-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8a26a-160">isFeatured</span></span>|<span data-ttu-id="8a26a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a26a-161">Boolean</span></span>|<span data-ttu-id="8a26a-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8a26a-163">privacyInformationUrl</span></span>|<span data-ttu-id="8a26a-164">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-164">String</span></span>|<span data-ttu-id="8a26a-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="8a26a-165">The privacy statement Url.</span></span> <span data-ttu-id="8a26a-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8a26a-167">informationUrl</span></span>|<span data-ttu-id="8a26a-168">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-168">String</span></span>|<span data-ttu-id="8a26a-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="8a26a-169">The more information Url.</span></span> <span data-ttu-id="8a26a-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-171">owner</span><span class="sxs-lookup"><span data-stu-id="8a26a-171">owner</span></span>|<span data-ttu-id="8a26a-172">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-172">String</span></span>|<span data-ttu-id="8a26a-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="8a26a-173">The owner of the app.</span></span> <span data-ttu-id="8a26a-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-175">developer</span><span class="sxs-lookup"><span data-stu-id="8a26a-175">developer</span></span>|<span data-ttu-id="8a26a-176">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-176">String</span></span>|<span data-ttu-id="8a26a-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="8a26a-177">The developer of the app.</span></span> <span data-ttu-id="8a26a-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-179">notes</span><span class="sxs-lookup"><span data-stu-id="8a26a-179">notes</span></span>|<span data-ttu-id="8a26a-180">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-180">String</span></span>|<span data-ttu-id="8a26a-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="8a26a-181">Notes for the app.</span></span> <span data-ttu-id="8a26a-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8a26a-183">uploadState</span></span>|<span data-ttu-id="8a26a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8a26a-184">Int32</span></span>|<span data-ttu-id="8a26a-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="8a26a-185">The upload state.</span></span> <span data-ttu-id="8a26a-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8a26a-187">publishingState</span></span>|[<span data-ttu-id="8a26a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8a26a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8a26a-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="8a26a-189">The publishing state for the app.</span></span> <span data-ttu-id="8a26a-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="8a26a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8a26a-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8a26a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8a26a-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="8a26a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8a26a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8a26a-193">isAssigned</span></span>|<span data-ttu-id="8a26a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a26a-194">Boolean</span></span>|<span data-ttu-id="8a26a-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="8a26a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8a26a-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a26a-197">roleScopeTagIds</span></span>|<span data-ttu-id="8a26a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="8a26a-198">String collection</span></span>|<span data-ttu-id="8a26a-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="8a26a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8a26a-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8a26a-201">dependentAppCount</span></span>|<span data-ttu-id="8a26a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="8a26a-202">Int32</span></span>|<span data-ttu-id="8a26a-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="8a26a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8a26a-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8a26a-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8a26a-205">appAvailability</span></span>|[<span data-ttu-id="8a26a-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8a26a-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8a26a-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="8a26a-207">The Application's availability.</span></span> <span data-ttu-id="8a26a-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8a26a-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8a26a-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="8a26a-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8a26a-210">version</span><span class="sxs-lookup"><span data-stu-id="8a26a-210">version</span></span>|<span data-ttu-id="8a26a-211">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-211">String</span></span>|<span data-ttu-id="8a26a-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8a26a-212">The Application's version.</span></span> <span data-ttu-id="8a26a-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a26a-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8a26a-214">packageId</span><span class="sxs-lookup"><span data-stu-id="8a26a-214">packageId</span></span>|<span data-ttu-id="8a26a-215">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-215">String</span></span>|<span data-ttu-id="8a26a-216">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="8a26a-216">The app's package ID.</span></span>|
|<span data-ttu-id="8a26a-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8a26a-217">appStoreUrl</span></span>|<span data-ttu-id="8a26a-218">String</span><span class="sxs-lookup"><span data-stu-id="8a26a-218">String</span></span>|<span data-ttu-id="8a26a-219">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="8a26a-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="8a26a-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8a26a-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8a26a-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8a26a-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8a26a-222">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="8a26a-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8a26a-223">応答</span><span class="sxs-lookup"><span data-stu-id="8a26a-223">Response</span></span>
<span data-ttu-id="8a26a-224">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a26a-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a26a-225">例</span><span class="sxs-lookup"><span data-stu-id="8a26a-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a26a-226">要求</span><span class="sxs-lookup"><span data-stu-id="8a26a-226">Request</span></span>
<span data-ttu-id="8a26a-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a26a-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a26a-228">応答</span><span class="sxs-lookup"><span data-stu-id="8a26a-228">Response</span></span>
<span data-ttu-id="8a26a-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a26a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




