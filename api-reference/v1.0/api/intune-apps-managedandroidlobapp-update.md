---
title: managedAndroidLobApp の更新
description: managedAndroidLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32ab9ae624386efd59b7824e8b900ae2ac1d2456
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002413"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="1743e-103">managedAndroidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="1743e-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="1743e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1743e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1743e-105">[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1743e-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1743e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1743e-106">Prerequisites</span></span>
<span data-ttu-id="1743e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1743e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1743e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1743e-109">Permission type</span></span>|<span data-ttu-id="1743e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1743e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1743e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1743e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1743e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1743e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1743e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1743e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1743e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1743e-114">Not supported.</span></span>|
|<span data-ttu-id="1743e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1743e-115">Application</span></span>|<span data-ttu-id="1743e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1743e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1743e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1743e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1743e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1743e-118">Request headers</span></span>
|<span data-ttu-id="1743e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1743e-119">Header</span></span>|<span data-ttu-id="1743e-120">値</span><span class="sxs-lookup"><span data-stu-id="1743e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1743e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1743e-121">Authorization</span></span>|<span data-ttu-id="1743e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1743e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1743e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1743e-123">Accept</span></span>|<span data-ttu-id="1743e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1743e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1743e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1743e-125">Request body</span></span>
<span data-ttu-id="1743e-126">要求本文で、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1743e-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="1743e-127">次の表に、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1743e-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="1743e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1743e-128">Property</span></span>|<span data-ttu-id="1743e-129">型</span><span class="sxs-lookup"><span data-stu-id="1743e-129">Type</span></span>|<span data-ttu-id="1743e-130">説明</span><span class="sxs-lookup"><span data-stu-id="1743e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1743e-131">id</span><span class="sxs-lookup"><span data-stu-id="1743e-131">id</span></span>|<span data-ttu-id="1743e-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1743e-132">String</span></span>|<span data-ttu-id="1743e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1743e-133">Key of the entity.</span></span> <span data-ttu-id="1743e-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1743e-135">displayName</span></span>|<span data-ttu-id="1743e-136">文字列</span><span class="sxs-lookup"><span data-stu-id="1743e-136">String</span></span>|<span data-ttu-id="1743e-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1743e-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1743e-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-139">description</span><span class="sxs-lookup"><span data-stu-id="1743e-139">description</span></span>|<span data-ttu-id="1743e-140">String</span><span class="sxs-lookup"><span data-stu-id="1743e-140">String</span></span>|<span data-ttu-id="1743e-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1743e-141">The description of the app.</span></span> <span data-ttu-id="1743e-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1743e-143">publisher</span></span>|<span data-ttu-id="1743e-144">String</span><span class="sxs-lookup"><span data-stu-id="1743e-144">String</span></span>|<span data-ttu-id="1743e-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1743e-145">The publisher of the app.</span></span> <span data-ttu-id="1743e-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1743e-147">largeIcon</span></span>|[<span data-ttu-id="1743e-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1743e-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1743e-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="1743e-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1743e-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1743e-151">createdDateTime</span></span>|<span data-ttu-id="1743e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1743e-152">DateTimeOffset</span></span>|<span data-ttu-id="1743e-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1743e-153">The date and time the app was created.</span></span> <span data-ttu-id="1743e-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1743e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1743e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1743e-156">DateTimeOffset</span></span>|<span data-ttu-id="1743e-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1743e-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1743e-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1743e-159">isFeatured</span></span>|<span data-ttu-id="1743e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1743e-160">Boolean</span></span>|<span data-ttu-id="1743e-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1743e-162">privacyInformationUrl</span></span>|<span data-ttu-id="1743e-163">String</span><span class="sxs-lookup"><span data-stu-id="1743e-163">String</span></span>|<span data-ttu-id="1743e-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1743e-164">The privacy statement Url.</span></span> <span data-ttu-id="1743e-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1743e-166">informationUrl</span></span>|<span data-ttu-id="1743e-167">String</span><span class="sxs-lookup"><span data-stu-id="1743e-167">String</span></span>|<span data-ttu-id="1743e-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1743e-168">The more information Url.</span></span> <span data-ttu-id="1743e-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-170">owner</span><span class="sxs-lookup"><span data-stu-id="1743e-170">owner</span></span>|<span data-ttu-id="1743e-171">String</span><span class="sxs-lookup"><span data-stu-id="1743e-171">String</span></span>|<span data-ttu-id="1743e-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1743e-172">The owner of the app.</span></span> <span data-ttu-id="1743e-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-174">developer</span><span class="sxs-lookup"><span data-stu-id="1743e-174">developer</span></span>|<span data-ttu-id="1743e-175">String</span><span class="sxs-lookup"><span data-stu-id="1743e-175">String</span></span>|<span data-ttu-id="1743e-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1743e-176">The developer of the app.</span></span> <span data-ttu-id="1743e-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-178">notes</span><span class="sxs-lookup"><span data-stu-id="1743e-178">notes</span></span>|<span data-ttu-id="1743e-179">String</span><span class="sxs-lookup"><span data-stu-id="1743e-179">String</span></span>|<span data-ttu-id="1743e-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1743e-180">Notes for the app.</span></span> <span data-ttu-id="1743e-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1743e-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1743e-182">publishingState</span></span>|[<span data-ttu-id="1743e-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1743e-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1743e-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1743e-184">The publishing state for the app.</span></span> <span data-ttu-id="1743e-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1743e-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1743e-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1743e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1743e-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1743e-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1743e-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1743e-188">appAvailability</span></span>|[<span data-ttu-id="1743e-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="1743e-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="1743e-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="1743e-190">The Application's availability.</span></span> <span data-ttu-id="1743e-191">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1743e-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="1743e-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="1743e-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1743e-193">version</span><span class="sxs-lookup"><span data-stu-id="1743e-193">version</span></span>|<span data-ttu-id="1743e-194">String</span><span class="sxs-lookup"><span data-stu-id="1743e-194">String</span></span>|<span data-ttu-id="1743e-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1743e-195">The Application's version.</span></span> <span data-ttu-id="1743e-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="1743e-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1743e-197">committedContentVersion</span></span>|<span data-ttu-id="1743e-198">String</span><span class="sxs-lookup"><span data-stu-id="1743e-198">String</span></span>|<span data-ttu-id="1743e-199">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1743e-199">The internal committed content version.</span></span> <span data-ttu-id="1743e-200">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1743e-201">fileName</span><span class="sxs-lookup"><span data-stu-id="1743e-201">fileName</span></span>|<span data-ttu-id="1743e-202">String</span><span class="sxs-lookup"><span data-stu-id="1743e-202">String</span></span>|<span data-ttu-id="1743e-203">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1743e-203">The name of the main Lob application file.</span></span> <span data-ttu-id="1743e-204">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1743e-205">size</span><span class="sxs-lookup"><span data-stu-id="1743e-205">size</span></span>|<span data-ttu-id="1743e-206">Int64</span><span class="sxs-lookup"><span data-stu-id="1743e-206">Int64</span></span>|<span data-ttu-id="1743e-207">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1743e-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="1743e-208">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1743e-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1743e-209">packageId</span><span class="sxs-lookup"><span data-stu-id="1743e-209">packageId</span></span>|<span data-ttu-id="1743e-210">String</span><span class="sxs-lookup"><span data-stu-id="1743e-210">String</span></span>|<span data-ttu-id="1743e-211">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="1743e-211">The package identifier.</span></span>|
|<span data-ttu-id="1743e-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1743e-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1743e-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1743e-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="1743e-214">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="1743e-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1743e-215">versionName</span><span class="sxs-lookup"><span data-stu-id="1743e-215">versionName</span></span>|<span data-ttu-id="1743e-216">String</span><span class="sxs-lookup"><span data-stu-id="1743e-216">String</span></span>|<span data-ttu-id="1743e-217">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="1743e-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1743e-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="1743e-218">versionCode</span></span>|<span data-ttu-id="1743e-219">String</span><span class="sxs-lookup"><span data-stu-id="1743e-219">String</span></span>|<span data-ttu-id="1743e-220">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="1743e-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="1743e-221">応答</span><span class="sxs-lookup"><span data-stu-id="1743e-221">Response</span></span>
<span data-ttu-id="1743e-222">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1743e-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1743e-223">例</span><span class="sxs-lookup"><span data-stu-id="1743e-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="1743e-224">要求</span><span class="sxs-lookup"><span data-stu-id="1743e-224">Request</span></span>
<span data-ttu-id="1743e-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1743e-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1153

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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="1743e-226">応答</span><span class="sxs-lookup"><span data-stu-id="1743e-226">Response</span></span>
<span data-ttu-id="1743e-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1743e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



