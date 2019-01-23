---
title: managedIOSStoreApp の作成
description: 新しい managedIOSStoreApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ccf4fe577d6704a9ebd3670d43c29d0f0d70523
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413172"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="78cba-103">managedIOSStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="78cba-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="78cba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78cba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78cba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78cba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78cba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78cba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78cba-107">新しい [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="78cba-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78cba-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="78cba-108">Prerequisites</span></span>
<span data-ttu-id="78cba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78cba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="78cba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78cba-111">Permission type</span></span>|<span data-ttu-id="78cba-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78cba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78cba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78cba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78cba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78cba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78cba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78cba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78cba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78cba-116">Not supported.</span></span>|
|<span data-ttu-id="78cba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78cba-117">Application</span></span>|<span data-ttu-id="78cba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78cba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78cba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78cba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="78cba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78cba-120">Request headers</span></span>
|<span data-ttu-id="78cba-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78cba-121">Header</span></span>|<span data-ttu-id="78cba-122">値</span><span class="sxs-lookup"><span data-stu-id="78cba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78cba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78cba-123">Authorization</span></span>|<span data-ttu-id="78cba-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="78cba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78cba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78cba-125">Accept</span></span>|<span data-ttu-id="78cba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78cba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78cba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="78cba-127">Request body</span></span>
<span data-ttu-id="78cba-128">要求本文で、managedIOSStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78cba-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="78cba-129">次の表に、managedIOSStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78cba-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="78cba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78cba-130">Property</span></span>|<span data-ttu-id="78cba-131">型</span><span class="sxs-lookup"><span data-stu-id="78cba-131">Type</span></span>|<span data-ttu-id="78cba-132">説明</span><span class="sxs-lookup"><span data-stu-id="78cba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78cba-133">id</span><span class="sxs-lookup"><span data-stu-id="78cba-133">id</span></span>|<span data-ttu-id="78cba-134">String</span><span class="sxs-lookup"><span data-stu-id="78cba-134">String</span></span>|<span data-ttu-id="78cba-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78cba-135">Key of the entity.</span></span> <span data-ttu-id="78cba-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-137">displayName</span><span class="sxs-lookup"><span data-stu-id="78cba-137">displayName</span></span>|<span data-ttu-id="78cba-138">String</span><span class="sxs-lookup"><span data-stu-id="78cba-138">String</span></span>|<span data-ttu-id="78cba-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="78cba-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="78cba-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-141">説明</span><span class="sxs-lookup"><span data-stu-id="78cba-141">description</span></span>|<span data-ttu-id="78cba-142">String</span><span class="sxs-lookup"><span data-stu-id="78cba-142">String</span></span>|<span data-ttu-id="78cba-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="78cba-143">The description of the app.</span></span> <span data-ttu-id="78cba-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-145">publisher</span><span class="sxs-lookup"><span data-stu-id="78cba-145">publisher</span></span>|<span data-ttu-id="78cba-146">String</span><span class="sxs-lookup"><span data-stu-id="78cba-146">String</span></span>|<span data-ttu-id="78cba-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="78cba-147">The publisher of the app.</span></span> <span data-ttu-id="78cba-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="78cba-149">largeIcon</span></span>|[<span data-ttu-id="78cba-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78cba-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="78cba-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="78cba-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="78cba-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78cba-153">createdDateTime</span></span>|<span data-ttu-id="78cba-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78cba-154">DateTimeOffset</span></span>|<span data-ttu-id="78cba-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="78cba-155">The date and time the app was created.</span></span> <span data-ttu-id="78cba-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78cba-157">lastModifiedDateTime</span></span>|<span data-ttu-id="78cba-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78cba-158">DateTimeOffset</span></span>|<span data-ttu-id="78cba-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="78cba-159">The date and time the app was last modified.</span></span> <span data-ttu-id="78cba-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="78cba-161">isFeatured</span></span>|<span data-ttu-id="78cba-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="78cba-162">Boolean</span></span>|<span data-ttu-id="78cba-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="78cba-164">privacyInformationUrl</span></span>|<span data-ttu-id="78cba-165">String</span><span class="sxs-lookup"><span data-stu-id="78cba-165">String</span></span>|<span data-ttu-id="78cba-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="78cba-166">The privacy statement Url.</span></span> <span data-ttu-id="78cba-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="78cba-168">informationUrl</span></span>|<span data-ttu-id="78cba-169">String</span><span class="sxs-lookup"><span data-stu-id="78cba-169">String</span></span>|<span data-ttu-id="78cba-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="78cba-170">The more information Url.</span></span> <span data-ttu-id="78cba-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-172">owner</span><span class="sxs-lookup"><span data-stu-id="78cba-172">owner</span></span>|<span data-ttu-id="78cba-173">String</span><span class="sxs-lookup"><span data-stu-id="78cba-173">String</span></span>|<span data-ttu-id="78cba-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="78cba-174">The owner of the app.</span></span> <span data-ttu-id="78cba-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-176">developer</span><span class="sxs-lookup"><span data-stu-id="78cba-176">developer</span></span>|<span data-ttu-id="78cba-177">String</span><span class="sxs-lookup"><span data-stu-id="78cba-177">String</span></span>|<span data-ttu-id="78cba-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="78cba-178">The developer of the app.</span></span> <span data-ttu-id="78cba-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-180">notes</span><span class="sxs-lookup"><span data-stu-id="78cba-180">notes</span></span>|<span data-ttu-id="78cba-181">String</span><span class="sxs-lookup"><span data-stu-id="78cba-181">String</span></span>|<span data-ttu-id="78cba-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="78cba-182">Notes for the app.</span></span> <span data-ttu-id="78cba-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="78cba-184">uploadState</span></span>|<span data-ttu-id="78cba-185">Int32</span><span class="sxs-lookup"><span data-stu-id="78cba-185">Int32</span></span>|<span data-ttu-id="78cba-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="78cba-186">The upload state.</span></span> <span data-ttu-id="78cba-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="78cba-188">publishingState</span></span>|[<span data-ttu-id="78cba-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="78cba-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="78cba-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="78cba-190">The publishing state for the app.</span></span> <span data-ttu-id="78cba-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="78cba-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="78cba-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="78cba-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="78cba-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="78cba-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="78cba-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="78cba-194">isAssigned</span></span>|<span data-ttu-id="78cba-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="78cba-195">Boolean</span></span>|<span data-ttu-id="78cba-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="78cba-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="78cba-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78cba-198">roleScopeTagIds</span></span>|<span data-ttu-id="78cba-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="78cba-199">String collection</span></span>|<span data-ttu-id="78cba-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="78cba-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="78cba-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78cba-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="78cba-202">appAvailability</span></span>|[<span data-ttu-id="78cba-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="78cba-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="78cba-204">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="78cba-204">The Application's availability.</span></span> <span data-ttu-id="78cba-205">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="78cba-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="78cba-206">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="78cba-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="78cba-207">version</span><span class="sxs-lookup"><span data-stu-id="78cba-207">version</span></span>|<span data-ttu-id="78cba-208">String</span><span class="sxs-lookup"><span data-stu-id="78cba-208">String</span></span>|<span data-ttu-id="78cba-209">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="78cba-209">The Application's version.</span></span> <span data-ttu-id="78cba-210">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78cba-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="78cba-211">bundleId</span><span class="sxs-lookup"><span data-stu-id="78cba-211">bundleId</span></span>|<span data-ttu-id="78cba-212">String</span><span class="sxs-lookup"><span data-stu-id="78cba-212">String</span></span>|<span data-ttu-id="78cba-213">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="78cba-213">The app's Bundle ID.</span></span>|
|<span data-ttu-id="78cba-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="78cba-214">appStoreUrl</span></span>|<span data-ttu-id="78cba-215">String</span><span class="sxs-lookup"><span data-stu-id="78cba-215">String</span></span>|<span data-ttu-id="78cba-216">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="78cba-216">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="78cba-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="78cba-217">applicableDeviceType</span></span>|[<span data-ttu-id="78cba-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="78cba-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="78cba-219">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="78cba-219">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="78cba-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78cba-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="78cba-221">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78cba-221">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="78cba-222">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="78cba-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="78cba-223">応答</span><span class="sxs-lookup"><span data-stu-id="78cba-223">Response</span></span>
<span data-ttu-id="78cba-224">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78cba-224">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78cba-225">例</span><span class="sxs-lookup"><span data-stu-id="78cba-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="78cba-226">要求</span><span class="sxs-lookup"><span data-stu-id="78cba-226">Request</span></span>
<span data-ttu-id="78cba-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78cba-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="78cba-228">応答</span><span class="sxs-lookup"><span data-stu-id="78cba-228">Response</span></span>
<span data-ttu-id="78cba-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78cba-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```




