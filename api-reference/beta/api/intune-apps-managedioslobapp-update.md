---
title: managedIOSLobApp の更新
description: managedIOSLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b3709c3556f94e35d441a124df789756a4e4493
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982813"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="4e33e-103">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="4e33e-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="4e33e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e33e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e33e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e33e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e33e-106">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4e33e-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e33e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e33e-107">Prerequisites</span></span>
<span data-ttu-id="4e33e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e33e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e33e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e33e-110">Permission type</span></span>|<span data-ttu-id="4e33e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e33e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e33e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e33e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e33e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e33e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e33e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e33e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e33e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e33e-115">Not supported.</span></span>|
|<span data-ttu-id="4e33e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e33e-116">Application</span></span>|<span data-ttu-id="4e33e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e33e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e33e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e33e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4e33e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e33e-119">Request headers</span></span>
|<span data-ttu-id="4e33e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e33e-120">Header</span></span>|<span data-ttu-id="4e33e-121">値</span><span class="sxs-lookup"><span data-stu-id="4e33e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e33e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e33e-122">Authorization</span></span>|<span data-ttu-id="4e33e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e33e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e33e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4e33e-124">Accept</span></span>|<span data-ttu-id="4e33e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e33e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e33e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e33e-126">Request body</span></span>
<span data-ttu-id="4e33e-127">要求本文で、[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e33e-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="4e33e-128">次の表に、[managedDeviceOverview](../resources/intune-apps-managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4e33e-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="4e33e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e33e-129">Property</span></span>|<span data-ttu-id="4e33e-130">型</span><span class="sxs-lookup"><span data-stu-id="4e33e-130">Type</span></span>|<span data-ttu-id="4e33e-131">説明</span><span class="sxs-lookup"><span data-stu-id="4e33e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e33e-132">id</span><span class="sxs-lookup"><span data-stu-id="4e33e-132">id</span></span>|<span data-ttu-id="4e33e-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4e33e-133">String</span></span>|<span data-ttu-id="4e33e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4e33e-134">Key of the entity.</span></span> <span data-ttu-id="4e33e-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4e33e-136">displayName</span></span>|<span data-ttu-id="4e33e-137">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-137">String</span></span>|<span data-ttu-id="4e33e-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="4e33e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4e33e-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-140">description</span><span class="sxs-lookup"><span data-stu-id="4e33e-140">description</span></span>|<span data-ttu-id="4e33e-141">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-141">String</span></span>|<span data-ttu-id="4e33e-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="4e33e-142">The description of the app.</span></span> <span data-ttu-id="4e33e-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4e33e-144">publisher</span></span>|<span data-ttu-id="4e33e-145">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-145">String</span></span>|<span data-ttu-id="4e33e-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="4e33e-146">The publisher of the app.</span></span> <span data-ttu-id="4e33e-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4e33e-148">largeIcon</span></span>|[<span data-ttu-id="4e33e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e33e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e33e-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="4e33e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4e33e-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e33e-152">createdDateTime</span></span>|<span data-ttu-id="4e33e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e33e-153">DateTimeOffset</span></span>|<span data-ttu-id="4e33e-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4e33e-154">The date and time the app was created.</span></span> <span data-ttu-id="4e33e-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e33e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4e33e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e33e-157">DateTimeOffset</span></span>|<span data-ttu-id="4e33e-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4e33e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4e33e-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4e33e-160">isFeatured</span></span>|<span data-ttu-id="4e33e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e33e-161">Boolean</span></span>|<span data-ttu-id="4e33e-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e33e-163">privacyInformationUrl</span></span>|<span data-ttu-id="4e33e-164">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-164">String</span></span>|<span data-ttu-id="4e33e-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="4e33e-165">The privacy statement Url.</span></span> <span data-ttu-id="4e33e-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e33e-167">informationUrl</span></span>|<span data-ttu-id="4e33e-168">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-168">String</span></span>|<span data-ttu-id="4e33e-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="4e33e-169">The more information Url.</span></span> <span data-ttu-id="4e33e-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-171">owner</span><span class="sxs-lookup"><span data-stu-id="4e33e-171">owner</span></span>|<span data-ttu-id="4e33e-172">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-172">String</span></span>|<span data-ttu-id="4e33e-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="4e33e-173">The owner of the app.</span></span> <span data-ttu-id="4e33e-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-175">developer</span><span class="sxs-lookup"><span data-stu-id="4e33e-175">developer</span></span>|<span data-ttu-id="4e33e-176">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-176">String</span></span>|<span data-ttu-id="4e33e-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="4e33e-177">The developer of the app.</span></span> <span data-ttu-id="4e33e-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-179">notes</span><span class="sxs-lookup"><span data-stu-id="4e33e-179">notes</span></span>|<span data-ttu-id="4e33e-180">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-180">String</span></span>|<span data-ttu-id="4e33e-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="4e33e-181">Notes for the app.</span></span> <span data-ttu-id="4e33e-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4e33e-183">uploadState</span></span>|<span data-ttu-id="4e33e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4e33e-184">Int32</span></span>|<span data-ttu-id="4e33e-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="4e33e-185">The upload state.</span></span> <span data-ttu-id="4e33e-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4e33e-187">publishingState</span></span>|[<span data-ttu-id="4e33e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4e33e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4e33e-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="4e33e-189">The publishing state for the app.</span></span> <span data-ttu-id="4e33e-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="4e33e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4e33e-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4e33e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4e33e-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="4e33e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4e33e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4e33e-193">isAssigned</span></span>|<span data-ttu-id="4e33e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e33e-194">Boolean</span></span>|<span data-ttu-id="4e33e-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="4e33e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4e33e-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e33e-197">roleScopeTagIds</span></span>|<span data-ttu-id="4e33e-198">String collection</span><span class="sxs-lookup"><span data-stu-id="4e33e-198">String collection</span></span>|<span data-ttu-id="4e33e-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="4e33e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4e33e-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e33e-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4e33e-201">appAvailability</span></span>|[<span data-ttu-id="4e33e-202">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="4e33e-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4e33e-203">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="4e33e-203">The Application's availability.</span></span> <span data-ttu-id="4e33e-204">[managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4e33e-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4e33e-205">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="4e33e-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4e33e-206">version</span><span class="sxs-lookup"><span data-stu-id="4e33e-206">version</span></span>|<span data-ttu-id="4e33e-207">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-207">String</span></span>|<span data-ttu-id="4e33e-208">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4e33e-208">The Application's version.</span></span> <span data-ttu-id="4e33e-209">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4e33e-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4e33e-210">committedContentVersion</span></span>|<span data-ttu-id="4e33e-211">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-211">String</span></span>|<span data-ttu-id="4e33e-212">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4e33e-212">The internal committed content version.</span></span> <span data-ttu-id="4e33e-213">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e33e-214">fileName</span><span class="sxs-lookup"><span data-stu-id="4e33e-214">fileName</span></span>|<span data-ttu-id="4e33e-215">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-215">String</span></span>|<span data-ttu-id="4e33e-216">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="4e33e-216">The name of the main Lob application file.</span></span> <span data-ttu-id="4e33e-217">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e33e-218">size</span><span class="sxs-lookup"><span data-stu-id="4e33e-218">size</span></span>|<span data-ttu-id="4e33e-219">Int64</span><span class="sxs-lookup"><span data-stu-id="4e33e-219">Int64</span></span>|<span data-ttu-id="4e33e-220">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="4e33e-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="4e33e-221">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4e33e-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4e33e-222">bundleId</span><span class="sxs-lookup"><span data-stu-id="4e33e-222">bundleId</span></span>|<span data-ttu-id="4e33e-223">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-223">String</span></span>|<span data-ttu-id="4e33e-224">ID 名。</span><span class="sxs-lookup"><span data-stu-id="4e33e-224">The Identity Name.</span></span>|
|<span data-ttu-id="4e33e-225">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4e33e-225">applicableDeviceType</span></span>|[<span data-ttu-id="4e33e-226">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4e33e-226">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4e33e-227">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="4e33e-227">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4e33e-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e33e-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4e33e-229">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e33e-229">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4e33e-230">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="4e33e-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4e33e-231">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4e33e-231">expirationDateTime</span></span>|<span data-ttu-id="4e33e-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e33e-232">DateTimeOffset</span></span>|<span data-ttu-id="4e33e-233">有効期限。</span><span class="sxs-lookup"><span data-stu-id="4e33e-233">The expiration time.</span></span>|
|<span data-ttu-id="4e33e-234">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="4e33e-234">versionNumber</span></span>|<span data-ttu-id="4e33e-235">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-235">String</span></span>|<span data-ttu-id="4e33e-236">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="4e33e-236">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4e33e-237">buildNumber</span><span class="sxs-lookup"><span data-stu-id="4e33e-237">buildNumber</span></span>|<span data-ttu-id="4e33e-238">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-238">String</span></span>|<span data-ttu-id="4e33e-239">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="4e33e-239">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4e33e-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4e33e-240">identityVersion</span></span>|<span data-ttu-id="4e33e-241">String</span><span class="sxs-lookup"><span data-stu-id="4e33e-241">String</span></span>|<span data-ttu-id="4e33e-242">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4e33e-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4e33e-243">応答</span><span class="sxs-lookup"><span data-stu-id="4e33e-243">Response</span></span>
<span data-ttu-id="4e33e-244">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4e33e-244">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e33e-245">例</span><span class="sxs-lookup"><span data-stu-id="4e33e-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e33e-246">要求</span><span class="sxs-lookup"><span data-stu-id="4e33e-246">Request</span></span>
<span data-ttu-id="4e33e-247">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e33e-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4e33e-248">応答</span><span class="sxs-lookup"><span data-stu-id="4e33e-248">Response</span></span>
<span data-ttu-id="4e33e-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e33e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




