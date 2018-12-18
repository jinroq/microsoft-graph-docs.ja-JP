---
title: managedIOSStoreApp の更新
description: managedIOSStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 27c91f6c22031ac7d4bfe9a69a339652104e025c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305104"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="f45de-103">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="f45de-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="f45de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f45de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f45de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f45de-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f45de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f45de-107">[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f45de-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f45de-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f45de-108">Prerequisites</span></span>
<span data-ttu-id="f45de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f45de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f45de-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f45de-111">Permission type</span></span>|<span data-ttu-id="f45de-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f45de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f45de-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f45de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f45de-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f45de-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f45de-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f45de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f45de-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45de-116">Not supported.</span></span>|
|<span data-ttu-id="f45de-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f45de-117">Application</span></span>|<span data-ttu-id="f45de-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f45de-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f45de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f45de-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f45de-120">Request headers</span></span>
|<span data-ttu-id="f45de-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f45de-121">Header</span></span>|<span data-ttu-id="f45de-122">値</span><span class="sxs-lookup"><span data-stu-id="f45de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f45de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f45de-123">Authorization</span></span>|<span data-ttu-id="f45de-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f45de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f45de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f45de-125">Accept</span></span>|<span data-ttu-id="f45de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f45de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f45de-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f45de-127">Request body</span></span>
<span data-ttu-id="f45de-128">要求本文で、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f45de-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="f45de-129">次の表に、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f45de-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="f45de-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f45de-130">Property</span></span>|<span data-ttu-id="f45de-131">種類</span><span class="sxs-lookup"><span data-stu-id="f45de-131">Type</span></span>|<span data-ttu-id="f45de-132">説明</span><span class="sxs-lookup"><span data-stu-id="f45de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f45de-133">ID</span><span class="sxs-lookup"><span data-stu-id="f45de-133">id</span></span>|<span data-ttu-id="f45de-134">String</span><span class="sxs-lookup"><span data-stu-id="f45de-134">String</span></span>|<span data-ttu-id="f45de-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f45de-135">Key of the entity.</span></span> <span data-ttu-id="f45de-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f45de-137">displayName</span></span>|<span data-ttu-id="f45de-138">String</span><span class="sxs-lookup"><span data-stu-id="f45de-138">String</span></span>|<span data-ttu-id="f45de-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f45de-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f45de-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-141">説明</span><span class="sxs-lookup"><span data-stu-id="f45de-141">description</span></span>|<span data-ttu-id="f45de-142">String</span><span class="sxs-lookup"><span data-stu-id="f45de-142">String</span></span>|<span data-ttu-id="f45de-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f45de-143">The description of the app.</span></span> <span data-ttu-id="f45de-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f45de-145">publisher</span></span>|<span data-ttu-id="f45de-146">String</span><span class="sxs-lookup"><span data-stu-id="f45de-146">String</span></span>|<span data-ttu-id="f45de-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f45de-147">The publisher of the app.</span></span> <span data-ttu-id="f45de-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f45de-149">largeIcon</span></span>|[<span data-ttu-id="f45de-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f45de-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f45de-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f45de-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f45de-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f45de-153">createdDateTime</span></span>|<span data-ttu-id="f45de-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45de-154">DateTimeOffset</span></span>|<span data-ttu-id="f45de-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f45de-155">The date and time the app was created.</span></span> <span data-ttu-id="f45de-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f45de-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f45de-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45de-158">DateTimeOffset</span></span>|<span data-ttu-id="f45de-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f45de-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f45de-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f45de-161">isFeatured</span></span>|<span data-ttu-id="f45de-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45de-162">Boolean</span></span>|<span data-ttu-id="f45de-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f45de-164">privacyInformationUrl</span></span>|<span data-ttu-id="f45de-165">String</span><span class="sxs-lookup"><span data-stu-id="f45de-165">String</span></span>|<span data-ttu-id="f45de-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f45de-166">The privacy statement Url.</span></span> <span data-ttu-id="f45de-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f45de-168">informationUrl</span></span>|<span data-ttu-id="f45de-169">String</span><span class="sxs-lookup"><span data-stu-id="f45de-169">String</span></span>|<span data-ttu-id="f45de-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f45de-170">The more information Url.</span></span> <span data-ttu-id="f45de-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-172">owner</span><span class="sxs-lookup"><span data-stu-id="f45de-172">owner</span></span>|<span data-ttu-id="f45de-173">String</span><span class="sxs-lookup"><span data-stu-id="f45de-173">String</span></span>|<span data-ttu-id="f45de-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f45de-174">The owner of the app.</span></span> <span data-ttu-id="f45de-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-176">developer</span><span class="sxs-lookup"><span data-stu-id="f45de-176">developer</span></span>|<span data-ttu-id="f45de-177">String</span><span class="sxs-lookup"><span data-stu-id="f45de-177">String</span></span>|<span data-ttu-id="f45de-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f45de-178">The developer of the app.</span></span> <span data-ttu-id="f45de-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-180">notes</span><span class="sxs-lookup"><span data-stu-id="f45de-180">notes</span></span>|<span data-ttu-id="f45de-181">String</span><span class="sxs-lookup"><span data-stu-id="f45de-181">String</span></span>|<span data-ttu-id="f45de-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f45de-182">Notes for the app.</span></span> <span data-ttu-id="f45de-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f45de-184">uploadState</span></span>|<span data-ttu-id="f45de-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f45de-185">Int32</span></span>|<span data-ttu-id="f45de-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="f45de-186">The upload state.</span></span> <span data-ttu-id="f45de-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f45de-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f45de-188">publishingState</span></span>|[<span data-ttu-id="f45de-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f45de-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f45de-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f45de-190">The publishing state for the app.</span></span> <span data-ttu-id="f45de-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f45de-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f45de-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f45de-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f45de-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f45de-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f45de-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f45de-194">appAvailability</span></span>|[<span data-ttu-id="f45de-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f45de-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f45de-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="f45de-196">The Application's availability.</span></span> <span data-ttu-id="f45de-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f45de-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f45de-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="f45de-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f45de-199">version</span><span class="sxs-lookup"><span data-stu-id="f45de-199">version</span></span>|<span data-ttu-id="f45de-200">String</span><span class="sxs-lookup"><span data-stu-id="f45de-200">String</span></span>|<span data-ttu-id="f45de-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f45de-201">The Application's version.</span></span> <span data-ttu-id="f45de-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45de-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f45de-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="f45de-203">bundleId</span></span>|<span data-ttu-id="f45de-204">String</span><span class="sxs-lookup"><span data-stu-id="f45de-204">String</span></span>|<span data-ttu-id="f45de-205">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="f45de-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="f45de-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f45de-206">appStoreUrl</span></span>|<span data-ttu-id="f45de-207">String</span><span class="sxs-lookup"><span data-stu-id="f45de-207">String</span></span>|<span data-ttu-id="f45de-208">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="f45de-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="f45de-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f45de-209">applicableDeviceType</span></span>|[<span data-ttu-id="f45de-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f45de-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f45de-211">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="f45de-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f45de-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f45de-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f45de-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f45de-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f45de-214">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="f45de-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f45de-215">応答</span><span class="sxs-lookup"><span data-stu-id="f45de-215">Response</span></span>
<span data-ttu-id="f45de-216">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f45de-216">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f45de-217">例</span><span class="sxs-lookup"><span data-stu-id="f45de-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="f45de-218">要求</span><span class="sxs-lookup"><span data-stu-id="f45de-218">Request</span></span>
<span data-ttu-id="f45de-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f45de-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1113

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

### <a name="response"></a><span data-ttu-id="f45de-220">応答</span><span class="sxs-lookup"><span data-stu-id="f45de-220">Response</span></span>
<span data-ttu-id="f45de-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f45de-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

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





