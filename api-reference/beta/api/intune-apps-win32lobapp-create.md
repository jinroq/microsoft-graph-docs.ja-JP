---
title: Win32LobApp を作成する
description: 新しい win32LobApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2c6eb2c8989c82320dc5f691ab01b48c19418f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960266"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="05ff8-103">Win32LobApp を作成する</span><span class="sxs-lookup"><span data-stu-id="05ff8-103">Create win32LobApp</span></span>

> <span data-ttu-id="05ff8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05ff8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05ff8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05ff8-106">新しい[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05ff8-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05ff8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="05ff8-107">Prerequisites</span></span>
<span data-ttu-id="05ff8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05ff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ff8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05ff8-110">Permission type</span></span>|<span data-ttu-id="05ff8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05ff8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05ff8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05ff8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05ff8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05ff8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05ff8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05ff8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05ff8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05ff8-115">Not supported.</span></span>|
|<span data-ttu-id="05ff8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05ff8-116">Application</span></span>|<span data-ttu-id="05ff8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05ff8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05ff8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05ff8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="05ff8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05ff8-119">Request headers</span></span>
|<span data-ttu-id="05ff8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05ff8-120">Header</span></span>|<span data-ttu-id="05ff8-121">値</span><span class="sxs-lookup"><span data-stu-id="05ff8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05ff8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05ff8-122">Authorization</span></span>|<span data-ttu-id="05ff8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="05ff8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05ff8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="05ff8-124">Accept</span></span>|<span data-ttu-id="05ff8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05ff8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ff8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="05ff8-126">Request body</span></span>
<span data-ttu-id="05ff8-127">要求本文で、win32LobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05ff8-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="05ff8-128">次の表に、win32LobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05ff8-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="05ff8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05ff8-129">Property</span></span>|<span data-ttu-id="05ff8-130">型</span><span class="sxs-lookup"><span data-stu-id="05ff8-130">Type</span></span>|<span data-ttu-id="05ff8-131">説明</span><span class="sxs-lookup"><span data-stu-id="05ff8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ff8-132">id</span><span class="sxs-lookup"><span data-stu-id="05ff8-132">id</span></span>|<span data-ttu-id="05ff8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="05ff8-133">String</span></span>|<span data-ttu-id="05ff8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="05ff8-134">Key of the entity.</span></span> <span data-ttu-id="05ff8-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="05ff8-136">displayName</span></span>|<span data-ttu-id="05ff8-137">文字列</span><span class="sxs-lookup"><span data-stu-id="05ff8-137">String</span></span>|<span data-ttu-id="05ff8-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="05ff8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="05ff8-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-140">description</span><span class="sxs-lookup"><span data-stu-id="05ff8-140">description</span></span>|<span data-ttu-id="05ff8-141">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-141">String</span></span>|<span data-ttu-id="05ff8-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="05ff8-142">The description of the app.</span></span> <span data-ttu-id="05ff8-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="05ff8-144">publisher</span></span>|<span data-ttu-id="05ff8-145">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-145">String</span></span>|<span data-ttu-id="05ff8-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="05ff8-146">The publisher of the app.</span></span> <span data-ttu-id="05ff8-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="05ff8-148">largeIcon</span></span>|[<span data-ttu-id="05ff8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05ff8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05ff8-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="05ff8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="05ff8-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05ff8-152">createdDateTime</span></span>|<span data-ttu-id="05ff8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05ff8-153">DateTimeOffset</span></span>|<span data-ttu-id="05ff8-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="05ff8-154">The date and time the app was created.</span></span> <span data-ttu-id="05ff8-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05ff8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="05ff8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05ff8-157">DateTimeOffset</span></span>|<span data-ttu-id="05ff8-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="05ff8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="05ff8-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="05ff8-160">isFeatured</span></span>|<span data-ttu-id="05ff8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="05ff8-161">Boolean</span></span>|<span data-ttu-id="05ff8-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="05ff8-163">privacyInformationUrl</span></span>|<span data-ttu-id="05ff8-164">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-164">String</span></span>|<span data-ttu-id="05ff8-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="05ff8-165">The privacy statement Url.</span></span> <span data-ttu-id="05ff8-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="05ff8-167">informationUrl</span></span>|<span data-ttu-id="05ff8-168">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-168">String</span></span>|<span data-ttu-id="05ff8-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="05ff8-169">The more information Url.</span></span> <span data-ttu-id="05ff8-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-171">owner</span><span class="sxs-lookup"><span data-stu-id="05ff8-171">owner</span></span>|<span data-ttu-id="05ff8-172">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-172">String</span></span>|<span data-ttu-id="05ff8-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="05ff8-173">The owner of the app.</span></span> <span data-ttu-id="05ff8-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-175">developer</span><span class="sxs-lookup"><span data-stu-id="05ff8-175">developer</span></span>|<span data-ttu-id="05ff8-176">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-176">String</span></span>|<span data-ttu-id="05ff8-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="05ff8-177">The developer of the app.</span></span> <span data-ttu-id="05ff8-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-179">notes</span><span class="sxs-lookup"><span data-stu-id="05ff8-179">notes</span></span>|<span data-ttu-id="05ff8-180">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-180">String</span></span>|<span data-ttu-id="05ff8-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="05ff8-181">Notes for the app.</span></span> <span data-ttu-id="05ff8-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="05ff8-183">uploadState</span></span>|<span data-ttu-id="05ff8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-184">Int32</span></span>|<span data-ttu-id="05ff8-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="05ff8-185">The upload state.</span></span> <span data-ttu-id="05ff8-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="05ff8-187">publishingState</span></span>|[<span data-ttu-id="05ff8-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="05ff8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="05ff8-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="05ff8-189">The publishing state for the app.</span></span> <span data-ttu-id="05ff8-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="05ff8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="05ff8-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="05ff8-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="05ff8-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="05ff8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="05ff8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="05ff8-193">isAssigned</span></span>|<span data-ttu-id="05ff8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="05ff8-194">Boolean</span></span>|<span data-ttu-id="05ff8-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="05ff8-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05ff8-197">roleScopeTagIds</span></span>|<span data-ttu-id="05ff8-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="05ff8-198">String collection</span></span>|<span data-ttu-id="05ff8-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="05ff8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="05ff8-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="05ff8-201">dependentAppCount</span></span>|<span data-ttu-id="05ff8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-202">Int32</span></span>|<span data-ttu-id="05ff8-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="05ff8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="05ff8-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05ff8-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="05ff8-205">committedContentVersion</span></span>|<span data-ttu-id="05ff8-206">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-206">String</span></span>|<span data-ttu-id="05ff8-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="05ff8-207">The internal committed content version.</span></span> <span data-ttu-id="05ff8-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="05ff8-209">fileName</span><span class="sxs-lookup"><span data-stu-id="05ff8-209">fileName</span></span>|<span data-ttu-id="05ff8-210">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-210">String</span></span>|<span data-ttu-id="05ff8-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="05ff8-211">The name of the main Lob application file.</span></span> <span data-ttu-id="05ff8-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="05ff8-213">size</span><span class="sxs-lookup"><span data-stu-id="05ff8-213">size</span></span>|<span data-ttu-id="05ff8-214">Int64</span><span class="sxs-lookup"><span data-stu-id="05ff8-214">Int64</span></span>|<span data-ttu-id="05ff8-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="05ff8-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="05ff8-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05ff8-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="05ff8-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="05ff8-217">installCommandLine</span></span>|<span data-ttu-id="05ff8-218">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-218">String</span></span>|<span data-ttu-id="05ff8-219">このアプリをインストールするためのコマンドライン</span><span class="sxs-lookup"><span data-stu-id="05ff8-219">The command line to install this app</span></span>|
|<span data-ttu-id="05ff8-220">アン Installcommandline</span><span class="sxs-lookup"><span data-stu-id="05ff8-220">uninstallCommandLine</span></span>|<span data-ttu-id="05ff8-221">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-221">String</span></span>|<span data-ttu-id="05ff8-222">このアプリをアンインストールするためのコマンドライン</span><span class="sxs-lookup"><span data-stu-id="05ff8-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="05ff8-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="05ff8-223">applicableArchitectures</span></span>|[<span data-ttu-id="05ff8-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="05ff8-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="05ff8-225">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="05ff8-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="05ff8-226">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="05ff8-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="05ff8-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05ff8-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="05ff8-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05ff8-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="05ff8-229">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="05ff8-230">Minimumfreediskspace Inmb</span><span class="sxs-lookup"><span data-stu-id="05ff8-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="05ff8-231">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-231">Int32</span></span>|<span data-ttu-id="05ff8-232">このアプリをインストールするのに必要な最小空きディスク領域の値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="05ff8-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="05ff8-233">minimumMemoryInMB</span></span>|<span data-ttu-id="05ff8-234">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-234">Int32</span></span>|<span data-ttu-id="05ff8-235">このアプリをインストールするのに必要な最小物理メモリの値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="05ff8-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="05ff8-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="05ff8-237">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-237">Int32</span></span>|<span data-ttu-id="05ff8-238">このアプリのインストールに必要なプロセッサの最小数の値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="05ff8-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="05ff8-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="05ff8-240">Int32</span><span class="sxs-lookup"><span data-stu-id="05ff8-240">Int32</span></span>|<span data-ttu-id="05ff8-241">このアプリをインストールするのに必要な最小 CPU 速度の値。</span><span class="sxs-lookup"><span data-stu-id="05ff8-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="05ff8-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="05ff8-242">detectionRules</span></span>|<span data-ttu-id="05ff8-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="05ff8-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="05ff8-244">Win32 基幹業務 (LoB) アプリを検出するための検出ルール。</span><span class="sxs-lookup"><span data-stu-id="05ff8-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="05ff8-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="05ff8-245">requirementRules</span></span>|<span data-ttu-id="05ff8-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="05ff8-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="05ff8-247">Win32 基幹業務 (LoB) アプリを検出するための要件の規則。</span><span class="sxs-lookup"><span data-stu-id="05ff8-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="05ff8-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="05ff8-248">installExperience</span></span>|[<span data-ttu-id="05ff8-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="05ff8-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="05ff8-250">このアプリのインストール手順。</span><span class="sxs-lookup"><span data-stu-id="05ff8-250">The install experience for this app.</span></span>|
|<span data-ttu-id="05ff8-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="05ff8-251">returnCodes</span></span>|<span data-ttu-id="05ff8-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="05ff8-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="05ff8-253">インストール後の動作のリターンコード。</span><span class="sxs-lookup"><span data-stu-id="05ff8-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="05ff8-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="05ff8-254">msiInformation</span></span>|[<span data-ttu-id="05ff8-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="05ff8-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="05ff8-256">この Win32 アプリが MSI アプリの場合、MSI の詳細。</span><span class="sxs-lookup"><span data-stu-id="05ff8-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="05ff8-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="05ff8-257">setupFilePath</span></span>|<span data-ttu-id="05ff8-258">String</span><span class="sxs-lookup"><span data-stu-id="05ff8-258">String</span></span>|<span data-ttu-id="05ff8-259">暗号化された Win32LobApp パッケージ内のセットアップファイルの相対パス。</span><span class="sxs-lookup"><span data-stu-id="05ff8-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="05ff8-260">応答</span><span class="sxs-lookup"><span data-stu-id="05ff8-260">Response</span></span>
<span data-ttu-id="05ff8-261">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05ff8-261">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05ff8-262">例</span><span class="sxs-lookup"><span data-stu-id="05ff8-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="05ff8-263">要求</span><span class="sxs-lookup"><span data-stu-id="05ff8-263">Request</span></span>
<span data-ttu-id="05ff8-264">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05ff8-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="05ff8-265">応答</span><span class="sxs-lookup"><span data-stu-id="05ff8-265">Response</span></span>
<span data-ttu-id="05ff8-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05ff8-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





