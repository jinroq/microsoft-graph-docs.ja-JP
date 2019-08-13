---
title: managedIOSStoreApp の作成
description: 新しい managedIOSStoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 749200c1c9d6e87eb65d34f264d862baab35ef34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329564"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="30358-103">managedIOSStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="30358-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="30358-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30358-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30358-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="30358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30358-106">新しい [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="30358-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30358-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="30358-107">Prerequisites</span></span>
<span data-ttu-id="30358-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30358-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30358-110">Permission type</span></span>|<span data-ttu-id="30358-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="30358-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30358-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30358-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30358-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30358-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30358-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30358-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30358-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30358-115">Not supported.</span></span>|
|<span data-ttu-id="30358-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30358-116">Application</span></span>|<span data-ttu-id="30358-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30358-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30358-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30358-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="30358-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30358-119">Request headers</span></span>
|<span data-ttu-id="30358-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30358-120">Header</span></span>|<span data-ttu-id="30358-121">値</span><span class="sxs-lookup"><span data-stu-id="30358-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30358-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30358-122">Authorization</span></span>|<span data-ttu-id="30358-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="30358-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30358-124">承諾</span><span class="sxs-lookup"><span data-stu-id="30358-124">Accept</span></span>|<span data-ttu-id="30358-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30358-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30358-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="30358-126">Request body</span></span>
<span data-ttu-id="30358-127">要求本文で、managedIOSStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="30358-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="30358-128">次の表に、managedIOSStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="30358-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="30358-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30358-129">Property</span></span>|<span data-ttu-id="30358-130">型</span><span class="sxs-lookup"><span data-stu-id="30358-130">Type</span></span>|<span data-ttu-id="30358-131">説明</span><span class="sxs-lookup"><span data-stu-id="30358-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30358-132">id</span><span class="sxs-lookup"><span data-stu-id="30358-132">id</span></span>|<span data-ttu-id="30358-133">文字列</span><span class="sxs-lookup"><span data-stu-id="30358-133">String</span></span>|<span data-ttu-id="30358-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="30358-134">Key of the entity.</span></span> <span data-ttu-id="30358-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-136">displayName</span><span class="sxs-lookup"><span data-stu-id="30358-136">displayName</span></span>|<span data-ttu-id="30358-137">文字列</span><span class="sxs-lookup"><span data-stu-id="30358-137">String</span></span>|<span data-ttu-id="30358-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="30358-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30358-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-140">description</span><span class="sxs-lookup"><span data-stu-id="30358-140">description</span></span>|<span data-ttu-id="30358-141">String</span><span class="sxs-lookup"><span data-stu-id="30358-141">String</span></span>|<span data-ttu-id="30358-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="30358-142">The description of the app.</span></span> <span data-ttu-id="30358-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-144">publisher</span><span class="sxs-lookup"><span data-stu-id="30358-144">publisher</span></span>|<span data-ttu-id="30358-145">String</span><span class="sxs-lookup"><span data-stu-id="30358-145">String</span></span>|<span data-ttu-id="30358-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="30358-146">The publisher of the app.</span></span> <span data-ttu-id="30358-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30358-148">largeIcon</span></span>|[<span data-ttu-id="30358-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30358-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30358-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="30358-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30358-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30358-152">createdDateTime</span></span>|<span data-ttu-id="30358-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30358-153">DateTimeOffset</span></span>|<span data-ttu-id="30358-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="30358-154">The date and time the app was created.</span></span> <span data-ttu-id="30358-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30358-156">lastModifiedDateTime</span></span>|<span data-ttu-id="30358-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30358-157">DateTimeOffset</span></span>|<span data-ttu-id="30358-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="30358-158">The date and time the app was last modified.</span></span> <span data-ttu-id="30358-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30358-160">isFeatured</span></span>|<span data-ttu-id="30358-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="30358-161">Boolean</span></span>|<span data-ttu-id="30358-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30358-163">privacyInformationUrl</span></span>|<span data-ttu-id="30358-164">String</span><span class="sxs-lookup"><span data-stu-id="30358-164">String</span></span>|<span data-ttu-id="30358-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="30358-165">The privacy statement Url.</span></span> <span data-ttu-id="30358-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30358-167">informationUrl</span></span>|<span data-ttu-id="30358-168">String</span><span class="sxs-lookup"><span data-stu-id="30358-168">String</span></span>|<span data-ttu-id="30358-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="30358-169">The more information Url.</span></span> <span data-ttu-id="30358-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-171">owner</span><span class="sxs-lookup"><span data-stu-id="30358-171">owner</span></span>|<span data-ttu-id="30358-172">String</span><span class="sxs-lookup"><span data-stu-id="30358-172">String</span></span>|<span data-ttu-id="30358-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="30358-173">The owner of the app.</span></span> <span data-ttu-id="30358-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-175">developer</span><span class="sxs-lookup"><span data-stu-id="30358-175">developer</span></span>|<span data-ttu-id="30358-176">String</span><span class="sxs-lookup"><span data-stu-id="30358-176">String</span></span>|<span data-ttu-id="30358-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="30358-177">The developer of the app.</span></span> <span data-ttu-id="30358-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-179">notes</span><span class="sxs-lookup"><span data-stu-id="30358-179">notes</span></span>|<span data-ttu-id="30358-180">String</span><span class="sxs-lookup"><span data-stu-id="30358-180">String</span></span>|<span data-ttu-id="30358-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="30358-181">Notes for the app.</span></span> <span data-ttu-id="30358-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="30358-183">uploadState</span></span>|<span data-ttu-id="30358-184">Int32</span><span class="sxs-lookup"><span data-stu-id="30358-184">Int32</span></span>|<span data-ttu-id="30358-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="30358-185">The upload state.</span></span> <span data-ttu-id="30358-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="30358-187">publishingState</span></span>|[<span data-ttu-id="30358-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="30358-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30358-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="30358-189">The publishing state for the app.</span></span> <span data-ttu-id="30358-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="30358-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30358-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="30358-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="30358-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="30358-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30358-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30358-193">isAssigned</span></span>|<span data-ttu-id="30358-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="30358-194">Boolean</span></span>|<span data-ttu-id="30358-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="30358-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30358-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30358-197">roleScopeTagIds</span></span>|<span data-ttu-id="30358-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="30358-198">String collection</span></span>|<span data-ttu-id="30358-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="30358-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30358-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="30358-201">dependentAppCount</span></span>|<span data-ttu-id="30358-202">Int32</span><span class="sxs-lookup"><span data-stu-id="30358-202">Int32</span></span>|<span data-ttu-id="30358-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="30358-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30358-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30358-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="30358-205">appAvailability</span></span>|[<span data-ttu-id="30358-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="30358-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="30358-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="30358-207">The Application's availability.</span></span> <span data-ttu-id="30358-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="30358-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="30358-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="30358-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="30358-210">version</span><span class="sxs-lookup"><span data-stu-id="30358-210">version</span></span>|<span data-ttu-id="30358-211">String</span><span class="sxs-lookup"><span data-stu-id="30358-211">String</span></span>|<span data-ttu-id="30358-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="30358-212">The Application's version.</span></span> <span data-ttu-id="30358-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="30358-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="30358-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="30358-214">bundleId</span></span>|<span data-ttu-id="30358-215">String</span><span class="sxs-lookup"><span data-stu-id="30358-215">String</span></span>|<span data-ttu-id="30358-216">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="30358-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="30358-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="30358-217">appStoreUrl</span></span>|<span data-ttu-id="30358-218">String</span><span class="sxs-lookup"><span data-stu-id="30358-218">String</span></span>|<span data-ttu-id="30358-219">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="30358-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="30358-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="30358-220">applicableDeviceType</span></span>|[<span data-ttu-id="30358-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="30358-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="30358-222">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="30358-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="30358-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30358-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="30358-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30358-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="30358-225">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="30358-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="30358-226">応答</span><span class="sxs-lookup"><span data-stu-id="30358-226">Response</span></span>
<span data-ttu-id="30358-227">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="30358-227">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30358-228">例</span><span class="sxs-lookup"><span data-stu-id="30358-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="30358-229">要求</span><span class="sxs-lookup"><span data-stu-id="30358-229">Request</span></span>
<span data-ttu-id="30358-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30358-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="30358-231">応答</span><span class="sxs-lookup"><span data-stu-id="30358-231">Response</span></span>
<span data-ttu-id="30358-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30358-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






