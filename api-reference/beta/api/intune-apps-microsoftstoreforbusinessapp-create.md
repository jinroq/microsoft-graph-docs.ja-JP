---
title: Create microsoftStoreForBusinessApp
description: 新しい microsoftStoreForBusinessApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3471bb6e06d3c201ed21c4b120ca4f37c8c4c2ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174962"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="835ad-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="835ad-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="835ad-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="835ad-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="835ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="835ad-106">新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="835ad-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="835ad-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="835ad-107">Prerequisites</span></span>
<span data-ttu-id="835ad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="835ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="835ad-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="835ad-110">Permission type</span></span>|<span data-ttu-id="835ad-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="835ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="835ad-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="835ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="835ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="835ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="835ad-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="835ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="835ad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835ad-115">Not supported.</span></span>|
|<span data-ttu-id="835ad-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="835ad-116">Application</span></span>|<span data-ttu-id="835ad-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="835ad-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="835ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="835ad-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="835ad-119">Request headers</span></span>
|<span data-ttu-id="835ad-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="835ad-120">Header</span></span>|<span data-ttu-id="835ad-121">値</span><span class="sxs-lookup"><span data-stu-id="835ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="835ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="835ad-122">Authorization</span></span>|<span data-ttu-id="835ad-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="835ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="835ad-124">承諾</span><span class="sxs-lookup"><span data-stu-id="835ad-124">Accept</span></span>|<span data-ttu-id="835ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="835ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="835ad-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="835ad-126">Request body</span></span>
<span data-ttu-id="835ad-127">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="835ad-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="835ad-128">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="835ad-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="835ad-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="835ad-129">Property</span></span>|<span data-ttu-id="835ad-130">型</span><span class="sxs-lookup"><span data-stu-id="835ad-130">Type</span></span>|<span data-ttu-id="835ad-131">説明</span><span class="sxs-lookup"><span data-stu-id="835ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="835ad-132">id</span><span class="sxs-lookup"><span data-stu-id="835ad-132">id</span></span>|<span data-ttu-id="835ad-133">文字列</span><span class="sxs-lookup"><span data-stu-id="835ad-133">String</span></span>|<span data-ttu-id="835ad-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="835ad-134">Key of the entity.</span></span> <span data-ttu-id="835ad-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-136">displayName</span><span class="sxs-lookup"><span data-stu-id="835ad-136">displayName</span></span>|<span data-ttu-id="835ad-137">String</span><span class="sxs-lookup"><span data-stu-id="835ad-137">String</span></span>|<span data-ttu-id="835ad-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="835ad-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="835ad-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-140">説明</span><span class="sxs-lookup"><span data-stu-id="835ad-140">description</span></span>|<span data-ttu-id="835ad-141">文字列</span><span class="sxs-lookup"><span data-stu-id="835ad-141">String</span></span>|<span data-ttu-id="835ad-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="835ad-142">The description of the app.</span></span> <span data-ttu-id="835ad-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-144">publisher</span><span class="sxs-lookup"><span data-stu-id="835ad-144">publisher</span></span>|<span data-ttu-id="835ad-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="835ad-145">String</span></span>|<span data-ttu-id="835ad-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="835ad-146">The publisher of the app.</span></span> <span data-ttu-id="835ad-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="835ad-148">largeIcon</span></span>|[<span data-ttu-id="835ad-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="835ad-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="835ad-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="835ad-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="835ad-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="835ad-152">createdDateTime</span></span>|<span data-ttu-id="835ad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="835ad-153">DateTimeOffset</span></span>|<span data-ttu-id="835ad-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="835ad-154">The date and time the app was created.</span></span> <span data-ttu-id="835ad-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="835ad-156">lastModifiedDateTime</span></span>|<span data-ttu-id="835ad-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="835ad-157">DateTimeOffset</span></span>|<span data-ttu-id="835ad-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="835ad-158">The date and time the app was last modified.</span></span> <span data-ttu-id="835ad-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="835ad-160">isFeatured</span></span>|<span data-ttu-id="835ad-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="835ad-161">Boolean</span></span>|<span data-ttu-id="835ad-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="835ad-163">privacyInformationUrl</span></span>|<span data-ttu-id="835ad-164">String</span><span class="sxs-lookup"><span data-stu-id="835ad-164">String</span></span>|<span data-ttu-id="835ad-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="835ad-165">The privacy statement Url.</span></span> <span data-ttu-id="835ad-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="835ad-167">informationUrl</span></span>|<span data-ttu-id="835ad-168">String</span><span class="sxs-lookup"><span data-stu-id="835ad-168">String</span></span>|<span data-ttu-id="835ad-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="835ad-169">The more information Url.</span></span> <span data-ttu-id="835ad-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-171">owner</span><span class="sxs-lookup"><span data-stu-id="835ad-171">owner</span></span>|<span data-ttu-id="835ad-172">String</span><span class="sxs-lookup"><span data-stu-id="835ad-172">String</span></span>|<span data-ttu-id="835ad-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="835ad-173">The owner of the app.</span></span> <span data-ttu-id="835ad-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-175">developer</span><span class="sxs-lookup"><span data-stu-id="835ad-175">developer</span></span>|<span data-ttu-id="835ad-176">String</span><span class="sxs-lookup"><span data-stu-id="835ad-176">String</span></span>|<span data-ttu-id="835ad-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="835ad-177">The developer of the app.</span></span> <span data-ttu-id="835ad-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-179">notes</span><span class="sxs-lookup"><span data-stu-id="835ad-179">notes</span></span>|<span data-ttu-id="835ad-180">String</span><span class="sxs-lookup"><span data-stu-id="835ad-180">String</span></span>|<span data-ttu-id="835ad-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="835ad-181">Notes for the app.</span></span> <span data-ttu-id="835ad-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="835ad-183">uploadState</span></span>|<span data-ttu-id="835ad-184">Int32</span><span class="sxs-lookup"><span data-stu-id="835ad-184">Int32</span></span>|<span data-ttu-id="835ad-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="835ad-185">The upload state.</span></span> <span data-ttu-id="835ad-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="835ad-187">publishingState</span></span>|[<span data-ttu-id="835ad-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="835ad-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="835ad-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="835ad-189">The publishing state for the app.</span></span> <span data-ttu-id="835ad-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="835ad-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="835ad-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="835ad-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="835ad-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="835ad-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="835ad-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="835ad-193">isAssigned</span></span>|<span data-ttu-id="835ad-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="835ad-194">Boolean</span></span>|<span data-ttu-id="835ad-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="835ad-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="835ad-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="835ad-197">roleScopeTagIds</span></span>|<span data-ttu-id="835ad-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="835ad-198">String collection</span></span>|<span data-ttu-id="835ad-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="835ad-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="835ad-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="835ad-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="835ad-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="835ad-201">usedLicenseCount</span></span>|<span data-ttu-id="835ad-202">Int32</span><span class="sxs-lookup"><span data-stu-id="835ad-202">Int32</span></span>|<span data-ttu-id="835ad-203">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="835ad-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="835ad-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="835ad-204">totalLicenseCount</span></span>|<span data-ttu-id="835ad-205">Int32</span><span class="sxs-lookup"><span data-stu-id="835ad-205">Int32</span></span>|<span data-ttu-id="835ad-206">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="835ad-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="835ad-207">productKey</span><span class="sxs-lookup"><span data-stu-id="835ad-207">productKey</span></span>|<span data-ttu-id="835ad-208">String</span><span class="sxs-lookup"><span data-stu-id="835ad-208">String</span></span>|<span data-ttu-id="835ad-209">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="835ad-209">The app product key</span></span>|
|<span data-ttu-id="835ad-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="835ad-210">licenseType</span></span>|[<span data-ttu-id="835ad-211">microsoft storeforbusinesslicensetype</span><span class="sxs-lookup"><span data-stu-id="835ad-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="835ad-212">アプリライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="835ad-212">The app license type.</span></span> <span data-ttu-id="835ad-213">使用可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="835ad-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="835ad-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="835ad-214">packageIdentityName</span></span>|<span data-ttu-id="835ad-215">String</span><span class="sxs-lookup"><span data-stu-id="835ad-215">String</span></span>|<span data-ttu-id="835ad-216">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="835ad-216">The app package identifier</span></span>|
|<span data-ttu-id="835ad-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="835ad-217">licensingType</span></span>|[<span data-ttu-id="835ad-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="835ad-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="835ad-219">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="835ad-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="835ad-220">応答</span><span class="sxs-lookup"><span data-stu-id="835ad-220">Response</span></span>
<span data-ttu-id="835ad-221">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="835ad-221">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="835ad-222">例</span><span class="sxs-lookup"><span data-stu-id="835ad-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="835ad-223">要求</span><span class="sxs-lookup"><span data-stu-id="835ad-223">Request</span></span>
<span data-ttu-id="835ad-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="835ad-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1105

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

### <a name="response"></a><span data-ttu-id="835ad-225">応答</span><span class="sxs-lookup"><span data-stu-id="835ad-225">Response</span></span>
<span data-ttu-id="835ad-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="835ad-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1277

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




