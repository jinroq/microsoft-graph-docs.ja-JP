---
title: androidLobApp の更新
description: androidLobApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 928620e0ac689d139fe1ae953b7697efd2371119
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952269"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="7dce2-103">androidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="7dce2-103">Update androidLobApp</span></span>

> <span data-ttu-id="7dce2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dce2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dce2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dce2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dce2-106">[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7dce2-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dce2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7dce2-107">Prerequisites</span></span>
<span data-ttu-id="7dce2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dce2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7dce2-110">Permission type</span></span>|<span data-ttu-id="7dce2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7dce2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dce2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7dce2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dce2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dce2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7dce2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7dce2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dce2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dce2-115">Not supported.</span></span>|
|<span data-ttu-id="7dce2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7dce2-116">Application</span></span>|<span data-ttu-id="7dce2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dce2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dce2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dce2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7dce2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dce2-119">Request headers</span></span>
|<span data-ttu-id="7dce2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dce2-120">Header</span></span>|<span data-ttu-id="7dce2-121">値</span><span class="sxs-lookup"><span data-stu-id="7dce2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dce2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dce2-122">Authorization</span></span>|<span data-ttu-id="7dce2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dce2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dce2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7dce2-124">Accept</span></span>|<span data-ttu-id="7dce2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7dce2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dce2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dce2-126">Request body</span></span>
<span data-ttu-id="7dce2-127">要求本文で、[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7dce2-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="7dce2-128">次の表に、[androidLobApp](../resources/intune-apps-androidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7dce2-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="7dce2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dce2-129">Property</span></span>|<span data-ttu-id="7dce2-130">型</span><span class="sxs-lookup"><span data-stu-id="7dce2-130">Type</span></span>|<span data-ttu-id="7dce2-131">説明</span><span class="sxs-lookup"><span data-stu-id="7dce2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dce2-132">id</span><span class="sxs-lookup"><span data-stu-id="7dce2-132">id</span></span>|<span data-ttu-id="7dce2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7dce2-133">String</span></span>|<span data-ttu-id="7dce2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7dce2-134">Key of the entity.</span></span> <span data-ttu-id="7dce2-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7dce2-136">displayName</span></span>|<span data-ttu-id="7dce2-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7dce2-137">String</span></span>|<span data-ttu-id="7dce2-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7dce2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7dce2-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-140">description</span><span class="sxs-lookup"><span data-stu-id="7dce2-140">description</span></span>|<span data-ttu-id="7dce2-141">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-141">String</span></span>|<span data-ttu-id="7dce2-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7dce2-142">The description of the app.</span></span> <span data-ttu-id="7dce2-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7dce2-144">publisher</span></span>|<span data-ttu-id="7dce2-145">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-145">String</span></span>|<span data-ttu-id="7dce2-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7dce2-146">The publisher of the app.</span></span> <span data-ttu-id="7dce2-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7dce2-148">largeIcon</span></span>|[<span data-ttu-id="7dce2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7dce2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7dce2-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7dce2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7dce2-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dce2-152">createdDateTime</span></span>|<span data-ttu-id="7dce2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dce2-153">DateTimeOffset</span></span>|<span data-ttu-id="7dce2-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7dce2-154">The date and time the app was created.</span></span> <span data-ttu-id="7dce2-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dce2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7dce2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dce2-157">DateTimeOffset</span></span>|<span data-ttu-id="7dce2-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7dce2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7dce2-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7dce2-160">isFeatured</span></span>|<span data-ttu-id="7dce2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dce2-161">Boolean</span></span>|<span data-ttu-id="7dce2-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7dce2-163">privacyInformationUrl</span></span>|<span data-ttu-id="7dce2-164">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-164">String</span></span>|<span data-ttu-id="7dce2-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7dce2-165">The privacy statement Url.</span></span> <span data-ttu-id="7dce2-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7dce2-167">informationUrl</span></span>|<span data-ttu-id="7dce2-168">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-168">String</span></span>|<span data-ttu-id="7dce2-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7dce2-169">The more information Url.</span></span> <span data-ttu-id="7dce2-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-171">owner</span><span class="sxs-lookup"><span data-stu-id="7dce2-171">owner</span></span>|<span data-ttu-id="7dce2-172">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-172">String</span></span>|<span data-ttu-id="7dce2-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7dce2-173">The owner of the app.</span></span> <span data-ttu-id="7dce2-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-175">developer</span><span class="sxs-lookup"><span data-stu-id="7dce2-175">developer</span></span>|<span data-ttu-id="7dce2-176">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-176">String</span></span>|<span data-ttu-id="7dce2-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7dce2-177">The developer of the app.</span></span> <span data-ttu-id="7dce2-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-179">notes</span><span class="sxs-lookup"><span data-stu-id="7dce2-179">notes</span></span>|<span data-ttu-id="7dce2-180">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-180">String</span></span>|<span data-ttu-id="7dce2-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7dce2-181">Notes for the app.</span></span> <span data-ttu-id="7dce2-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7dce2-183">uploadState</span></span>|<span data-ttu-id="7dce2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7dce2-184">Int32</span></span>|<span data-ttu-id="7dce2-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="7dce2-185">The upload state.</span></span> <span data-ttu-id="7dce2-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7dce2-187">publishingState</span></span>|[<span data-ttu-id="7dce2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7dce2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7dce2-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7dce2-189">The publishing state for the app.</span></span> <span data-ttu-id="7dce2-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7dce2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7dce2-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7dce2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7dce2-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7dce2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7dce2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7dce2-193">isAssigned</span></span>|<span data-ttu-id="7dce2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dce2-194">Boolean</span></span>|<span data-ttu-id="7dce2-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7dce2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7dce2-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7dce2-197">roleScopeTagIds</span></span>|<span data-ttu-id="7dce2-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7dce2-198">String collection</span></span>|<span data-ttu-id="7dce2-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="7dce2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7dce2-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7dce2-201">dependentAppCount</span></span>|<span data-ttu-id="7dce2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7dce2-202">Int32</span></span>|<span data-ttu-id="7dce2-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="7dce2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7dce2-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dce2-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7dce2-205">committedContentVersion</span></span>|<span data-ttu-id="7dce2-206">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-206">String</span></span>|<span data-ttu-id="7dce2-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7dce2-207">The internal committed content version.</span></span> <span data-ttu-id="7dce2-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dce2-209">fileName</span><span class="sxs-lookup"><span data-stu-id="7dce2-209">fileName</span></span>|<span data-ttu-id="7dce2-210">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-210">String</span></span>|<span data-ttu-id="7dce2-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="7dce2-211">The name of the main Lob application file.</span></span> <span data-ttu-id="7dce2-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dce2-213">size</span><span class="sxs-lookup"><span data-stu-id="7dce2-213">size</span></span>|<span data-ttu-id="7dce2-214">Int64</span><span class="sxs-lookup"><span data-stu-id="7dce2-214">Int64</span></span>|<span data-ttu-id="7dce2-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="7dce2-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="7dce2-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7dce2-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dce2-217">packageId</span><span class="sxs-lookup"><span data-stu-id="7dce2-217">packageId</span></span>|<span data-ttu-id="7dce2-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7dce2-218">String</span></span>|<span data-ttu-id="7dce2-219">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="7dce2-219">The package identifier.</span></span>|
|<span data-ttu-id="7dce2-220">identityName</span><span class="sxs-lookup"><span data-stu-id="7dce2-220">identityName</span></span>|<span data-ttu-id="7dce2-221">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-221">String</span></span>|<span data-ttu-id="7dce2-222">ID 名。</span><span class="sxs-lookup"><span data-stu-id="7dce2-222">The Identity Name.</span></span>|
|<span data-ttu-id="7dce2-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dce2-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7dce2-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dce2-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7dce2-225">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="7dce2-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7dce2-226">versionName</span><span class="sxs-lookup"><span data-stu-id="7dce2-226">versionName</span></span>|<span data-ttu-id="7dce2-227">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-227">String</span></span>|<span data-ttu-id="7dce2-228">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="7dce2-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7dce2-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="7dce2-229">versionCode</span></span>|<span data-ttu-id="7dce2-230">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-230">String</span></span>|<span data-ttu-id="7dce2-231">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="7dce2-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7dce2-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7dce2-232">identityVersion</span></span>|<span data-ttu-id="7dce2-233">String</span><span class="sxs-lookup"><span data-stu-id="7dce2-233">String</span></span>|<span data-ttu-id="7dce2-234">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7dce2-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7dce2-235">応答</span><span class="sxs-lookup"><span data-stu-id="7dce2-235">Response</span></span>
<span data-ttu-id="7dce2-236">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7dce2-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dce2-237">例</span><span class="sxs-lookup"><span data-stu-id="7dce2-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dce2-238">要求</span><span class="sxs-lookup"><span data-stu-id="7dce2-238">Request</span></span>
<span data-ttu-id="7dce2-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7dce2-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="7dce2-240">応答</span><span class="sxs-lookup"><span data-stu-id="7dce2-240">Response</span></span>
<span data-ttu-id="7dce2-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7dce2-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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





