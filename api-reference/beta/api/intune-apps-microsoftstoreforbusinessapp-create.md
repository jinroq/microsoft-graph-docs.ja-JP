---
title: Create microsoftStoreForBusinessApp
description: 新しい microsoftStoreForBusinessApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b866c2ada395144c779b59fb4b0fc096117ff7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404758"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="70e4c-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="70e4c-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="70e4c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70e4c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70e4c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70e4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70e4c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70e4c-107">新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="70e4c-107">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70e4c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="70e4c-108">Prerequisites</span></span>
<span data-ttu-id="70e4c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70e4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="70e4c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70e4c-111">Permission type</span></span>|<span data-ttu-id="70e4c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="70e4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70e4c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70e4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70e4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70e4c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70e4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70e4c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70e4c-116">Not supported.</span></span>|
|<span data-ttu-id="70e4c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70e4c-117">Application</span></span>|<span data-ttu-id="70e4c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70e4c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70e4c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70e4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="70e4c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70e4c-120">Request headers</span></span>
|<span data-ttu-id="70e4c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70e4c-121">Header</span></span>|<span data-ttu-id="70e4c-122">値</span><span class="sxs-lookup"><span data-stu-id="70e4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70e4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e4c-123">Authorization</span></span>|<span data-ttu-id="70e4c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="70e4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70e4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70e4c-125">Accept</span></span>|<span data-ttu-id="70e4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70e4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70e4c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="70e4c-127">Request body</span></span>
<span data-ttu-id="70e4c-128">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="70e4c-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="70e4c-129">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="70e4c-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="70e4c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70e4c-130">Property</span></span>|<span data-ttu-id="70e4c-131">型</span><span class="sxs-lookup"><span data-stu-id="70e4c-131">Type</span></span>|<span data-ttu-id="70e4c-132">説明</span><span class="sxs-lookup"><span data-stu-id="70e4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70e4c-133">id</span><span class="sxs-lookup"><span data-stu-id="70e4c-133">id</span></span>|<span data-ttu-id="70e4c-134">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-134">String</span></span>|<span data-ttu-id="70e4c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="70e4c-135">Key of the entity.</span></span> <span data-ttu-id="70e4c-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="70e4c-137">displayName</span></span>|<span data-ttu-id="70e4c-138">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-138">String</span></span>|<span data-ttu-id="70e4c-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="70e4c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="70e4c-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-141">説明</span><span class="sxs-lookup"><span data-stu-id="70e4c-141">description</span></span>|<span data-ttu-id="70e4c-142">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-142">String</span></span>|<span data-ttu-id="70e4c-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="70e4c-143">The description of the app.</span></span> <span data-ttu-id="70e4c-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="70e4c-145">publisher</span></span>|<span data-ttu-id="70e4c-146">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-146">String</span></span>|<span data-ttu-id="70e4c-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="70e4c-147">The publisher of the app.</span></span> <span data-ttu-id="70e4c-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="70e4c-149">largeIcon</span></span>|[<span data-ttu-id="70e4c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="70e4c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="70e4c-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="70e4c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="70e4c-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70e4c-153">createdDateTime</span></span>|<span data-ttu-id="70e4c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70e4c-154">DateTimeOffset</span></span>|<span data-ttu-id="70e4c-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="70e4c-155">The date and time the app was created.</span></span> <span data-ttu-id="70e4c-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70e4c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="70e4c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70e4c-158">DateTimeOffset</span></span>|<span data-ttu-id="70e4c-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="70e4c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="70e4c-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="70e4c-161">isFeatured</span></span>|<span data-ttu-id="70e4c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="70e4c-162">Boolean</span></span>|<span data-ttu-id="70e4c-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="70e4c-164">privacyInformationUrl</span></span>|<span data-ttu-id="70e4c-165">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-165">String</span></span>|<span data-ttu-id="70e4c-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="70e4c-166">The privacy statement Url.</span></span> <span data-ttu-id="70e4c-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="70e4c-168">informationUrl</span></span>|<span data-ttu-id="70e4c-169">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-169">String</span></span>|<span data-ttu-id="70e4c-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="70e4c-170">The more information Url.</span></span> <span data-ttu-id="70e4c-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-172">owner</span><span class="sxs-lookup"><span data-stu-id="70e4c-172">owner</span></span>|<span data-ttu-id="70e4c-173">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-173">String</span></span>|<span data-ttu-id="70e4c-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="70e4c-174">The owner of the app.</span></span> <span data-ttu-id="70e4c-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-176">developer</span><span class="sxs-lookup"><span data-stu-id="70e4c-176">developer</span></span>|<span data-ttu-id="70e4c-177">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-177">String</span></span>|<span data-ttu-id="70e4c-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="70e4c-178">The developer of the app.</span></span> <span data-ttu-id="70e4c-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-180">notes</span><span class="sxs-lookup"><span data-stu-id="70e4c-180">notes</span></span>|<span data-ttu-id="70e4c-181">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-181">String</span></span>|<span data-ttu-id="70e4c-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="70e4c-182">Notes for the app.</span></span> <span data-ttu-id="70e4c-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="70e4c-184">uploadState</span></span>|<span data-ttu-id="70e4c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="70e4c-185">Int32</span></span>|<span data-ttu-id="70e4c-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-186">The upload state.</span></span> <span data-ttu-id="70e4c-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="70e4c-188">publishingState</span></span>|[<span data-ttu-id="70e4c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="70e4c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="70e4c-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="70e4c-190">The publishing state for the app.</span></span> <span data-ttu-id="70e4c-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="70e4c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="70e4c-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="70e4c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="70e4c-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="70e4c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="70e4c-194">isAssigned</span></span>|<span data-ttu-id="70e4c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="70e4c-195">Boolean</span></span>|<span data-ttu-id="70e4c-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="70e4c-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70e4c-198">roleScopeTagIds</span></span>|<span data-ttu-id="70e4c-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="70e4c-199">String collection</span></span>|<span data-ttu-id="70e4c-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="70e4c-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="70e4c-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70e4c-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="70e4c-202">usedLicenseCount</span></span>|<span data-ttu-id="70e4c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="70e4c-203">Int32</span></span>|<span data-ttu-id="70e4c-204">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="70e4c-204">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="70e4c-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="70e4c-205">totalLicenseCount</span></span>|<span data-ttu-id="70e4c-206">Int32</span><span class="sxs-lookup"><span data-stu-id="70e4c-206">Int32</span></span>|<span data-ttu-id="70e4c-207">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="70e4c-207">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="70e4c-208">productKey</span><span class="sxs-lookup"><span data-stu-id="70e4c-208">productKey</span></span>|<span data-ttu-id="70e4c-209">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-209">String</span></span>|<span data-ttu-id="70e4c-210">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="70e4c-210">The app product key</span></span>|
|<span data-ttu-id="70e4c-211">licenseType</span><span class="sxs-lookup"><span data-stu-id="70e4c-211">licenseType</span></span>|[<span data-ttu-id="70e4c-212">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="70e4c-212">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="70e4c-213">アプリケーション ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="70e4c-213">The app license type.</span></span> <span data-ttu-id="70e4c-214">使用可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-214">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="70e4c-215">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="70e4c-215">packageIdentityName</span></span>|<span data-ttu-id="70e4c-216">String</span><span class="sxs-lookup"><span data-stu-id="70e4c-216">String</span></span>|<span data-ttu-id="70e4c-217">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="70e4c-217">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="70e4c-218">応答</span><span class="sxs-lookup"><span data-stu-id="70e4c-218">Response</span></span>
<span data-ttu-id="70e4c-219">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="70e4c-219">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70e4c-220">例</span><span class="sxs-lookup"><span data-stu-id="70e4c-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="70e4c-221">要求</span><span class="sxs-lookup"><span data-stu-id="70e4c-221">Request</span></span>
<span data-ttu-id="70e4c-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70e4c-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="70e4c-223">応答</span><span class="sxs-lookup"><span data-stu-id="70e4c-223">Response</span></span>
<span data-ttu-id="70e4c-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="70e4c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




