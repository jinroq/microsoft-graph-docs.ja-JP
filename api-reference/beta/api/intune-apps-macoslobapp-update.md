---
title: MacOSLobApp を更新します。
description: MacOSLobApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bcf3301fb022f672db1340f45296ca19763a4d63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413599"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="15845-103">MacOSLobApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="15845-103">Update macOSLobApp</span></span>

> <span data-ttu-id="15845-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15845-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15845-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15845-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15845-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15845-107">[MacOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15845-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15845-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="15845-108">Prerequisites</span></span>
<span data-ttu-id="15845-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15845-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15845-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15845-111">Permission type</span></span>|<span data-ttu-id="15845-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15845-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15845-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15845-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15845-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15845-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15845-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15845-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15845-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15845-116">Not supported.</span></span>|
|<span data-ttu-id="15845-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15845-117">Application</span></span>|<span data-ttu-id="15845-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15845-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15845-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15845-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="15845-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15845-120">Request headers</span></span>
|<span data-ttu-id="15845-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15845-121">Header</span></span>|<span data-ttu-id="15845-122">値</span><span class="sxs-lookup"><span data-stu-id="15845-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15845-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15845-123">Authorization</span></span>|<span data-ttu-id="15845-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="15845-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15845-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15845-125">Accept</span></span>|<span data-ttu-id="15845-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15845-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15845-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="15845-127">Request body</span></span>
<span data-ttu-id="15845-128">要求の本文に[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="15845-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="15845-129">[MacOSLobApp](../resources/intune-apps-macoslobapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="15845-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="15845-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15845-130">Property</span></span>|<span data-ttu-id="15845-131">型</span><span class="sxs-lookup"><span data-stu-id="15845-131">Type</span></span>|<span data-ttu-id="15845-132">説明</span><span class="sxs-lookup"><span data-stu-id="15845-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15845-133">id</span><span class="sxs-lookup"><span data-stu-id="15845-133">id</span></span>|<span data-ttu-id="15845-134">String</span><span class="sxs-lookup"><span data-stu-id="15845-134">String</span></span>|<span data-ttu-id="15845-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="15845-135">Key of the entity.</span></span> <span data-ttu-id="15845-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-137">displayName</span><span class="sxs-lookup"><span data-stu-id="15845-137">displayName</span></span>|<span data-ttu-id="15845-138">String</span><span class="sxs-lookup"><span data-stu-id="15845-138">String</span></span>|<span data-ttu-id="15845-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="15845-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="15845-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-141">説明</span><span class="sxs-lookup"><span data-stu-id="15845-141">description</span></span>|<span data-ttu-id="15845-142">String</span><span class="sxs-lookup"><span data-stu-id="15845-142">String</span></span>|<span data-ttu-id="15845-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="15845-143">The description of the app.</span></span> <span data-ttu-id="15845-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-145">publisher</span><span class="sxs-lookup"><span data-stu-id="15845-145">publisher</span></span>|<span data-ttu-id="15845-146">String</span><span class="sxs-lookup"><span data-stu-id="15845-146">String</span></span>|<span data-ttu-id="15845-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="15845-147">The publisher of the app.</span></span> <span data-ttu-id="15845-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="15845-149">largeIcon</span></span>|[<span data-ttu-id="15845-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="15845-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="15845-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="15845-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="15845-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15845-153">createdDateTime</span></span>|<span data-ttu-id="15845-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15845-154">DateTimeOffset</span></span>|<span data-ttu-id="15845-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="15845-155">The date and time the app was created.</span></span> <span data-ttu-id="15845-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15845-157">lastModifiedDateTime</span></span>|<span data-ttu-id="15845-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15845-158">DateTimeOffset</span></span>|<span data-ttu-id="15845-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="15845-159">The date and time the app was last modified.</span></span> <span data-ttu-id="15845-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="15845-161">isFeatured</span></span>|<span data-ttu-id="15845-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="15845-162">Boolean</span></span>|<span data-ttu-id="15845-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="15845-164">privacyInformationUrl</span></span>|<span data-ttu-id="15845-165">String</span><span class="sxs-lookup"><span data-stu-id="15845-165">String</span></span>|<span data-ttu-id="15845-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="15845-166">The privacy statement Url.</span></span> <span data-ttu-id="15845-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="15845-168">informationUrl</span></span>|<span data-ttu-id="15845-169">String</span><span class="sxs-lookup"><span data-stu-id="15845-169">String</span></span>|<span data-ttu-id="15845-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="15845-170">The more information Url.</span></span> <span data-ttu-id="15845-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-172">owner</span><span class="sxs-lookup"><span data-stu-id="15845-172">owner</span></span>|<span data-ttu-id="15845-173">String</span><span class="sxs-lookup"><span data-stu-id="15845-173">String</span></span>|<span data-ttu-id="15845-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="15845-174">The owner of the app.</span></span> <span data-ttu-id="15845-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-176">developer</span><span class="sxs-lookup"><span data-stu-id="15845-176">developer</span></span>|<span data-ttu-id="15845-177">String</span><span class="sxs-lookup"><span data-stu-id="15845-177">String</span></span>|<span data-ttu-id="15845-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="15845-178">The developer of the app.</span></span> <span data-ttu-id="15845-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-180">notes</span><span class="sxs-lookup"><span data-stu-id="15845-180">notes</span></span>|<span data-ttu-id="15845-181">String</span><span class="sxs-lookup"><span data-stu-id="15845-181">String</span></span>|<span data-ttu-id="15845-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="15845-182">Notes for the app.</span></span> <span data-ttu-id="15845-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="15845-184">uploadState</span></span>|<span data-ttu-id="15845-185">Int32</span><span class="sxs-lookup"><span data-stu-id="15845-185">Int32</span></span>|<span data-ttu-id="15845-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="15845-186">The upload state.</span></span> <span data-ttu-id="15845-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="15845-188">publishingState</span></span>|[<span data-ttu-id="15845-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="15845-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="15845-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="15845-190">The publishing state for the app.</span></span> <span data-ttu-id="15845-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="15845-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="15845-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="15845-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="15845-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="15845-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="15845-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="15845-194">isAssigned</span></span>|<span data-ttu-id="15845-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="15845-195">Boolean</span></span>|<span data-ttu-id="15845-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="15845-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="15845-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15845-198">roleScopeTagIds</span></span>|<span data-ttu-id="15845-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="15845-199">String collection</span></span>|<span data-ttu-id="15845-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="15845-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="15845-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15845-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="15845-202">committedContentVersion</span></span>|<span data-ttu-id="15845-203">String</span><span class="sxs-lookup"><span data-stu-id="15845-203">String</span></span>|<span data-ttu-id="15845-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="15845-204">The internal committed content version.</span></span> <span data-ttu-id="15845-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="15845-206">fileName</span><span class="sxs-lookup"><span data-stu-id="15845-206">fileName</span></span>|<span data-ttu-id="15845-207">String</span><span class="sxs-lookup"><span data-stu-id="15845-207">String</span></span>|<span data-ttu-id="15845-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="15845-208">The name of the main Lob application file.</span></span> <span data-ttu-id="15845-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="15845-210">size</span><span class="sxs-lookup"><span data-stu-id="15845-210">size</span></span>|<span data-ttu-id="15845-211">Int64</span><span class="sxs-lookup"><span data-stu-id="15845-211">Int64</span></span>|<span data-ttu-id="15845-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="15845-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="15845-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15845-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="15845-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="15845-214">bundleId</span></span>|<span data-ttu-id="15845-215">String</span><span class="sxs-lookup"><span data-stu-id="15845-215">String</span></span>|<span data-ttu-id="15845-216">バンドル id です。</span><span class="sxs-lookup"><span data-stu-id="15845-216">The bundle id.</span></span>|
|<span data-ttu-id="15845-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="15845-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="15845-218">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="15845-218">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="15845-219">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="15845-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="15845-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="15845-220">buildNumber</span></span>|<span data-ttu-id="15845-221">String</span><span class="sxs-lookup"><span data-stu-id="15845-221">String</span></span>|<span data-ttu-id="15845-222">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="15845-222">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="15845-223">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="15845-223">versionNumber</span></span>|<span data-ttu-id="15845-224">String</span><span class="sxs-lookup"><span data-stu-id="15845-224">String</span></span>|<span data-ttu-id="15845-225">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="15845-225">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="15845-226">childApps</span><span class="sxs-lookup"><span data-stu-id="15845-226">childApps</span></span>|<span data-ttu-id="15845-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15845-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="15845-228">このバンドル パッケージ内のアプリケーションのリスト</span><span class="sxs-lookup"><span data-stu-id="15845-228">The app list in this bundle package</span></span>|
|<span data-ttu-id="15845-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="15845-229">identityVersion</span></span>|<span data-ttu-id="15845-230">String</span><span class="sxs-lookup"><span data-stu-id="15845-230">String</span></span>|<span data-ttu-id="15845-231">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="15845-231">The identity version.</span></span>|
|<span data-ttu-id="15845-232">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="15845-232">md5HashChunkSize</span></span>|<span data-ttu-id="15845-233">Int32</span><span class="sxs-lookup"><span data-stu-id="15845-233">Int32</span></span>|<span data-ttu-id="15845-234">MD5 ハッシュのチャンク ・ サイズ</span><span class="sxs-lookup"><span data-stu-id="15845-234">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="15845-235">md5Hash</span><span class="sxs-lookup"><span data-stu-id="15845-235">md5Hash</span></span>|<span data-ttu-id="15845-236">String コレクション</span><span class="sxs-lookup"><span data-stu-id="15845-236">String collection</span></span>|<span data-ttu-id="15845-237">MD5 のハッシュ コード</span><span class="sxs-lookup"><span data-stu-id="15845-237">The MD5 hash codes</span></span>|
|<span data-ttu-id="15845-238">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="15845-238">ignoreVersionDetection</span></span>|<span data-ttu-id="15845-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="15845-239">Boolean</span></span>|<span data-ttu-id="15845-240">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="15845-240">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="15845-241">MacOS の自己更新機能を使用する基幹業務 (LoB) アプリケーションは、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="15845-241">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="15845-242">応答</span><span class="sxs-lookup"><span data-stu-id="15845-242">Response</span></span>
<span data-ttu-id="15845-243">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOSLobApp](../resources/intune-apps-macoslobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="15845-243">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15845-244">例</span><span class="sxs-lookup"><span data-stu-id="15845-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="15845-245">要求</span><span class="sxs-lookup"><span data-stu-id="15845-245">Request</span></span>
<span data-ttu-id="15845-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15845-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="15845-247">応答</span><span class="sxs-lookup"><span data-stu-id="15845-247">Response</span></span>
<span data-ttu-id="15845-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15845-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




