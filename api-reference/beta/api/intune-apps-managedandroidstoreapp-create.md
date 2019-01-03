---
title: managedAndroidStoreApp の作成
description: 新しい managedAndroidStoreApp オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: f7b54f9da6197e9f4c1cbf3265a58fc7aa11e1c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316276"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="f8f05-103">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="f8f05-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="f8f05-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8f05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8f05-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8f05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8f05-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8f05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8f05-107">新しい [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f8f05-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8f05-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f8f05-108">Prerequisites</span></span>
<span data-ttu-id="f8f05-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8f05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f05-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8f05-111">Permission type</span></span>|<span data-ttu-id="f8f05-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8f05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8f05-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8f05-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f05-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8f05-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8f05-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8f05-116">Not supported.</span></span>|
|<span data-ttu-id="f8f05-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8f05-117">Application</span></span>|<span data-ttu-id="f8f05-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8f05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8f05-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f8f05-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8f05-120">Request headers</span></span>
|<span data-ttu-id="f8f05-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8f05-121">Header</span></span>|<span data-ttu-id="f8f05-122">値</span><span class="sxs-lookup"><span data-stu-id="f8f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8f05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f05-123">Authorization</span></span>|<span data-ttu-id="f8f05-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f8f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8f05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8f05-125">Accept</span></span>|<span data-ttu-id="f8f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8f05-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8f05-127">Request body</span></span>
<span data-ttu-id="f8f05-128">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8f05-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="f8f05-129">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f8f05-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="f8f05-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8f05-130">Property</span></span>|<span data-ttu-id="f8f05-131">種類</span><span class="sxs-lookup"><span data-stu-id="f8f05-131">Type</span></span>|<span data-ttu-id="f8f05-132">説明</span><span class="sxs-lookup"><span data-stu-id="f8f05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f05-133">ID</span><span class="sxs-lookup"><span data-stu-id="f8f05-133">id</span></span>|<span data-ttu-id="f8f05-134">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-134">String</span></span>|<span data-ttu-id="f8f05-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f8f05-135">Key of the entity.</span></span> <span data-ttu-id="f8f05-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f8f05-137">displayName</span></span>|<span data-ttu-id="f8f05-138">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-138">String</span></span>|<span data-ttu-id="f8f05-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f8f05-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f8f05-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-141">説明</span><span class="sxs-lookup"><span data-stu-id="f8f05-141">description</span></span>|<span data-ttu-id="f8f05-142">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-142">String</span></span>|<span data-ttu-id="f8f05-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f8f05-143">The description of the app.</span></span> <span data-ttu-id="f8f05-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f8f05-145">publisher</span></span>|<span data-ttu-id="f8f05-146">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-146">String</span></span>|<span data-ttu-id="f8f05-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f8f05-147">The publisher of the app.</span></span> <span data-ttu-id="f8f05-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f8f05-149">largeIcon</span></span>|[<span data-ttu-id="f8f05-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f8f05-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f8f05-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f8f05-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f8f05-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f05-153">createdDateTime</span></span>|<span data-ttu-id="f8f05-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f05-154">DateTimeOffset</span></span>|<span data-ttu-id="f8f05-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f8f05-155">The date and time the app was created.</span></span> <span data-ttu-id="f8f05-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f05-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f8f05-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f05-158">DateTimeOffset</span></span>|<span data-ttu-id="f8f05-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f8f05-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f8f05-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f8f05-161">isFeatured</span></span>|<span data-ttu-id="f8f05-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f05-162">Boolean</span></span>|<span data-ttu-id="f8f05-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f8f05-164">privacyInformationUrl</span></span>|<span data-ttu-id="f8f05-165">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-165">String</span></span>|<span data-ttu-id="f8f05-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f8f05-166">The privacy statement Url.</span></span> <span data-ttu-id="f8f05-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f8f05-168">informationUrl</span></span>|<span data-ttu-id="f8f05-169">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-169">String</span></span>|<span data-ttu-id="f8f05-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f8f05-170">The more information Url.</span></span> <span data-ttu-id="f8f05-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-172">owner</span><span class="sxs-lookup"><span data-stu-id="f8f05-172">owner</span></span>|<span data-ttu-id="f8f05-173">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-173">String</span></span>|<span data-ttu-id="f8f05-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f8f05-174">The owner of the app.</span></span> <span data-ttu-id="f8f05-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-176">developer</span><span class="sxs-lookup"><span data-stu-id="f8f05-176">developer</span></span>|<span data-ttu-id="f8f05-177">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-177">String</span></span>|<span data-ttu-id="f8f05-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f8f05-178">The developer of the app.</span></span> <span data-ttu-id="f8f05-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-180">notes</span><span class="sxs-lookup"><span data-stu-id="f8f05-180">notes</span></span>|<span data-ttu-id="f8f05-181">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-181">String</span></span>|<span data-ttu-id="f8f05-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f8f05-182">Notes for the app.</span></span> <span data-ttu-id="f8f05-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f8f05-184">uploadState</span></span>|<span data-ttu-id="f8f05-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f05-185">Int32</span></span>|<span data-ttu-id="f8f05-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="f8f05-186">The upload state.</span></span> <span data-ttu-id="f8f05-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f8f05-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f8f05-188">publishingState</span></span>|[<span data-ttu-id="f8f05-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f8f05-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f8f05-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f8f05-190">The publishing state for the app.</span></span> <span data-ttu-id="f8f05-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f8f05-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f8f05-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f8f05-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f8f05-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f8f05-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f8f05-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f8f05-194">appAvailability</span></span>|[<span data-ttu-id="f8f05-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f8f05-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f8f05-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="f8f05-196">The Application's availability.</span></span> <span data-ttu-id="f8f05-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f8f05-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f8f05-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="f8f05-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f8f05-199">version</span><span class="sxs-lookup"><span data-stu-id="f8f05-199">version</span></span>|<span data-ttu-id="f8f05-200">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-200">String</span></span>|<span data-ttu-id="f8f05-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f8f05-201">The Application's version.</span></span> <span data-ttu-id="f8f05-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f8f05-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f8f05-203">packageId</span><span class="sxs-lookup"><span data-stu-id="f8f05-203">packageId</span></span>|<span data-ttu-id="f8f05-204">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-204">String</span></span>|<span data-ttu-id="f8f05-205">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="f8f05-205">The app's package ID.</span></span>|
|<span data-ttu-id="f8f05-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f8f05-206">appStoreUrl</span></span>|<span data-ttu-id="f8f05-207">String</span><span class="sxs-lookup"><span data-stu-id="f8f05-207">String</span></span>|<span data-ttu-id="f8f05-208">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="f8f05-208">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="f8f05-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f8f05-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f8f05-210">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f8f05-210">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f8f05-211">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="f8f05-211">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f8f05-212">応答</span><span class="sxs-lookup"><span data-stu-id="f8f05-212">Response</span></span>
<span data-ttu-id="f8f05-213">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f8f05-213">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f05-214">例</span><span class="sxs-lookup"><span data-stu-id="f8f05-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8f05-215">要求</span><span class="sxs-lookup"><span data-stu-id="f8f05-215">Request</span></span>
<span data-ttu-id="f8f05-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8f05-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1216

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="f8f05-217">応答</span><span class="sxs-lookup"><span data-stu-id="f8f05-217">Response</span></span>
<span data-ttu-id="f8f05-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8f05-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1324

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




