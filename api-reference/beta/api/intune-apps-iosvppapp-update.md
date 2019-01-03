---
title: iosVppApp の更新
description: iosVppApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 0f95b23bcde4d48e8e17724e6fd5b4b26992df1a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341525"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="94b9a-103">iosVppApp の更新</span><span class="sxs-lookup"><span data-stu-id="94b9a-103">Update iosVppApp</span></span>

> <span data-ttu-id="94b9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94b9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94b9a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="94b9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94b9a-107">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94b9a-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94b9a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="94b9a-108">Prerequisites</span></span>
<span data-ttu-id="94b9a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94b9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b9a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94b9a-111">Permission type</span></span>|<span data-ttu-id="94b9a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94b9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94b9a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94b9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94b9a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b9a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94b9a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94b9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94b9a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b9a-116">Not supported.</span></span>|
|<span data-ttu-id="94b9a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94b9a-117">Application</span></span>|<span data-ttu-id="94b9a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94b9a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94b9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="94b9a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94b9a-120">Request headers</span></span>
|<span data-ttu-id="94b9a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94b9a-121">Header</span></span>|<span data-ttu-id="94b9a-122">値</span><span class="sxs-lookup"><span data-stu-id="94b9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94b9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94b9a-123">Authorization</span></span>|<span data-ttu-id="94b9a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="94b9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94b9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94b9a-125">Accept</span></span>|<span data-ttu-id="94b9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94b9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94b9a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="94b9a-127">Request body</span></span>
<span data-ttu-id="94b9a-128">要求本文で、[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94b9a-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="94b9a-129">次の表に、[iosVppApp](../resources/intune-apps-iosvppapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="94b9a-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="94b9a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94b9a-130">Property</span></span>|<span data-ttu-id="94b9a-131">種類</span><span class="sxs-lookup"><span data-stu-id="94b9a-131">Type</span></span>|<span data-ttu-id="94b9a-132">説明</span><span class="sxs-lookup"><span data-stu-id="94b9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b9a-133">ID</span><span class="sxs-lookup"><span data-stu-id="94b9a-133">id</span></span>|<span data-ttu-id="94b9a-134">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-134">String</span></span>|<span data-ttu-id="94b9a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="94b9a-135">Key of the entity.</span></span> <span data-ttu-id="94b9a-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="94b9a-137">displayName</span></span>|<span data-ttu-id="94b9a-138">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-138">String</span></span>|<span data-ttu-id="94b9a-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="94b9a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="94b9a-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-141">説明</span><span class="sxs-lookup"><span data-stu-id="94b9a-141">description</span></span>|<span data-ttu-id="94b9a-142">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-142">String</span></span>|<span data-ttu-id="94b9a-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="94b9a-143">The description of the app.</span></span> <span data-ttu-id="94b9a-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="94b9a-145">publisher</span></span>|<span data-ttu-id="94b9a-146">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-146">String</span></span>|<span data-ttu-id="94b9a-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="94b9a-147">The publisher of the app.</span></span> <span data-ttu-id="94b9a-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="94b9a-149">largeIcon</span></span>|[<span data-ttu-id="94b9a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="94b9a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="94b9a-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="94b9a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="94b9a-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94b9a-153">createdDateTime</span></span>|<span data-ttu-id="94b9a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b9a-154">DateTimeOffset</span></span>|<span data-ttu-id="94b9a-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="94b9a-155">The date and time the app was created.</span></span> <span data-ttu-id="94b9a-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94b9a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="94b9a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b9a-158">DateTimeOffset</span></span>|<span data-ttu-id="94b9a-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="94b9a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="94b9a-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="94b9a-161">isFeatured</span></span>|<span data-ttu-id="94b9a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="94b9a-162">Boolean</span></span>|<span data-ttu-id="94b9a-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="94b9a-164">privacyInformationUrl</span></span>|<span data-ttu-id="94b9a-165">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-165">String</span></span>|<span data-ttu-id="94b9a-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="94b9a-166">The privacy statement Url.</span></span> <span data-ttu-id="94b9a-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="94b9a-168">informationUrl</span></span>|<span data-ttu-id="94b9a-169">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-169">String</span></span>|<span data-ttu-id="94b9a-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="94b9a-170">The more information Url.</span></span> <span data-ttu-id="94b9a-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-172">owner</span><span class="sxs-lookup"><span data-stu-id="94b9a-172">owner</span></span>|<span data-ttu-id="94b9a-173">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-173">String</span></span>|<span data-ttu-id="94b9a-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="94b9a-174">The owner of the app.</span></span> <span data-ttu-id="94b9a-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-176">developer</span><span class="sxs-lookup"><span data-stu-id="94b9a-176">developer</span></span>|<span data-ttu-id="94b9a-177">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-177">String</span></span>|<span data-ttu-id="94b9a-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="94b9a-178">The developer of the app.</span></span> <span data-ttu-id="94b9a-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-180">notes</span><span class="sxs-lookup"><span data-stu-id="94b9a-180">notes</span></span>|<span data-ttu-id="94b9a-181">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-181">String</span></span>|<span data-ttu-id="94b9a-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="94b9a-182">Notes for the app.</span></span> <span data-ttu-id="94b9a-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="94b9a-184">uploadState</span></span>|<span data-ttu-id="94b9a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="94b9a-185">Int32</span></span>|<span data-ttu-id="94b9a-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-186">The upload state.</span></span> <span data-ttu-id="94b9a-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94b9a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94b9a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="94b9a-188">publishingState</span></span>|[<span data-ttu-id="94b9a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="94b9a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="94b9a-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="94b9a-190">The publishing state for the app.</span></span> <span data-ttu-id="94b9a-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="94b9a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="94b9a-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="94b9a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="94b9a-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="94b9a-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="94b9a-194">usedLicenseCount</span></span>|<span data-ttu-id="94b9a-195">Int32</span><span class="sxs-lookup"><span data-stu-id="94b9a-195">Int32</span></span>|<span data-ttu-id="94b9a-196">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="94b9a-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="94b9a-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="94b9a-197">totalLicenseCount</span></span>|<span data-ttu-id="94b9a-198">Int32</span><span class="sxs-lookup"><span data-stu-id="94b9a-198">Int32</span></span>|<span data-ttu-id="94b9a-199">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="94b9a-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="94b9a-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="94b9a-200">releaseDateTime</span></span>|<span data-ttu-id="94b9a-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b9a-201">DateTimeOffset</span></span>|<span data-ttu-id="94b9a-202">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="94b9a-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="94b9a-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="94b9a-203">appStoreUrl</span></span>|<span data-ttu-id="94b9a-204">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-204">String</span></span>|<span data-ttu-id="94b9a-205">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="94b9a-205">The store URL.</span></span>|
|<span data-ttu-id="94b9a-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="94b9a-206">licensingType</span></span>|[<span data-ttu-id="94b9a-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="94b9a-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="94b9a-208">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="94b9a-208">The supported License Type.</span></span>|
|<span data-ttu-id="94b9a-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="94b9a-209">applicableDeviceType</span></span>|[<span data-ttu-id="94b9a-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="94b9a-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="94b9a-211">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="94b9a-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="94b9a-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="94b9a-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="94b9a-213">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-213">String</span></span>|<span data-ttu-id="94b9a-214">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="94b9a-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="94b9a-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="94b9a-215">vppTokenAccountType</span></span>|[<span data-ttu-id="94b9a-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="94b9a-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="94b9a-217">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="94b9a-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="94b9a-218">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="94b9a-219">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="94b9a-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="94b9a-220">vppTokenAppleId</span></span>|<span data-ttu-id="94b9a-221">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-221">String</span></span>|<span data-ttu-id="94b9a-222">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="94b9a-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="94b9a-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="94b9a-223">bundleId</span></span>|<span data-ttu-id="94b9a-224">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-224">String</span></span>|<span data-ttu-id="94b9a-225">ID 名。</span><span class="sxs-lookup"><span data-stu-id="94b9a-225">The Identity Name.</span></span>|
|<span data-ttu-id="94b9a-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="94b9a-226">vppTokenId</span></span>|<span data-ttu-id="94b9a-227">String</span><span class="sxs-lookup"><span data-stu-id="94b9a-227">String</span></span>|<span data-ttu-id="94b9a-228">このアプリケーションに関連付けられている VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="94b9a-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="94b9a-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="94b9a-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="94b9a-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="94b9a-231">結果は、このアプリケーションについてのライセンスを失効します。</span><span class="sxs-lookup"><span data-stu-id="94b9a-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="94b9a-232">応答</span><span class="sxs-lookup"><span data-stu-id="94b9a-232">Response</span></span>
<span data-ttu-id="94b9a-233">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="94b9a-233">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94b9a-234">例</span><span class="sxs-lookup"><span data-stu-id="94b9a-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="94b9a-235">要求</span><span class="sxs-lookup"><span data-stu-id="94b9a-235">Request</span></span>
<span data-ttu-id="94b9a-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94b9a-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1903

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="94b9a-237">応答</span><span class="sxs-lookup"><span data-stu-id="94b9a-237">Response</span></span>
<span data-ttu-id="94b9a-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94b9a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




