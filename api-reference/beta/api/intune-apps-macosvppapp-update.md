---
title: MacOsVppApp の更新
description: MacOsVppApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94dcb03417fd23367b263704bb099c23e5e255ea
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330133"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="85c05-103">MacOsVppApp の更新</span><span class="sxs-lookup"><span data-stu-id="85c05-103">Update macOsVppApp</span></span>

> <span data-ttu-id="85c05-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85c05-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85c05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85c05-106">[MacOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="85c05-106">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85c05-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="85c05-107">Prerequisites</span></span>
<span data-ttu-id="85c05-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85c05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c05-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85c05-110">Permission type</span></span>|<span data-ttu-id="85c05-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85c05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85c05-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85c05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85c05-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c05-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85c05-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85c05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85c05-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c05-115">Not supported.</span></span>|
|<span data-ttu-id="85c05-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85c05-116">Application</span></span>|<span data-ttu-id="85c05-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c05-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85c05-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85c05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="85c05-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85c05-119">Request headers</span></span>
|<span data-ttu-id="85c05-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85c05-120">Header</span></span>|<span data-ttu-id="85c05-121">値</span><span class="sxs-lookup"><span data-stu-id="85c05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85c05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c05-122">Authorization</span></span>|<span data-ttu-id="85c05-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="85c05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85c05-124">承諾</span><span class="sxs-lookup"><span data-stu-id="85c05-124">Accept</span></span>|<span data-ttu-id="85c05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85c05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85c05-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="85c05-126">Request body</span></span>
<span data-ttu-id="85c05-127">要求本文で、 [macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="85c05-127">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="85c05-128">次の表に、 [macOsVppApp](../resources/intune-apps-macosvppapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="85c05-128">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="85c05-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85c05-129">Property</span></span>|<span data-ttu-id="85c05-130">型</span><span class="sxs-lookup"><span data-stu-id="85c05-130">Type</span></span>|<span data-ttu-id="85c05-131">説明</span><span class="sxs-lookup"><span data-stu-id="85c05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c05-132">id</span><span class="sxs-lookup"><span data-stu-id="85c05-132">id</span></span>|<span data-ttu-id="85c05-133">文字列</span><span class="sxs-lookup"><span data-stu-id="85c05-133">String</span></span>|<span data-ttu-id="85c05-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="85c05-134">Key of the entity.</span></span> <span data-ttu-id="85c05-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85c05-136">displayName</span></span>|<span data-ttu-id="85c05-137">文字列</span><span class="sxs-lookup"><span data-stu-id="85c05-137">String</span></span>|<span data-ttu-id="85c05-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="85c05-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85c05-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-140">description</span><span class="sxs-lookup"><span data-stu-id="85c05-140">description</span></span>|<span data-ttu-id="85c05-141">String</span><span class="sxs-lookup"><span data-stu-id="85c05-141">String</span></span>|<span data-ttu-id="85c05-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="85c05-142">The description of the app.</span></span> <span data-ttu-id="85c05-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-144">publisher</span><span class="sxs-lookup"><span data-stu-id="85c05-144">publisher</span></span>|<span data-ttu-id="85c05-145">String</span><span class="sxs-lookup"><span data-stu-id="85c05-145">String</span></span>|<span data-ttu-id="85c05-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="85c05-146">The publisher of the app.</span></span> <span data-ttu-id="85c05-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85c05-148">largeIcon</span></span>|[<span data-ttu-id="85c05-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85c05-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85c05-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="85c05-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85c05-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85c05-152">createdDateTime</span></span>|<span data-ttu-id="85c05-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c05-153">DateTimeOffset</span></span>|<span data-ttu-id="85c05-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="85c05-154">The date and time the app was created.</span></span> <span data-ttu-id="85c05-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85c05-156">lastModifiedDateTime</span></span>|<span data-ttu-id="85c05-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c05-157">DateTimeOffset</span></span>|<span data-ttu-id="85c05-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="85c05-158">The date and time the app was last modified.</span></span> <span data-ttu-id="85c05-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85c05-160">isFeatured</span></span>|<span data-ttu-id="85c05-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="85c05-161">Boolean</span></span>|<span data-ttu-id="85c05-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85c05-163">privacyInformationUrl</span></span>|<span data-ttu-id="85c05-164">String</span><span class="sxs-lookup"><span data-stu-id="85c05-164">String</span></span>|<span data-ttu-id="85c05-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="85c05-165">The privacy statement Url.</span></span> <span data-ttu-id="85c05-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85c05-167">informationUrl</span></span>|<span data-ttu-id="85c05-168">String</span><span class="sxs-lookup"><span data-stu-id="85c05-168">String</span></span>|<span data-ttu-id="85c05-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="85c05-169">The more information Url.</span></span> <span data-ttu-id="85c05-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-171">owner</span><span class="sxs-lookup"><span data-stu-id="85c05-171">owner</span></span>|<span data-ttu-id="85c05-172">String</span><span class="sxs-lookup"><span data-stu-id="85c05-172">String</span></span>|<span data-ttu-id="85c05-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="85c05-173">The owner of the app.</span></span> <span data-ttu-id="85c05-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-175">developer</span><span class="sxs-lookup"><span data-stu-id="85c05-175">developer</span></span>|<span data-ttu-id="85c05-176">String</span><span class="sxs-lookup"><span data-stu-id="85c05-176">String</span></span>|<span data-ttu-id="85c05-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="85c05-177">The developer of the app.</span></span> <span data-ttu-id="85c05-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-179">notes</span><span class="sxs-lookup"><span data-stu-id="85c05-179">notes</span></span>|<span data-ttu-id="85c05-180">String</span><span class="sxs-lookup"><span data-stu-id="85c05-180">String</span></span>|<span data-ttu-id="85c05-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="85c05-181">Notes for the app.</span></span> <span data-ttu-id="85c05-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="85c05-183">uploadState</span></span>|<span data-ttu-id="85c05-184">Int32</span><span class="sxs-lookup"><span data-stu-id="85c05-184">Int32</span></span>|<span data-ttu-id="85c05-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="85c05-185">The upload state.</span></span> <span data-ttu-id="85c05-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="85c05-187">publishingState</span></span>|[<span data-ttu-id="85c05-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="85c05-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="85c05-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="85c05-189">The publishing state for the app.</span></span> <span data-ttu-id="85c05-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="85c05-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85c05-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="85c05-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="85c05-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="85c05-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="85c05-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="85c05-193">isAssigned</span></span>|<span data-ttu-id="85c05-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="85c05-194">Boolean</span></span>|<span data-ttu-id="85c05-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="85c05-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="85c05-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85c05-197">roleScopeTagIds</span></span>|<span data-ttu-id="85c05-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="85c05-198">String collection</span></span>|<span data-ttu-id="85c05-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="85c05-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="85c05-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="85c05-201">dependentAppCount</span></span>|<span data-ttu-id="85c05-202">Int32</span><span class="sxs-lookup"><span data-stu-id="85c05-202">Int32</span></span>|<span data-ttu-id="85c05-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="85c05-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="85c05-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="85c05-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85c05-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="85c05-205">usedLicenseCount</span></span>|<span data-ttu-id="85c05-206">Int32</span><span class="sxs-lookup"><span data-stu-id="85c05-206">Int32</span></span>|<span data-ttu-id="85c05-207">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="85c05-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="85c05-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="85c05-208">totalLicenseCount</span></span>|<span data-ttu-id="85c05-209">Int32</span><span class="sxs-lookup"><span data-stu-id="85c05-209">Int32</span></span>|<span data-ttu-id="85c05-210">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="85c05-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="85c05-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="85c05-211">releaseDateTime</span></span>|<span data-ttu-id="85c05-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c05-212">DateTimeOffset</span></span>|<span data-ttu-id="85c05-213">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="85c05-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="85c05-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="85c05-214">appStoreUrl</span></span>|<span data-ttu-id="85c05-215">String</span><span class="sxs-lookup"><span data-stu-id="85c05-215">String</span></span>|<span data-ttu-id="85c05-216">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="85c05-216">The store URL.</span></span>|
|<span data-ttu-id="85c05-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="85c05-217">licensingType</span></span>|[<span data-ttu-id="85c05-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="85c05-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="85c05-219">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="85c05-219">The supported License Type.</span></span>|
|<span data-ttu-id="85c05-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="85c05-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="85c05-221">String</span><span class="sxs-lookup"><span data-stu-id="85c05-221">String</span></span>|<span data-ttu-id="85c05-222">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="85c05-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="85c05-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="85c05-223">vppTokenAccountType</span></span>|[<span data-ttu-id="85c05-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="85c05-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="85c05-225">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="85c05-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="85c05-226">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="85c05-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="85c05-227">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="85c05-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="85c05-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="85c05-228">vppTokenAppleId</span></span>|<span data-ttu-id="85c05-229">String</span><span class="sxs-lookup"><span data-stu-id="85c05-229">String</span></span>|<span data-ttu-id="85c05-230">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="85c05-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="85c05-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="85c05-231">bundleId</span></span>|<span data-ttu-id="85c05-232">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="85c05-232">String</span></span>|<span data-ttu-id="85c05-233">ID 名。</span><span class="sxs-lookup"><span data-stu-id="85c05-233">The Identity Name.</span></span>|
|<span data-ttu-id="85c05-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="85c05-234">vppTokenId</span></span>|<span data-ttu-id="85c05-235">String</span><span class="sxs-lookup"><span data-stu-id="85c05-235">String</span></span>|<span data-ttu-id="85c05-236">このアプリに関連付けられている VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="85c05-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="85c05-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="85c05-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="85c05-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85c05-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="85c05-239">このアプリでのライセンスの取り消しアクションの結果。</span><span class="sxs-lookup"><span data-stu-id="85c05-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="85c05-240">応答</span><span class="sxs-lookup"><span data-stu-id="85c05-240">Response</span></span>
<span data-ttu-id="85c05-241">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="85c05-241">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c05-242">例</span><span class="sxs-lookup"><span data-stu-id="85c05-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="85c05-243">要求</span><span class="sxs-lookup"><span data-stu-id="85c05-243">Request</span></span>
<span data-ttu-id="85c05-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85c05-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1869

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="85c05-245">応答</span><span class="sxs-lookup"><span data-stu-id="85c05-245">Response</span></span>
<span data-ttu-id="85c05-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85c05-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2041

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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






