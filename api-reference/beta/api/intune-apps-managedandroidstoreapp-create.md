---
title: managedAndroidStoreApp の作成
description: 新しい managedAndroidStoreApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a7bd4cf3b84140c61cdd84b024c6574271440620
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405206"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="802af-103">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="802af-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="802af-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="802af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="802af-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="802af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="802af-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="802af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="802af-107">新しい [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="802af-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="802af-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="802af-108">Prerequisites</span></span>
<span data-ttu-id="802af-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="802af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="802af-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="802af-111">Permission type</span></span>|<span data-ttu-id="802af-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="802af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="802af-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="802af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="802af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="802af-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="802af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="802af-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="802af-116">Not supported.</span></span>|
|<span data-ttu-id="802af-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="802af-117">Application</span></span>|<span data-ttu-id="802af-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="802af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="802af-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="802af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="802af-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="802af-120">Request headers</span></span>
|<span data-ttu-id="802af-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="802af-121">Header</span></span>|<span data-ttu-id="802af-122">値</span><span class="sxs-lookup"><span data-stu-id="802af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="802af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="802af-123">Authorization</span></span>|<span data-ttu-id="802af-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="802af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="802af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="802af-125">Accept</span></span>|<span data-ttu-id="802af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="802af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="802af-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="802af-127">Request body</span></span>
<span data-ttu-id="802af-128">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="802af-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="802af-129">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="802af-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="802af-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="802af-130">Property</span></span>|<span data-ttu-id="802af-131">型</span><span class="sxs-lookup"><span data-stu-id="802af-131">Type</span></span>|<span data-ttu-id="802af-132">説明</span><span class="sxs-lookup"><span data-stu-id="802af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="802af-133">id</span><span class="sxs-lookup"><span data-stu-id="802af-133">id</span></span>|<span data-ttu-id="802af-134">String</span><span class="sxs-lookup"><span data-stu-id="802af-134">String</span></span>|<span data-ttu-id="802af-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="802af-135">Key of the entity.</span></span> <span data-ttu-id="802af-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="802af-137">displayName</span></span>|<span data-ttu-id="802af-138">String</span><span class="sxs-lookup"><span data-stu-id="802af-138">String</span></span>|<span data-ttu-id="802af-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="802af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="802af-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-141">説明</span><span class="sxs-lookup"><span data-stu-id="802af-141">description</span></span>|<span data-ttu-id="802af-142">String</span><span class="sxs-lookup"><span data-stu-id="802af-142">String</span></span>|<span data-ttu-id="802af-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="802af-143">The description of the app.</span></span> <span data-ttu-id="802af-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="802af-145">publisher</span></span>|<span data-ttu-id="802af-146">String</span><span class="sxs-lookup"><span data-stu-id="802af-146">String</span></span>|<span data-ttu-id="802af-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="802af-147">The publisher of the app.</span></span> <span data-ttu-id="802af-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="802af-149">largeIcon</span></span>|[<span data-ttu-id="802af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="802af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="802af-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="802af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="802af-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="802af-153">createdDateTime</span></span>|<span data-ttu-id="802af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="802af-154">DateTimeOffset</span></span>|<span data-ttu-id="802af-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="802af-155">The date and time the app was created.</span></span> <span data-ttu-id="802af-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="802af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="802af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="802af-158">DateTimeOffset</span></span>|<span data-ttu-id="802af-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="802af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="802af-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="802af-161">isFeatured</span></span>|<span data-ttu-id="802af-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="802af-162">Boolean</span></span>|<span data-ttu-id="802af-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="802af-164">privacyInformationUrl</span></span>|<span data-ttu-id="802af-165">String</span><span class="sxs-lookup"><span data-stu-id="802af-165">String</span></span>|<span data-ttu-id="802af-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="802af-166">The privacy statement Url.</span></span> <span data-ttu-id="802af-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="802af-168">informationUrl</span></span>|<span data-ttu-id="802af-169">String</span><span class="sxs-lookup"><span data-stu-id="802af-169">String</span></span>|<span data-ttu-id="802af-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="802af-170">The more information Url.</span></span> <span data-ttu-id="802af-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-172">owner</span><span class="sxs-lookup"><span data-stu-id="802af-172">owner</span></span>|<span data-ttu-id="802af-173">String</span><span class="sxs-lookup"><span data-stu-id="802af-173">String</span></span>|<span data-ttu-id="802af-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="802af-174">The owner of the app.</span></span> <span data-ttu-id="802af-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-176">developer</span><span class="sxs-lookup"><span data-stu-id="802af-176">developer</span></span>|<span data-ttu-id="802af-177">String</span><span class="sxs-lookup"><span data-stu-id="802af-177">String</span></span>|<span data-ttu-id="802af-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="802af-178">The developer of the app.</span></span> <span data-ttu-id="802af-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-180">notes</span><span class="sxs-lookup"><span data-stu-id="802af-180">notes</span></span>|<span data-ttu-id="802af-181">String</span><span class="sxs-lookup"><span data-stu-id="802af-181">String</span></span>|<span data-ttu-id="802af-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="802af-182">Notes for the app.</span></span> <span data-ttu-id="802af-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="802af-184">uploadState</span></span>|<span data-ttu-id="802af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="802af-185">Int32</span></span>|<span data-ttu-id="802af-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="802af-186">The upload state.</span></span> <span data-ttu-id="802af-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="802af-188">publishingState</span></span>|[<span data-ttu-id="802af-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="802af-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="802af-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="802af-190">The publishing state for the app.</span></span> <span data-ttu-id="802af-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="802af-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="802af-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="802af-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="802af-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="802af-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="802af-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="802af-194">isAssigned</span></span>|<span data-ttu-id="802af-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="802af-195">Boolean</span></span>|<span data-ttu-id="802af-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="802af-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="802af-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="802af-198">roleScopeTagIds</span></span>|<span data-ttu-id="802af-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="802af-199">String collection</span></span>|<span data-ttu-id="802af-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="802af-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="802af-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="802af-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="802af-202">appAvailability</span></span>|[<span data-ttu-id="802af-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="802af-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="802af-204">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="802af-204">The Application's availability.</span></span> <span data-ttu-id="802af-205">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="802af-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="802af-206">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="802af-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="802af-207">version</span><span class="sxs-lookup"><span data-stu-id="802af-207">version</span></span>|<span data-ttu-id="802af-208">String</span><span class="sxs-lookup"><span data-stu-id="802af-208">String</span></span>|<span data-ttu-id="802af-209">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="802af-209">The Application's version.</span></span> <span data-ttu-id="802af-210">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="802af-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="802af-211">packageId</span><span class="sxs-lookup"><span data-stu-id="802af-211">packageId</span></span>|<span data-ttu-id="802af-212">String</span><span class="sxs-lookup"><span data-stu-id="802af-212">String</span></span>|<span data-ttu-id="802af-213">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="802af-213">The app's package ID.</span></span>|
|<span data-ttu-id="802af-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="802af-214">appStoreUrl</span></span>|<span data-ttu-id="802af-215">String</span><span class="sxs-lookup"><span data-stu-id="802af-215">String</span></span>|<span data-ttu-id="802af-216">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="802af-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="802af-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="802af-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="802af-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="802af-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="802af-219">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="802af-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="802af-220">応答</span><span class="sxs-lookup"><span data-stu-id="802af-220">Response</span></span>
<span data-ttu-id="802af-221">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="802af-221">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802af-222">例</span><span class="sxs-lookup"><span data-stu-id="802af-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="802af-223">要求</span><span class="sxs-lookup"><span data-stu-id="802af-223">Request</span></span>
<span data-ttu-id="802af-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="802af-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="802af-225">応答</span><span class="sxs-lookup"><span data-stu-id="802af-225">Response</span></span>
<span data-ttu-id="802af-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="802af-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




