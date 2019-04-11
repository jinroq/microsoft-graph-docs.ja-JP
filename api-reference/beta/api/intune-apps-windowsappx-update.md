---
title: windowsappx の更新
description: windowsappx オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cc1fc2c72cab28d2ed6602673eb13793190d892
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785049"
---
# <a name="update-windowsappx"></a><span data-ttu-id="dfce4-103">windowsappx の更新</span><span class="sxs-lookup"><span data-stu-id="dfce4-103">Update windowsAppX</span></span>

> <span data-ttu-id="dfce4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfce4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfce4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfce4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfce4-106">[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dfce4-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfce4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dfce4-107">Prerequisites</span></span>
<span data-ttu-id="dfce4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfce4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfce4-110">Permission type</span></span>|<span data-ttu-id="dfce4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfce4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfce4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfce4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfce4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfce4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfce4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfce4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfce4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfce4-115">Not supported.</span></span>|
|<span data-ttu-id="dfce4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfce4-116">Application</span></span>|<span data-ttu-id="dfce4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfce4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfce4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfce4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dfce4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfce4-119">Request headers</span></span>
|<span data-ttu-id="dfce4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfce4-120">Header</span></span>|<span data-ttu-id="dfce4-121">値</span><span class="sxs-lookup"><span data-stu-id="dfce4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfce4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfce4-122">Authorization</span></span>|<span data-ttu-id="dfce4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfce4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfce4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dfce4-124">Accept</span></span>|<span data-ttu-id="dfce4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfce4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfce4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfce4-126">Request body</span></span>
<span data-ttu-id="dfce4-127">要求本文で、 [windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dfce4-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="dfce4-128">次の表に、 [windowsappx](../resources/intune-apps-windowsappx.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dfce4-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="dfce4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfce4-129">Property</span></span>|<span data-ttu-id="dfce4-130">型</span><span class="sxs-lookup"><span data-stu-id="dfce4-130">Type</span></span>|<span data-ttu-id="dfce4-131">説明</span><span class="sxs-lookup"><span data-stu-id="dfce4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfce4-132">id</span><span class="sxs-lookup"><span data-stu-id="dfce4-132">id</span></span>|<span data-ttu-id="dfce4-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dfce4-133">String</span></span>|<span data-ttu-id="dfce4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dfce4-134">Key of the entity.</span></span> <span data-ttu-id="dfce4-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dfce4-136">displayName</span></span>|<span data-ttu-id="dfce4-137">String</span><span class="sxs-lookup"><span data-stu-id="dfce4-137">String</span></span>|<span data-ttu-id="dfce4-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="dfce4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dfce4-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-140">説明</span><span class="sxs-lookup"><span data-stu-id="dfce4-140">description</span></span>|<span data-ttu-id="dfce4-141">String</span><span class="sxs-lookup"><span data-stu-id="dfce4-141">String</span></span>|<span data-ttu-id="dfce4-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="dfce4-142">The description of the app.</span></span> <span data-ttu-id="dfce4-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dfce4-144">publisher</span></span>|<span data-ttu-id="dfce4-145">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-145">String</span></span>|<span data-ttu-id="dfce4-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="dfce4-146">The publisher of the app.</span></span> <span data-ttu-id="dfce4-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dfce4-148">largeIcon</span></span>|[<span data-ttu-id="dfce4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dfce4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dfce4-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="dfce4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dfce4-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfce4-152">createdDateTime</span></span>|<span data-ttu-id="dfce4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfce4-153">DateTimeOffset</span></span>|<span data-ttu-id="dfce4-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="dfce4-154">The date and time the app was created.</span></span> <span data-ttu-id="dfce4-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfce4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dfce4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfce4-157">DateTimeOffset</span></span>|<span data-ttu-id="dfce4-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="dfce4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dfce4-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dfce4-160">isFeatured</span></span>|<span data-ttu-id="dfce4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfce4-161">Boolean</span></span>|<span data-ttu-id="dfce4-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dfce4-163">privacyInformationUrl</span></span>|<span data-ttu-id="dfce4-164">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-164">String</span></span>|<span data-ttu-id="dfce4-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="dfce4-165">The privacy statement Url.</span></span> <span data-ttu-id="dfce4-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dfce4-167">informationUrl</span></span>|<span data-ttu-id="dfce4-168">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-168">String</span></span>|<span data-ttu-id="dfce4-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="dfce4-169">The more information Url.</span></span> <span data-ttu-id="dfce4-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-171">owner</span><span class="sxs-lookup"><span data-stu-id="dfce4-171">owner</span></span>|<span data-ttu-id="dfce4-172">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-172">String</span></span>|<span data-ttu-id="dfce4-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="dfce4-173">The owner of the app.</span></span> <span data-ttu-id="dfce4-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-175">developer</span><span class="sxs-lookup"><span data-stu-id="dfce4-175">developer</span></span>|<span data-ttu-id="dfce4-176">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-176">String</span></span>|<span data-ttu-id="dfce4-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="dfce4-177">The developer of the app.</span></span> <span data-ttu-id="dfce4-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-179">notes</span><span class="sxs-lookup"><span data-stu-id="dfce4-179">notes</span></span>|<span data-ttu-id="dfce4-180">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-180">String</span></span>|<span data-ttu-id="dfce4-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="dfce4-181">Notes for the app.</span></span> <span data-ttu-id="dfce4-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="dfce4-183">uploadState</span></span>|<span data-ttu-id="dfce4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dfce4-184">Int32</span></span>|<span data-ttu-id="dfce4-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="dfce4-185">The upload state.</span></span> <span data-ttu-id="dfce4-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="dfce4-187">publishingState</span></span>|[<span data-ttu-id="dfce4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dfce4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dfce4-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="dfce4-189">The publishing state for the app.</span></span> <span data-ttu-id="dfce4-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="dfce4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dfce4-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="dfce4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dfce4-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="dfce4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dfce4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dfce4-193">isAssigned</span></span>|<span data-ttu-id="dfce4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfce4-194">Boolean</span></span>|<span data-ttu-id="dfce4-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="dfce4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dfce4-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfce4-197">roleScopeTagIds</span></span>|<span data-ttu-id="dfce4-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dfce4-198">String collection</span></span>|<span data-ttu-id="dfce4-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="dfce4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dfce4-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="dfce4-201">dependentAppCount</span></span>|<span data-ttu-id="dfce4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dfce4-202">Int32</span></span>|<span data-ttu-id="dfce4-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="dfce4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dfce4-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfce4-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dfce4-205">committedContentVersion</span></span>|<span data-ttu-id="dfce4-206">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-206">String</span></span>|<span data-ttu-id="dfce4-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="dfce4-207">The internal committed content version.</span></span> <span data-ttu-id="dfce4-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfce4-209">fileName</span><span class="sxs-lookup"><span data-stu-id="dfce4-209">fileName</span></span>|<span data-ttu-id="dfce4-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dfce4-210">String</span></span>|<span data-ttu-id="dfce4-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="dfce4-211">The name of the main Lob application file.</span></span> <span data-ttu-id="dfce4-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfce4-213">size</span><span class="sxs-lookup"><span data-stu-id="dfce4-213">size</span></span>|<span data-ttu-id="dfce4-214">Int64</span><span class="sxs-lookup"><span data-stu-id="dfce4-214">Int64</span></span>|<span data-ttu-id="dfce4-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="dfce4-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="dfce4-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfce4-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfce4-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="dfce4-217">applicableArchitectures</span></span>|[<span data-ttu-id="dfce4-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="dfce4-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="dfce4-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="dfce4-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="dfce4-220">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="dfce4-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="dfce4-221">identityName</span><span class="sxs-lookup"><span data-stu-id="dfce4-221">identityName</span></span>|<span data-ttu-id="dfce4-222">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-222">String</span></span>|<span data-ttu-id="dfce4-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="dfce4-223">The Identity Name.</span></span>|
|<span data-ttu-id="dfce4-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="dfce4-224">identityPublisherHash</span></span>|<span data-ttu-id="dfce4-225">String</span><span class="sxs-lookup"><span data-stu-id="dfce4-225">String</span></span>|<span data-ttu-id="dfce4-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="dfce4-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="dfce4-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="dfce4-227">identityResourceIdentifier</span></span>|<span data-ttu-id="dfce4-228">文字列</span><span class="sxs-lookup"><span data-stu-id="dfce4-228">String</span></span>|<span data-ttu-id="dfce4-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="dfce4-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="dfce4-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="dfce4-230">isBundle</span></span>|<span data-ttu-id="dfce4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfce4-231">Boolean</span></span>|<span data-ttu-id="dfce4-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="dfce4-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="dfce4-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dfce4-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dfce4-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dfce4-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="dfce4-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="dfce4-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dfce4-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dfce4-236">identityVersion</span></span>|<span data-ttu-id="dfce4-237">String</span><span class="sxs-lookup"><span data-stu-id="dfce4-237">String</span></span>|<span data-ttu-id="dfce4-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dfce4-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="dfce4-239">応答</span><span class="sxs-lookup"><span data-stu-id="dfce4-239">Response</span></span>
<span data-ttu-id="dfce4-240">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dfce4-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfce4-241">例</span><span class="sxs-lookup"><span data-stu-id="dfce4-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfce4-242">要求</span><span class="sxs-lookup"><span data-stu-id="dfce4-242">Request</span></span>
<span data-ttu-id="dfce4-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dfce4-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1367

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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="dfce4-244">応答</span><span class="sxs-lookup"><span data-stu-id="dfce4-244">Response</span></span>
<span data-ttu-id="dfce4-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dfce4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1539

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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```





