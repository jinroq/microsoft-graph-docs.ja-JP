---
title: managedIOSStoreApp の更新
description: managedIOSStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e7f46d334eb1842b96d764d1e7865a6840978965
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825061"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="8f508-103">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="8f508-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="8f508-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8f508-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f508-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f508-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f508-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8f508-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f508-107">[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8f508-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f508-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8f508-108">Prerequisites</span></span>
<span data-ttu-id="8f508-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f508-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f508-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f508-111">Permission type</span></span>|<span data-ttu-id="8f508-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f508-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f508-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f508-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f508-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f508-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f508-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f508-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f508-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f508-116">Not supported.</span></span>|
|<span data-ttu-id="8f508-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f508-117">Application</span></span>|<span data-ttu-id="8f508-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f508-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f508-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f508-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8f508-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f508-120">Request headers</span></span>
|<span data-ttu-id="8f508-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f508-121">Header</span></span>|<span data-ttu-id="8f508-122">値</span><span class="sxs-lookup"><span data-stu-id="8f508-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f508-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f508-123">Authorization</span></span>|<span data-ttu-id="8f508-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8f508-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f508-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f508-125">Accept</span></span>|<span data-ttu-id="8f508-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f508-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f508-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f508-127">Request body</span></span>
<span data-ttu-id="8f508-128">要求本文で、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f508-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="8f508-129">次の表に、[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8f508-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="8f508-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f508-130">Property</span></span>|<span data-ttu-id="8f508-131">種類</span><span class="sxs-lookup"><span data-stu-id="8f508-131">Type</span></span>|<span data-ttu-id="8f508-132">説明</span><span class="sxs-lookup"><span data-stu-id="8f508-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f508-133">ID</span><span class="sxs-lookup"><span data-stu-id="8f508-133">id</span></span>|<span data-ttu-id="8f508-134">String</span><span class="sxs-lookup"><span data-stu-id="8f508-134">String</span></span>|<span data-ttu-id="8f508-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8f508-135">Key of the entity.</span></span> <span data-ttu-id="8f508-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8f508-137">displayName</span></span>|<span data-ttu-id="8f508-138">String</span><span class="sxs-lookup"><span data-stu-id="8f508-138">String</span></span>|<span data-ttu-id="8f508-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="8f508-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8f508-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-141">説明</span><span class="sxs-lookup"><span data-stu-id="8f508-141">description</span></span>|<span data-ttu-id="8f508-142">String</span><span class="sxs-lookup"><span data-stu-id="8f508-142">String</span></span>|<span data-ttu-id="8f508-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8f508-143">The description of the app.</span></span> <span data-ttu-id="8f508-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8f508-145">publisher</span></span>|<span data-ttu-id="8f508-146">String</span><span class="sxs-lookup"><span data-stu-id="8f508-146">String</span></span>|<span data-ttu-id="8f508-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="8f508-147">The publisher of the app.</span></span> <span data-ttu-id="8f508-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8f508-149">largeIcon</span></span>|[<span data-ttu-id="8f508-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8f508-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8f508-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="8f508-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8f508-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f508-153">createdDateTime</span></span>|<span data-ttu-id="8f508-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f508-154">DateTimeOffset</span></span>|<span data-ttu-id="8f508-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8f508-155">The date and time the app was created.</span></span> <span data-ttu-id="8f508-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f508-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8f508-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f508-158">DateTimeOffset</span></span>|<span data-ttu-id="8f508-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8f508-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8f508-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8f508-161">isFeatured</span></span>|<span data-ttu-id="8f508-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f508-162">Boolean</span></span>|<span data-ttu-id="8f508-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8f508-164">privacyInformationUrl</span></span>|<span data-ttu-id="8f508-165">String</span><span class="sxs-lookup"><span data-stu-id="8f508-165">String</span></span>|<span data-ttu-id="8f508-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="8f508-166">The privacy statement Url.</span></span> <span data-ttu-id="8f508-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8f508-168">informationUrl</span></span>|<span data-ttu-id="8f508-169">String</span><span class="sxs-lookup"><span data-stu-id="8f508-169">String</span></span>|<span data-ttu-id="8f508-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="8f508-170">The more information Url.</span></span> <span data-ttu-id="8f508-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-172">owner</span><span class="sxs-lookup"><span data-stu-id="8f508-172">owner</span></span>|<span data-ttu-id="8f508-173">String</span><span class="sxs-lookup"><span data-stu-id="8f508-173">String</span></span>|<span data-ttu-id="8f508-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="8f508-174">The owner of the app.</span></span> <span data-ttu-id="8f508-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-176">developer</span><span class="sxs-lookup"><span data-stu-id="8f508-176">developer</span></span>|<span data-ttu-id="8f508-177">String</span><span class="sxs-lookup"><span data-stu-id="8f508-177">String</span></span>|<span data-ttu-id="8f508-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="8f508-178">The developer of the app.</span></span> <span data-ttu-id="8f508-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-180">notes</span><span class="sxs-lookup"><span data-stu-id="8f508-180">notes</span></span>|<span data-ttu-id="8f508-181">String</span><span class="sxs-lookup"><span data-stu-id="8f508-181">String</span></span>|<span data-ttu-id="8f508-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="8f508-182">Notes for the app.</span></span> <span data-ttu-id="8f508-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8f508-184">uploadState</span></span>|<span data-ttu-id="8f508-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8f508-185">Int32</span></span>|<span data-ttu-id="8f508-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="8f508-186">The upload state.</span></span> <span data-ttu-id="8f508-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f508-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8f508-188">publishingState</span></span>|[<span data-ttu-id="8f508-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8f508-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8f508-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="8f508-190">The publishing state for the app.</span></span> <span data-ttu-id="8f508-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="8f508-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8f508-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8f508-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8f508-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="8f508-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8f508-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8f508-194">appAvailability</span></span>|[<span data-ttu-id="8f508-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8f508-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8f508-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="8f508-196">The Application's availability.</span></span> <span data-ttu-id="8f508-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8f508-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8f508-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="8f508-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8f508-199">version</span><span class="sxs-lookup"><span data-stu-id="8f508-199">version</span></span>|<span data-ttu-id="8f508-200">String</span><span class="sxs-lookup"><span data-stu-id="8f508-200">String</span></span>|<span data-ttu-id="8f508-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8f508-201">The Application's version.</span></span> <span data-ttu-id="8f508-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8f508-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8f508-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="8f508-203">bundleId</span></span>|<span data-ttu-id="8f508-204">String</span><span class="sxs-lookup"><span data-stu-id="8f508-204">String</span></span>|<span data-ttu-id="8f508-205">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="8f508-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="8f508-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8f508-206">appStoreUrl</span></span>|<span data-ttu-id="8f508-207">String</span><span class="sxs-lookup"><span data-stu-id="8f508-207">String</span></span>|<span data-ttu-id="8f508-208">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="8f508-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="8f508-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8f508-209">applicableDeviceType</span></span>|[<span data-ttu-id="8f508-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8f508-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8f508-211">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="8f508-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8f508-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8f508-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8f508-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8f508-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8f508-214">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="8f508-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8f508-215">応答</span><span class="sxs-lookup"><span data-stu-id="8f508-215">Response</span></span>
<span data-ttu-id="8f508-216">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8f508-216">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f508-217">例</span><span class="sxs-lookup"><span data-stu-id="8f508-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f508-218">要求</span><span class="sxs-lookup"><span data-stu-id="8f508-218">Request</span></span>
<span data-ttu-id="8f508-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f508-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f508-220">応答</span><span class="sxs-lookup"><span data-stu-id="8f508-220">Response</span></span>
<span data-ttu-id="8f508-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f508-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





