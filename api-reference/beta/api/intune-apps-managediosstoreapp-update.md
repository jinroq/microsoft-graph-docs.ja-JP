---
title: managedIOSStoreApp の更新
description: managedIOSStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83f706bbcd82dbe528076bcfc9884a5697473e49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961288"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="180c3-103">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="180c3-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="180c3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="180c3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="180c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="180c3-106">[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="180c3-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="180c3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="180c3-107">Prerequisites</span></span>
<span data-ttu-id="180c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="180c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="180c3-110">Permission type</span></span>|<span data-ttu-id="180c3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="180c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="180c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="180c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="180c3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180c3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="180c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="180c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="180c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180c3-115">Not supported.</span></span>|
|<span data-ttu-id="180c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="180c3-116">Application</span></span>|<span data-ttu-id="180c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="180c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="180c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="180c3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="180c3-119">Request headers</span></span>
|<span data-ttu-id="180c3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="180c3-120">Header</span></span>|<span data-ttu-id="180c3-121">値</span><span class="sxs-lookup"><span data-stu-id="180c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="180c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="180c3-122">Authorization</span></span>|<span data-ttu-id="180c3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="180c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="180c3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="180c3-124">Accept</span></span>|<span data-ttu-id="180c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="180c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="180c3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="180c3-126">Request body</span></span>
<span data-ttu-id="180c3-127">要求本文で、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="180c3-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="180c3-128">次の表に、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="180c3-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="180c3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="180c3-129">Property</span></span>|<span data-ttu-id="180c3-130">型</span><span class="sxs-lookup"><span data-stu-id="180c3-130">Type</span></span>|<span data-ttu-id="180c3-131">説明</span><span class="sxs-lookup"><span data-stu-id="180c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180c3-132">id</span><span class="sxs-lookup"><span data-stu-id="180c3-132">id</span></span>|<span data-ttu-id="180c3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="180c3-133">String</span></span>|<span data-ttu-id="180c3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="180c3-134">Key of the entity.</span></span> <span data-ttu-id="180c3-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="180c3-136">displayName</span></span>|<span data-ttu-id="180c3-137">文字列</span><span class="sxs-lookup"><span data-stu-id="180c3-137">String</span></span>|<span data-ttu-id="180c3-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="180c3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="180c3-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-140">description</span><span class="sxs-lookup"><span data-stu-id="180c3-140">description</span></span>|<span data-ttu-id="180c3-141">String</span><span class="sxs-lookup"><span data-stu-id="180c3-141">String</span></span>|<span data-ttu-id="180c3-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="180c3-142">The description of the app.</span></span> <span data-ttu-id="180c3-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-144">publisher</span><span class="sxs-lookup"><span data-stu-id="180c3-144">publisher</span></span>|<span data-ttu-id="180c3-145">String</span><span class="sxs-lookup"><span data-stu-id="180c3-145">String</span></span>|<span data-ttu-id="180c3-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="180c3-146">The publisher of the app.</span></span> <span data-ttu-id="180c3-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="180c3-148">largeIcon</span></span>|[<span data-ttu-id="180c3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="180c3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="180c3-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="180c3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="180c3-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="180c3-152">createdDateTime</span></span>|<span data-ttu-id="180c3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180c3-153">DateTimeOffset</span></span>|<span data-ttu-id="180c3-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="180c3-154">The date and time the app was created.</span></span> <span data-ttu-id="180c3-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="180c3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="180c3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180c3-157">DateTimeOffset</span></span>|<span data-ttu-id="180c3-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="180c3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="180c3-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="180c3-160">isFeatured</span></span>|<span data-ttu-id="180c3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="180c3-161">Boolean</span></span>|<span data-ttu-id="180c3-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="180c3-163">privacyInformationUrl</span></span>|<span data-ttu-id="180c3-164">String</span><span class="sxs-lookup"><span data-stu-id="180c3-164">String</span></span>|<span data-ttu-id="180c3-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="180c3-165">The privacy statement Url.</span></span> <span data-ttu-id="180c3-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="180c3-167">informationUrl</span></span>|<span data-ttu-id="180c3-168">String</span><span class="sxs-lookup"><span data-stu-id="180c3-168">String</span></span>|<span data-ttu-id="180c3-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="180c3-169">The more information Url.</span></span> <span data-ttu-id="180c3-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-171">owner</span><span class="sxs-lookup"><span data-stu-id="180c3-171">owner</span></span>|<span data-ttu-id="180c3-172">String</span><span class="sxs-lookup"><span data-stu-id="180c3-172">String</span></span>|<span data-ttu-id="180c3-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="180c3-173">The owner of the app.</span></span> <span data-ttu-id="180c3-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-175">developer</span><span class="sxs-lookup"><span data-stu-id="180c3-175">developer</span></span>|<span data-ttu-id="180c3-176">String</span><span class="sxs-lookup"><span data-stu-id="180c3-176">String</span></span>|<span data-ttu-id="180c3-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="180c3-177">The developer of the app.</span></span> <span data-ttu-id="180c3-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-179">notes</span><span class="sxs-lookup"><span data-stu-id="180c3-179">notes</span></span>|<span data-ttu-id="180c3-180">String</span><span class="sxs-lookup"><span data-stu-id="180c3-180">String</span></span>|<span data-ttu-id="180c3-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="180c3-181">Notes for the app.</span></span> <span data-ttu-id="180c3-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="180c3-183">uploadState</span></span>|<span data-ttu-id="180c3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="180c3-184">Int32</span></span>|<span data-ttu-id="180c3-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="180c3-185">The upload state.</span></span> <span data-ttu-id="180c3-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="180c3-187">publishingState</span></span>|[<span data-ttu-id="180c3-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="180c3-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="180c3-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="180c3-189">The publishing state for the app.</span></span> <span data-ttu-id="180c3-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="180c3-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="180c3-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="180c3-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="180c3-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="180c3-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="180c3-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="180c3-193">isAssigned</span></span>|<span data-ttu-id="180c3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="180c3-194">Boolean</span></span>|<span data-ttu-id="180c3-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="180c3-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="180c3-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="180c3-197">roleScopeTagIds</span></span>|<span data-ttu-id="180c3-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="180c3-198">String collection</span></span>|<span data-ttu-id="180c3-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="180c3-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="180c3-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="180c3-201">dependentAppCount</span></span>|<span data-ttu-id="180c3-202">Int32</span><span class="sxs-lookup"><span data-stu-id="180c3-202">Int32</span></span>|<span data-ttu-id="180c3-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="180c3-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="180c3-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="180c3-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="180c3-205">appAvailability</span></span>|[<span data-ttu-id="180c3-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="180c3-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="180c3-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="180c3-207">The Application's availability.</span></span> <span data-ttu-id="180c3-208">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="180c3-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="180c3-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="180c3-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="180c3-210">version</span><span class="sxs-lookup"><span data-stu-id="180c3-210">version</span></span>|<span data-ttu-id="180c3-211">String</span><span class="sxs-lookup"><span data-stu-id="180c3-211">String</span></span>|<span data-ttu-id="180c3-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="180c3-212">The Application's version.</span></span> <span data-ttu-id="180c3-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="180c3-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="180c3-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="180c3-214">bundleId</span></span>|<span data-ttu-id="180c3-215">String</span><span class="sxs-lookup"><span data-stu-id="180c3-215">String</span></span>|<span data-ttu-id="180c3-216">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="180c3-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="180c3-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="180c3-217">appStoreUrl</span></span>|<span data-ttu-id="180c3-218">String</span><span class="sxs-lookup"><span data-stu-id="180c3-218">String</span></span>|<span data-ttu-id="180c3-219">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="180c3-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="180c3-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="180c3-220">applicableDeviceType</span></span>|[<span data-ttu-id="180c3-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="180c3-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="180c3-222">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="180c3-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="180c3-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="180c3-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="180c3-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="180c3-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="180c3-225">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="180c3-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="180c3-226">応答</span><span class="sxs-lookup"><span data-stu-id="180c3-226">Response</span></span>
<span data-ttu-id="180c3-227">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="180c3-227">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="180c3-228">例</span><span class="sxs-lookup"><span data-stu-id="180c3-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="180c3-229">要求</span><span class="sxs-lookup"><span data-stu-id="180c3-229">Request</span></span>
<span data-ttu-id="180c3-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="180c3-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="180c3-231">応答</span><span class="sxs-lookup"><span data-stu-id="180c3-231">Response</span></span>
<span data-ttu-id="180c3-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="180c3-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





