---
title: Create microsoftStoreForBusinessApp
description: 新しい microsoftStoreForBusinessApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15592dbce6bb1fc2665dbfcbc5fc9075cc1420c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961246"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="e5ef1-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="e5ef1-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="e5ef1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5ef1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ef1-106">新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5ef1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5ef1-107">Prerequisites</span></span>
<span data-ttu-id="e5ef1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5ef1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5ef1-110">Permission type</span></span>|<span data-ttu-id="e5ef1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5ef1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5ef1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5ef1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5ef1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ef1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5ef1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5ef1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5ef1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-115">Not supported.</span></span>|
|<span data-ttu-id="e5ef1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5ef1-116">Application</span></span>|<span data-ttu-id="e5ef1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5ef1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5ef1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5ef1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5ef1-119">Request headers</span></span>
|<span data-ttu-id="e5ef1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5ef1-120">Header</span></span>|<span data-ttu-id="e5ef1-121">値</span><span class="sxs-lookup"><span data-stu-id="e5ef1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5ef1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5ef1-122">Authorization</span></span>|<span data-ttu-id="e5ef1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5ef1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e5ef1-124">Accept</span></span>|<span data-ttu-id="e5ef1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5ef1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5ef1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5ef1-126">Request body</span></span>
<span data-ttu-id="e5ef1-127">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="e5ef1-128">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="e5ef1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5ef1-129">Property</span></span>|<span data-ttu-id="e5ef1-130">型</span><span class="sxs-lookup"><span data-stu-id="e5ef1-130">Type</span></span>|<span data-ttu-id="e5ef1-131">説明</span><span class="sxs-lookup"><span data-stu-id="e5ef1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5ef1-132">id</span><span class="sxs-lookup"><span data-stu-id="e5ef1-132">id</span></span>|<span data-ttu-id="e5ef1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e5ef1-133">String</span></span>|<span data-ttu-id="e5ef1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-134">Key of the entity.</span></span> <span data-ttu-id="e5ef1-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e5ef1-136">displayName</span></span>|<span data-ttu-id="e5ef1-137">文字列</span><span class="sxs-lookup"><span data-stu-id="e5ef1-137">String</span></span>|<span data-ttu-id="e5ef1-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5ef1-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-140">description</span><span class="sxs-lookup"><span data-stu-id="e5ef1-140">description</span></span>|<span data-ttu-id="e5ef1-141">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-141">String</span></span>|<span data-ttu-id="e5ef1-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-142">The description of the app.</span></span> <span data-ttu-id="e5ef1-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e5ef1-144">publisher</span></span>|<span data-ttu-id="e5ef1-145">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-145">String</span></span>|<span data-ttu-id="e5ef1-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-146">The publisher of the app.</span></span> <span data-ttu-id="e5ef1-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5ef1-148">largeIcon</span></span>|[<span data-ttu-id="e5ef1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5ef1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5ef1-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5ef1-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5ef1-152">createdDateTime</span></span>|<span data-ttu-id="e5ef1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5ef1-153">DateTimeOffset</span></span>|<span data-ttu-id="e5ef1-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-154">The date and time the app was created.</span></span> <span data-ttu-id="e5ef1-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5ef1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e5ef1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5ef1-157">DateTimeOffset</span></span>|<span data-ttu-id="e5ef1-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e5ef1-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5ef1-160">isFeatured</span></span>|<span data-ttu-id="e5ef1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5ef1-161">Boolean</span></span>|<span data-ttu-id="e5ef1-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5ef1-163">privacyInformationUrl</span></span>|<span data-ttu-id="e5ef1-164">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-164">String</span></span>|<span data-ttu-id="e5ef1-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-165">The privacy statement Url.</span></span> <span data-ttu-id="e5ef1-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5ef1-167">informationUrl</span></span>|<span data-ttu-id="e5ef1-168">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-168">String</span></span>|<span data-ttu-id="e5ef1-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-169">The more information Url.</span></span> <span data-ttu-id="e5ef1-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-171">owner</span><span class="sxs-lookup"><span data-stu-id="e5ef1-171">owner</span></span>|<span data-ttu-id="e5ef1-172">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-172">String</span></span>|<span data-ttu-id="e5ef1-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-173">The owner of the app.</span></span> <span data-ttu-id="e5ef1-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-175">developer</span><span class="sxs-lookup"><span data-stu-id="e5ef1-175">developer</span></span>|<span data-ttu-id="e5ef1-176">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-176">String</span></span>|<span data-ttu-id="e5ef1-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-177">The developer of the app.</span></span> <span data-ttu-id="e5ef1-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-179">notes</span><span class="sxs-lookup"><span data-stu-id="e5ef1-179">notes</span></span>|<span data-ttu-id="e5ef1-180">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-180">String</span></span>|<span data-ttu-id="e5ef1-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-181">Notes for the app.</span></span> <span data-ttu-id="e5ef1-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5ef1-183">uploadState</span></span>|<span data-ttu-id="e5ef1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ef1-184">Int32</span></span>|<span data-ttu-id="e5ef1-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-185">The upload state.</span></span> <span data-ttu-id="e5ef1-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5ef1-187">publishingState</span></span>|[<span data-ttu-id="e5ef1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e5ef1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5ef1-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-189">The publishing state for the app.</span></span> <span data-ttu-id="e5ef1-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5ef1-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e5ef1-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5ef1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e5ef1-193">isAssigned</span></span>|<span data-ttu-id="e5ef1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5ef1-194">Boolean</span></span>|<span data-ttu-id="e5ef1-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e5ef1-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5ef1-197">roleScopeTagIds</span></span>|<span data-ttu-id="e5ef1-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e5ef1-198">String collection</span></span>|<span data-ttu-id="e5ef1-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e5ef1-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e5ef1-201">dependentAppCount</span></span>|<span data-ttu-id="e5ef1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ef1-202">Int32</span></span>|<span data-ttu-id="e5ef1-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e5ef1-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5ef1-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5ef1-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5ef1-205">usedLicenseCount</span></span>|<span data-ttu-id="e5ef1-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ef1-206">Int32</span></span>|<span data-ttu-id="e5ef1-207">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="e5ef1-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5ef1-208">totalLicenseCount</span></span>|<span data-ttu-id="e5ef1-209">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ef1-209">Int32</span></span>|<span data-ttu-id="e5ef1-210">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="e5ef1-211">productKey</span><span class="sxs-lookup"><span data-stu-id="e5ef1-211">productKey</span></span>|<span data-ttu-id="e5ef1-212">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-212">String</span></span>|<span data-ttu-id="e5ef1-213">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="e5ef1-213">The app product key</span></span>|
|<span data-ttu-id="e5ef1-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="e5ef1-214">licenseType</span></span>|[<span data-ttu-id="e5ef1-215">Microsoft Storeforbusinesslicensetype</span><span class="sxs-lookup"><span data-stu-id="e5ef1-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="e5ef1-216">アプリライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-216">The app license type.</span></span> <span data-ttu-id="e5ef1-217">可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="e5ef1-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="e5ef1-218">packageIdentityName</span></span>|<span data-ttu-id="e5ef1-219">String</span><span class="sxs-lookup"><span data-stu-id="e5ef1-219">String</span></span>|<span data-ttu-id="e5ef1-220">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="e5ef1-220">The app package identifier</span></span>|
|<span data-ttu-id="e5ef1-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="e5ef1-221">licensingType</span></span>|[<span data-ttu-id="e5ef1-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e5ef1-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="e5ef1-223">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="e5ef1-224">応答</span><span class="sxs-lookup"><span data-stu-id="e5ef1-224">Response</span></span>
<span data-ttu-id="e5ef1-225">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-225">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5ef1-226">例</span><span class="sxs-lookup"><span data-stu-id="e5ef1-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5ef1-227">要求</span><span class="sxs-lookup"><span data-stu-id="e5ef1-227">Request</span></span>
<span data-ttu-id="e5ef1-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1132

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
  "dependentAppCount": 1,
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="e5ef1-229">応答</span><span class="sxs-lookup"><span data-stu-id="e5ef1-229">Response</span></span>
<span data-ttu-id="e5ef1-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5ef1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1304

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
  "dependentAppCount": 1,
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```





