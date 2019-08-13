---
title: iosLobApp の作成
description: 新しい iosLobApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27868a0c42645db9b6f83f2146dc047e11a82385
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330917"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="9e288-103">iosLobApp の作成</span><span class="sxs-lookup"><span data-stu-id="9e288-103">Create iosLobApp</span></span>

> <span data-ttu-id="9e288-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e288-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e288-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e288-106">新しい [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e288-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e288-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e288-107">Prerequisites</span></span>
<span data-ttu-id="9e288-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e288-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e288-110">Permission type</span></span>|<span data-ttu-id="9e288-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e288-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e288-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e288-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e288-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e288-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e288-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e288-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e288-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e288-115">Not supported.</span></span>|
|<span data-ttu-id="9e288-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e288-116">Application</span></span>|<span data-ttu-id="9e288-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e288-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e288-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e288-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9e288-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e288-119">Request headers</span></span>
|<span data-ttu-id="9e288-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e288-120">Header</span></span>|<span data-ttu-id="9e288-121">値</span><span class="sxs-lookup"><span data-stu-id="9e288-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e288-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e288-122">Authorization</span></span>|<span data-ttu-id="9e288-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e288-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e288-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9e288-124">Accept</span></span>|<span data-ttu-id="9e288-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e288-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e288-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e288-126">Request body</span></span>
<span data-ttu-id="9e288-127">要求本文で、iosLobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e288-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="9e288-128">次の表に、iosLobApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e288-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="9e288-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e288-129">Property</span></span>|<span data-ttu-id="9e288-130">型</span><span class="sxs-lookup"><span data-stu-id="9e288-130">Type</span></span>|<span data-ttu-id="9e288-131">説明</span><span class="sxs-lookup"><span data-stu-id="9e288-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e288-132">id</span><span class="sxs-lookup"><span data-stu-id="9e288-132">id</span></span>|<span data-ttu-id="9e288-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9e288-133">String</span></span>|<span data-ttu-id="9e288-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e288-134">Key of the entity.</span></span> <span data-ttu-id="9e288-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9e288-136">displayName</span></span>|<span data-ttu-id="9e288-137">文字列</span><span class="sxs-lookup"><span data-stu-id="9e288-137">String</span></span>|<span data-ttu-id="9e288-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="9e288-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9e288-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-140">description</span><span class="sxs-lookup"><span data-stu-id="9e288-140">description</span></span>|<span data-ttu-id="9e288-141">String</span><span class="sxs-lookup"><span data-stu-id="9e288-141">String</span></span>|<span data-ttu-id="9e288-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="9e288-142">The description of the app.</span></span> <span data-ttu-id="9e288-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9e288-144">publisher</span></span>|<span data-ttu-id="9e288-145">String</span><span class="sxs-lookup"><span data-stu-id="9e288-145">String</span></span>|<span data-ttu-id="9e288-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="9e288-146">The publisher of the app.</span></span> <span data-ttu-id="9e288-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9e288-148">largeIcon</span></span>|[<span data-ttu-id="9e288-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9e288-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9e288-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="9e288-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9e288-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e288-152">createdDateTime</span></span>|<span data-ttu-id="9e288-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e288-153">DateTimeOffset</span></span>|<span data-ttu-id="9e288-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="9e288-154">The date and time the app was created.</span></span> <span data-ttu-id="9e288-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e288-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9e288-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e288-157">DateTimeOffset</span></span>|<span data-ttu-id="9e288-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="9e288-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9e288-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9e288-160">isFeatured</span></span>|<span data-ttu-id="9e288-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e288-161">Boolean</span></span>|<span data-ttu-id="9e288-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9e288-163">privacyInformationUrl</span></span>|<span data-ttu-id="9e288-164">String</span><span class="sxs-lookup"><span data-stu-id="9e288-164">String</span></span>|<span data-ttu-id="9e288-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="9e288-165">The privacy statement Url.</span></span> <span data-ttu-id="9e288-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9e288-167">informationUrl</span></span>|<span data-ttu-id="9e288-168">String</span><span class="sxs-lookup"><span data-stu-id="9e288-168">String</span></span>|<span data-ttu-id="9e288-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="9e288-169">The more information Url.</span></span> <span data-ttu-id="9e288-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-171">owner</span><span class="sxs-lookup"><span data-stu-id="9e288-171">owner</span></span>|<span data-ttu-id="9e288-172">String</span><span class="sxs-lookup"><span data-stu-id="9e288-172">String</span></span>|<span data-ttu-id="9e288-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="9e288-173">The owner of the app.</span></span> <span data-ttu-id="9e288-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-175">developer</span><span class="sxs-lookup"><span data-stu-id="9e288-175">developer</span></span>|<span data-ttu-id="9e288-176">String</span><span class="sxs-lookup"><span data-stu-id="9e288-176">String</span></span>|<span data-ttu-id="9e288-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="9e288-177">The developer of the app.</span></span> <span data-ttu-id="9e288-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-179">notes</span><span class="sxs-lookup"><span data-stu-id="9e288-179">notes</span></span>|<span data-ttu-id="9e288-180">String</span><span class="sxs-lookup"><span data-stu-id="9e288-180">String</span></span>|<span data-ttu-id="9e288-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="9e288-181">Notes for the app.</span></span> <span data-ttu-id="9e288-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9e288-183">uploadState</span></span>|<span data-ttu-id="9e288-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9e288-184">Int32</span></span>|<span data-ttu-id="9e288-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="9e288-185">The upload state.</span></span> <span data-ttu-id="9e288-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9e288-187">publishingState</span></span>|[<span data-ttu-id="9e288-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9e288-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9e288-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="9e288-189">The publishing state for the app.</span></span> <span data-ttu-id="9e288-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="9e288-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9e288-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9e288-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9e288-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="9e288-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9e288-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9e288-193">isAssigned</span></span>|<span data-ttu-id="9e288-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e288-194">Boolean</span></span>|<span data-ttu-id="9e288-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9e288-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9e288-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e288-197">roleScopeTagIds</span></span>|<span data-ttu-id="9e288-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9e288-198">String collection</span></span>|<span data-ttu-id="9e288-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="9e288-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9e288-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9e288-201">dependentAppCount</span></span>|<span data-ttu-id="9e288-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9e288-202">Int32</span></span>|<span data-ttu-id="9e288-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="9e288-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9e288-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e288-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9e288-205">committedContentVersion</span></span>|<span data-ttu-id="9e288-206">String</span><span class="sxs-lookup"><span data-stu-id="9e288-206">String</span></span>|<span data-ttu-id="9e288-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e288-207">The internal committed content version.</span></span> <span data-ttu-id="9e288-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e288-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9e288-209">fileName</span></span>|<span data-ttu-id="9e288-210">String</span><span class="sxs-lookup"><span data-stu-id="9e288-210">String</span></span>|<span data-ttu-id="9e288-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="9e288-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9e288-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e288-213">size</span><span class="sxs-lookup"><span data-stu-id="9e288-213">size</span></span>|<span data-ttu-id="9e288-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9e288-214">Int64</span></span>|<span data-ttu-id="9e288-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="9e288-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9e288-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e288-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e288-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="9e288-217">bundleId</span></span>|<span data-ttu-id="9e288-218">String</span><span class="sxs-lookup"><span data-stu-id="9e288-218">String</span></span>|<span data-ttu-id="9e288-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="9e288-219">The Identity Name.</span></span>|
|<span data-ttu-id="9e288-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9e288-220">applicableDeviceType</span></span>|[<span data-ttu-id="9e288-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9e288-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9e288-222">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="9e288-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9e288-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e288-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9e288-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e288-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9e288-225">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="9e288-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9e288-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e288-226">expirationDateTime</span></span>|<span data-ttu-id="9e288-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e288-227">DateTimeOffset</span></span>|<span data-ttu-id="9e288-228">有効期限。</span><span class="sxs-lookup"><span data-stu-id="9e288-228">The expiration time.</span></span>|
|<span data-ttu-id="9e288-229">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="9e288-229">versionNumber</span></span>|<span data-ttu-id="9e288-230">String</span><span class="sxs-lookup"><span data-stu-id="9e288-230">String</span></span>|<span data-ttu-id="9e288-231">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="9e288-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9e288-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9e288-232">buildNumber</span></span>|<span data-ttu-id="9e288-233">String</span><span class="sxs-lookup"><span data-stu-id="9e288-233">String</span></span>|<span data-ttu-id="9e288-234">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="9e288-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9e288-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9e288-235">identityVersion</span></span>|<span data-ttu-id="9e288-236">String</span><span class="sxs-lookup"><span data-stu-id="9e288-236">String</span></span>|<span data-ttu-id="9e288-237">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e288-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9e288-238">応答</span><span class="sxs-lookup"><span data-stu-id="9e288-238">Response</span></span>
<span data-ttu-id="9e288-239">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e288-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e288-240">例</span><span class="sxs-lookup"><span data-stu-id="9e288-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e288-241">要求</span><span class="sxs-lookup"><span data-stu-id="9e288-241">Request</span></span>
<span data-ttu-id="9e288-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e288-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1391

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="9e288-243">応答</span><span class="sxs-lookup"><span data-stu-id="9e288-243">Response</span></span>
<span data-ttu-id="9e288-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e288-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1563

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```






