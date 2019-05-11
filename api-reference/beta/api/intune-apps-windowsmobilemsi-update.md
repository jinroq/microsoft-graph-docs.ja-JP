---
title: windowsMobileMSI の更新
description: windowsMobileMSI オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad7bd8beb2572fa6c9f92976ab9a33f46b99fd70
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934706"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="694a0-103">windowsMobileMSI の更新</span><span class="sxs-lookup"><span data-stu-id="694a0-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="694a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="694a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="694a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="694a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="694a0-106">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="694a0-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="694a0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="694a0-107">Prerequisites</span></span>
<span data-ttu-id="694a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="694a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="694a0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="694a0-110">Permission type</span></span>|<span data-ttu-id="694a0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="694a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="694a0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="694a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="694a0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="694a0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="694a0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="694a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="694a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="694a0-115">Not supported.</span></span>|
|<span data-ttu-id="694a0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="694a0-116">Application</span></span>|<span data-ttu-id="694a0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="694a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="694a0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="694a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="694a0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="694a0-119">Request headers</span></span>
|<span data-ttu-id="694a0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="694a0-120">Header</span></span>|<span data-ttu-id="694a0-121">値</span><span class="sxs-lookup"><span data-stu-id="694a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="694a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="694a0-122">Authorization</span></span>|<span data-ttu-id="694a0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="694a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="694a0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="694a0-124">Accept</span></span>|<span data-ttu-id="694a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="694a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="694a0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="694a0-126">Request body</span></span>
<span data-ttu-id="694a0-127">要求本文で、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="694a0-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="694a0-128">次の表に、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="694a0-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="694a0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="694a0-129">Property</span></span>|<span data-ttu-id="694a0-130">型</span><span class="sxs-lookup"><span data-stu-id="694a0-130">Type</span></span>|<span data-ttu-id="694a0-131">説明</span><span class="sxs-lookup"><span data-stu-id="694a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="694a0-132">id</span><span class="sxs-lookup"><span data-stu-id="694a0-132">id</span></span>|<span data-ttu-id="694a0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="694a0-133">String</span></span>|<span data-ttu-id="694a0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="694a0-134">Key of the entity.</span></span> <span data-ttu-id="694a0-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="694a0-136">displayName</span></span>|<span data-ttu-id="694a0-137">文字列</span><span class="sxs-lookup"><span data-stu-id="694a0-137">String</span></span>|<span data-ttu-id="694a0-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="694a0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="694a0-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-140">description</span><span class="sxs-lookup"><span data-stu-id="694a0-140">description</span></span>|<span data-ttu-id="694a0-141">String</span><span class="sxs-lookup"><span data-stu-id="694a0-141">String</span></span>|<span data-ttu-id="694a0-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="694a0-142">The description of the app.</span></span> <span data-ttu-id="694a0-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="694a0-144">publisher</span></span>|<span data-ttu-id="694a0-145">String</span><span class="sxs-lookup"><span data-stu-id="694a0-145">String</span></span>|<span data-ttu-id="694a0-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="694a0-146">The publisher of the app.</span></span> <span data-ttu-id="694a0-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="694a0-148">largeIcon</span></span>|[<span data-ttu-id="694a0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="694a0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="694a0-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="694a0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="694a0-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="694a0-152">createdDateTime</span></span>|<span data-ttu-id="694a0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="694a0-153">DateTimeOffset</span></span>|<span data-ttu-id="694a0-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="694a0-154">The date and time the app was created.</span></span> <span data-ttu-id="694a0-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="694a0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="694a0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="694a0-157">DateTimeOffset</span></span>|<span data-ttu-id="694a0-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="694a0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="694a0-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="694a0-160">isFeatured</span></span>|<span data-ttu-id="694a0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="694a0-161">Boolean</span></span>|<span data-ttu-id="694a0-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="694a0-163">privacyInformationUrl</span></span>|<span data-ttu-id="694a0-164">String</span><span class="sxs-lookup"><span data-stu-id="694a0-164">String</span></span>|<span data-ttu-id="694a0-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="694a0-165">The privacy statement Url.</span></span> <span data-ttu-id="694a0-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="694a0-167">informationUrl</span></span>|<span data-ttu-id="694a0-168">String</span><span class="sxs-lookup"><span data-stu-id="694a0-168">String</span></span>|<span data-ttu-id="694a0-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="694a0-169">The more information Url.</span></span> <span data-ttu-id="694a0-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-171">owner</span><span class="sxs-lookup"><span data-stu-id="694a0-171">owner</span></span>|<span data-ttu-id="694a0-172">String</span><span class="sxs-lookup"><span data-stu-id="694a0-172">String</span></span>|<span data-ttu-id="694a0-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="694a0-173">The owner of the app.</span></span> <span data-ttu-id="694a0-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-175">developer</span><span class="sxs-lookup"><span data-stu-id="694a0-175">developer</span></span>|<span data-ttu-id="694a0-176">String</span><span class="sxs-lookup"><span data-stu-id="694a0-176">String</span></span>|<span data-ttu-id="694a0-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="694a0-177">The developer of the app.</span></span> <span data-ttu-id="694a0-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-179">notes</span><span class="sxs-lookup"><span data-stu-id="694a0-179">notes</span></span>|<span data-ttu-id="694a0-180">String</span><span class="sxs-lookup"><span data-stu-id="694a0-180">String</span></span>|<span data-ttu-id="694a0-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="694a0-181">Notes for the app.</span></span> <span data-ttu-id="694a0-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="694a0-183">uploadState</span></span>|<span data-ttu-id="694a0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="694a0-184">Int32</span></span>|<span data-ttu-id="694a0-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="694a0-185">The upload state.</span></span> <span data-ttu-id="694a0-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="694a0-187">publishingState</span></span>|[<span data-ttu-id="694a0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="694a0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="694a0-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="694a0-189">The publishing state for the app.</span></span> <span data-ttu-id="694a0-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="694a0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="694a0-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="694a0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="694a0-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="694a0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="694a0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="694a0-193">isAssigned</span></span>|<span data-ttu-id="694a0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="694a0-194">Boolean</span></span>|<span data-ttu-id="694a0-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="694a0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="694a0-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="694a0-197">roleScopeTagIds</span></span>|<span data-ttu-id="694a0-198">String collection</span><span class="sxs-lookup"><span data-stu-id="694a0-198">String collection</span></span>|<span data-ttu-id="694a0-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="694a0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="694a0-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="694a0-201">dependentAppCount</span></span>|<span data-ttu-id="694a0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="694a0-202">Int32</span></span>|<span data-ttu-id="694a0-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="694a0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="694a0-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="694a0-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="694a0-205">committedContentVersion</span></span>|<span data-ttu-id="694a0-206">String</span><span class="sxs-lookup"><span data-stu-id="694a0-206">String</span></span>|<span data-ttu-id="694a0-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="694a0-207">The internal committed content version.</span></span> <span data-ttu-id="694a0-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="694a0-209">fileName</span><span class="sxs-lookup"><span data-stu-id="694a0-209">fileName</span></span>|<span data-ttu-id="694a0-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="694a0-210">String</span></span>|<span data-ttu-id="694a0-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="694a0-211">The name of the main Lob application file.</span></span> <span data-ttu-id="694a0-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="694a0-213">size</span><span class="sxs-lookup"><span data-stu-id="694a0-213">size</span></span>|<span data-ttu-id="694a0-214">Int64</span><span class="sxs-lookup"><span data-stu-id="694a0-214">Int64</span></span>|<span data-ttu-id="694a0-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="694a0-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="694a0-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="694a0-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="694a0-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="694a0-217">commandLine</span></span>|<span data-ttu-id="694a0-218">String</span><span class="sxs-lookup"><span data-stu-id="694a0-218">String</span></span>|<span data-ttu-id="694a0-219">コマンド ライン。</span><span class="sxs-lookup"><span data-stu-id="694a0-219">The command line.</span></span>|
|<span data-ttu-id="694a0-220">productCode</span><span class="sxs-lookup"><span data-stu-id="694a0-220">productCode</span></span>|<span data-ttu-id="694a0-221">String</span><span class="sxs-lookup"><span data-stu-id="694a0-221">String</span></span>|<span data-ttu-id="694a0-222">製品コード。</span><span class="sxs-lookup"><span data-stu-id="694a0-222">The product code.</span></span>|
|<span data-ttu-id="694a0-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="694a0-223">productVersion</span></span>|<span data-ttu-id="694a0-224">String</span><span class="sxs-lookup"><span data-stu-id="694a0-224">String</span></span>|<span data-ttu-id="694a0-225">Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。</span><span class="sxs-lookup"><span data-stu-id="694a0-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="694a0-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="694a0-226">ignoreVersionDetection</span></span>|<span data-ttu-id="694a0-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="694a0-227">Boolean</span></span>|<span data-ttu-id="694a0-228">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="694a0-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="694a0-229">自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="694a0-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="694a0-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="694a0-230">identityVersion</span></span>|<span data-ttu-id="694a0-231">String</span><span class="sxs-lookup"><span data-stu-id="694a0-231">String</span></span>|<span data-ttu-id="694a0-232">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="694a0-232">The identity version.</span></span>|
|<span data-ttu-id="694a0-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="694a0-233">useDeviceContext</span></span>|<span data-ttu-id="694a0-234">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="694a0-234">Boolean</span></span>|<span data-ttu-id="694a0-235">デバイスコンテキストにデュアルモード MSI をインストールするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="694a0-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="694a0-236">True の場合、すべてのユーザーに対してアプリがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="694a0-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="694a0-237">False の場合、アプリはユーザーごとにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="694a0-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="694a0-238">Null の場合、サービスは MSI パッケージの既定のインストールコンテキストを使用します。</span><span class="sxs-lookup"><span data-stu-id="694a0-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="694a0-239">デュアルモード MSI の場合、この既定値はユーザーごとになります。</span><span class="sxs-lookup"><span data-stu-id="694a0-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="694a0-240">デュアルモード以外のアプリには設定できません。</span><span class="sxs-lookup"><span data-stu-id="694a0-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="694a0-241">アプリケーションを最初に作成した後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="694a0-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="694a0-242">応答</span><span class="sxs-lookup"><span data-stu-id="694a0-242">Response</span></span>
<span data-ttu-id="694a0-243">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="694a0-243">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="694a0-244">例</span><span class="sxs-lookup"><span data-stu-id="694a0-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="694a0-245">要求</span><span class="sxs-lookup"><span data-stu-id="694a0-245">Request</span></span>
<span data-ttu-id="694a0-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="694a0-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="694a0-247">応答</span><span class="sxs-lookup"><span data-stu-id="694a0-247">Response</span></span>
<span data-ttu-id="694a0-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="694a0-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




