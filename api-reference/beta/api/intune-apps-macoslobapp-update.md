---
title: MacOSLobApp を更新します。
description: MacOSLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03ffd4ade590a53502f220a3dff852201bdaf1b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985222"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="c911c-103">MacOSLobApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="c911c-103">Update macOSLobApp</span></span>

> <span data-ttu-id="c911c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c911c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c911c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c911c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c911c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c911c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c911c-107">[MacOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c911c-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c911c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c911c-108">Prerequisites</span></span>
<span data-ttu-id="c911c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c911c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c911c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c911c-111">Permission type</span></span>|<span data-ttu-id="c911c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c911c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c911c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c911c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c911c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c911c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c911c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c911c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c911c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c911c-116">Not supported.</span></span>|
|<span data-ttu-id="c911c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c911c-117">Application</span></span>|<span data-ttu-id="c911c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c911c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c911c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c911c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c911c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c911c-120">Request headers</span></span>
|<span data-ttu-id="c911c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c911c-121">Header</span></span>|<span data-ttu-id="c911c-122">値</span><span class="sxs-lookup"><span data-stu-id="c911c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c911c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c911c-123">Authorization</span></span>|<span data-ttu-id="c911c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c911c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c911c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c911c-125">Accept</span></span>|<span data-ttu-id="c911c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c911c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c911c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c911c-127">Request body</span></span>
<span data-ttu-id="c911c-128">要求の本文に[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c911c-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="c911c-129">[MacOSLobApp](../resources/intune-apps-macoslobapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c911c-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="c911c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c911c-130">Property</span></span>|<span data-ttu-id="c911c-131">型</span><span class="sxs-lookup"><span data-stu-id="c911c-131">Type</span></span>|<span data-ttu-id="c911c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c911c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c911c-133">id</span><span class="sxs-lookup"><span data-stu-id="c911c-133">id</span></span>|<span data-ttu-id="c911c-134">String</span><span class="sxs-lookup"><span data-stu-id="c911c-134">String</span></span>|<span data-ttu-id="c911c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c911c-135">Key of the entity.</span></span> <span data-ttu-id="c911c-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c911c-137">displayName</span></span>|<span data-ttu-id="c911c-138">String</span><span class="sxs-lookup"><span data-stu-id="c911c-138">String</span></span>|<span data-ttu-id="c911c-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c911c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c911c-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-141">説明</span><span class="sxs-lookup"><span data-stu-id="c911c-141">description</span></span>|<span data-ttu-id="c911c-142">String</span><span class="sxs-lookup"><span data-stu-id="c911c-142">String</span></span>|<span data-ttu-id="c911c-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c911c-143">The description of the app.</span></span> <span data-ttu-id="c911c-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c911c-145">publisher</span></span>|<span data-ttu-id="c911c-146">String</span><span class="sxs-lookup"><span data-stu-id="c911c-146">String</span></span>|<span data-ttu-id="c911c-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c911c-147">The publisher of the app.</span></span> <span data-ttu-id="c911c-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c911c-149">largeIcon</span></span>|[<span data-ttu-id="c911c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c911c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c911c-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="c911c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c911c-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c911c-153">createdDateTime</span></span>|<span data-ttu-id="c911c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c911c-154">DateTimeOffset</span></span>|<span data-ttu-id="c911c-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c911c-155">The date and time the app was created.</span></span> <span data-ttu-id="c911c-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c911c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c911c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c911c-158">DateTimeOffset</span></span>|<span data-ttu-id="c911c-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c911c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c911c-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c911c-161">isFeatured</span></span>|<span data-ttu-id="c911c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c911c-162">Boolean</span></span>|<span data-ttu-id="c911c-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c911c-164">privacyInformationUrl</span></span>|<span data-ttu-id="c911c-165">String</span><span class="sxs-lookup"><span data-stu-id="c911c-165">String</span></span>|<span data-ttu-id="c911c-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c911c-166">The privacy statement Url.</span></span> <span data-ttu-id="c911c-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c911c-168">informationUrl</span></span>|<span data-ttu-id="c911c-169">String</span><span class="sxs-lookup"><span data-stu-id="c911c-169">String</span></span>|<span data-ttu-id="c911c-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c911c-170">The more information Url.</span></span> <span data-ttu-id="c911c-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-172">owner</span><span class="sxs-lookup"><span data-stu-id="c911c-172">owner</span></span>|<span data-ttu-id="c911c-173">String</span><span class="sxs-lookup"><span data-stu-id="c911c-173">String</span></span>|<span data-ttu-id="c911c-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c911c-174">The owner of the app.</span></span> <span data-ttu-id="c911c-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-176">developer</span><span class="sxs-lookup"><span data-stu-id="c911c-176">developer</span></span>|<span data-ttu-id="c911c-177">String</span><span class="sxs-lookup"><span data-stu-id="c911c-177">String</span></span>|<span data-ttu-id="c911c-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c911c-178">The developer of the app.</span></span> <span data-ttu-id="c911c-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-180">notes</span><span class="sxs-lookup"><span data-stu-id="c911c-180">notes</span></span>|<span data-ttu-id="c911c-181">String</span><span class="sxs-lookup"><span data-stu-id="c911c-181">String</span></span>|<span data-ttu-id="c911c-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c911c-182">Notes for the app.</span></span> <span data-ttu-id="c911c-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c911c-184">uploadState</span></span>|<span data-ttu-id="c911c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c911c-185">Int32</span></span>|<span data-ttu-id="c911c-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="c911c-186">The upload state.</span></span> <span data-ttu-id="c911c-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c911c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c911c-188">publishingState</span></span>|[<span data-ttu-id="c911c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c911c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c911c-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c911c-190">The publishing state for the app.</span></span> <span data-ttu-id="c911c-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c911c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c911c-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c911c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c911c-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c911c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c911c-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c911c-194">committedContentVersion</span></span>|<span data-ttu-id="c911c-195">String</span><span class="sxs-lookup"><span data-stu-id="c911c-195">String</span></span>|<span data-ttu-id="c911c-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c911c-196">The internal committed content version.</span></span> <span data-ttu-id="c911c-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c911c-198">fileName</span><span class="sxs-lookup"><span data-stu-id="c911c-198">fileName</span></span>|<span data-ttu-id="c911c-199">String</span><span class="sxs-lookup"><span data-stu-id="c911c-199">String</span></span>|<span data-ttu-id="c911c-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="c911c-200">The name of the main Lob application file.</span></span> <span data-ttu-id="c911c-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c911c-202">size</span><span class="sxs-lookup"><span data-stu-id="c911c-202">size</span></span>|<span data-ttu-id="c911c-203">Int64</span><span class="sxs-lookup"><span data-stu-id="c911c-203">Int64</span></span>|<span data-ttu-id="c911c-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="c911c-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="c911c-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c911c-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c911c-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="c911c-206">bundleId</span></span>|<span data-ttu-id="c911c-207">String</span><span class="sxs-lookup"><span data-stu-id="c911c-207">String</span></span>|<span data-ttu-id="c911c-208">バンドル id です。</span><span class="sxs-lookup"><span data-stu-id="c911c-208">The bundle id.</span></span>|
|<span data-ttu-id="c911c-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c911c-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c911c-210">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c911c-210">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="c911c-211">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="c911c-211">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c911c-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c911c-212">buildNumber</span></span>|<span data-ttu-id="c911c-213">String</span><span class="sxs-lookup"><span data-stu-id="c911c-213">String</span></span>|<span data-ttu-id="c911c-214">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="c911c-214">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c911c-215">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="c911c-215">versionNumber</span></span>|<span data-ttu-id="c911c-216">String</span><span class="sxs-lookup"><span data-stu-id="c911c-216">String</span></span>|<span data-ttu-id="c911c-217">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="c911c-217">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c911c-218">childApps</span><span class="sxs-lookup"><span data-stu-id="c911c-218">childApps</span></span>|<span data-ttu-id="c911c-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c911c-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="c911c-220">このバンドル パッケージ内のアプリケーションのリスト</span><span class="sxs-lookup"><span data-stu-id="c911c-220">The app list in this bundle package</span></span>|
|<span data-ttu-id="c911c-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c911c-221">identityVersion</span></span>|<span data-ttu-id="c911c-222">String</span><span class="sxs-lookup"><span data-stu-id="c911c-222">String</span></span>|<span data-ttu-id="c911c-223">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c911c-223">The identity version.</span></span>|
|<span data-ttu-id="c911c-224">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="c911c-224">md5HashChunkSize</span></span>|<span data-ttu-id="c911c-225">Int32</span><span class="sxs-lookup"><span data-stu-id="c911c-225">Int32</span></span>|<span data-ttu-id="c911c-226">MD5 ハッシュのチャンク ・ サイズ</span><span class="sxs-lookup"><span data-stu-id="c911c-226">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="c911c-227">md5Hash</span><span class="sxs-lookup"><span data-stu-id="c911c-227">md5Hash</span></span>|<span data-ttu-id="c911c-228">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c911c-228">String collection</span></span>|<span data-ttu-id="c911c-229">MD5 のハッシュ コード</span><span class="sxs-lookup"><span data-stu-id="c911c-229">The MD5 hash codes</span></span>|
|<span data-ttu-id="c911c-230">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="c911c-230">ignoreVersionDetection</span></span>|<span data-ttu-id="c911c-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c911c-231">Boolean</span></span>|<span data-ttu-id="c911c-232">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="c911c-232">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="c911c-233">MacOS の自己更新機能を使用する基幹業務 (LoB) アプリケーションは、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="c911c-233">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="c911c-234">応答</span><span class="sxs-lookup"><span data-stu-id="c911c-234">Response</span></span>
<span data-ttu-id="c911c-235">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c911c-235">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c911c-236">例</span><span class="sxs-lookup"><span data-stu-id="c911c-236">Example</span></span>
### <a name="request"></a><span data-ttu-id="c911c-237">要求</span><span class="sxs-lookup"><span data-stu-id="c911c-237">Request</span></span>
<span data-ttu-id="c911c-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c911c-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1476

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="c911c-239">応答</span><span class="sxs-lookup"><span data-stu-id="c911c-239">Response</span></span>
<span data-ttu-id="c911c-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c911c-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```





