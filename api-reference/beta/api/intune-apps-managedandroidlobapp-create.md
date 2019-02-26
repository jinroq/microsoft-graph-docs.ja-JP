---
title: Create managedAndroidLobApp
description: 新しい managedAndroidLobApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6029450f517e08876c124b9f5bcfb7e0b6d31880
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151913"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="71d2d-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="71d2d-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="71d2d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71d2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71d2d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71d2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d2d-106">新しい [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="71d2d-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d2d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="71d2d-107">Prerequisites</span></span>
<span data-ttu-id="71d2d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71d2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71d2d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71d2d-110">Permission type</span></span>|<span data-ttu-id="71d2d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71d2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d2d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71d2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71d2d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d2d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71d2d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71d2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d2d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71d2d-115">Not supported.</span></span>|
|<span data-ttu-id="71d2d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71d2d-116">Application</span></span>|<span data-ttu-id="71d2d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71d2d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d2d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71d2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="71d2d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71d2d-119">Request headers</span></span>
|<span data-ttu-id="71d2d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71d2d-120">Header</span></span>|<span data-ttu-id="71d2d-121">値</span><span class="sxs-lookup"><span data-stu-id="71d2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71d2d-122">Authorization</span></span>|<span data-ttu-id="71d2d-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="71d2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d2d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="71d2d-124">Accept</span></span>|<span data-ttu-id="71d2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71d2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d2d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71d2d-126">Request body</span></span>
<span data-ttu-id="71d2d-127">要求本文で、managedAndroidLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71d2d-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="71d2d-128">次の表に、managedAndroidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="71d2d-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="71d2d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71d2d-129">Property</span></span>|<span data-ttu-id="71d2d-130">型</span><span class="sxs-lookup"><span data-stu-id="71d2d-130">Type</span></span>|<span data-ttu-id="71d2d-131">説明</span><span class="sxs-lookup"><span data-stu-id="71d2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d2d-132">id</span><span class="sxs-lookup"><span data-stu-id="71d2d-132">id</span></span>|<span data-ttu-id="71d2d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="71d2d-133">String</span></span>|<span data-ttu-id="71d2d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="71d2d-134">Key of the entity.</span></span> <span data-ttu-id="71d2d-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71d2d-136">displayName</span></span>|<span data-ttu-id="71d2d-137">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-137">String</span></span>|<span data-ttu-id="71d2d-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="71d2d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="71d2d-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-140">説明</span><span class="sxs-lookup"><span data-stu-id="71d2d-140">description</span></span>|<span data-ttu-id="71d2d-141">文字列</span><span class="sxs-lookup"><span data-stu-id="71d2d-141">String</span></span>|<span data-ttu-id="71d2d-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="71d2d-142">The description of the app.</span></span> <span data-ttu-id="71d2d-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="71d2d-144">publisher</span></span>|<span data-ttu-id="71d2d-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71d2d-145">String</span></span>|<span data-ttu-id="71d2d-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="71d2d-146">The publisher of the app.</span></span> <span data-ttu-id="71d2d-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="71d2d-148">largeIcon</span></span>|[<span data-ttu-id="71d2d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71d2d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71d2d-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="71d2d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="71d2d-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71d2d-152">createdDateTime</span></span>|<span data-ttu-id="71d2d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71d2d-153">DateTimeOffset</span></span>|<span data-ttu-id="71d2d-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="71d2d-154">The date and time the app was created.</span></span> <span data-ttu-id="71d2d-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71d2d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="71d2d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71d2d-157">DateTimeOffset</span></span>|<span data-ttu-id="71d2d-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="71d2d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="71d2d-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="71d2d-160">isFeatured</span></span>|<span data-ttu-id="71d2d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="71d2d-161">Boolean</span></span>|<span data-ttu-id="71d2d-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="71d2d-163">privacyInformationUrl</span></span>|<span data-ttu-id="71d2d-164">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-164">String</span></span>|<span data-ttu-id="71d2d-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="71d2d-165">The privacy statement Url.</span></span> <span data-ttu-id="71d2d-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="71d2d-167">informationUrl</span></span>|<span data-ttu-id="71d2d-168">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-168">String</span></span>|<span data-ttu-id="71d2d-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="71d2d-169">The more information Url.</span></span> <span data-ttu-id="71d2d-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-171">owner</span><span class="sxs-lookup"><span data-stu-id="71d2d-171">owner</span></span>|<span data-ttu-id="71d2d-172">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-172">String</span></span>|<span data-ttu-id="71d2d-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="71d2d-173">The owner of the app.</span></span> <span data-ttu-id="71d2d-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-175">developer</span><span class="sxs-lookup"><span data-stu-id="71d2d-175">developer</span></span>|<span data-ttu-id="71d2d-176">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-176">String</span></span>|<span data-ttu-id="71d2d-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="71d2d-177">The developer of the app.</span></span> <span data-ttu-id="71d2d-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-179">notes</span><span class="sxs-lookup"><span data-stu-id="71d2d-179">notes</span></span>|<span data-ttu-id="71d2d-180">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-180">String</span></span>|<span data-ttu-id="71d2d-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="71d2d-181">Notes for the app.</span></span> <span data-ttu-id="71d2d-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="71d2d-183">uploadState</span></span>|<span data-ttu-id="71d2d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="71d2d-184">Int32</span></span>|<span data-ttu-id="71d2d-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="71d2d-185">The upload state.</span></span> <span data-ttu-id="71d2d-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="71d2d-187">publishingState</span></span>|[<span data-ttu-id="71d2d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="71d2d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="71d2d-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="71d2d-189">The publishing state for the app.</span></span> <span data-ttu-id="71d2d-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="71d2d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="71d2d-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="71d2d-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="71d2d-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="71d2d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="71d2d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="71d2d-193">isAssigned</span></span>|<span data-ttu-id="71d2d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="71d2d-194">Boolean</span></span>|<span data-ttu-id="71d2d-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="71d2d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="71d2d-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71d2d-197">roleScopeTagIds</span></span>|<span data-ttu-id="71d2d-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="71d2d-198">String collection</span></span>|<span data-ttu-id="71d2d-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="71d2d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="71d2d-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71d2d-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="71d2d-201">appAvailability</span></span>|[<span data-ttu-id="71d2d-202">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="71d2d-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="71d2d-203">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="71d2d-203">The Application's availability.</span></span> <span data-ttu-id="71d2d-204">[managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="71d2d-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="71d2d-205">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="71d2d-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="71d2d-206">version</span><span class="sxs-lookup"><span data-stu-id="71d2d-206">version</span></span>|<span data-ttu-id="71d2d-207">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-207">String</span></span>|<span data-ttu-id="71d2d-208">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="71d2d-208">The Application's version.</span></span> <span data-ttu-id="71d2d-209">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="71d2d-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="71d2d-210">committedContentVersion</span></span>|<span data-ttu-id="71d2d-211">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-211">String</span></span>|<span data-ttu-id="71d2d-212">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="71d2d-212">The internal committed content version.</span></span> <span data-ttu-id="71d2d-213">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="71d2d-214">fileName</span><span class="sxs-lookup"><span data-stu-id="71d2d-214">fileName</span></span>|<span data-ttu-id="71d2d-215">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-215">String</span></span>|<span data-ttu-id="71d2d-216">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="71d2d-216">The name of the main Lob application file.</span></span> <span data-ttu-id="71d2d-217">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="71d2d-218">size</span><span class="sxs-lookup"><span data-stu-id="71d2d-218">size</span></span>|<span data-ttu-id="71d2d-219">Int64</span><span class="sxs-lookup"><span data-stu-id="71d2d-219">Int64</span></span>|<span data-ttu-id="71d2d-220">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="71d2d-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="71d2d-221">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71d2d-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="71d2d-222">packageId</span><span class="sxs-lookup"><span data-stu-id="71d2d-222">packageId</span></span>|<span data-ttu-id="71d2d-223">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-223">String</span></span>|<span data-ttu-id="71d2d-224">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="71d2d-224">The package identifier.</span></span>|
|<span data-ttu-id="71d2d-225">identityName</span><span class="sxs-lookup"><span data-stu-id="71d2d-225">identityName</span></span>|<span data-ttu-id="71d2d-226">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-226">String</span></span>|<span data-ttu-id="71d2d-227">ID 名。</span><span class="sxs-lookup"><span data-stu-id="71d2d-227">The Identity Name.</span></span>|
|<span data-ttu-id="71d2d-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71d2d-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="71d2d-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71d2d-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="71d2d-230">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="71d2d-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="71d2d-231">versionName</span><span class="sxs-lookup"><span data-stu-id="71d2d-231">versionName</span></span>|<span data-ttu-id="71d2d-232">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-232">String</span></span>|<span data-ttu-id="71d2d-233">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="71d2d-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="71d2d-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="71d2d-234">versionCode</span></span>|<span data-ttu-id="71d2d-235">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-235">String</span></span>|<span data-ttu-id="71d2d-236">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="71d2d-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="71d2d-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="71d2d-237">identityVersion</span></span>|<span data-ttu-id="71d2d-238">String</span><span class="sxs-lookup"><span data-stu-id="71d2d-238">String</span></span>|<span data-ttu-id="71d2d-239">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="71d2d-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="71d2d-240">応答</span><span class="sxs-lookup"><span data-stu-id="71d2d-240">Response</span></span>
<span data-ttu-id="71d2d-241">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71d2d-241">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d2d-242">例</span><span class="sxs-lookup"><span data-stu-id="71d2d-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d2d-243">要求</span><span class="sxs-lookup"><span data-stu-id="71d2d-243">Request</span></span>
<span data-ttu-id="71d2d-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71d2d-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="71d2d-245">応答</span><span class="sxs-lookup"><span data-stu-id="71d2d-245">Response</span></span>
<span data-ttu-id="71d2d-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71d2d-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




