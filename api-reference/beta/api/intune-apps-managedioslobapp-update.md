---
title: managedIOSLobApp の更新
description: managedIOSLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: af73dac3e1ccb785664f48a02837cec369b91297
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325509"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="e256e-103">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="e256e-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="e256e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e256e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e256e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e256e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e256e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e256e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e256e-107">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e256e-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e256e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e256e-108">Prerequisites</span></span>
<span data-ttu-id="e256e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e256e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e256e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e256e-111">Permission type</span></span>|<span data-ttu-id="e256e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e256e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e256e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e256e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e256e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e256e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e256e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e256e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e256e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e256e-116">Not supported.</span></span>|
|<span data-ttu-id="e256e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e256e-117">Application</span></span>|<span data-ttu-id="e256e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e256e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e256e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e256e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e256e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e256e-120">Request headers</span></span>
|<span data-ttu-id="e256e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e256e-121">Header</span></span>|<span data-ttu-id="e256e-122">値</span><span class="sxs-lookup"><span data-stu-id="e256e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e256e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e256e-123">Authorization</span></span>|<span data-ttu-id="e256e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e256e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e256e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e256e-125">Accept</span></span>|<span data-ttu-id="e256e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e256e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e256e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e256e-127">Request body</span></span>
<span data-ttu-id="e256e-128">要求本文で、[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e256e-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="e256e-129">次の表に、[managedDeviceOverview](../resources/intune-apps-managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e256e-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="e256e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e256e-130">Property</span></span>|<span data-ttu-id="e256e-131">種類</span><span class="sxs-lookup"><span data-stu-id="e256e-131">Type</span></span>|<span data-ttu-id="e256e-132">説明</span><span class="sxs-lookup"><span data-stu-id="e256e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e256e-133">ID</span><span class="sxs-lookup"><span data-stu-id="e256e-133">id</span></span>|<span data-ttu-id="e256e-134">String</span><span class="sxs-lookup"><span data-stu-id="e256e-134">String</span></span>|<span data-ttu-id="e256e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e256e-135">Key of the entity.</span></span> <span data-ttu-id="e256e-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e256e-137">displayName</span></span>|<span data-ttu-id="e256e-138">String</span><span class="sxs-lookup"><span data-stu-id="e256e-138">String</span></span>|<span data-ttu-id="e256e-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e256e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e256e-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-141">説明</span><span class="sxs-lookup"><span data-stu-id="e256e-141">description</span></span>|<span data-ttu-id="e256e-142">String</span><span class="sxs-lookup"><span data-stu-id="e256e-142">String</span></span>|<span data-ttu-id="e256e-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e256e-143">The description of the app.</span></span> <span data-ttu-id="e256e-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e256e-145">publisher</span></span>|<span data-ttu-id="e256e-146">String</span><span class="sxs-lookup"><span data-stu-id="e256e-146">String</span></span>|<span data-ttu-id="e256e-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e256e-147">The publisher of the app.</span></span> <span data-ttu-id="e256e-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e256e-149">largeIcon</span></span>|[<span data-ttu-id="e256e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e256e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e256e-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="e256e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e256e-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e256e-153">createdDateTime</span></span>|<span data-ttu-id="e256e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e256e-154">DateTimeOffset</span></span>|<span data-ttu-id="e256e-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e256e-155">The date and time the app was created.</span></span> <span data-ttu-id="e256e-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e256e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e256e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e256e-158">DateTimeOffset</span></span>|<span data-ttu-id="e256e-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e256e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e256e-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e256e-161">isFeatured</span></span>|<span data-ttu-id="e256e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e256e-162">Boolean</span></span>|<span data-ttu-id="e256e-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e256e-164">privacyInformationUrl</span></span>|<span data-ttu-id="e256e-165">String</span><span class="sxs-lookup"><span data-stu-id="e256e-165">String</span></span>|<span data-ttu-id="e256e-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e256e-166">The privacy statement Url.</span></span> <span data-ttu-id="e256e-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e256e-168">informationUrl</span></span>|<span data-ttu-id="e256e-169">String</span><span class="sxs-lookup"><span data-stu-id="e256e-169">String</span></span>|<span data-ttu-id="e256e-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e256e-170">The more information Url.</span></span> <span data-ttu-id="e256e-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-172">owner</span><span class="sxs-lookup"><span data-stu-id="e256e-172">owner</span></span>|<span data-ttu-id="e256e-173">String</span><span class="sxs-lookup"><span data-stu-id="e256e-173">String</span></span>|<span data-ttu-id="e256e-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e256e-174">The owner of the app.</span></span> <span data-ttu-id="e256e-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-176">developer</span><span class="sxs-lookup"><span data-stu-id="e256e-176">developer</span></span>|<span data-ttu-id="e256e-177">String</span><span class="sxs-lookup"><span data-stu-id="e256e-177">String</span></span>|<span data-ttu-id="e256e-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e256e-178">The developer of the app.</span></span> <span data-ttu-id="e256e-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-180">notes</span><span class="sxs-lookup"><span data-stu-id="e256e-180">notes</span></span>|<span data-ttu-id="e256e-181">String</span><span class="sxs-lookup"><span data-stu-id="e256e-181">String</span></span>|<span data-ttu-id="e256e-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e256e-182">Notes for the app.</span></span> <span data-ttu-id="e256e-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e256e-184">uploadState</span></span>|<span data-ttu-id="e256e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e256e-185">Int32</span></span>|<span data-ttu-id="e256e-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="e256e-186">The upload state.</span></span> <span data-ttu-id="e256e-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e256e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e256e-188">publishingState</span></span>|[<span data-ttu-id="e256e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e256e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e256e-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e256e-190">The publishing state for the app.</span></span> <span data-ttu-id="e256e-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e256e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e256e-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e256e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e256e-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e256e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e256e-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e256e-194">appAvailability</span></span>|[<span data-ttu-id="e256e-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e256e-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e256e-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="e256e-196">The Application's availability.</span></span> <span data-ttu-id="e256e-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e256e-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e256e-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="e256e-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e256e-199">version</span><span class="sxs-lookup"><span data-stu-id="e256e-199">version</span></span>|<span data-ttu-id="e256e-200">String</span><span class="sxs-lookup"><span data-stu-id="e256e-200">String</span></span>|<span data-ttu-id="e256e-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e256e-201">The Application's version.</span></span> <span data-ttu-id="e256e-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e256e-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e256e-203">committedContentVersion</span></span>|<span data-ttu-id="e256e-204">String</span><span class="sxs-lookup"><span data-stu-id="e256e-204">String</span></span>|<span data-ttu-id="e256e-205">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e256e-205">The internal committed content version.</span></span> <span data-ttu-id="e256e-206">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e256e-207">fileName</span><span class="sxs-lookup"><span data-stu-id="e256e-207">fileName</span></span>|<span data-ttu-id="e256e-208">String</span><span class="sxs-lookup"><span data-stu-id="e256e-208">String</span></span>|<span data-ttu-id="e256e-209">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="e256e-209">The name of the main Lob application file.</span></span> <span data-ttu-id="e256e-210">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e256e-211">size</span><span class="sxs-lookup"><span data-stu-id="e256e-211">size</span></span>|<span data-ttu-id="e256e-212">Int64</span><span class="sxs-lookup"><span data-stu-id="e256e-212">Int64</span></span>|<span data-ttu-id="e256e-213">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="e256e-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="e256e-214">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e256e-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e256e-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="e256e-215">bundleId</span></span>|<span data-ttu-id="e256e-216">String</span><span class="sxs-lookup"><span data-stu-id="e256e-216">String</span></span>|<span data-ttu-id="e256e-217">ID 名。</span><span class="sxs-lookup"><span data-stu-id="e256e-217">The Identity Name.</span></span>|
|<span data-ttu-id="e256e-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e256e-218">applicableDeviceType</span></span>|[<span data-ttu-id="e256e-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e256e-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e256e-220">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="e256e-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e256e-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e256e-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e256e-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e256e-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="e256e-223">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="e256e-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e256e-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e256e-224">expirationDateTime</span></span>|<span data-ttu-id="e256e-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e256e-225">DateTimeOffset</span></span>|<span data-ttu-id="e256e-226">有効期限。</span><span class="sxs-lookup"><span data-stu-id="e256e-226">The expiration time.</span></span>|
|<span data-ttu-id="e256e-227">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="e256e-227">versionNumber</span></span>|<span data-ttu-id="e256e-228">String</span><span class="sxs-lookup"><span data-stu-id="e256e-228">String</span></span>|<span data-ttu-id="e256e-229">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="e256e-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e256e-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e256e-230">buildNumber</span></span>|<span data-ttu-id="e256e-231">String</span><span class="sxs-lookup"><span data-stu-id="e256e-231">String</span></span>|<span data-ttu-id="e256e-232">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="e256e-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e256e-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e256e-233">identityVersion</span></span>|<span data-ttu-id="e256e-234">String</span><span class="sxs-lookup"><span data-stu-id="e256e-234">String</span></span>|<span data-ttu-id="e256e-235">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e256e-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e256e-236">応答</span><span class="sxs-lookup"><span data-stu-id="e256e-236">Response</span></span>
<span data-ttu-id="e256e-237">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e256e-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e256e-238">例</span><span class="sxs-lookup"><span data-stu-id="e256e-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="e256e-239">要求</span><span class="sxs-lookup"><span data-stu-id="e256e-239">Request</span></span>
<span data-ttu-id="e256e-240">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e256e-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1366

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e256e-241">応答</span><span class="sxs-lookup"><span data-stu-id="e256e-241">Response</span></span>
<span data-ttu-id="e256e-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e256e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1529

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




