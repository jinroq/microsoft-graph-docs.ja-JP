---
title: Update iosStoreApp
description: iosStoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189b81d352d71a284670270fce0387e3b4eb650c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966041"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="8acda-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="8acda-103">Update iosStoreApp</span></span>

> <span data-ttu-id="8acda-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8acda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8acda-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8acda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8acda-106">[iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8acda-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8acda-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8acda-107">Prerequisites</span></span>
<span data-ttu-id="8acda-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8acda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8acda-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8acda-110">Permission type</span></span>|<span data-ttu-id="8acda-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8acda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8acda-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8acda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8acda-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8acda-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8acda-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8acda-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8acda-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8acda-115">Not supported.</span></span>|
|<span data-ttu-id="8acda-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8acda-116">Application</span></span>|<span data-ttu-id="8acda-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8acda-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8acda-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8acda-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8acda-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8acda-119">Request headers</span></span>
|<span data-ttu-id="8acda-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8acda-120">Header</span></span>|<span data-ttu-id="8acda-121">値</span><span class="sxs-lookup"><span data-stu-id="8acda-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8acda-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8acda-122">Authorization</span></span>|<span data-ttu-id="8acda-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8acda-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8acda-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8acda-124">Accept</span></span>|<span data-ttu-id="8acda-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8acda-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8acda-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8acda-126">Request body</span></span>
<span data-ttu-id="8acda-127">要求本文で、[iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8acda-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="8acda-128">次の表に、[iosStoreApp](../resources/intune-apps-iosstoreapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8acda-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="8acda-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8acda-129">Property</span></span>|<span data-ttu-id="8acda-130">型</span><span class="sxs-lookup"><span data-stu-id="8acda-130">Type</span></span>|<span data-ttu-id="8acda-131">説明</span><span class="sxs-lookup"><span data-stu-id="8acda-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8acda-132">id</span><span class="sxs-lookup"><span data-stu-id="8acda-132">id</span></span>|<span data-ttu-id="8acda-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8acda-133">String</span></span>|<span data-ttu-id="8acda-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8acda-134">Key of the entity.</span></span> <span data-ttu-id="8acda-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8acda-136">displayName</span></span>|<span data-ttu-id="8acda-137">文字列</span><span class="sxs-lookup"><span data-stu-id="8acda-137">String</span></span>|<span data-ttu-id="8acda-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="8acda-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8acda-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-140">description</span><span class="sxs-lookup"><span data-stu-id="8acda-140">description</span></span>|<span data-ttu-id="8acda-141">String</span><span class="sxs-lookup"><span data-stu-id="8acda-141">String</span></span>|<span data-ttu-id="8acda-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8acda-142">The description of the app.</span></span> <span data-ttu-id="8acda-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8acda-144">publisher</span></span>|<span data-ttu-id="8acda-145">String</span><span class="sxs-lookup"><span data-stu-id="8acda-145">String</span></span>|<span data-ttu-id="8acda-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="8acda-146">The publisher of the app.</span></span> <span data-ttu-id="8acda-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8acda-148">largeIcon</span></span>|[<span data-ttu-id="8acda-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8acda-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8acda-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="8acda-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8acda-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8acda-152">createdDateTime</span></span>|<span data-ttu-id="8acda-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8acda-153">DateTimeOffset</span></span>|<span data-ttu-id="8acda-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8acda-154">The date and time the app was created.</span></span> <span data-ttu-id="8acda-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8acda-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8acda-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8acda-157">DateTimeOffset</span></span>|<span data-ttu-id="8acda-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8acda-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8acda-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8acda-160">isFeatured</span></span>|<span data-ttu-id="8acda-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8acda-161">Boolean</span></span>|<span data-ttu-id="8acda-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8acda-163">privacyInformationUrl</span></span>|<span data-ttu-id="8acda-164">String</span><span class="sxs-lookup"><span data-stu-id="8acda-164">String</span></span>|<span data-ttu-id="8acda-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="8acda-165">The privacy statement Url.</span></span> <span data-ttu-id="8acda-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8acda-167">informationUrl</span></span>|<span data-ttu-id="8acda-168">String</span><span class="sxs-lookup"><span data-stu-id="8acda-168">String</span></span>|<span data-ttu-id="8acda-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="8acda-169">The more information Url.</span></span> <span data-ttu-id="8acda-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-171">owner</span><span class="sxs-lookup"><span data-stu-id="8acda-171">owner</span></span>|<span data-ttu-id="8acda-172">String</span><span class="sxs-lookup"><span data-stu-id="8acda-172">String</span></span>|<span data-ttu-id="8acda-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="8acda-173">The owner of the app.</span></span> <span data-ttu-id="8acda-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-175">developer</span><span class="sxs-lookup"><span data-stu-id="8acda-175">developer</span></span>|<span data-ttu-id="8acda-176">String</span><span class="sxs-lookup"><span data-stu-id="8acda-176">String</span></span>|<span data-ttu-id="8acda-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="8acda-177">The developer of the app.</span></span> <span data-ttu-id="8acda-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-179">notes</span><span class="sxs-lookup"><span data-stu-id="8acda-179">notes</span></span>|<span data-ttu-id="8acda-180">String</span><span class="sxs-lookup"><span data-stu-id="8acda-180">String</span></span>|<span data-ttu-id="8acda-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="8acda-181">Notes for the app.</span></span> <span data-ttu-id="8acda-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8acda-183">uploadState</span></span>|<span data-ttu-id="8acda-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8acda-184">Int32</span></span>|<span data-ttu-id="8acda-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="8acda-185">The upload state.</span></span> <span data-ttu-id="8acda-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8acda-187">publishingState</span></span>|[<span data-ttu-id="8acda-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8acda-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8acda-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="8acda-189">The publishing state for the app.</span></span> <span data-ttu-id="8acda-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="8acda-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8acda-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8acda-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8acda-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="8acda-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8acda-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8acda-193">isAssigned</span></span>|<span data-ttu-id="8acda-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8acda-194">Boolean</span></span>|<span data-ttu-id="8acda-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="8acda-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8acda-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8acda-197">roleScopeTagIds</span></span>|<span data-ttu-id="8acda-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8acda-198">String collection</span></span>|<span data-ttu-id="8acda-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="8acda-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8acda-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8acda-201">dependentAppCount</span></span>|<span data-ttu-id="8acda-202">Int32</span><span class="sxs-lookup"><span data-stu-id="8acda-202">Int32</span></span>|<span data-ttu-id="8acda-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="8acda-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8acda-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8acda-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8acda-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="8acda-205">bundleId</span></span>|<span data-ttu-id="8acda-206">String</span><span class="sxs-lookup"><span data-stu-id="8acda-206">String</span></span>|<span data-ttu-id="8acda-207">ID 名。</span><span class="sxs-lookup"><span data-stu-id="8acda-207">The Identity Name.</span></span>|
|<span data-ttu-id="8acda-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8acda-208">appStoreUrl</span></span>|<span data-ttu-id="8acda-209">String</span><span class="sxs-lookup"><span data-stu-id="8acda-209">String</span></span>|<span data-ttu-id="8acda-210">Apple App Store の URL。</span><span class="sxs-lookup"><span data-stu-id="8acda-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="8acda-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8acda-211">applicableDeviceType</span></span>|[<span data-ttu-id="8acda-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8acda-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8acda-213">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="8acda-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8acda-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8acda-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8acda-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8acda-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8acda-216">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="8acda-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8acda-217">応答</span><span class="sxs-lookup"><span data-stu-id="8acda-217">Response</span></span>
<span data-ttu-id="8acda-218">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosStoreApp](../resources/intune-apps-iosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8acda-218">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8acda-219">例</span><span class="sxs-lookup"><span data-stu-id="8acda-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="8acda-220">要求</span><span class="sxs-lookup"><span data-stu-id="8acda-220">Request</span></span>
<span data-ttu-id="8acda-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8acda-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="8acda-222">応答</span><span class="sxs-lookup"><span data-stu-id="8acda-222">Response</span></span>
<span data-ttu-id="8acda-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8acda-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1312

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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





