---
title: managedAndroidLobApp の更新
description: managedAndroidLobApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3eb0ae249a08e6326be46f5258090fef1fb4c28
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935756"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="dd878-103">managedAndroidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="dd878-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="dd878-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd878-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd878-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd878-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd878-106">[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dd878-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd878-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dd878-107">Prerequisites</span></span>
<span data-ttu-id="dd878-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd878-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd878-110">Permission type</span></span>|<span data-ttu-id="dd878-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd878-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd878-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd878-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd878-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd878-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd878-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd878-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd878-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd878-115">Not supported.</span></span>|
|<span data-ttu-id="dd878-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd878-116">Application</span></span>|<span data-ttu-id="dd878-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd878-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd878-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd878-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dd878-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd878-119">Request headers</span></span>
|<span data-ttu-id="dd878-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd878-120">Header</span></span>|<span data-ttu-id="dd878-121">値</span><span class="sxs-lookup"><span data-stu-id="dd878-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd878-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd878-122">Authorization</span></span>|<span data-ttu-id="dd878-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd878-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd878-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dd878-124">Accept</span></span>|<span data-ttu-id="dd878-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd878-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd878-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd878-126">Request body</span></span>
<span data-ttu-id="dd878-127">要求本文で、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dd878-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="dd878-128">次の表に、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dd878-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="dd878-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd878-129">Property</span></span>|<span data-ttu-id="dd878-130">型</span><span class="sxs-lookup"><span data-stu-id="dd878-130">Type</span></span>|<span data-ttu-id="dd878-131">説明</span><span class="sxs-lookup"><span data-stu-id="dd878-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd878-132">id</span><span class="sxs-lookup"><span data-stu-id="dd878-132">id</span></span>|<span data-ttu-id="dd878-133">文字列</span><span class="sxs-lookup"><span data-stu-id="dd878-133">String</span></span>|<span data-ttu-id="dd878-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dd878-134">Key of the entity.</span></span> <span data-ttu-id="dd878-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dd878-136">displayName</span></span>|<span data-ttu-id="dd878-137">文字列</span><span class="sxs-lookup"><span data-stu-id="dd878-137">String</span></span>|<span data-ttu-id="dd878-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="dd878-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dd878-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-140">description</span><span class="sxs-lookup"><span data-stu-id="dd878-140">description</span></span>|<span data-ttu-id="dd878-141">String</span><span class="sxs-lookup"><span data-stu-id="dd878-141">String</span></span>|<span data-ttu-id="dd878-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="dd878-142">The description of the app.</span></span> <span data-ttu-id="dd878-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dd878-144">publisher</span></span>|<span data-ttu-id="dd878-145">String</span><span class="sxs-lookup"><span data-stu-id="dd878-145">String</span></span>|<span data-ttu-id="dd878-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="dd878-146">The publisher of the app.</span></span> <span data-ttu-id="dd878-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dd878-148">largeIcon</span></span>|[<span data-ttu-id="dd878-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dd878-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dd878-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="dd878-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dd878-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd878-152">createdDateTime</span></span>|<span data-ttu-id="dd878-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd878-153">DateTimeOffset</span></span>|<span data-ttu-id="dd878-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="dd878-154">The date and time the app was created.</span></span> <span data-ttu-id="dd878-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd878-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dd878-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd878-157">DateTimeOffset</span></span>|<span data-ttu-id="dd878-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="dd878-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dd878-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dd878-160">isFeatured</span></span>|<span data-ttu-id="dd878-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd878-161">Boolean</span></span>|<span data-ttu-id="dd878-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dd878-163">privacyInformationUrl</span></span>|<span data-ttu-id="dd878-164">String</span><span class="sxs-lookup"><span data-stu-id="dd878-164">String</span></span>|<span data-ttu-id="dd878-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="dd878-165">The privacy statement Url.</span></span> <span data-ttu-id="dd878-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dd878-167">informationUrl</span></span>|<span data-ttu-id="dd878-168">String</span><span class="sxs-lookup"><span data-stu-id="dd878-168">String</span></span>|<span data-ttu-id="dd878-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="dd878-169">The more information Url.</span></span> <span data-ttu-id="dd878-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-171">owner</span><span class="sxs-lookup"><span data-stu-id="dd878-171">owner</span></span>|<span data-ttu-id="dd878-172">String</span><span class="sxs-lookup"><span data-stu-id="dd878-172">String</span></span>|<span data-ttu-id="dd878-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="dd878-173">The owner of the app.</span></span> <span data-ttu-id="dd878-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-175">developer</span><span class="sxs-lookup"><span data-stu-id="dd878-175">developer</span></span>|<span data-ttu-id="dd878-176">String</span><span class="sxs-lookup"><span data-stu-id="dd878-176">String</span></span>|<span data-ttu-id="dd878-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="dd878-177">The developer of the app.</span></span> <span data-ttu-id="dd878-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-179">notes</span><span class="sxs-lookup"><span data-stu-id="dd878-179">notes</span></span>|<span data-ttu-id="dd878-180">String</span><span class="sxs-lookup"><span data-stu-id="dd878-180">String</span></span>|<span data-ttu-id="dd878-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="dd878-181">Notes for the app.</span></span> <span data-ttu-id="dd878-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="dd878-183">uploadState</span></span>|<span data-ttu-id="dd878-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dd878-184">Int32</span></span>|<span data-ttu-id="dd878-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="dd878-185">The upload state.</span></span> <span data-ttu-id="dd878-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="dd878-187">publishingState</span></span>|[<span data-ttu-id="dd878-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dd878-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dd878-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="dd878-189">The publishing state for the app.</span></span> <span data-ttu-id="dd878-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="dd878-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dd878-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="dd878-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dd878-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="dd878-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dd878-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dd878-193">isAssigned</span></span>|<span data-ttu-id="dd878-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd878-194">Boolean</span></span>|<span data-ttu-id="dd878-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="dd878-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dd878-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd878-197">roleScopeTagIds</span></span>|<span data-ttu-id="dd878-198">String collection</span><span class="sxs-lookup"><span data-stu-id="dd878-198">String collection</span></span>|<span data-ttu-id="dd878-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="dd878-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dd878-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="dd878-201">dependentAppCount</span></span>|<span data-ttu-id="dd878-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dd878-202">Int32</span></span>|<span data-ttu-id="dd878-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="dd878-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dd878-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd878-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="dd878-205">appAvailability</span></span>|[<span data-ttu-id="dd878-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="dd878-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="dd878-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="dd878-207">The Application's availability.</span></span> <span data-ttu-id="dd878-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="dd878-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="dd878-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="dd878-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="dd878-210">version</span><span class="sxs-lookup"><span data-stu-id="dd878-210">version</span></span>|<span data-ttu-id="dd878-211">String</span><span class="sxs-lookup"><span data-stu-id="dd878-211">String</span></span>|<span data-ttu-id="dd878-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="dd878-212">The Application's version.</span></span> <span data-ttu-id="dd878-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="dd878-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dd878-214">committedContentVersion</span></span>|<span data-ttu-id="dd878-215">String</span><span class="sxs-lookup"><span data-stu-id="dd878-215">String</span></span>|<span data-ttu-id="dd878-216">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="dd878-216">The internal committed content version.</span></span> <span data-ttu-id="dd878-217">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd878-218">fileName</span><span class="sxs-lookup"><span data-stu-id="dd878-218">fileName</span></span>|<span data-ttu-id="dd878-219">String</span><span class="sxs-lookup"><span data-stu-id="dd878-219">String</span></span>|<span data-ttu-id="dd878-220">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="dd878-220">The name of the main Lob application file.</span></span> <span data-ttu-id="dd878-221">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd878-222">size</span><span class="sxs-lookup"><span data-stu-id="dd878-222">size</span></span>|<span data-ttu-id="dd878-223">Int64</span><span class="sxs-lookup"><span data-stu-id="dd878-223">Int64</span></span>|<span data-ttu-id="dd878-224">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="dd878-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="dd878-225">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd878-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd878-226">packageId</span><span class="sxs-lookup"><span data-stu-id="dd878-226">packageId</span></span>|<span data-ttu-id="dd878-227">String</span><span class="sxs-lookup"><span data-stu-id="dd878-227">String</span></span>|<span data-ttu-id="dd878-228">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="dd878-228">The package identifier.</span></span>|
|<span data-ttu-id="dd878-229">identityName</span><span class="sxs-lookup"><span data-stu-id="dd878-229">identityName</span></span>|<span data-ttu-id="dd878-230">String</span><span class="sxs-lookup"><span data-stu-id="dd878-230">String</span></span>|<span data-ttu-id="dd878-231">ID 名。</span><span class="sxs-lookup"><span data-stu-id="dd878-231">The Identity Name.</span></span>|
|<span data-ttu-id="dd878-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd878-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dd878-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd878-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="dd878-234">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="dd878-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dd878-235">versionName</span><span class="sxs-lookup"><span data-stu-id="dd878-235">versionName</span></span>|<span data-ttu-id="dd878-236">String</span><span class="sxs-lookup"><span data-stu-id="dd878-236">String</span></span>|<span data-ttu-id="dd878-237">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="dd878-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd878-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="dd878-238">versionCode</span></span>|<span data-ttu-id="dd878-239">String</span><span class="sxs-lookup"><span data-stu-id="dd878-239">String</span></span>|<span data-ttu-id="dd878-240">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="dd878-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd878-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dd878-241">identityVersion</span></span>|<span data-ttu-id="dd878-242">String</span><span class="sxs-lookup"><span data-stu-id="dd878-242">String</span></span>|<span data-ttu-id="dd878-243">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dd878-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="dd878-244">応答</span><span class="sxs-lookup"><span data-stu-id="dd878-244">Response</span></span>
<span data-ttu-id="dd878-245">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="dd878-245">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd878-246">例</span><span class="sxs-lookup"><span data-stu-id="dd878-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd878-247">要求</span><span class="sxs-lookup"><span data-stu-id="dd878-247">Request</span></span>
<span data-ttu-id="dd878-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dd878-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="dd878-249">応答</span><span class="sxs-lookup"><span data-stu-id="dd878-249">Response</span></span>
<span data-ttu-id="dd878-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dd878-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




