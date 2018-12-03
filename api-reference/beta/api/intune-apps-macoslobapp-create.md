---
title: MacOSLobApp を作成します。
description: 新しい macOSLobApp オブジェクトを作成します。
ms.openlocfilehash: 71f925bd2279365c0d3d73e4f63eca74bde46c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071408"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="2de23-103">MacOSLobApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="2de23-103">Create macOSLobApp</span></span>

> <span data-ttu-id="2de23-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2de23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2de23-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2de23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2de23-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2de23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2de23-107">新しい[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2de23-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2de23-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2de23-108">Prerequisites</span></span>
<span data-ttu-id="2de23-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2de23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2de23-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2de23-111">Permission type</span></span>|<span data-ttu-id="2de23-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2de23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2de23-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2de23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2de23-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de23-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2de23-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2de23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2de23-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2de23-116">Not supported.</span></span>|
|<span data-ttu-id="2de23-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2de23-117">Application</span></span>|<span data-ttu-id="2de23-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2de23-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2de23-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2de23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2de23-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2de23-120">Request headers</span></span>
|<span data-ttu-id="2de23-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2de23-121">Header</span></span>|<span data-ttu-id="2de23-122">値</span><span class="sxs-lookup"><span data-stu-id="2de23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2de23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2de23-123">Authorization</span></span>|<span data-ttu-id="2de23-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2de23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2de23-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2de23-125">Accept</span></span>|<span data-ttu-id="2de23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2de23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2de23-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2de23-127">Request body</span></span>
<span data-ttu-id="2de23-128">要求の本文に macOSLobApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2de23-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="2de23-129">次の表は、macOSLobApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2de23-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="2de23-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2de23-130">Property</span></span>|<span data-ttu-id="2de23-131">型</span><span class="sxs-lookup"><span data-stu-id="2de23-131">Type</span></span>|<span data-ttu-id="2de23-132">説明</span><span class="sxs-lookup"><span data-stu-id="2de23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2de23-133">id</span><span class="sxs-lookup"><span data-stu-id="2de23-133">id</span></span>|<span data-ttu-id="2de23-134">String</span><span class="sxs-lookup"><span data-stu-id="2de23-134">String</span></span>|<span data-ttu-id="2de23-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2de23-135">Key of the entity.</span></span> <span data-ttu-id="2de23-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2de23-137">displayName</span></span>|<span data-ttu-id="2de23-138">String</span><span class="sxs-lookup"><span data-stu-id="2de23-138">String</span></span>|<span data-ttu-id="2de23-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2de23-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2de23-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-141">説明</span><span class="sxs-lookup"><span data-stu-id="2de23-141">description</span></span>|<span data-ttu-id="2de23-142">String</span><span class="sxs-lookup"><span data-stu-id="2de23-142">String</span></span>|<span data-ttu-id="2de23-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="2de23-143">The description of the app.</span></span> <span data-ttu-id="2de23-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2de23-145">publisher</span></span>|<span data-ttu-id="2de23-146">String</span><span class="sxs-lookup"><span data-stu-id="2de23-146">String</span></span>|<span data-ttu-id="2de23-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="2de23-147">The publisher of the app.</span></span> <span data-ttu-id="2de23-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2de23-149">largeIcon</span></span>|[<span data-ttu-id="2de23-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2de23-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2de23-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="2de23-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2de23-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2de23-153">createdDateTime</span></span>|<span data-ttu-id="2de23-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2de23-154">DateTimeOffset</span></span>|<span data-ttu-id="2de23-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2de23-155">The date and time the app was created.</span></span> <span data-ttu-id="2de23-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2de23-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2de23-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2de23-158">DateTimeOffset</span></span>|<span data-ttu-id="2de23-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="2de23-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2de23-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2de23-161">isFeatured</span></span>|<span data-ttu-id="2de23-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2de23-162">Boolean</span></span>|<span data-ttu-id="2de23-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2de23-164">privacyInformationUrl</span></span>|<span data-ttu-id="2de23-165">String</span><span class="sxs-lookup"><span data-stu-id="2de23-165">String</span></span>|<span data-ttu-id="2de23-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="2de23-166">The privacy statement Url.</span></span> <span data-ttu-id="2de23-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2de23-168">informationUrl</span></span>|<span data-ttu-id="2de23-169">String</span><span class="sxs-lookup"><span data-stu-id="2de23-169">String</span></span>|<span data-ttu-id="2de23-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="2de23-170">The more information Url.</span></span> <span data-ttu-id="2de23-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-172">owner</span><span class="sxs-lookup"><span data-stu-id="2de23-172">owner</span></span>|<span data-ttu-id="2de23-173">String</span><span class="sxs-lookup"><span data-stu-id="2de23-173">String</span></span>|<span data-ttu-id="2de23-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="2de23-174">The owner of the app.</span></span> <span data-ttu-id="2de23-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-176">developer</span><span class="sxs-lookup"><span data-stu-id="2de23-176">developer</span></span>|<span data-ttu-id="2de23-177">String</span><span class="sxs-lookup"><span data-stu-id="2de23-177">String</span></span>|<span data-ttu-id="2de23-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="2de23-178">The developer of the app.</span></span> <span data-ttu-id="2de23-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-180">notes</span><span class="sxs-lookup"><span data-stu-id="2de23-180">notes</span></span>|<span data-ttu-id="2de23-181">String</span><span class="sxs-lookup"><span data-stu-id="2de23-181">String</span></span>|<span data-ttu-id="2de23-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="2de23-182">Notes for the app.</span></span> <span data-ttu-id="2de23-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2de23-184">uploadState</span></span>|<span data-ttu-id="2de23-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2de23-185">Int32</span></span>|<span data-ttu-id="2de23-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="2de23-186">The upload state.</span></span> <span data-ttu-id="2de23-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2de23-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2de23-188">publishingState</span></span>|[<span data-ttu-id="2de23-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2de23-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2de23-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="2de23-190">The publishing state for the app.</span></span> <span data-ttu-id="2de23-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="2de23-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2de23-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2de23-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2de23-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="2de23-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2de23-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2de23-194">committedContentVersion</span></span>|<span data-ttu-id="2de23-195">String</span><span class="sxs-lookup"><span data-stu-id="2de23-195">String</span></span>|<span data-ttu-id="2de23-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2de23-196">The internal committed content version.</span></span> <span data-ttu-id="2de23-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2de23-198">fileName</span><span class="sxs-lookup"><span data-stu-id="2de23-198">fileName</span></span>|<span data-ttu-id="2de23-199">String</span><span class="sxs-lookup"><span data-stu-id="2de23-199">String</span></span>|<span data-ttu-id="2de23-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="2de23-200">The name of the main Lob application file.</span></span> <span data-ttu-id="2de23-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2de23-202">size</span><span class="sxs-lookup"><span data-stu-id="2de23-202">size</span></span>|<span data-ttu-id="2de23-203">Int64</span><span class="sxs-lookup"><span data-stu-id="2de23-203">Int64</span></span>|<span data-ttu-id="2de23-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="2de23-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="2de23-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2de23-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2de23-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="2de23-206">bundleId</span></span>|<span data-ttu-id="2de23-207">String</span><span class="sxs-lookup"><span data-stu-id="2de23-207">String</span></span>|<span data-ttu-id="2de23-208">バンドル id です。</span><span class="sxs-lookup"><span data-stu-id="2de23-208">The bundle id.</span></span>|
|<span data-ttu-id="2de23-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2de23-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2de23-210">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2de23-210">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="2de23-211">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="2de23-211">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2de23-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2de23-212">buildNumber</span></span>|<span data-ttu-id="2de23-213">String</span><span class="sxs-lookup"><span data-stu-id="2de23-213">String</span></span>|<span data-ttu-id="2de23-214">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="2de23-214">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2de23-215">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="2de23-215">versionNumber</span></span>|<span data-ttu-id="2de23-216">String</span><span class="sxs-lookup"><span data-stu-id="2de23-216">String</span></span>|<span data-ttu-id="2de23-217">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="2de23-217">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2de23-218">childApps</span><span class="sxs-lookup"><span data-stu-id="2de23-218">childApps</span></span>|<span data-ttu-id="2de23-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2de23-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="2de23-220">このバンドル パッケージ内のアプリケーションのリスト</span><span class="sxs-lookup"><span data-stu-id="2de23-220">The app list in this bundle package</span></span>|
|<span data-ttu-id="2de23-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2de23-221">identityVersion</span></span>|<span data-ttu-id="2de23-222">String</span><span class="sxs-lookup"><span data-stu-id="2de23-222">String</span></span>|<span data-ttu-id="2de23-223">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2de23-223">The identity version.</span></span>|
|<span data-ttu-id="2de23-224">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="2de23-224">md5HashChunkSize</span></span>|<span data-ttu-id="2de23-225">Int32</span><span class="sxs-lookup"><span data-stu-id="2de23-225">Int32</span></span>|<span data-ttu-id="2de23-226">MD5 ハッシュのチャンク ・ サイズ</span><span class="sxs-lookup"><span data-stu-id="2de23-226">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="2de23-227">md5Hash</span><span class="sxs-lookup"><span data-stu-id="2de23-227">md5Hash</span></span>|<span data-ttu-id="2de23-228">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2de23-228">String collection</span></span>|<span data-ttu-id="2de23-229">MD5 のハッシュ コード</span><span class="sxs-lookup"><span data-stu-id="2de23-229">The MD5 hash codes</span></span>|
|<span data-ttu-id="2de23-230">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="2de23-230">ignoreVersionDetection</span></span>|<span data-ttu-id="2de23-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="2de23-231">Boolean</span></span>|<span data-ttu-id="2de23-232">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="2de23-232">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="2de23-233">MacOS の自己更新機能を使用する基幹業務 (LoB) アプリケーションは、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="2de23-233">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="2de23-234">応答</span><span class="sxs-lookup"><span data-stu-id="2de23-234">Response</span></span>
<span data-ttu-id="2de23-235">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2de23-235">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2de23-236">例</span><span class="sxs-lookup"><span data-stu-id="2de23-236">Example</span></span>
### <a name="request"></a><span data-ttu-id="2de23-237">要求</span><span class="sxs-lookup"><span data-stu-id="2de23-237">Request</span></span>
<span data-ttu-id="2de23-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2de23-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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

### <a name="response"></a><span data-ttu-id="2de23-239">応答</span><span class="sxs-lookup"><span data-stu-id="2de23-239">Response</span></span>
<span data-ttu-id="2de23-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2de23-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





