---
title: androidmanagedstoreapp の更新
description: androidmanagedstoreapp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5030ce96a61cb3f69ab2de5ab518cff3136d41c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496878"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="c93cc-103">androidmanagedstoreapp の更新</span><span class="sxs-lookup"><span data-stu-id="c93cc-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="c93cc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c93cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c93cc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c93cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c93cc-106">[androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c93cc-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c93cc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c93cc-107">Prerequisites</span></span>
<span data-ttu-id="c93cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c93cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c93cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c93cc-110">Permission type</span></span>|<span data-ttu-id="c93cc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c93cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c93cc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c93cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c93cc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93cc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c93cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c93cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c93cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c93cc-115">Not supported.</span></span>|
|<span data-ttu-id="c93cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c93cc-116">Application</span></span>|<span data-ttu-id="c93cc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c93cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c93cc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c93cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c93cc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c93cc-119">Request headers</span></span>
|<span data-ttu-id="c93cc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c93cc-120">Header</span></span>|<span data-ttu-id="c93cc-121">値</span><span class="sxs-lookup"><span data-stu-id="c93cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c93cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c93cc-122">Authorization</span></span>|<span data-ttu-id="c93cc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c93cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c93cc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c93cc-124">Accept</span></span>|<span data-ttu-id="c93cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c93cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c93cc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c93cc-126">Request body</span></span>
<span data-ttu-id="c93cc-127">要求本文で、 [androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c93cc-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="c93cc-128">次の表に、 [androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c93cc-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="c93cc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c93cc-129">Property</span></span>|<span data-ttu-id="c93cc-130">型</span><span class="sxs-lookup"><span data-stu-id="c93cc-130">Type</span></span>|<span data-ttu-id="c93cc-131">説明</span><span class="sxs-lookup"><span data-stu-id="c93cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c93cc-132">id</span><span class="sxs-lookup"><span data-stu-id="c93cc-132">id</span></span>|<span data-ttu-id="c93cc-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c93cc-133">String</span></span>|<span data-ttu-id="c93cc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c93cc-134">Key of the entity.</span></span> <span data-ttu-id="c93cc-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c93cc-136">displayName</span></span>|<span data-ttu-id="c93cc-137">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-137">String</span></span>|<span data-ttu-id="c93cc-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c93cc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c93cc-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-140">説明</span><span class="sxs-lookup"><span data-stu-id="c93cc-140">description</span></span>|<span data-ttu-id="c93cc-141">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-141">String</span></span>|<span data-ttu-id="c93cc-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c93cc-142">The description of the app.</span></span> <span data-ttu-id="c93cc-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c93cc-144">publisher</span></span>|<span data-ttu-id="c93cc-145">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-145">String</span></span>|<span data-ttu-id="c93cc-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c93cc-146">The publisher of the app.</span></span> <span data-ttu-id="c93cc-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c93cc-148">largeIcon</span></span>|[<span data-ttu-id="c93cc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c93cc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c93cc-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="c93cc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c93cc-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c93cc-152">createdDateTime</span></span>|<span data-ttu-id="c93cc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c93cc-153">DateTimeOffset</span></span>|<span data-ttu-id="c93cc-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c93cc-154">The date and time the app was created.</span></span> <span data-ttu-id="c93cc-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c93cc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c93cc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c93cc-157">DateTimeOffset</span></span>|<span data-ttu-id="c93cc-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c93cc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c93cc-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c93cc-160">isFeatured</span></span>|<span data-ttu-id="c93cc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c93cc-161">Boolean</span></span>|<span data-ttu-id="c93cc-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c93cc-163">privacyInformationUrl</span></span>|<span data-ttu-id="c93cc-164">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-164">String</span></span>|<span data-ttu-id="c93cc-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c93cc-165">The privacy statement Url.</span></span> <span data-ttu-id="c93cc-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c93cc-167">informationUrl</span></span>|<span data-ttu-id="c93cc-168">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-168">String</span></span>|<span data-ttu-id="c93cc-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c93cc-169">The more information Url.</span></span> <span data-ttu-id="c93cc-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-171">owner</span><span class="sxs-lookup"><span data-stu-id="c93cc-171">owner</span></span>|<span data-ttu-id="c93cc-172">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-172">String</span></span>|<span data-ttu-id="c93cc-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c93cc-173">The owner of the app.</span></span> <span data-ttu-id="c93cc-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-175">developer</span><span class="sxs-lookup"><span data-stu-id="c93cc-175">developer</span></span>|<span data-ttu-id="c93cc-176">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-176">String</span></span>|<span data-ttu-id="c93cc-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c93cc-177">The developer of the app.</span></span> <span data-ttu-id="c93cc-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-179">notes</span><span class="sxs-lookup"><span data-stu-id="c93cc-179">notes</span></span>|<span data-ttu-id="c93cc-180">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-180">String</span></span>|<span data-ttu-id="c93cc-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c93cc-181">Notes for the app.</span></span> <span data-ttu-id="c93cc-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c93cc-183">uploadState</span></span>|<span data-ttu-id="c93cc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c93cc-184">Int32</span></span>|<span data-ttu-id="c93cc-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="c93cc-185">The upload state.</span></span> <span data-ttu-id="c93cc-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c93cc-187">publishingState</span></span>|[<span data-ttu-id="c93cc-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c93cc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c93cc-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c93cc-189">The publishing state for the app.</span></span> <span data-ttu-id="c93cc-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c93cc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c93cc-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c93cc-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c93cc-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c93cc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c93cc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c93cc-193">isAssigned</span></span>|<span data-ttu-id="c93cc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c93cc-194">Boolean</span></span>|<span data-ttu-id="c93cc-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c93cc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c93cc-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c93cc-197">roleScopeTagIds</span></span>|<span data-ttu-id="c93cc-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c93cc-198">String collection</span></span>|<span data-ttu-id="c93cc-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="c93cc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c93cc-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="c93cc-201">dependentAppCount</span></span>|<span data-ttu-id="c93cc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c93cc-202">Int32</span></span>|<span data-ttu-id="c93cc-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="c93cc-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c93cc-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c93cc-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c93cc-205">packageId</span><span class="sxs-lookup"><span data-stu-id="c93cc-205">packageId</span></span>|<span data-ttu-id="c93cc-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c93cc-206">String</span></span>|<span data-ttu-id="c93cc-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="c93cc-207">The package identifier.</span></span>|
|<span data-ttu-id="c93cc-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c93cc-208">appIdentifier</span></span>|<span data-ttu-id="c93cc-209">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-209">String</span></span>|<span data-ttu-id="c93cc-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="c93cc-210">The Identity Name.</span></span>|
|<span data-ttu-id="c93cc-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c93cc-211">usedLicenseCount</span></span>|<span data-ttu-id="c93cc-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c93cc-212">Int32</span></span>|<span data-ttu-id="c93cc-213">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="c93cc-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c93cc-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c93cc-214">totalLicenseCount</span></span>|<span data-ttu-id="c93cc-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c93cc-215">Int32</span></span>|<span data-ttu-id="c93cc-216">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="c93cc-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c93cc-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c93cc-217">appStoreUrl</span></span>|<span data-ttu-id="c93cc-218">String</span><span class="sxs-lookup"><span data-stu-id="c93cc-218">String</span></span>|<span data-ttu-id="c93cc-219">ワークストアアプリの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="c93cc-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="c93cc-220">supportsoemconfig</span><span class="sxs-lookup"><span data-stu-id="c93cc-220">supportsOemConfig</span></span>|<span data-ttu-id="c93cc-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c93cc-221">Boolean</span></span>|<span data-ttu-id="c93cc-222">このアプリが oemconfig ポリシーをサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="c93cc-222">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c93cc-223">応答</span><span class="sxs-lookup"><span data-stu-id="c93cc-223">Response</span></span>
<span data-ttu-id="c93cc-224">成功した場合、このメソッド`200 OK`は応答コードと、更新された[androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c93cc-224">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c93cc-225">例</span><span class="sxs-lookup"><span data-stu-id="c93cc-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="c93cc-226">要求</span><span class="sxs-lookup"><span data-stu-id="c93cc-226">Request</span></span>
<span data-ttu-id="c93cc-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c93cc-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="c93cc-228">応答</span><span class="sxs-lookup"><span data-stu-id="c93cc-228">Response</span></span>
<span data-ttu-id="c93cc-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c93cc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```





