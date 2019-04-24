---
title: managedAndroidStoreApp の作成
description: 新しい managedAndroidStoreApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bc2cdee760340f22c291a441a5219c80fba461b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495009"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="6a2a8-103">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="6a2a8-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="6a2a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a2a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a2a8-106">新しい [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a2a8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a2a8-107">Prerequisites</span></span>
<span data-ttu-id="6a2a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a2a8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a2a8-110">Permission type</span></span>|<span data-ttu-id="6a2a8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a2a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a2a8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a2a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a2a8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2a8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a2a8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a2a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a2a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-115">Not supported.</span></span>|
|<span data-ttu-id="6a2a8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a2a8-116">Application</span></span>|<span data-ttu-id="6a2a8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a2a8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a2a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6a2a8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a2a8-119">Request headers</span></span>
|<span data-ttu-id="6a2a8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a2a8-120">Header</span></span>|<span data-ttu-id="6a2a8-121">値</span><span class="sxs-lookup"><span data-stu-id="6a2a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a2a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a2a8-122">Authorization</span></span>|<span data-ttu-id="6a2a8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a2a8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a2a8-124">Accept</span></span>|<span data-ttu-id="6a2a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a2a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a2a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a2a8-126">Request body</span></span>
<span data-ttu-id="6a2a8-127">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="6a2a8-128">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="6a2a8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a2a8-129">Property</span></span>|<span data-ttu-id="6a2a8-130">型</span><span class="sxs-lookup"><span data-stu-id="6a2a8-130">Type</span></span>|<span data-ttu-id="6a2a8-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a2a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a2a8-132">id</span><span class="sxs-lookup"><span data-stu-id="6a2a8-132">id</span></span>|<span data-ttu-id="6a2a8-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6a2a8-133">String</span></span>|<span data-ttu-id="6a2a8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-134">Key of the entity.</span></span> <span data-ttu-id="6a2a8-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6a2a8-136">displayName</span></span>|<span data-ttu-id="6a2a8-137">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-137">String</span></span>|<span data-ttu-id="6a2a8-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6a2a8-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-140">説明</span><span class="sxs-lookup"><span data-stu-id="6a2a8-140">description</span></span>|<span data-ttu-id="6a2a8-141">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-141">String</span></span>|<span data-ttu-id="6a2a8-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-142">The description of the app.</span></span> <span data-ttu-id="6a2a8-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="6a2a8-144">publisher</span></span>|<span data-ttu-id="6a2a8-145">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-145">String</span></span>|<span data-ttu-id="6a2a8-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-146">The publisher of the app.</span></span> <span data-ttu-id="6a2a8-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6a2a8-148">largeIcon</span></span>|[<span data-ttu-id="6a2a8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6a2a8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6a2a8-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6a2a8-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2a8-152">createdDateTime</span></span>|<span data-ttu-id="6a2a8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2a8-153">DateTimeOffset</span></span>|<span data-ttu-id="6a2a8-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-154">The date and time the app was created.</span></span> <span data-ttu-id="6a2a8-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2a8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6a2a8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2a8-157">DateTimeOffset</span></span>|<span data-ttu-id="6a2a8-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6a2a8-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6a2a8-160">isFeatured</span></span>|<span data-ttu-id="6a2a8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a2a8-161">Boolean</span></span>|<span data-ttu-id="6a2a8-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6a2a8-163">privacyInformationUrl</span></span>|<span data-ttu-id="6a2a8-164">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-164">String</span></span>|<span data-ttu-id="6a2a8-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-165">The privacy statement Url.</span></span> <span data-ttu-id="6a2a8-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6a2a8-167">informationUrl</span></span>|<span data-ttu-id="6a2a8-168">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-168">String</span></span>|<span data-ttu-id="6a2a8-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-169">The more information Url.</span></span> <span data-ttu-id="6a2a8-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-171">owner</span><span class="sxs-lookup"><span data-stu-id="6a2a8-171">owner</span></span>|<span data-ttu-id="6a2a8-172">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-172">String</span></span>|<span data-ttu-id="6a2a8-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-173">The owner of the app.</span></span> <span data-ttu-id="6a2a8-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-175">developer</span><span class="sxs-lookup"><span data-stu-id="6a2a8-175">developer</span></span>|<span data-ttu-id="6a2a8-176">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-176">String</span></span>|<span data-ttu-id="6a2a8-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-177">The developer of the app.</span></span> <span data-ttu-id="6a2a8-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-179">notes</span><span class="sxs-lookup"><span data-stu-id="6a2a8-179">notes</span></span>|<span data-ttu-id="6a2a8-180">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-180">String</span></span>|<span data-ttu-id="6a2a8-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-181">Notes for the app.</span></span> <span data-ttu-id="6a2a8-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6a2a8-183">uploadState</span></span>|<span data-ttu-id="6a2a8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6a2a8-184">Int32</span></span>|<span data-ttu-id="6a2a8-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-185">The upload state.</span></span> <span data-ttu-id="6a2a8-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6a2a8-187">publishingState</span></span>|[<span data-ttu-id="6a2a8-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6a2a8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6a2a8-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-189">The publishing state for the app.</span></span> <span data-ttu-id="6a2a8-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6a2a8-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6a2a8-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6a2a8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6a2a8-193">isAssigned</span></span>|<span data-ttu-id="6a2a8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a2a8-194">Boolean</span></span>|<span data-ttu-id="6a2a8-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6a2a8-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a2a8-197">roleScopeTagIds</span></span>|<span data-ttu-id="6a2a8-198">String collection</span><span class="sxs-lookup"><span data-stu-id="6a2a8-198">String collection</span></span>|<span data-ttu-id="6a2a8-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6a2a8-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="6a2a8-201">dependentAppCount</span></span>|<span data-ttu-id="6a2a8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6a2a8-202">Int32</span></span>|<span data-ttu-id="6a2a8-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6a2a8-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2a8-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6a2a8-205">appAvailability</span></span>|[<span data-ttu-id="6a2a8-206">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="6a2a8-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6a2a8-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-207">The Application's availability.</span></span> <span data-ttu-id="6a2a8-208">[managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6a2a8-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6a2a8-210">version</span><span class="sxs-lookup"><span data-stu-id="6a2a8-210">version</span></span>|<span data-ttu-id="6a2a8-211">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-211">String</span></span>|<span data-ttu-id="6a2a8-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-212">The Application's version.</span></span> <span data-ttu-id="6a2a8-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a2a8-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6a2a8-214">packageId</span><span class="sxs-lookup"><span data-stu-id="6a2a8-214">packageId</span></span>|<span data-ttu-id="6a2a8-215">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-215">String</span></span>|<span data-ttu-id="6a2a8-216">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-216">The app's package ID.</span></span>|
|<span data-ttu-id="6a2a8-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6a2a8-217">appStoreUrl</span></span>|<span data-ttu-id="6a2a8-218">String</span><span class="sxs-lookup"><span data-stu-id="6a2a8-218">String</span></span>|<span data-ttu-id="6a2a8-219">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="6a2a8-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a2a8-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6a2a8-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a2a8-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="6a2a8-222">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="6a2a8-223">応答</span><span class="sxs-lookup"><span data-stu-id="6a2a8-223">Response</span></span>
<span data-ttu-id="6a2a8-224">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a2a8-225">例</span><span class="sxs-lookup"><span data-stu-id="6a2a8-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a2a8-226">要求</span><span class="sxs-lookup"><span data-stu-id="6a2a8-226">Request</span></span>
<span data-ttu-id="6a2a8-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1264

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="6a2a8-228">応答</span><span class="sxs-lookup"><span data-stu-id="6a2a8-228">Response</span></span>
<span data-ttu-id="6a2a8-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a2a8-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

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
  "dependentAppCount": 1,
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





