---
title: MacOSLobApp の更新
description: MacOSLobApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69a2a938d142ac98c0eb705abe871228e707eb46
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962128"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="04e12-103">MacOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="04e12-103">Update macOSLobApp</span></span>

> <span data-ttu-id="04e12-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04e12-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04e12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e12-106">[Macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04e12-106">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04e12-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="04e12-107">Prerequisites</span></span>
<span data-ttu-id="04e12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e12-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04e12-110">Permission type</span></span>|<span data-ttu-id="04e12-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04e12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e12-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04e12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04e12-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e12-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04e12-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04e12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e12-115">Not supported.</span></span>|
|<span data-ttu-id="04e12-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04e12-116">Application</span></span>|<span data-ttu-id="04e12-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e12-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04e12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="04e12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e12-119">Request headers</span></span>
|<span data-ttu-id="04e12-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e12-120">Header</span></span>|<span data-ttu-id="04e12-121">値</span><span class="sxs-lookup"><span data-stu-id="04e12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e12-122">Authorization</span></span>|<span data-ttu-id="04e12-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="04e12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e12-124">承諾</span><span class="sxs-lookup"><span data-stu-id="04e12-124">Accept</span></span>|<span data-ttu-id="04e12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04e12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e12-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04e12-126">Request body</span></span>
<span data-ttu-id="04e12-127">要求本文で、 [Macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04e12-127">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="04e12-128">次の表に、 [Macoslobapp](../resources/intune-apps-macoslobapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04e12-128">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="04e12-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04e12-129">Property</span></span>|<span data-ttu-id="04e12-130">型</span><span class="sxs-lookup"><span data-stu-id="04e12-130">Type</span></span>|<span data-ttu-id="04e12-131">説明</span><span class="sxs-lookup"><span data-stu-id="04e12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e12-132">id</span><span class="sxs-lookup"><span data-stu-id="04e12-132">id</span></span>|<span data-ttu-id="04e12-133">文字列</span><span class="sxs-lookup"><span data-stu-id="04e12-133">String</span></span>|<span data-ttu-id="04e12-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04e12-134">Key of the entity.</span></span> <span data-ttu-id="04e12-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-136">displayName</span><span class="sxs-lookup"><span data-stu-id="04e12-136">displayName</span></span>|<span data-ttu-id="04e12-137">文字列</span><span class="sxs-lookup"><span data-stu-id="04e12-137">String</span></span>|<span data-ttu-id="04e12-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="04e12-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="04e12-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-140">description</span><span class="sxs-lookup"><span data-stu-id="04e12-140">description</span></span>|<span data-ttu-id="04e12-141">String</span><span class="sxs-lookup"><span data-stu-id="04e12-141">String</span></span>|<span data-ttu-id="04e12-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="04e12-142">The description of the app.</span></span> <span data-ttu-id="04e12-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-144">publisher</span><span class="sxs-lookup"><span data-stu-id="04e12-144">publisher</span></span>|<span data-ttu-id="04e12-145">String</span><span class="sxs-lookup"><span data-stu-id="04e12-145">String</span></span>|<span data-ttu-id="04e12-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="04e12-146">The publisher of the app.</span></span> <span data-ttu-id="04e12-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="04e12-148">largeIcon</span></span>|[<span data-ttu-id="04e12-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="04e12-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="04e12-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="04e12-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="04e12-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04e12-152">createdDateTime</span></span>|<span data-ttu-id="04e12-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e12-153">DateTimeOffset</span></span>|<span data-ttu-id="04e12-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="04e12-154">The date and time the app was created.</span></span> <span data-ttu-id="04e12-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04e12-156">lastModifiedDateTime</span></span>|<span data-ttu-id="04e12-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e12-157">DateTimeOffset</span></span>|<span data-ttu-id="04e12-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="04e12-158">The date and time the app was last modified.</span></span> <span data-ttu-id="04e12-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="04e12-160">isFeatured</span></span>|<span data-ttu-id="04e12-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e12-161">Boolean</span></span>|<span data-ttu-id="04e12-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="04e12-163">privacyInformationUrl</span></span>|<span data-ttu-id="04e12-164">String</span><span class="sxs-lookup"><span data-stu-id="04e12-164">String</span></span>|<span data-ttu-id="04e12-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="04e12-165">The privacy statement Url.</span></span> <span data-ttu-id="04e12-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="04e12-167">informationUrl</span></span>|<span data-ttu-id="04e12-168">String</span><span class="sxs-lookup"><span data-stu-id="04e12-168">String</span></span>|<span data-ttu-id="04e12-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="04e12-169">The more information Url.</span></span> <span data-ttu-id="04e12-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-171">owner</span><span class="sxs-lookup"><span data-stu-id="04e12-171">owner</span></span>|<span data-ttu-id="04e12-172">String</span><span class="sxs-lookup"><span data-stu-id="04e12-172">String</span></span>|<span data-ttu-id="04e12-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="04e12-173">The owner of the app.</span></span> <span data-ttu-id="04e12-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-175">developer</span><span class="sxs-lookup"><span data-stu-id="04e12-175">developer</span></span>|<span data-ttu-id="04e12-176">String</span><span class="sxs-lookup"><span data-stu-id="04e12-176">String</span></span>|<span data-ttu-id="04e12-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="04e12-177">The developer of the app.</span></span> <span data-ttu-id="04e12-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-179">notes</span><span class="sxs-lookup"><span data-stu-id="04e12-179">notes</span></span>|<span data-ttu-id="04e12-180">String</span><span class="sxs-lookup"><span data-stu-id="04e12-180">String</span></span>|<span data-ttu-id="04e12-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="04e12-181">Notes for the app.</span></span> <span data-ttu-id="04e12-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="04e12-183">uploadState</span></span>|<span data-ttu-id="04e12-184">Int32</span><span class="sxs-lookup"><span data-stu-id="04e12-184">Int32</span></span>|<span data-ttu-id="04e12-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="04e12-185">The upload state.</span></span> <span data-ttu-id="04e12-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="04e12-187">publishingState</span></span>|[<span data-ttu-id="04e12-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="04e12-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="04e12-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="04e12-189">The publishing state for the app.</span></span> <span data-ttu-id="04e12-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="04e12-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="04e12-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04e12-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="04e12-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="04e12-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="04e12-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="04e12-193">isAssigned</span></span>|<span data-ttu-id="04e12-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e12-194">Boolean</span></span>|<span data-ttu-id="04e12-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="04e12-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="04e12-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04e12-197">roleScopeTagIds</span></span>|<span data-ttu-id="04e12-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="04e12-198">String collection</span></span>|<span data-ttu-id="04e12-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="04e12-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="04e12-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="04e12-201">dependentAppCount</span></span>|<span data-ttu-id="04e12-202">Int32</span><span class="sxs-lookup"><span data-stu-id="04e12-202">Int32</span></span>|<span data-ttu-id="04e12-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="04e12-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="04e12-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04e12-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="04e12-205">committedContentVersion</span></span>|<span data-ttu-id="04e12-206">String</span><span class="sxs-lookup"><span data-stu-id="04e12-206">String</span></span>|<span data-ttu-id="04e12-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="04e12-207">The internal committed content version.</span></span> <span data-ttu-id="04e12-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e12-209">fileName</span><span class="sxs-lookup"><span data-stu-id="04e12-209">fileName</span></span>|<span data-ttu-id="04e12-210">String</span><span class="sxs-lookup"><span data-stu-id="04e12-210">String</span></span>|<span data-ttu-id="04e12-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="04e12-211">The name of the main Lob application file.</span></span> <span data-ttu-id="04e12-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e12-213">size</span><span class="sxs-lookup"><span data-stu-id="04e12-213">size</span></span>|<span data-ttu-id="04e12-214">Int64</span><span class="sxs-lookup"><span data-stu-id="04e12-214">Int64</span></span>|<span data-ttu-id="04e12-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="04e12-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="04e12-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e12-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e12-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="04e12-217">bundleId</span></span>|<span data-ttu-id="04e12-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="04e12-218">String</span></span>|<span data-ttu-id="04e12-219">バンドル id。</span><span class="sxs-lookup"><span data-stu-id="04e12-219">The bundle id.</span></span>|
|<span data-ttu-id="04e12-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04e12-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="04e12-221">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04e12-221">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="04e12-222">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="04e12-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="04e12-223">buildNumber</span><span class="sxs-lookup"><span data-stu-id="04e12-223">buildNumber</span></span>|<span data-ttu-id="04e12-224">String</span><span class="sxs-lookup"><span data-stu-id="04e12-224">String</span></span>|<span data-ttu-id="04e12-225">MacOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="04e12-225">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04e12-226">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="04e12-226">versionNumber</span></span>|<span data-ttu-id="04e12-227">String</span><span class="sxs-lookup"><span data-stu-id="04e12-227">String</span></span>|<span data-ttu-id="04e12-228">MacOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="04e12-228">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04e12-229">childApps</span><span class="sxs-lookup"><span data-stu-id="04e12-229">childApps</span></span>|<span data-ttu-id="04e12-230">[Macoslobchildapp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04e12-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="04e12-231">このバンドルパッケージのアプリリスト</span><span class="sxs-lookup"><span data-stu-id="04e12-231">The app list in this bundle package</span></span>|
|<span data-ttu-id="04e12-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="04e12-232">identityVersion</span></span>|<span data-ttu-id="04e12-233">String</span><span class="sxs-lookup"><span data-stu-id="04e12-233">String</span></span>|<span data-ttu-id="04e12-234">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="04e12-234">The identity version.</span></span>|
|<span data-ttu-id="04e12-235">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="04e12-235">md5HashChunkSize</span></span>|<span data-ttu-id="04e12-236">Int32</span><span class="sxs-lookup"><span data-stu-id="04e12-236">Int32</span></span>|<span data-ttu-id="04e12-237">MD5 ハッシュのチャンクサイズ</span><span class="sxs-lookup"><span data-stu-id="04e12-237">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="04e12-238">md5Hash</span><span class="sxs-lookup"><span data-stu-id="04e12-238">md5Hash</span></span>|<span data-ttu-id="04e12-239">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="04e12-239">String collection</span></span>|<span data-ttu-id="04e12-240">MD5 ハッシュコード</span><span class="sxs-lookup"><span data-stu-id="04e12-240">The MD5 hash codes</span></span>|
|<span data-ttu-id="04e12-241">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="04e12-241">ignoreVersionDetection</span></span>|<span data-ttu-id="04e12-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e12-242">Boolean</span></span>|<span data-ttu-id="04e12-243">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="04e12-243">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="04e12-244">自己更新機能を使用する macOS 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="04e12-244">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="04e12-245">応答</span><span class="sxs-lookup"><span data-stu-id="04e12-245">Response</span></span>
<span data-ttu-id="04e12-246">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04e12-246">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e12-247">例</span><span class="sxs-lookup"><span data-stu-id="04e12-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="04e12-248">要求</span><span class="sxs-lookup"><span data-stu-id="04e12-248">Request</span></span>
<span data-ttu-id="04e12-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04e12-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1574

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="04e12-250">応答</span><span class="sxs-lookup"><span data-stu-id="04e12-250">Response</span></span>
<span data-ttu-id="04e12-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04e12-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1746

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
  "dependentAppCount": 1,
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





