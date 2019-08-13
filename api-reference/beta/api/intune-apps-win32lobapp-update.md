---
title: Win32LobApp の更新
description: Win32LobApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b2e7b365dd21902c6c0ab3c8139f1e1996ecc48
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328740"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="b79d0-103">Win32LobApp の更新</span><span class="sxs-lookup"><span data-stu-id="b79d0-103">Update win32LobApp</span></span>

> <span data-ttu-id="b79d0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b79d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b79d0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b79d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b79d0-106">[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b79d0-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b79d0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b79d0-107">Prerequisites</span></span>
<span data-ttu-id="b79d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b79d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79d0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b79d0-110">Permission type</span></span>|<span data-ttu-id="b79d0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b79d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b79d0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b79d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b79d0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b79d0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b79d0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b79d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b79d0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b79d0-115">Not supported.</span></span>|
|<span data-ttu-id="b79d0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b79d0-116">Application</span></span>|<span data-ttu-id="b79d0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b79d0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b79d0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b79d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b79d0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b79d0-119">Request headers</span></span>
|<span data-ttu-id="b79d0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b79d0-120">Header</span></span>|<span data-ttu-id="b79d0-121">値</span><span class="sxs-lookup"><span data-stu-id="b79d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b79d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79d0-122">Authorization</span></span>|<span data-ttu-id="b79d0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b79d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b79d0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b79d0-124">Accept</span></span>|<span data-ttu-id="b79d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b79d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79d0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b79d0-126">Request body</span></span>
<span data-ttu-id="b79d0-127">要求本文で、 [win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b79d0-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="b79d0-128">次の表に、 [win32LobApp](../resources/intune-apps-win32lobapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b79d0-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="b79d0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b79d0-129">Property</span></span>|<span data-ttu-id="b79d0-130">型</span><span class="sxs-lookup"><span data-stu-id="b79d0-130">Type</span></span>|<span data-ttu-id="b79d0-131">説明</span><span class="sxs-lookup"><span data-stu-id="b79d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79d0-132">id</span><span class="sxs-lookup"><span data-stu-id="b79d0-132">id</span></span>|<span data-ttu-id="b79d0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b79d0-133">String</span></span>|<span data-ttu-id="b79d0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b79d0-134">Key of the entity.</span></span> <span data-ttu-id="b79d0-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b79d0-136">displayName</span></span>|<span data-ttu-id="b79d0-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b79d0-137">String</span></span>|<span data-ttu-id="b79d0-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b79d0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b79d0-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-140">description</span><span class="sxs-lookup"><span data-stu-id="b79d0-140">description</span></span>|<span data-ttu-id="b79d0-141">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-141">String</span></span>|<span data-ttu-id="b79d0-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b79d0-142">The description of the app.</span></span> <span data-ttu-id="b79d0-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b79d0-144">publisher</span></span>|<span data-ttu-id="b79d0-145">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-145">String</span></span>|<span data-ttu-id="b79d0-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b79d0-146">The publisher of the app.</span></span> <span data-ttu-id="b79d0-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b79d0-148">largeIcon</span></span>|[<span data-ttu-id="b79d0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b79d0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b79d0-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="b79d0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b79d0-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b79d0-152">createdDateTime</span></span>|<span data-ttu-id="b79d0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b79d0-153">DateTimeOffset</span></span>|<span data-ttu-id="b79d0-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b79d0-154">The date and time the app was created.</span></span> <span data-ttu-id="b79d0-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b79d0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b79d0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b79d0-157">DateTimeOffset</span></span>|<span data-ttu-id="b79d0-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b79d0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b79d0-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b79d0-160">isFeatured</span></span>|<span data-ttu-id="b79d0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b79d0-161">Boolean</span></span>|<span data-ttu-id="b79d0-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b79d0-163">privacyInformationUrl</span></span>|<span data-ttu-id="b79d0-164">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-164">String</span></span>|<span data-ttu-id="b79d0-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b79d0-165">The privacy statement Url.</span></span> <span data-ttu-id="b79d0-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b79d0-167">informationUrl</span></span>|<span data-ttu-id="b79d0-168">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-168">String</span></span>|<span data-ttu-id="b79d0-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b79d0-169">The more information Url.</span></span> <span data-ttu-id="b79d0-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-171">owner</span><span class="sxs-lookup"><span data-stu-id="b79d0-171">owner</span></span>|<span data-ttu-id="b79d0-172">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-172">String</span></span>|<span data-ttu-id="b79d0-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b79d0-173">The owner of the app.</span></span> <span data-ttu-id="b79d0-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-175">developer</span><span class="sxs-lookup"><span data-stu-id="b79d0-175">developer</span></span>|<span data-ttu-id="b79d0-176">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-176">String</span></span>|<span data-ttu-id="b79d0-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b79d0-177">The developer of the app.</span></span> <span data-ttu-id="b79d0-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-179">notes</span><span class="sxs-lookup"><span data-stu-id="b79d0-179">notes</span></span>|<span data-ttu-id="b79d0-180">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-180">String</span></span>|<span data-ttu-id="b79d0-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b79d0-181">Notes for the app.</span></span> <span data-ttu-id="b79d0-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b79d0-183">uploadState</span></span>|<span data-ttu-id="b79d0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-184">Int32</span></span>|<span data-ttu-id="b79d0-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="b79d0-185">The upload state.</span></span> <span data-ttu-id="b79d0-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b79d0-187">publishingState</span></span>|[<span data-ttu-id="b79d0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b79d0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b79d0-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b79d0-189">The publishing state for the app.</span></span> <span data-ttu-id="b79d0-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b79d0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b79d0-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b79d0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b79d0-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b79d0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b79d0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b79d0-193">isAssigned</span></span>|<span data-ttu-id="b79d0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b79d0-194">Boolean</span></span>|<span data-ttu-id="b79d0-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b79d0-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b79d0-197">roleScopeTagIds</span></span>|<span data-ttu-id="b79d0-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b79d0-198">String collection</span></span>|<span data-ttu-id="b79d0-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b79d0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b79d0-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b79d0-201">dependentAppCount</span></span>|<span data-ttu-id="b79d0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-202">Int32</span></span>|<span data-ttu-id="b79d0-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="b79d0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b79d0-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b79d0-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b79d0-205">committedContentVersion</span></span>|<span data-ttu-id="b79d0-206">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-206">String</span></span>|<span data-ttu-id="b79d0-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b79d0-207">The internal committed content version.</span></span> <span data-ttu-id="b79d0-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b79d0-209">fileName</span><span class="sxs-lookup"><span data-stu-id="b79d0-209">fileName</span></span>|<span data-ttu-id="b79d0-210">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-210">String</span></span>|<span data-ttu-id="b79d0-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="b79d0-211">The name of the main Lob application file.</span></span> <span data-ttu-id="b79d0-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b79d0-213">size</span><span class="sxs-lookup"><span data-stu-id="b79d0-213">size</span></span>|<span data-ttu-id="b79d0-214">Int64</span><span class="sxs-lookup"><span data-stu-id="b79d0-214">Int64</span></span>|<span data-ttu-id="b79d0-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="b79d0-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="b79d0-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b79d0-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b79d0-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="b79d0-217">installCommandLine</span></span>|<span data-ttu-id="b79d0-218">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-218">String</span></span>|<span data-ttu-id="b79d0-219">このアプリをインストールするためのコマンドライン</span><span class="sxs-lookup"><span data-stu-id="b79d0-219">The command line to install this app</span></span>|
|<span data-ttu-id="b79d0-220">アン Installcommandline</span><span class="sxs-lookup"><span data-stu-id="b79d0-220">uninstallCommandLine</span></span>|<span data-ttu-id="b79d0-221">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-221">String</span></span>|<span data-ttu-id="b79d0-222">このアプリをアンインストールするためのコマンドライン</span><span class="sxs-lookup"><span data-stu-id="b79d0-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="b79d0-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b79d0-223">applicableArchitectures</span></span>|[<span data-ttu-id="b79d0-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b79d0-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b79d0-225">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="b79d0-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b79d0-226">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b79d0-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b79d0-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b79d0-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b79d0-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b79d0-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b79d0-229">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b79d0-230">Minimumfreediskspace Inmb</span><span class="sxs-lookup"><span data-stu-id="b79d0-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="b79d0-231">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-231">Int32</span></span>|<span data-ttu-id="b79d0-232">このアプリをインストールするのに必要な最小空きディスク領域の値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="b79d0-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="b79d0-233">minimumMemoryInMB</span></span>|<span data-ttu-id="b79d0-234">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-234">Int32</span></span>|<span data-ttu-id="b79d0-235">このアプリをインストールするのに必要な最小物理メモリの値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="b79d0-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="b79d0-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="b79d0-237">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-237">Int32</span></span>|<span data-ttu-id="b79d0-238">このアプリのインストールに必要なプロセッサの最小数の値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="b79d0-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="b79d0-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="b79d0-240">Int32</span><span class="sxs-lookup"><span data-stu-id="b79d0-240">Int32</span></span>|<span data-ttu-id="b79d0-241">このアプリをインストールするのに必要な最小 CPU 速度の値。</span><span class="sxs-lookup"><span data-stu-id="b79d0-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="b79d0-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="b79d0-242">detectionRules</span></span>|<span data-ttu-id="b79d0-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b79d0-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="b79d0-244">Win32 基幹業務 (LoB) アプリを検出するための検出ルール。</span><span class="sxs-lookup"><span data-stu-id="b79d0-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b79d0-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="b79d0-245">requirementRules</span></span>|<span data-ttu-id="b79d0-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b79d0-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="b79d0-247">Win32 基幹業務 (LoB) アプリを検出するための要件の規則。</span><span class="sxs-lookup"><span data-stu-id="b79d0-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b79d0-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="b79d0-248">installExperience</span></span>|[<span data-ttu-id="b79d0-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="b79d0-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="b79d0-250">このアプリのインストール手順。</span><span class="sxs-lookup"><span data-stu-id="b79d0-250">The install experience for this app.</span></span>|
|<span data-ttu-id="b79d0-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="b79d0-251">returnCodes</span></span>|<span data-ttu-id="b79d0-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b79d0-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="b79d0-253">インストール後の動作のリターンコード。</span><span class="sxs-lookup"><span data-stu-id="b79d0-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="b79d0-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="b79d0-254">msiInformation</span></span>|[<span data-ttu-id="b79d0-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="b79d0-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="b79d0-256">この Win32 アプリが MSI アプリの場合、MSI の詳細。</span><span class="sxs-lookup"><span data-stu-id="b79d0-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="b79d0-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="b79d0-257">setupFilePath</span></span>|<span data-ttu-id="b79d0-258">String</span><span class="sxs-lookup"><span data-stu-id="b79d0-258">String</span></span>|<span data-ttu-id="b79d0-259">暗号化された Win32LobApp パッケージ内のセットアップファイルの相対パス。</span><span class="sxs-lookup"><span data-stu-id="b79d0-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="b79d0-260">応答</span><span class="sxs-lookup"><span data-stu-id="b79d0-260">Response</span></span>
<span data-ttu-id="b79d0-261">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b79d0-261">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b79d0-262">例</span><span class="sxs-lookup"><span data-stu-id="b79d0-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="b79d0-263">要求</span><span class="sxs-lookup"><span data-stu-id="b79d0-263">Request</span></span>
<span data-ttu-id="b79d0-264">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b79d0-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2778

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="b79d0-265">応答</span><span class="sxs-lookup"><span data-stu-id="b79d0-265">Response</span></span>
<span data-ttu-id="b79d0-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b79d0-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2950

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```






