---
title: androidLobApp の更新
description: androidLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f2cc9177d374e7720821b9195a8b4d40bf2cf55
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784601"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="9e0fe-103">androidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="9e0fe-103">Update androidLobApp</span></span>

> <span data-ttu-id="9e0fe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e0fe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e0fe-106">[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e0fe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e0fe-107">Prerequisites</span></span>
<span data-ttu-id="9e0fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e0fe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e0fe-110">Permission type</span></span>|<span data-ttu-id="9e0fe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e0fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e0fe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e0fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e0fe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e0fe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e0fe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e0fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e0fe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-115">Not supported.</span></span>|
|<span data-ttu-id="9e0fe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e0fe-116">Application</span></span>|<span data-ttu-id="9e0fe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e0fe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e0fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9e0fe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e0fe-119">Request headers</span></span>
|<span data-ttu-id="9e0fe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e0fe-120">Header</span></span>|<span data-ttu-id="9e0fe-121">値</span><span class="sxs-lookup"><span data-stu-id="9e0fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e0fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e0fe-122">Authorization</span></span>|<span data-ttu-id="9e0fe-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e0fe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9e0fe-124">Accept</span></span>|<span data-ttu-id="9e0fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e0fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e0fe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e0fe-126">Request body</span></span>
<span data-ttu-id="9e0fe-127">要求本文で、[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="9e0fe-128">次の表に、[androidLobApp](../resources/intune-apps-androidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="9e0fe-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e0fe-129">Property</span></span>|<span data-ttu-id="9e0fe-130">型</span><span class="sxs-lookup"><span data-stu-id="9e0fe-130">Type</span></span>|<span data-ttu-id="9e0fe-131">説明</span><span class="sxs-lookup"><span data-stu-id="9e0fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e0fe-132">id</span><span class="sxs-lookup"><span data-stu-id="9e0fe-132">id</span></span>|<span data-ttu-id="9e0fe-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9e0fe-133">String</span></span>|<span data-ttu-id="9e0fe-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-134">Key of the entity.</span></span> <span data-ttu-id="9e0fe-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9e0fe-136">displayName</span></span>|<span data-ttu-id="9e0fe-137">String</span><span class="sxs-lookup"><span data-stu-id="9e0fe-137">String</span></span>|<span data-ttu-id="9e0fe-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9e0fe-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-140">説明</span><span class="sxs-lookup"><span data-stu-id="9e0fe-140">description</span></span>|<span data-ttu-id="9e0fe-141">String</span><span class="sxs-lookup"><span data-stu-id="9e0fe-141">String</span></span>|<span data-ttu-id="9e0fe-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-142">The description of the app.</span></span> <span data-ttu-id="9e0fe-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9e0fe-144">publisher</span></span>|<span data-ttu-id="9e0fe-145">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-145">String</span></span>|<span data-ttu-id="9e0fe-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-146">The publisher of the app.</span></span> <span data-ttu-id="9e0fe-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9e0fe-148">largeIcon</span></span>|[<span data-ttu-id="9e0fe-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9e0fe-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9e0fe-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9e0fe-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0fe-152">createdDateTime</span></span>|<span data-ttu-id="9e0fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0fe-153">DateTimeOffset</span></span>|<span data-ttu-id="9e0fe-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-154">The date and time the app was created.</span></span> <span data-ttu-id="9e0fe-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0fe-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9e0fe-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0fe-157">DateTimeOffset</span></span>|<span data-ttu-id="9e0fe-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9e0fe-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9e0fe-160">isFeatured</span></span>|<span data-ttu-id="9e0fe-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e0fe-161">Boolean</span></span>|<span data-ttu-id="9e0fe-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9e0fe-163">privacyInformationUrl</span></span>|<span data-ttu-id="9e0fe-164">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-164">String</span></span>|<span data-ttu-id="9e0fe-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-165">The privacy statement Url.</span></span> <span data-ttu-id="9e0fe-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9e0fe-167">informationUrl</span></span>|<span data-ttu-id="9e0fe-168">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-168">String</span></span>|<span data-ttu-id="9e0fe-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-169">The more information Url.</span></span> <span data-ttu-id="9e0fe-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-171">owner</span><span class="sxs-lookup"><span data-stu-id="9e0fe-171">owner</span></span>|<span data-ttu-id="9e0fe-172">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-172">String</span></span>|<span data-ttu-id="9e0fe-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-173">The owner of the app.</span></span> <span data-ttu-id="9e0fe-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-175">developer</span><span class="sxs-lookup"><span data-stu-id="9e0fe-175">developer</span></span>|<span data-ttu-id="9e0fe-176">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-176">String</span></span>|<span data-ttu-id="9e0fe-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-177">The developer of the app.</span></span> <span data-ttu-id="9e0fe-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-179">notes</span><span class="sxs-lookup"><span data-stu-id="9e0fe-179">notes</span></span>|<span data-ttu-id="9e0fe-180">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-180">String</span></span>|<span data-ttu-id="9e0fe-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-181">Notes for the app.</span></span> <span data-ttu-id="9e0fe-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9e0fe-183">uploadState</span></span>|<span data-ttu-id="9e0fe-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9e0fe-184">Int32</span></span>|<span data-ttu-id="9e0fe-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-185">The upload state.</span></span> <span data-ttu-id="9e0fe-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9e0fe-187">publishingState</span></span>|[<span data-ttu-id="9e0fe-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9e0fe-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9e0fe-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-189">The publishing state for the app.</span></span> <span data-ttu-id="9e0fe-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9e0fe-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9e0fe-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9e0fe-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9e0fe-193">isAssigned</span></span>|<span data-ttu-id="9e0fe-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e0fe-194">Boolean</span></span>|<span data-ttu-id="9e0fe-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9e0fe-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e0fe-197">roleScopeTagIds</span></span>|<span data-ttu-id="9e0fe-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9e0fe-198">String collection</span></span>|<span data-ttu-id="9e0fe-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9e0fe-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="9e0fe-201">dependentAppCount</span></span>|<span data-ttu-id="9e0fe-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9e0fe-202">Int32</span></span>|<span data-ttu-id="9e0fe-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9e0fe-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e0fe-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9e0fe-205">committedContentVersion</span></span>|<span data-ttu-id="9e0fe-206">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-206">String</span></span>|<span data-ttu-id="9e0fe-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-207">The internal committed content version.</span></span> <span data-ttu-id="9e0fe-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e0fe-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9e0fe-209">fileName</span></span>|<span data-ttu-id="9e0fe-210">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-210">String</span></span>|<span data-ttu-id="9e0fe-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9e0fe-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e0fe-213">size</span><span class="sxs-lookup"><span data-stu-id="9e0fe-213">size</span></span>|<span data-ttu-id="9e0fe-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9e0fe-214">Int64</span></span>|<span data-ttu-id="9e0fe-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9e0fe-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e0fe-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e0fe-217">packageId</span><span class="sxs-lookup"><span data-stu-id="9e0fe-217">packageId</span></span>|<span data-ttu-id="9e0fe-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9e0fe-218">String</span></span>|<span data-ttu-id="9e0fe-219">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-219">The package identifier.</span></span>|
|<span data-ttu-id="9e0fe-220">identityName</span><span class="sxs-lookup"><span data-stu-id="9e0fe-220">identityName</span></span>|<span data-ttu-id="9e0fe-221">String</span><span class="sxs-lookup"><span data-stu-id="9e0fe-221">String</span></span>|<span data-ttu-id="9e0fe-222">ID 名。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-222">The Identity Name.</span></span>|
|<span data-ttu-id="9e0fe-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e0fe-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9e0fe-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e0fe-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="9e0fe-225">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9e0fe-226">versionName</span><span class="sxs-lookup"><span data-stu-id="9e0fe-226">versionName</span></span>|<span data-ttu-id="9e0fe-227">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-227">String</span></span>|<span data-ttu-id="9e0fe-228">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9e0fe-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="9e0fe-229">versionCode</span></span>|<span data-ttu-id="9e0fe-230">文字列</span><span class="sxs-lookup"><span data-stu-id="9e0fe-230">String</span></span>|<span data-ttu-id="9e0fe-231">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9e0fe-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9e0fe-232">identityVersion</span></span>|<span data-ttu-id="9e0fe-233">String</span><span class="sxs-lookup"><span data-stu-id="9e0fe-233">String</span></span>|<span data-ttu-id="9e0fe-234">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9e0fe-235">応答</span><span class="sxs-lookup"><span data-stu-id="9e0fe-235">Response</span></span>
<span data-ttu-id="9e0fe-236">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e0fe-237">例</span><span class="sxs-lookup"><span data-stu-id="9e0fe-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e0fe-238">要求</span><span class="sxs-lookup"><span data-stu-id="9e0fe-238">Request</span></span>
<span data-ttu-id="9e0fe-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e0fe-240">応答</span><span class="sxs-lookup"><span data-stu-id="9e0fe-240">Response</span></span>
<span data-ttu-id="9e0fe-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e0fe-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





