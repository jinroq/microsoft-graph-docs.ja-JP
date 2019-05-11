---
title: androidLobApp の作成
description: 新しい androidLobApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f87b90118975bd6f8fa89d8142c970249cdfd052
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937345"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="18bc9-103">androidLobApp の作成</span><span class="sxs-lookup"><span data-stu-id="18bc9-103">Create androidLobApp</span></span>

> <span data-ttu-id="18bc9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18bc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18bc9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18bc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18bc9-106">新しい [androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="18bc9-106">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18bc9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="18bc9-107">Prerequisites</span></span>
<span data-ttu-id="18bc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18bc9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18bc9-110">Permission type</span></span>|<span data-ttu-id="18bc9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18bc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18bc9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18bc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18bc9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18bc9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18bc9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18bc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18bc9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18bc9-115">Not supported.</span></span>|
|<span data-ttu-id="18bc9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18bc9-116">Application</span></span>|<span data-ttu-id="18bc9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18bc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18bc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18bc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="18bc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18bc9-119">Request headers</span></span>
|<span data-ttu-id="18bc9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18bc9-120">Header</span></span>|<span data-ttu-id="18bc9-121">値</span><span class="sxs-lookup"><span data-stu-id="18bc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18bc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18bc9-122">Authorization</span></span>|<span data-ttu-id="18bc9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="18bc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18bc9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="18bc9-124">Accept</span></span>|<span data-ttu-id="18bc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18bc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18bc9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="18bc9-126">Request body</span></span>
<span data-ttu-id="18bc9-127">要求本文で、androidLobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18bc9-127">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="18bc9-128">次の表に、androidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="18bc9-128">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="18bc9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18bc9-129">Property</span></span>|<span data-ttu-id="18bc9-130">型</span><span class="sxs-lookup"><span data-stu-id="18bc9-130">Type</span></span>|<span data-ttu-id="18bc9-131">説明</span><span class="sxs-lookup"><span data-stu-id="18bc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18bc9-132">id</span><span class="sxs-lookup"><span data-stu-id="18bc9-132">id</span></span>|<span data-ttu-id="18bc9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="18bc9-133">String</span></span>|<span data-ttu-id="18bc9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18bc9-134">Key of the entity.</span></span> <span data-ttu-id="18bc9-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="18bc9-136">displayName</span></span>|<span data-ttu-id="18bc9-137">文字列</span><span class="sxs-lookup"><span data-stu-id="18bc9-137">String</span></span>|<span data-ttu-id="18bc9-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="18bc9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18bc9-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-140">description</span><span class="sxs-lookup"><span data-stu-id="18bc9-140">description</span></span>|<span data-ttu-id="18bc9-141">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-141">String</span></span>|<span data-ttu-id="18bc9-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="18bc9-142">The description of the app.</span></span> <span data-ttu-id="18bc9-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="18bc9-144">publisher</span></span>|<span data-ttu-id="18bc9-145">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-145">String</span></span>|<span data-ttu-id="18bc9-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="18bc9-146">The publisher of the app.</span></span> <span data-ttu-id="18bc9-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18bc9-148">largeIcon</span></span>|[<span data-ttu-id="18bc9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18bc9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18bc9-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="18bc9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18bc9-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18bc9-152">createdDateTime</span></span>|<span data-ttu-id="18bc9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18bc9-153">DateTimeOffset</span></span>|<span data-ttu-id="18bc9-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="18bc9-154">The date and time the app was created.</span></span> <span data-ttu-id="18bc9-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18bc9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="18bc9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18bc9-157">DateTimeOffset</span></span>|<span data-ttu-id="18bc9-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="18bc9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="18bc9-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18bc9-160">isFeatured</span></span>|<span data-ttu-id="18bc9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="18bc9-161">Boolean</span></span>|<span data-ttu-id="18bc9-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18bc9-163">privacyInformationUrl</span></span>|<span data-ttu-id="18bc9-164">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-164">String</span></span>|<span data-ttu-id="18bc9-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="18bc9-165">The privacy statement Url.</span></span> <span data-ttu-id="18bc9-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18bc9-167">informationUrl</span></span>|<span data-ttu-id="18bc9-168">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-168">String</span></span>|<span data-ttu-id="18bc9-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="18bc9-169">The more information Url.</span></span> <span data-ttu-id="18bc9-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-171">owner</span><span class="sxs-lookup"><span data-stu-id="18bc9-171">owner</span></span>|<span data-ttu-id="18bc9-172">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-172">String</span></span>|<span data-ttu-id="18bc9-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="18bc9-173">The owner of the app.</span></span> <span data-ttu-id="18bc9-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-175">developer</span><span class="sxs-lookup"><span data-stu-id="18bc9-175">developer</span></span>|<span data-ttu-id="18bc9-176">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-176">String</span></span>|<span data-ttu-id="18bc9-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="18bc9-177">The developer of the app.</span></span> <span data-ttu-id="18bc9-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-179">notes</span><span class="sxs-lookup"><span data-stu-id="18bc9-179">notes</span></span>|<span data-ttu-id="18bc9-180">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-180">String</span></span>|<span data-ttu-id="18bc9-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="18bc9-181">Notes for the app.</span></span> <span data-ttu-id="18bc9-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="18bc9-183">uploadState</span></span>|<span data-ttu-id="18bc9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="18bc9-184">Int32</span></span>|<span data-ttu-id="18bc9-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="18bc9-185">The upload state.</span></span> <span data-ttu-id="18bc9-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="18bc9-187">publishingState</span></span>|[<span data-ttu-id="18bc9-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18bc9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18bc9-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="18bc9-189">The publishing state for the app.</span></span> <span data-ttu-id="18bc9-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="18bc9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18bc9-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="18bc9-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18bc9-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="18bc9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18bc9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="18bc9-193">isAssigned</span></span>|<span data-ttu-id="18bc9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="18bc9-194">Boolean</span></span>|<span data-ttu-id="18bc9-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="18bc9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="18bc9-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18bc9-197">roleScopeTagIds</span></span>|<span data-ttu-id="18bc9-198">String collection</span><span class="sxs-lookup"><span data-stu-id="18bc9-198">String collection</span></span>|<span data-ttu-id="18bc9-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="18bc9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="18bc9-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="18bc9-201">dependentAppCount</span></span>|<span data-ttu-id="18bc9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="18bc9-202">Int32</span></span>|<span data-ttu-id="18bc9-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="18bc9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="18bc9-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18bc9-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="18bc9-205">committedContentVersion</span></span>|<span data-ttu-id="18bc9-206">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-206">String</span></span>|<span data-ttu-id="18bc9-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="18bc9-207">The internal committed content version.</span></span> <span data-ttu-id="18bc9-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18bc9-209">fileName</span><span class="sxs-lookup"><span data-stu-id="18bc9-209">fileName</span></span>|<span data-ttu-id="18bc9-210">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-210">String</span></span>|<span data-ttu-id="18bc9-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="18bc9-211">The name of the main Lob application file.</span></span> <span data-ttu-id="18bc9-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18bc9-213">size</span><span class="sxs-lookup"><span data-stu-id="18bc9-213">size</span></span>|<span data-ttu-id="18bc9-214">Int64</span><span class="sxs-lookup"><span data-stu-id="18bc9-214">Int64</span></span>|<span data-ttu-id="18bc9-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="18bc9-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="18bc9-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18bc9-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18bc9-217">packageId</span><span class="sxs-lookup"><span data-stu-id="18bc9-217">packageId</span></span>|<span data-ttu-id="18bc9-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="18bc9-218">String</span></span>|<span data-ttu-id="18bc9-219">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="18bc9-219">The package identifier.</span></span>|
|<span data-ttu-id="18bc9-220">identityName</span><span class="sxs-lookup"><span data-stu-id="18bc9-220">identityName</span></span>|<span data-ttu-id="18bc9-221">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-221">String</span></span>|<span data-ttu-id="18bc9-222">ID 名。</span><span class="sxs-lookup"><span data-stu-id="18bc9-222">The Identity Name.</span></span>|
|<span data-ttu-id="18bc9-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18bc9-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18bc9-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18bc9-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="18bc9-225">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="18bc9-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="18bc9-226">versionName</span><span class="sxs-lookup"><span data-stu-id="18bc9-226">versionName</span></span>|<span data-ttu-id="18bc9-227">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-227">String</span></span>|<span data-ttu-id="18bc9-228">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="18bc9-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18bc9-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="18bc9-229">versionCode</span></span>|<span data-ttu-id="18bc9-230">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-230">String</span></span>|<span data-ttu-id="18bc9-231">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="18bc9-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18bc9-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="18bc9-232">identityVersion</span></span>|<span data-ttu-id="18bc9-233">String</span><span class="sxs-lookup"><span data-stu-id="18bc9-233">String</span></span>|<span data-ttu-id="18bc9-234">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="18bc9-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="18bc9-235">応答</span><span class="sxs-lookup"><span data-stu-id="18bc9-235">Response</span></span>
<span data-ttu-id="18bc9-236">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18bc9-236">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18bc9-237">例</span><span class="sxs-lookup"><span data-stu-id="18bc9-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="18bc9-238">要求</span><span class="sxs-lookup"><span data-stu-id="18bc9-238">Request</span></span>
<span data-ttu-id="18bc9-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18bc9-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="18bc9-240">応答</span><span class="sxs-lookup"><span data-stu-id="18bc9-240">Response</span></span>
<span data-ttu-id="18bc9-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18bc9-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




