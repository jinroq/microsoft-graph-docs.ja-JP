---
title: androidStoreApp の更新
description: androidStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 580fc24bbc82a585430250d1b0e2125a01f106b6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937261"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="36c34-103">androidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="36c34-103">Update androidStoreApp</span></span>

> <span data-ttu-id="36c34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36c34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36c34-106">[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="36c34-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36c34-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="36c34-107">Prerequisites</span></span>
<span data-ttu-id="36c34-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36c34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c34-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36c34-110">Permission type</span></span>|<span data-ttu-id="36c34-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36c34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36c34-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36c34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36c34-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c34-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36c34-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36c34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36c34-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c34-115">Not supported.</span></span>|
|<span data-ttu-id="36c34-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36c34-116">Application</span></span>|<span data-ttu-id="36c34-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c34-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36c34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="36c34-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36c34-119">Request headers</span></span>
|<span data-ttu-id="36c34-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36c34-120">Header</span></span>|<span data-ttu-id="36c34-121">値</span><span class="sxs-lookup"><span data-stu-id="36c34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36c34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c34-122">Authorization</span></span>|<span data-ttu-id="36c34-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="36c34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36c34-124">承諾</span><span class="sxs-lookup"><span data-stu-id="36c34-124">Accept</span></span>|<span data-ttu-id="36c34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36c34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c34-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="36c34-126">Request body</span></span>
<span data-ttu-id="36c34-127">要求本文で、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36c34-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="36c34-128">次の表に、[androidStoreApp](../resources/intune-apps-androidstoreapp.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36c34-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="36c34-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36c34-129">Property</span></span>|<span data-ttu-id="36c34-130">型</span><span class="sxs-lookup"><span data-stu-id="36c34-130">Type</span></span>|<span data-ttu-id="36c34-131">説明</span><span class="sxs-lookup"><span data-stu-id="36c34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36c34-132">id</span><span class="sxs-lookup"><span data-stu-id="36c34-132">id</span></span>|<span data-ttu-id="36c34-133">文字列</span><span class="sxs-lookup"><span data-stu-id="36c34-133">String</span></span>|<span data-ttu-id="36c34-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="36c34-134">Key of the entity.</span></span> <span data-ttu-id="36c34-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-136">displayName</span><span class="sxs-lookup"><span data-stu-id="36c34-136">displayName</span></span>|<span data-ttu-id="36c34-137">文字列</span><span class="sxs-lookup"><span data-stu-id="36c34-137">String</span></span>|<span data-ttu-id="36c34-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="36c34-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="36c34-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-140">description</span><span class="sxs-lookup"><span data-stu-id="36c34-140">description</span></span>|<span data-ttu-id="36c34-141">String</span><span class="sxs-lookup"><span data-stu-id="36c34-141">String</span></span>|<span data-ttu-id="36c34-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="36c34-142">The description of the app.</span></span> <span data-ttu-id="36c34-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-144">publisher</span><span class="sxs-lookup"><span data-stu-id="36c34-144">publisher</span></span>|<span data-ttu-id="36c34-145">String</span><span class="sxs-lookup"><span data-stu-id="36c34-145">String</span></span>|<span data-ttu-id="36c34-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="36c34-146">The publisher of the app.</span></span> <span data-ttu-id="36c34-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="36c34-148">largeIcon</span></span>|[<span data-ttu-id="36c34-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="36c34-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="36c34-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="36c34-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="36c34-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36c34-152">createdDateTime</span></span>|<span data-ttu-id="36c34-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c34-153">DateTimeOffset</span></span>|<span data-ttu-id="36c34-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="36c34-154">The date and time the app was created.</span></span> <span data-ttu-id="36c34-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36c34-156">lastModifiedDateTime</span></span>|<span data-ttu-id="36c34-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c34-157">DateTimeOffset</span></span>|<span data-ttu-id="36c34-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="36c34-158">The date and time the app was last modified.</span></span> <span data-ttu-id="36c34-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="36c34-160">isFeatured</span></span>|<span data-ttu-id="36c34-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="36c34-161">Boolean</span></span>|<span data-ttu-id="36c34-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="36c34-163">privacyInformationUrl</span></span>|<span data-ttu-id="36c34-164">String</span><span class="sxs-lookup"><span data-stu-id="36c34-164">String</span></span>|<span data-ttu-id="36c34-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="36c34-165">The privacy statement Url.</span></span> <span data-ttu-id="36c34-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="36c34-167">informationUrl</span></span>|<span data-ttu-id="36c34-168">String</span><span class="sxs-lookup"><span data-stu-id="36c34-168">String</span></span>|<span data-ttu-id="36c34-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="36c34-169">The more information Url.</span></span> <span data-ttu-id="36c34-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-171">owner</span><span class="sxs-lookup"><span data-stu-id="36c34-171">owner</span></span>|<span data-ttu-id="36c34-172">String</span><span class="sxs-lookup"><span data-stu-id="36c34-172">String</span></span>|<span data-ttu-id="36c34-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="36c34-173">The owner of the app.</span></span> <span data-ttu-id="36c34-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-175">developer</span><span class="sxs-lookup"><span data-stu-id="36c34-175">developer</span></span>|<span data-ttu-id="36c34-176">String</span><span class="sxs-lookup"><span data-stu-id="36c34-176">String</span></span>|<span data-ttu-id="36c34-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="36c34-177">The developer of the app.</span></span> <span data-ttu-id="36c34-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-179">notes</span><span class="sxs-lookup"><span data-stu-id="36c34-179">notes</span></span>|<span data-ttu-id="36c34-180">String</span><span class="sxs-lookup"><span data-stu-id="36c34-180">String</span></span>|<span data-ttu-id="36c34-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="36c34-181">Notes for the app.</span></span> <span data-ttu-id="36c34-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="36c34-183">uploadState</span></span>|<span data-ttu-id="36c34-184">Int32</span><span class="sxs-lookup"><span data-stu-id="36c34-184">Int32</span></span>|<span data-ttu-id="36c34-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="36c34-185">The upload state.</span></span> <span data-ttu-id="36c34-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="36c34-187">publishingState</span></span>|[<span data-ttu-id="36c34-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="36c34-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="36c34-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="36c34-189">The publishing state for the app.</span></span> <span data-ttu-id="36c34-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="36c34-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="36c34-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="36c34-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="36c34-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="36c34-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="36c34-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="36c34-193">isAssigned</span></span>|<span data-ttu-id="36c34-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="36c34-194">Boolean</span></span>|<span data-ttu-id="36c34-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="36c34-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="36c34-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36c34-197">roleScopeTagIds</span></span>|<span data-ttu-id="36c34-198">String collection</span><span class="sxs-lookup"><span data-stu-id="36c34-198">String collection</span></span>|<span data-ttu-id="36c34-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="36c34-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="36c34-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="36c34-201">dependentAppCount</span></span>|<span data-ttu-id="36c34-202">Int32</span><span class="sxs-lookup"><span data-stu-id="36c34-202">Int32</span></span>|<span data-ttu-id="36c34-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="36c34-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="36c34-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36c34-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="36c34-205">packageId</span><span class="sxs-lookup"><span data-stu-id="36c34-205">packageId</span></span>|<span data-ttu-id="36c34-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36c34-206">String</span></span>|<span data-ttu-id="36c34-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="36c34-207">The package identifier.</span></span>|
|<span data-ttu-id="36c34-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="36c34-208">appIdentifier</span></span>|<span data-ttu-id="36c34-209">String</span><span class="sxs-lookup"><span data-stu-id="36c34-209">String</span></span>|<span data-ttu-id="36c34-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="36c34-210">The Identity Name.</span></span>|
|<span data-ttu-id="36c34-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="36c34-211">appStoreUrl</span></span>|<span data-ttu-id="36c34-212">String</span><span class="sxs-lookup"><span data-stu-id="36c34-212">String</span></span>|<span data-ttu-id="36c34-213">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="36c34-213">The Android app store URL.</span></span>|
|<span data-ttu-id="36c34-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="36c34-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="36c34-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="36c34-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="36c34-216">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="36c34-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="36c34-217">応答</span><span class="sxs-lookup"><span data-stu-id="36c34-217">Response</span></span>
<span data-ttu-id="36c34-218">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="36c34-218">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c34-219">例</span><span class="sxs-lookup"><span data-stu-id="36c34-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="36c34-220">要求</span><span class="sxs-lookup"><span data-stu-id="36c34-220">Request</span></span>
<span data-ttu-id="36c34-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36c34-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1230

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="36c34-222">応答</span><span class="sxs-lookup"><span data-stu-id="36c34-222">Response</span></span>
<span data-ttu-id="36c34-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36c34-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1402

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
  "dependentAppCount": 1,
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




