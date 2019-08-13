---
title: WindowsAppX の更新
description: WindowsAppX オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ed9204a5f0a3aee19ffd44613e547248fcf520c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322542"
---
# <a name="update-windowsappx"></a><span data-ttu-id="11f6c-103">WindowsAppX の更新</span><span class="sxs-lookup"><span data-stu-id="11f6c-103">Update windowsAppX</span></span>

> <span data-ttu-id="11f6c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11f6c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11f6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11f6c-106">[Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="11f6c-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11f6c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="11f6c-107">Prerequisites</span></span>
<span data-ttu-id="11f6c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f6c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11f6c-110">Permission type</span></span>|<span data-ttu-id="11f6c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="11f6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11f6c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11f6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11f6c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f6c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11f6c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11f6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11f6c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f6c-115">Not supported.</span></span>|
|<span data-ttu-id="11f6c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11f6c-116">Application</span></span>|<span data-ttu-id="11f6c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f6c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11f6c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11f6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="11f6c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11f6c-119">Request headers</span></span>
|<span data-ttu-id="11f6c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11f6c-120">Header</span></span>|<span data-ttu-id="11f6c-121">値</span><span class="sxs-lookup"><span data-stu-id="11f6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11f6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11f6c-122">Authorization</span></span>|<span data-ttu-id="11f6c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="11f6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11f6c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="11f6c-124">Accept</span></span>|<span data-ttu-id="11f6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11f6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11f6c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="11f6c-126">Request body</span></span>
<span data-ttu-id="11f6c-127">要求本文で、 [Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="11f6c-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="11f6c-128">次の表に、 [Windowsappx](../resources/intune-apps-windowsappx.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="11f6c-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="11f6c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11f6c-129">Property</span></span>|<span data-ttu-id="11f6c-130">型</span><span class="sxs-lookup"><span data-stu-id="11f6c-130">Type</span></span>|<span data-ttu-id="11f6c-131">説明</span><span class="sxs-lookup"><span data-stu-id="11f6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f6c-132">id</span><span class="sxs-lookup"><span data-stu-id="11f6c-132">id</span></span>|<span data-ttu-id="11f6c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="11f6c-133">String</span></span>|<span data-ttu-id="11f6c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="11f6c-134">Key of the entity.</span></span> <span data-ttu-id="11f6c-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11f6c-136">displayName</span></span>|<span data-ttu-id="11f6c-137">文字列</span><span class="sxs-lookup"><span data-stu-id="11f6c-137">String</span></span>|<span data-ttu-id="11f6c-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="11f6c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="11f6c-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-140">description</span><span class="sxs-lookup"><span data-stu-id="11f6c-140">description</span></span>|<span data-ttu-id="11f6c-141">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-141">String</span></span>|<span data-ttu-id="11f6c-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="11f6c-142">The description of the app.</span></span> <span data-ttu-id="11f6c-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="11f6c-144">publisher</span></span>|<span data-ttu-id="11f6c-145">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-145">String</span></span>|<span data-ttu-id="11f6c-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="11f6c-146">The publisher of the app.</span></span> <span data-ttu-id="11f6c-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="11f6c-148">largeIcon</span></span>|[<span data-ttu-id="11f6c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="11f6c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="11f6c-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="11f6c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="11f6c-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11f6c-152">createdDateTime</span></span>|<span data-ttu-id="11f6c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11f6c-153">DateTimeOffset</span></span>|<span data-ttu-id="11f6c-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="11f6c-154">The date and time the app was created.</span></span> <span data-ttu-id="11f6c-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11f6c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="11f6c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11f6c-157">DateTimeOffset</span></span>|<span data-ttu-id="11f6c-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="11f6c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="11f6c-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="11f6c-160">isFeatured</span></span>|<span data-ttu-id="11f6c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6c-161">Boolean</span></span>|<span data-ttu-id="11f6c-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="11f6c-163">privacyInformationUrl</span></span>|<span data-ttu-id="11f6c-164">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-164">String</span></span>|<span data-ttu-id="11f6c-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="11f6c-165">The privacy statement Url.</span></span> <span data-ttu-id="11f6c-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="11f6c-167">informationUrl</span></span>|<span data-ttu-id="11f6c-168">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-168">String</span></span>|<span data-ttu-id="11f6c-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="11f6c-169">The more information Url.</span></span> <span data-ttu-id="11f6c-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-171">owner</span><span class="sxs-lookup"><span data-stu-id="11f6c-171">owner</span></span>|<span data-ttu-id="11f6c-172">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-172">String</span></span>|<span data-ttu-id="11f6c-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="11f6c-173">The owner of the app.</span></span> <span data-ttu-id="11f6c-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-175">developer</span><span class="sxs-lookup"><span data-stu-id="11f6c-175">developer</span></span>|<span data-ttu-id="11f6c-176">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-176">String</span></span>|<span data-ttu-id="11f6c-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="11f6c-177">The developer of the app.</span></span> <span data-ttu-id="11f6c-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-179">notes</span><span class="sxs-lookup"><span data-stu-id="11f6c-179">notes</span></span>|<span data-ttu-id="11f6c-180">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-180">String</span></span>|<span data-ttu-id="11f6c-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="11f6c-181">Notes for the app.</span></span> <span data-ttu-id="11f6c-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="11f6c-183">uploadState</span></span>|<span data-ttu-id="11f6c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="11f6c-184">Int32</span></span>|<span data-ttu-id="11f6c-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="11f6c-185">The upload state.</span></span> <span data-ttu-id="11f6c-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="11f6c-187">publishingState</span></span>|[<span data-ttu-id="11f6c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="11f6c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="11f6c-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="11f6c-189">The publishing state for the app.</span></span> <span data-ttu-id="11f6c-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="11f6c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="11f6c-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="11f6c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="11f6c-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="11f6c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="11f6c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="11f6c-193">isAssigned</span></span>|<span data-ttu-id="11f6c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6c-194">Boolean</span></span>|<span data-ttu-id="11f6c-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="11f6c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="11f6c-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11f6c-197">roleScopeTagIds</span></span>|<span data-ttu-id="11f6c-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="11f6c-198">String collection</span></span>|<span data-ttu-id="11f6c-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="11f6c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="11f6c-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="11f6c-201">dependentAppCount</span></span>|<span data-ttu-id="11f6c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="11f6c-202">Int32</span></span>|<span data-ttu-id="11f6c-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="11f6c-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="11f6c-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11f6c-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="11f6c-205">committedContentVersion</span></span>|<span data-ttu-id="11f6c-206">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-206">String</span></span>|<span data-ttu-id="11f6c-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="11f6c-207">The internal committed content version.</span></span> <span data-ttu-id="11f6c-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11f6c-209">fileName</span><span class="sxs-lookup"><span data-stu-id="11f6c-209">fileName</span></span>|<span data-ttu-id="11f6c-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11f6c-210">String</span></span>|<span data-ttu-id="11f6c-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="11f6c-211">The name of the main Lob application file.</span></span> <span data-ttu-id="11f6c-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11f6c-213">size</span><span class="sxs-lookup"><span data-stu-id="11f6c-213">size</span></span>|<span data-ttu-id="11f6c-214">Int64</span><span class="sxs-lookup"><span data-stu-id="11f6c-214">Int64</span></span>|<span data-ttu-id="11f6c-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="11f6c-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="11f6c-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11f6c-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11f6c-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="11f6c-217">applicableArchitectures</span></span>|[<span data-ttu-id="11f6c-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="11f6c-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="11f6c-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="11f6c-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="11f6c-220">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="11f6c-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="11f6c-221">identityName</span><span class="sxs-lookup"><span data-stu-id="11f6c-221">identityName</span></span>|<span data-ttu-id="11f6c-222">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-222">String</span></span>|<span data-ttu-id="11f6c-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="11f6c-223">The Identity Name.</span></span>|
|<span data-ttu-id="11f6c-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="11f6c-224">identityPublisherHash</span></span>|<span data-ttu-id="11f6c-225">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-225">String</span></span>|<span data-ttu-id="11f6c-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="11f6c-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="11f6c-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="11f6c-227">identityResourceIdentifier</span></span>|<span data-ttu-id="11f6c-228">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-228">String</span></span>|<span data-ttu-id="11f6c-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="11f6c-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="11f6c-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="11f6c-230">isBundle</span></span>|<span data-ttu-id="11f6c-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6c-231">Boolean</span></span>|<span data-ttu-id="11f6c-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="11f6c-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="11f6c-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11f6c-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="11f6c-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11f6c-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="11f6c-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="11f6c-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="11f6c-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="11f6c-236">identityVersion</span></span>|<span data-ttu-id="11f6c-237">String</span><span class="sxs-lookup"><span data-stu-id="11f6c-237">String</span></span>|<span data-ttu-id="11f6c-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="11f6c-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="11f6c-239">応答</span><span class="sxs-lookup"><span data-stu-id="11f6c-239">Response</span></span>
<span data-ttu-id="11f6c-240">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="11f6c-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f6c-241">例</span><span class="sxs-lookup"><span data-stu-id="11f6c-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="11f6c-242">要求</span><span class="sxs-lookup"><span data-stu-id="11f6c-242">Request</span></span>
<span data-ttu-id="11f6c-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11f6c-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="11f6c-244">応答</span><span class="sxs-lookup"><span data-stu-id="11f6c-244">Response</span></span>
<span data-ttu-id="11f6c-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11f6c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```






