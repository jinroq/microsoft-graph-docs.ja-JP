---
title: microsoftStoreForBusinessApp の更新
description: microsoftStoreForBusinessApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5f2bee3e2cbbdd1f02bbd7a1779ea80b2340772
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417498"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="e2f3f-103">microsoftStoreForBusinessApp の更新</span><span class="sxs-lookup"><span data-stu-id="e2f3f-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="e2f3f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2f3f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2f3f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2f3f-107">[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2f3f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2f3f-108">Prerequisites</span></span>
<span data-ttu-id="e2f3f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e2f3f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2f3f-111">Permission type</span></span>|<span data-ttu-id="e2f3f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2f3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2f3f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2f3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2f3f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f3f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2f3f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2f3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f3f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-116">Not supported.</span></span>|
|<span data-ttu-id="e2f3f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2f3f-117">Application</span></span>|<span data-ttu-id="e2f3f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f3f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2f3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e2f3f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2f3f-120">Request headers</span></span>
|<span data-ttu-id="e2f3f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2f3f-121">Header</span></span>|<span data-ttu-id="e2f3f-122">値</span><span class="sxs-lookup"><span data-stu-id="e2f3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2f3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2f3f-123">Authorization</span></span>|<span data-ttu-id="e2f3f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2f3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2f3f-125">Accept</span></span>|<span data-ttu-id="e2f3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2f3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f3f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2f3f-127">Request body</span></span>
<span data-ttu-id="e2f3f-128">要求本文で、[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="e2f3f-129">次の表に、[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="e2f3f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2f3f-130">Property</span></span>|<span data-ttu-id="e2f3f-131">型</span><span class="sxs-lookup"><span data-stu-id="e2f3f-131">Type</span></span>|<span data-ttu-id="e2f3f-132">説明</span><span class="sxs-lookup"><span data-stu-id="e2f3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f3f-133">id</span><span class="sxs-lookup"><span data-stu-id="e2f3f-133">id</span></span>|<span data-ttu-id="e2f3f-134">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-134">String</span></span>|<span data-ttu-id="e2f3f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-135">Key of the entity.</span></span> <span data-ttu-id="e2f3f-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e2f3f-137">displayName</span></span>|<span data-ttu-id="e2f3f-138">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-138">String</span></span>|<span data-ttu-id="e2f3f-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e2f3f-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-141">説明</span><span class="sxs-lookup"><span data-stu-id="e2f3f-141">description</span></span>|<span data-ttu-id="e2f3f-142">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-142">String</span></span>|<span data-ttu-id="e2f3f-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-143">The description of the app.</span></span> <span data-ttu-id="e2f3f-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e2f3f-145">publisher</span></span>|<span data-ttu-id="e2f3f-146">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-146">String</span></span>|<span data-ttu-id="e2f3f-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-147">The publisher of the app.</span></span> <span data-ttu-id="e2f3f-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e2f3f-149">largeIcon</span></span>|[<span data-ttu-id="e2f3f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2f3f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2f3f-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e2f3f-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f3f-153">createdDateTime</span></span>|<span data-ttu-id="e2f3f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f3f-154">DateTimeOffset</span></span>|<span data-ttu-id="e2f3f-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-155">The date and time the app was created.</span></span> <span data-ttu-id="e2f3f-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f3f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e2f3f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f3f-158">DateTimeOffset</span></span>|<span data-ttu-id="e2f3f-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e2f3f-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e2f3f-161">isFeatured</span></span>|<span data-ttu-id="e2f3f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2f3f-162">Boolean</span></span>|<span data-ttu-id="e2f3f-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2f3f-164">privacyInformationUrl</span></span>|<span data-ttu-id="e2f3f-165">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-165">String</span></span>|<span data-ttu-id="e2f3f-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-166">The privacy statement Url.</span></span> <span data-ttu-id="e2f3f-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2f3f-168">informationUrl</span></span>|<span data-ttu-id="e2f3f-169">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-169">String</span></span>|<span data-ttu-id="e2f3f-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-170">The more information Url.</span></span> <span data-ttu-id="e2f3f-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-172">owner</span><span class="sxs-lookup"><span data-stu-id="e2f3f-172">owner</span></span>|<span data-ttu-id="e2f3f-173">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-173">String</span></span>|<span data-ttu-id="e2f3f-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-174">The owner of the app.</span></span> <span data-ttu-id="e2f3f-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-176">developer</span><span class="sxs-lookup"><span data-stu-id="e2f3f-176">developer</span></span>|<span data-ttu-id="e2f3f-177">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-177">String</span></span>|<span data-ttu-id="e2f3f-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-178">The developer of the app.</span></span> <span data-ttu-id="e2f3f-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-180">notes</span><span class="sxs-lookup"><span data-stu-id="e2f3f-180">notes</span></span>|<span data-ttu-id="e2f3f-181">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-181">String</span></span>|<span data-ttu-id="e2f3f-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-182">Notes for the app.</span></span> <span data-ttu-id="e2f3f-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e2f3f-184">uploadState</span></span>|<span data-ttu-id="e2f3f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f3f-185">Int32</span></span>|<span data-ttu-id="e2f3f-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-186">The upload state.</span></span> <span data-ttu-id="e2f3f-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e2f3f-188">publishingState</span></span>|[<span data-ttu-id="e2f3f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e2f3f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e2f3f-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-190">The publishing state for the app.</span></span> <span data-ttu-id="e2f3f-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e2f3f-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e2f3f-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e2f3f-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e2f3f-194">isAssigned</span></span>|<span data-ttu-id="e2f3f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2f3f-195">Boolean</span></span>|<span data-ttu-id="e2f3f-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e2f3f-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2f3f-198">roleScopeTagIds</span></span>|<span data-ttu-id="e2f3f-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e2f3f-199">String collection</span></span>|<span data-ttu-id="e2f3f-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e2f3f-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e2f3f-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2f3f-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e2f3f-202">usedLicenseCount</span></span>|<span data-ttu-id="e2f3f-203">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f3f-203">Int32</span></span>|<span data-ttu-id="e2f3f-204">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-204">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="e2f3f-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e2f3f-205">totalLicenseCount</span></span>|<span data-ttu-id="e2f3f-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f3f-206">Int32</span></span>|<span data-ttu-id="e2f3f-207">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-207">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="e2f3f-208">productKey</span><span class="sxs-lookup"><span data-stu-id="e2f3f-208">productKey</span></span>|<span data-ttu-id="e2f3f-209">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-209">String</span></span>|<span data-ttu-id="e2f3f-210">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="e2f3f-210">The app product key</span></span>|
|<span data-ttu-id="e2f3f-211">licenseType</span><span class="sxs-lookup"><span data-stu-id="e2f3f-211">licenseType</span></span>|[<span data-ttu-id="e2f3f-212">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="e2f3f-212">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="e2f3f-213">アプリケーション ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-213">The app license type.</span></span> <span data-ttu-id="e2f3f-214">使用可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-214">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="e2f3f-215">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="e2f3f-215">packageIdentityName</span></span>|<span data-ttu-id="e2f3f-216">String</span><span class="sxs-lookup"><span data-stu-id="e2f3f-216">String</span></span>|<span data-ttu-id="e2f3f-217">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="e2f3f-217">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="e2f3f-218">応答</span><span class="sxs-lookup"><span data-stu-id="e2f3f-218">Response</span></span>
<span data-ttu-id="e2f3f-219">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-219">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2f3f-220">例</span><span class="sxs-lookup"><span data-stu-id="e2f3f-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2f3f-221">要求</span><span class="sxs-lookup"><span data-stu-id="e2f3f-221">Request</span></span>
<span data-ttu-id="e2f3f-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="e2f3f-223">応答</span><span class="sxs-lookup"><span data-stu-id="e2f3f-223">Response</span></span>
<span data-ttu-id="e2f3f-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2f3f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```




