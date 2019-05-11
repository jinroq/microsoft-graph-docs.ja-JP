---
title: windowsUniversalAppX の更新
description: windowsUniversalAppX オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87fb009d1056a87af5a58252f5eb11765747009d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934475"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="46044-103">windowsUniversalAppX の更新</span><span class="sxs-lookup"><span data-stu-id="46044-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="46044-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46044-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46044-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46044-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46044-106">[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="46044-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46044-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="46044-107">Prerequisites</span></span>
<span data-ttu-id="46044-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46044-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46044-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46044-110">Permission type</span></span>|<span data-ttu-id="46044-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="46044-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46044-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46044-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46044-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46044-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46044-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46044-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46044-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46044-115">Not supported.</span></span>|
|<span data-ttu-id="46044-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46044-116">Application</span></span>|<span data-ttu-id="46044-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46044-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46044-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46044-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="46044-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46044-119">Request headers</span></span>
|<span data-ttu-id="46044-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46044-120">Header</span></span>|<span data-ttu-id="46044-121">値</span><span class="sxs-lookup"><span data-stu-id="46044-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46044-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46044-122">Authorization</span></span>|<span data-ttu-id="46044-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="46044-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46044-124">承諾</span><span class="sxs-lookup"><span data-stu-id="46044-124">Accept</span></span>|<span data-ttu-id="46044-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46044-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46044-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="46044-126">Request body</span></span>
<span data-ttu-id="46044-127">要求本文で、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="46044-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="46044-128">次の表に、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="46044-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="46044-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46044-129">Property</span></span>|<span data-ttu-id="46044-130">型</span><span class="sxs-lookup"><span data-stu-id="46044-130">Type</span></span>|<span data-ttu-id="46044-131">説明</span><span class="sxs-lookup"><span data-stu-id="46044-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46044-132">id</span><span class="sxs-lookup"><span data-stu-id="46044-132">id</span></span>|<span data-ttu-id="46044-133">文字列</span><span class="sxs-lookup"><span data-stu-id="46044-133">String</span></span>|<span data-ttu-id="46044-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46044-134">Key of the entity.</span></span> <span data-ttu-id="46044-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-136">displayName</span><span class="sxs-lookup"><span data-stu-id="46044-136">displayName</span></span>|<span data-ttu-id="46044-137">文字列</span><span class="sxs-lookup"><span data-stu-id="46044-137">String</span></span>|<span data-ttu-id="46044-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="46044-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="46044-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-140">description</span><span class="sxs-lookup"><span data-stu-id="46044-140">description</span></span>|<span data-ttu-id="46044-141">String</span><span class="sxs-lookup"><span data-stu-id="46044-141">String</span></span>|<span data-ttu-id="46044-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="46044-142">The description of the app.</span></span> <span data-ttu-id="46044-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-144">publisher</span><span class="sxs-lookup"><span data-stu-id="46044-144">publisher</span></span>|<span data-ttu-id="46044-145">String</span><span class="sxs-lookup"><span data-stu-id="46044-145">String</span></span>|<span data-ttu-id="46044-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="46044-146">The publisher of the app.</span></span> <span data-ttu-id="46044-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="46044-148">largeIcon</span></span>|[<span data-ttu-id="46044-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="46044-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="46044-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="46044-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="46044-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46044-152">createdDateTime</span></span>|<span data-ttu-id="46044-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46044-153">DateTimeOffset</span></span>|<span data-ttu-id="46044-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="46044-154">The date and time the app was created.</span></span> <span data-ttu-id="46044-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46044-156">lastModifiedDateTime</span></span>|<span data-ttu-id="46044-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46044-157">DateTimeOffset</span></span>|<span data-ttu-id="46044-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="46044-158">The date and time the app was last modified.</span></span> <span data-ttu-id="46044-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="46044-160">isFeatured</span></span>|<span data-ttu-id="46044-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="46044-161">Boolean</span></span>|<span data-ttu-id="46044-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="46044-163">privacyInformationUrl</span></span>|<span data-ttu-id="46044-164">String</span><span class="sxs-lookup"><span data-stu-id="46044-164">String</span></span>|<span data-ttu-id="46044-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="46044-165">The privacy statement Url.</span></span> <span data-ttu-id="46044-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="46044-167">informationUrl</span></span>|<span data-ttu-id="46044-168">String</span><span class="sxs-lookup"><span data-stu-id="46044-168">String</span></span>|<span data-ttu-id="46044-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="46044-169">The more information Url.</span></span> <span data-ttu-id="46044-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-171">owner</span><span class="sxs-lookup"><span data-stu-id="46044-171">owner</span></span>|<span data-ttu-id="46044-172">String</span><span class="sxs-lookup"><span data-stu-id="46044-172">String</span></span>|<span data-ttu-id="46044-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="46044-173">The owner of the app.</span></span> <span data-ttu-id="46044-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-175">developer</span><span class="sxs-lookup"><span data-stu-id="46044-175">developer</span></span>|<span data-ttu-id="46044-176">String</span><span class="sxs-lookup"><span data-stu-id="46044-176">String</span></span>|<span data-ttu-id="46044-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="46044-177">The developer of the app.</span></span> <span data-ttu-id="46044-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-179">notes</span><span class="sxs-lookup"><span data-stu-id="46044-179">notes</span></span>|<span data-ttu-id="46044-180">String</span><span class="sxs-lookup"><span data-stu-id="46044-180">String</span></span>|<span data-ttu-id="46044-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="46044-181">Notes for the app.</span></span> <span data-ttu-id="46044-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="46044-183">uploadState</span></span>|<span data-ttu-id="46044-184">Int32</span><span class="sxs-lookup"><span data-stu-id="46044-184">Int32</span></span>|<span data-ttu-id="46044-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="46044-185">The upload state.</span></span> <span data-ttu-id="46044-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="46044-187">publishingState</span></span>|[<span data-ttu-id="46044-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="46044-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="46044-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="46044-189">The publishing state for the app.</span></span> <span data-ttu-id="46044-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="46044-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="46044-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="46044-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="46044-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="46044-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="46044-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="46044-193">isAssigned</span></span>|<span data-ttu-id="46044-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="46044-194">Boolean</span></span>|<span data-ttu-id="46044-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="46044-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="46044-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="46044-197">roleScopeTagIds</span></span>|<span data-ttu-id="46044-198">String collection</span><span class="sxs-lookup"><span data-stu-id="46044-198">String collection</span></span>|<span data-ttu-id="46044-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="46044-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="46044-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="46044-201">dependentAppCount</span></span>|<span data-ttu-id="46044-202">Int32</span><span class="sxs-lookup"><span data-stu-id="46044-202">Int32</span></span>|<span data-ttu-id="46044-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="46044-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="46044-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46044-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="46044-205">committedContentVersion</span></span>|<span data-ttu-id="46044-206">String</span><span class="sxs-lookup"><span data-stu-id="46044-206">String</span></span>|<span data-ttu-id="46044-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="46044-207">The internal committed content version.</span></span> <span data-ttu-id="46044-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46044-209">fileName</span><span class="sxs-lookup"><span data-stu-id="46044-209">fileName</span></span>|<span data-ttu-id="46044-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="46044-210">String</span></span>|<span data-ttu-id="46044-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="46044-211">The name of the main Lob application file.</span></span> <span data-ttu-id="46044-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46044-213">size</span><span class="sxs-lookup"><span data-stu-id="46044-213">size</span></span>|<span data-ttu-id="46044-214">Int64</span><span class="sxs-lookup"><span data-stu-id="46044-214">Int64</span></span>|<span data-ttu-id="46044-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="46044-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="46044-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46044-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46044-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="46044-217">applicableArchitectures</span></span>|[<span data-ttu-id="46044-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="46044-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="46044-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="46044-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="46044-220">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="46044-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="46044-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="46044-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="46044-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="46044-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="46044-223">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="46044-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="46044-224">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="46044-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="46044-225">identityName</span><span class="sxs-lookup"><span data-stu-id="46044-225">identityName</span></span>|<span data-ttu-id="46044-226">String</span><span class="sxs-lookup"><span data-stu-id="46044-226">String</span></span>|<span data-ttu-id="46044-227">ID 名。</span><span class="sxs-lookup"><span data-stu-id="46044-227">The Identity Name.</span></span>|
|<span data-ttu-id="46044-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="46044-228">identityPublisherHash</span></span>|<span data-ttu-id="46044-229">String</span><span class="sxs-lookup"><span data-stu-id="46044-229">String</span></span>|<span data-ttu-id="46044-230">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="46044-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="46044-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="46044-231">identityResourceIdentifier</span></span>|<span data-ttu-id="46044-232">String</span><span class="sxs-lookup"><span data-stu-id="46044-232">String</span></span>|<span data-ttu-id="46044-233">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="46044-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="46044-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="46044-234">isBundle</span></span>|<span data-ttu-id="46044-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="46044-235">Boolean</span></span>|<span data-ttu-id="46044-236">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="46044-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="46044-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="46044-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="46044-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="46044-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="46044-239">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="46044-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="46044-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="46044-240">identityVersion</span></span>|<span data-ttu-id="46044-241">String</span><span class="sxs-lookup"><span data-stu-id="46044-241">String</span></span>|<span data-ttu-id="46044-242">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="46044-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="46044-243">応答</span><span class="sxs-lookup"><span data-stu-id="46044-243">Response</span></span>
<span data-ttu-id="46044-244">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="46044-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46044-245">例</span><span class="sxs-lookup"><span data-stu-id="46044-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="46044-246">要求</span><span class="sxs-lookup"><span data-stu-id="46044-246">Request</span></span>
<span data-ttu-id="46044-247">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46044-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1415

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="46044-248">応答</span><span class="sxs-lookup"><span data-stu-id="46044-248">Response</span></span>
<span data-ttu-id="46044-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46044-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1587

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




