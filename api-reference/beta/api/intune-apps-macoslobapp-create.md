---
title: MacOSLobApp を作成します。
description: 新しい macOSLobApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 264bc1e104e7b582f3a15f38d2f5a8a585095789
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418100"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="07130-103">MacOSLobApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="07130-103">Create macOSLobApp</span></span>

> <span data-ttu-id="07130-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07130-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07130-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07130-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07130-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07130-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07130-107">新しい[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="07130-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07130-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="07130-108">Prerequisites</span></span>
<span data-ttu-id="07130-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07130-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07130-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07130-111">Permission type</span></span>|<span data-ttu-id="07130-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="07130-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07130-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07130-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07130-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07130-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07130-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07130-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07130-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07130-116">Not supported.</span></span>|
|<span data-ttu-id="07130-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07130-117">Application</span></span>|<span data-ttu-id="07130-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07130-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07130-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07130-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="07130-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07130-120">Request headers</span></span>
|<span data-ttu-id="07130-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07130-121">Header</span></span>|<span data-ttu-id="07130-122">値</span><span class="sxs-lookup"><span data-stu-id="07130-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07130-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07130-123">Authorization</span></span>|<span data-ttu-id="07130-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="07130-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07130-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07130-125">Accept</span></span>|<span data-ttu-id="07130-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07130-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07130-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="07130-127">Request body</span></span>
<span data-ttu-id="07130-128">要求の本文に macOSLobApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="07130-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="07130-129">次の表は、macOSLobApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="07130-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="07130-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07130-130">Property</span></span>|<span data-ttu-id="07130-131">型</span><span class="sxs-lookup"><span data-stu-id="07130-131">Type</span></span>|<span data-ttu-id="07130-132">説明</span><span class="sxs-lookup"><span data-stu-id="07130-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07130-133">id</span><span class="sxs-lookup"><span data-stu-id="07130-133">id</span></span>|<span data-ttu-id="07130-134">String</span><span class="sxs-lookup"><span data-stu-id="07130-134">String</span></span>|<span data-ttu-id="07130-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="07130-135">Key of the entity.</span></span> <span data-ttu-id="07130-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-137">displayName</span><span class="sxs-lookup"><span data-stu-id="07130-137">displayName</span></span>|<span data-ttu-id="07130-138">String</span><span class="sxs-lookup"><span data-stu-id="07130-138">String</span></span>|<span data-ttu-id="07130-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="07130-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="07130-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-141">説明</span><span class="sxs-lookup"><span data-stu-id="07130-141">description</span></span>|<span data-ttu-id="07130-142">String</span><span class="sxs-lookup"><span data-stu-id="07130-142">String</span></span>|<span data-ttu-id="07130-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="07130-143">The description of the app.</span></span> <span data-ttu-id="07130-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-145">publisher</span><span class="sxs-lookup"><span data-stu-id="07130-145">publisher</span></span>|<span data-ttu-id="07130-146">String</span><span class="sxs-lookup"><span data-stu-id="07130-146">String</span></span>|<span data-ttu-id="07130-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="07130-147">The publisher of the app.</span></span> <span data-ttu-id="07130-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="07130-149">largeIcon</span></span>|[<span data-ttu-id="07130-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07130-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07130-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="07130-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="07130-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07130-153">createdDateTime</span></span>|<span data-ttu-id="07130-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07130-154">DateTimeOffset</span></span>|<span data-ttu-id="07130-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="07130-155">The date and time the app was created.</span></span> <span data-ttu-id="07130-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07130-157">lastModifiedDateTime</span></span>|<span data-ttu-id="07130-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07130-158">DateTimeOffset</span></span>|<span data-ttu-id="07130-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="07130-159">The date and time the app was last modified.</span></span> <span data-ttu-id="07130-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="07130-161">isFeatured</span></span>|<span data-ttu-id="07130-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="07130-162">Boolean</span></span>|<span data-ttu-id="07130-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="07130-164">privacyInformationUrl</span></span>|<span data-ttu-id="07130-165">String</span><span class="sxs-lookup"><span data-stu-id="07130-165">String</span></span>|<span data-ttu-id="07130-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="07130-166">The privacy statement Url.</span></span> <span data-ttu-id="07130-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="07130-168">informationUrl</span></span>|<span data-ttu-id="07130-169">String</span><span class="sxs-lookup"><span data-stu-id="07130-169">String</span></span>|<span data-ttu-id="07130-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="07130-170">The more information Url.</span></span> <span data-ttu-id="07130-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-172">owner</span><span class="sxs-lookup"><span data-stu-id="07130-172">owner</span></span>|<span data-ttu-id="07130-173">String</span><span class="sxs-lookup"><span data-stu-id="07130-173">String</span></span>|<span data-ttu-id="07130-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="07130-174">The owner of the app.</span></span> <span data-ttu-id="07130-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-176">developer</span><span class="sxs-lookup"><span data-stu-id="07130-176">developer</span></span>|<span data-ttu-id="07130-177">String</span><span class="sxs-lookup"><span data-stu-id="07130-177">String</span></span>|<span data-ttu-id="07130-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="07130-178">The developer of the app.</span></span> <span data-ttu-id="07130-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-180">notes</span><span class="sxs-lookup"><span data-stu-id="07130-180">notes</span></span>|<span data-ttu-id="07130-181">String</span><span class="sxs-lookup"><span data-stu-id="07130-181">String</span></span>|<span data-ttu-id="07130-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="07130-182">Notes for the app.</span></span> <span data-ttu-id="07130-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="07130-184">uploadState</span></span>|<span data-ttu-id="07130-185">Int32</span><span class="sxs-lookup"><span data-stu-id="07130-185">Int32</span></span>|<span data-ttu-id="07130-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="07130-186">The upload state.</span></span> <span data-ttu-id="07130-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="07130-188">publishingState</span></span>|[<span data-ttu-id="07130-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="07130-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="07130-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="07130-190">The publishing state for the app.</span></span> <span data-ttu-id="07130-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="07130-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="07130-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="07130-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="07130-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="07130-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="07130-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="07130-194">isAssigned</span></span>|<span data-ttu-id="07130-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="07130-195">Boolean</span></span>|<span data-ttu-id="07130-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="07130-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="07130-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07130-198">roleScopeTagIds</span></span>|<span data-ttu-id="07130-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="07130-199">String collection</span></span>|<span data-ttu-id="07130-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="07130-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="07130-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07130-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="07130-202">committedContentVersion</span></span>|<span data-ttu-id="07130-203">String</span><span class="sxs-lookup"><span data-stu-id="07130-203">String</span></span>|<span data-ttu-id="07130-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="07130-204">The internal committed content version.</span></span> <span data-ttu-id="07130-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="07130-206">fileName</span><span class="sxs-lookup"><span data-stu-id="07130-206">fileName</span></span>|<span data-ttu-id="07130-207">String</span><span class="sxs-lookup"><span data-stu-id="07130-207">String</span></span>|<span data-ttu-id="07130-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="07130-208">The name of the main Lob application file.</span></span> <span data-ttu-id="07130-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="07130-210">size</span><span class="sxs-lookup"><span data-stu-id="07130-210">size</span></span>|<span data-ttu-id="07130-211">Int64</span><span class="sxs-lookup"><span data-stu-id="07130-211">Int64</span></span>|<span data-ttu-id="07130-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="07130-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="07130-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07130-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="07130-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="07130-214">bundleId</span></span>|<span data-ttu-id="07130-215">String</span><span class="sxs-lookup"><span data-stu-id="07130-215">String</span></span>|<span data-ttu-id="07130-216">バンドル id です。</span><span class="sxs-lookup"><span data-stu-id="07130-216">The bundle id.</span></span>|
|<span data-ttu-id="07130-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="07130-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="07130-218">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="07130-218">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="07130-219">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="07130-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="07130-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="07130-220">buildNumber</span></span>|<span data-ttu-id="07130-221">String</span><span class="sxs-lookup"><span data-stu-id="07130-221">String</span></span>|<span data-ttu-id="07130-222">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="07130-222">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="07130-223">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="07130-223">versionNumber</span></span>|<span data-ttu-id="07130-224">String</span><span class="sxs-lookup"><span data-stu-id="07130-224">String</span></span>|<span data-ttu-id="07130-225">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="07130-225">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="07130-226">childApps</span><span class="sxs-lookup"><span data-stu-id="07130-226">childApps</span></span>|<span data-ttu-id="07130-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07130-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="07130-228">このバンドル パッケージ内のアプリケーションのリスト</span><span class="sxs-lookup"><span data-stu-id="07130-228">The app list in this bundle package</span></span>|
|<span data-ttu-id="07130-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="07130-229">identityVersion</span></span>|<span data-ttu-id="07130-230">String</span><span class="sxs-lookup"><span data-stu-id="07130-230">String</span></span>|<span data-ttu-id="07130-231">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="07130-231">The identity version.</span></span>|
|<span data-ttu-id="07130-232">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="07130-232">md5HashChunkSize</span></span>|<span data-ttu-id="07130-233">Int32</span><span class="sxs-lookup"><span data-stu-id="07130-233">Int32</span></span>|<span data-ttu-id="07130-234">MD5 ハッシュのチャンク ・ サイズ</span><span class="sxs-lookup"><span data-stu-id="07130-234">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="07130-235">md5Hash</span><span class="sxs-lookup"><span data-stu-id="07130-235">md5Hash</span></span>|<span data-ttu-id="07130-236">String コレクション</span><span class="sxs-lookup"><span data-stu-id="07130-236">String collection</span></span>|<span data-ttu-id="07130-237">MD5 のハッシュ コード</span><span class="sxs-lookup"><span data-stu-id="07130-237">The MD5 hash codes</span></span>|
|<span data-ttu-id="07130-238">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="07130-238">ignoreVersionDetection</span></span>|<span data-ttu-id="07130-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="07130-239">Boolean</span></span>|<span data-ttu-id="07130-240">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="07130-240">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="07130-241">MacOS の自己更新機能を使用する基幹業務 (LoB) アプリケーションは、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="07130-241">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="07130-242">応答</span><span class="sxs-lookup"><span data-stu-id="07130-242">Response</span></span>
<span data-ttu-id="07130-243">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="07130-243">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07130-244">例</span><span class="sxs-lookup"><span data-stu-id="07130-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="07130-245">要求</span><span class="sxs-lookup"><span data-stu-id="07130-245">Request</span></span>
<span data-ttu-id="07130-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07130-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1547

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

### <a name="response"></a><span data-ttu-id="07130-247">応答</span><span class="sxs-lookup"><span data-stu-id="07130-247">Response</span></span>
<span data-ttu-id="07130-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07130-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1719

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




