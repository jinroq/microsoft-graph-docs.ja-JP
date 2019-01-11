---
title: managedAndroidStoreApp の更新
description: managedAndroidStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: de0301bb2bf56f71008eb6764d35fbb7479bafe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849022"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="3cd33-103">managedAndroidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="3cd33-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="3cd33-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3cd33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cd33-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cd33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cd33-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cd33-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cd33-107">[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3cd33-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cd33-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3cd33-108">Prerequisites</span></span>
<span data-ttu-id="3cd33-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cd33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd33-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cd33-111">Permission type</span></span>|<span data-ttu-id="3cd33-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cd33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd33-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cd33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd33-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd33-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3cd33-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cd33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd33-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cd33-116">Not supported.</span></span>|
|<span data-ttu-id="3cd33-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cd33-117">Application</span></span>|<span data-ttu-id="3cd33-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cd33-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd33-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cd33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3cd33-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cd33-120">Request headers</span></span>
|<span data-ttu-id="3cd33-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cd33-121">Header</span></span>|<span data-ttu-id="3cd33-122">値</span><span class="sxs-lookup"><span data-stu-id="3cd33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cd33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd33-123">Authorization</span></span>|<span data-ttu-id="3cd33-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3cd33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cd33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3cd33-125">Accept</span></span>|<span data-ttu-id="3cd33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cd33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd33-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cd33-127">Request body</span></span>
<span data-ttu-id="3cd33-128">要求本文で、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cd33-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="3cd33-129">次の表に、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cd33-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="3cd33-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cd33-130">Property</span></span>|<span data-ttu-id="3cd33-131">種類</span><span class="sxs-lookup"><span data-stu-id="3cd33-131">Type</span></span>|<span data-ttu-id="3cd33-132">説明</span><span class="sxs-lookup"><span data-stu-id="3cd33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd33-133">ID</span><span class="sxs-lookup"><span data-stu-id="3cd33-133">id</span></span>|<span data-ttu-id="3cd33-134">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-134">String</span></span>|<span data-ttu-id="3cd33-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3cd33-135">Key of the entity.</span></span> <span data-ttu-id="3cd33-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3cd33-137">displayName</span></span>|<span data-ttu-id="3cd33-138">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-138">String</span></span>|<span data-ttu-id="3cd33-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="3cd33-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3cd33-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-141">説明</span><span class="sxs-lookup"><span data-stu-id="3cd33-141">description</span></span>|<span data-ttu-id="3cd33-142">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-142">String</span></span>|<span data-ttu-id="3cd33-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="3cd33-143">The description of the app.</span></span> <span data-ttu-id="3cd33-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3cd33-145">publisher</span></span>|<span data-ttu-id="3cd33-146">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-146">String</span></span>|<span data-ttu-id="3cd33-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="3cd33-147">The publisher of the app.</span></span> <span data-ttu-id="3cd33-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3cd33-149">largeIcon</span></span>|[<span data-ttu-id="3cd33-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3cd33-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3cd33-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="3cd33-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3cd33-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd33-153">createdDateTime</span></span>|<span data-ttu-id="3cd33-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd33-154">DateTimeOffset</span></span>|<span data-ttu-id="3cd33-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="3cd33-155">The date and time the app was created.</span></span> <span data-ttu-id="3cd33-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd33-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3cd33-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd33-158">DateTimeOffset</span></span>|<span data-ttu-id="3cd33-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="3cd33-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3cd33-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3cd33-161">isFeatured</span></span>|<span data-ttu-id="3cd33-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cd33-162">Boolean</span></span>|<span data-ttu-id="3cd33-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3cd33-164">privacyInformationUrl</span></span>|<span data-ttu-id="3cd33-165">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-165">String</span></span>|<span data-ttu-id="3cd33-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="3cd33-166">The privacy statement Url.</span></span> <span data-ttu-id="3cd33-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3cd33-168">informationUrl</span></span>|<span data-ttu-id="3cd33-169">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-169">String</span></span>|<span data-ttu-id="3cd33-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="3cd33-170">The more information Url.</span></span> <span data-ttu-id="3cd33-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-172">owner</span><span class="sxs-lookup"><span data-stu-id="3cd33-172">owner</span></span>|<span data-ttu-id="3cd33-173">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-173">String</span></span>|<span data-ttu-id="3cd33-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="3cd33-174">The owner of the app.</span></span> <span data-ttu-id="3cd33-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-176">developer</span><span class="sxs-lookup"><span data-stu-id="3cd33-176">developer</span></span>|<span data-ttu-id="3cd33-177">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-177">String</span></span>|<span data-ttu-id="3cd33-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="3cd33-178">The developer of the app.</span></span> <span data-ttu-id="3cd33-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-180">notes</span><span class="sxs-lookup"><span data-stu-id="3cd33-180">notes</span></span>|<span data-ttu-id="3cd33-181">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-181">String</span></span>|<span data-ttu-id="3cd33-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="3cd33-182">Notes for the app.</span></span> <span data-ttu-id="3cd33-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3cd33-184">uploadState</span></span>|<span data-ttu-id="3cd33-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd33-185">Int32</span></span>|<span data-ttu-id="3cd33-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="3cd33-186">The upload state.</span></span> <span data-ttu-id="3cd33-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3cd33-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3cd33-188">publishingState</span></span>|[<span data-ttu-id="3cd33-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3cd33-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3cd33-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="3cd33-190">The publishing state for the app.</span></span> <span data-ttu-id="3cd33-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="3cd33-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3cd33-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3cd33-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3cd33-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="3cd33-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3cd33-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3cd33-194">appAvailability</span></span>|[<span data-ttu-id="3cd33-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="3cd33-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="3cd33-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="3cd33-196">The Application's availability.</span></span> <span data-ttu-id="3cd33-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3cd33-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="3cd33-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="3cd33-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3cd33-199">version</span><span class="sxs-lookup"><span data-stu-id="3cd33-199">version</span></span>|<span data-ttu-id="3cd33-200">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-200">String</span></span>|<span data-ttu-id="3cd33-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3cd33-201">The Application's version.</span></span> <span data-ttu-id="3cd33-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cd33-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="3cd33-203">packageId</span><span class="sxs-lookup"><span data-stu-id="3cd33-203">packageId</span></span>|<span data-ttu-id="3cd33-204">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-204">String</span></span>|<span data-ttu-id="3cd33-205">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="3cd33-205">The app's package ID.</span></span>|
|<span data-ttu-id="3cd33-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3cd33-206">appStoreUrl</span></span>|<span data-ttu-id="3cd33-207">String</span><span class="sxs-lookup"><span data-stu-id="3cd33-207">String</span></span>|<span data-ttu-id="3cd33-208">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="3cd33-208">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="3cd33-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3cd33-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3cd33-210">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3cd33-210">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3cd33-211">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="3cd33-211">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3cd33-212">応答</span><span class="sxs-lookup"><span data-stu-id="3cd33-212">Response</span></span>
<span data-ttu-id="3cd33-213">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3cd33-213">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd33-214">例</span><span class="sxs-lookup"><span data-stu-id="3cd33-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cd33-215">要求</span><span class="sxs-lookup"><span data-stu-id="3cd33-215">Request</span></span>
<span data-ttu-id="3cd33-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cd33-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1155

{
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

### <a name="response"></a><span data-ttu-id="3cd33-217">応答</span><span class="sxs-lookup"><span data-stu-id="3cd33-217">Response</span></span>
<span data-ttu-id="3cd33-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3cd33-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





