---
title: iosLobApp の更新
description: iosLobApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a0974cfb57d793f4b51143e0e2e1445dca33392
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966167"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="03c78-103">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="03c78-103">Update iosLobApp</span></span>

> <span data-ttu-id="03c78-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03c78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03c78-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03c78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03c78-106">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="03c78-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03c78-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="03c78-107">Prerequisites</span></span>
<span data-ttu-id="03c78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03c78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c78-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03c78-110">Permission type</span></span>|<span data-ttu-id="03c78-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="03c78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03c78-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03c78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03c78-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c78-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03c78-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03c78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03c78-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03c78-115">Not supported.</span></span>|
|<span data-ttu-id="03c78-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03c78-116">Application</span></span>|<span data-ttu-id="03c78-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03c78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03c78-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03c78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="03c78-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03c78-119">Request headers</span></span>
|<span data-ttu-id="03c78-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03c78-120">Header</span></span>|<span data-ttu-id="03c78-121">値</span><span class="sxs-lookup"><span data-stu-id="03c78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03c78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03c78-122">Authorization</span></span>|<span data-ttu-id="03c78-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="03c78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03c78-124">承諾</span><span class="sxs-lookup"><span data-stu-id="03c78-124">Accept</span></span>|<span data-ttu-id="03c78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03c78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c78-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="03c78-126">Request body</span></span>
<span data-ttu-id="03c78-127">要求本文で、[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="03c78-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="03c78-128">次の表に、[iosLobApp](../resources/intune-apps-ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="03c78-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="03c78-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03c78-129">Property</span></span>|<span data-ttu-id="03c78-130">型</span><span class="sxs-lookup"><span data-stu-id="03c78-130">Type</span></span>|<span data-ttu-id="03c78-131">説明</span><span class="sxs-lookup"><span data-stu-id="03c78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03c78-132">id</span><span class="sxs-lookup"><span data-stu-id="03c78-132">id</span></span>|<span data-ttu-id="03c78-133">文字列</span><span class="sxs-lookup"><span data-stu-id="03c78-133">String</span></span>|<span data-ttu-id="03c78-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="03c78-134">Key of the entity.</span></span> <span data-ttu-id="03c78-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-136">displayName</span><span class="sxs-lookup"><span data-stu-id="03c78-136">displayName</span></span>|<span data-ttu-id="03c78-137">文字列</span><span class="sxs-lookup"><span data-stu-id="03c78-137">String</span></span>|<span data-ttu-id="03c78-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="03c78-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="03c78-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-140">description</span><span class="sxs-lookup"><span data-stu-id="03c78-140">description</span></span>|<span data-ttu-id="03c78-141">String</span><span class="sxs-lookup"><span data-stu-id="03c78-141">String</span></span>|<span data-ttu-id="03c78-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="03c78-142">The description of the app.</span></span> <span data-ttu-id="03c78-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-144">publisher</span><span class="sxs-lookup"><span data-stu-id="03c78-144">publisher</span></span>|<span data-ttu-id="03c78-145">String</span><span class="sxs-lookup"><span data-stu-id="03c78-145">String</span></span>|<span data-ttu-id="03c78-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="03c78-146">The publisher of the app.</span></span> <span data-ttu-id="03c78-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="03c78-148">largeIcon</span></span>|[<span data-ttu-id="03c78-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="03c78-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="03c78-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="03c78-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="03c78-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03c78-152">createdDateTime</span></span>|<span data-ttu-id="03c78-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03c78-153">DateTimeOffset</span></span>|<span data-ttu-id="03c78-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="03c78-154">The date and time the app was created.</span></span> <span data-ttu-id="03c78-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03c78-156">lastModifiedDateTime</span></span>|<span data-ttu-id="03c78-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03c78-157">DateTimeOffset</span></span>|<span data-ttu-id="03c78-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="03c78-158">The date and time the app was last modified.</span></span> <span data-ttu-id="03c78-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="03c78-160">isFeatured</span></span>|<span data-ttu-id="03c78-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c78-161">Boolean</span></span>|<span data-ttu-id="03c78-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="03c78-163">privacyInformationUrl</span></span>|<span data-ttu-id="03c78-164">String</span><span class="sxs-lookup"><span data-stu-id="03c78-164">String</span></span>|<span data-ttu-id="03c78-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="03c78-165">The privacy statement Url.</span></span> <span data-ttu-id="03c78-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="03c78-167">informationUrl</span></span>|<span data-ttu-id="03c78-168">String</span><span class="sxs-lookup"><span data-stu-id="03c78-168">String</span></span>|<span data-ttu-id="03c78-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="03c78-169">The more information Url.</span></span> <span data-ttu-id="03c78-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-171">owner</span><span class="sxs-lookup"><span data-stu-id="03c78-171">owner</span></span>|<span data-ttu-id="03c78-172">String</span><span class="sxs-lookup"><span data-stu-id="03c78-172">String</span></span>|<span data-ttu-id="03c78-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="03c78-173">The owner of the app.</span></span> <span data-ttu-id="03c78-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-175">developer</span><span class="sxs-lookup"><span data-stu-id="03c78-175">developer</span></span>|<span data-ttu-id="03c78-176">String</span><span class="sxs-lookup"><span data-stu-id="03c78-176">String</span></span>|<span data-ttu-id="03c78-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="03c78-177">The developer of the app.</span></span> <span data-ttu-id="03c78-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-179">notes</span><span class="sxs-lookup"><span data-stu-id="03c78-179">notes</span></span>|<span data-ttu-id="03c78-180">String</span><span class="sxs-lookup"><span data-stu-id="03c78-180">String</span></span>|<span data-ttu-id="03c78-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="03c78-181">Notes for the app.</span></span> <span data-ttu-id="03c78-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="03c78-183">uploadState</span></span>|<span data-ttu-id="03c78-184">Int32</span><span class="sxs-lookup"><span data-stu-id="03c78-184">Int32</span></span>|<span data-ttu-id="03c78-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="03c78-185">The upload state.</span></span> <span data-ttu-id="03c78-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="03c78-187">publishingState</span></span>|[<span data-ttu-id="03c78-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="03c78-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="03c78-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="03c78-189">The publishing state for the app.</span></span> <span data-ttu-id="03c78-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="03c78-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="03c78-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="03c78-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="03c78-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="03c78-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="03c78-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="03c78-193">isAssigned</span></span>|<span data-ttu-id="03c78-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c78-194">Boolean</span></span>|<span data-ttu-id="03c78-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="03c78-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="03c78-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03c78-197">roleScopeTagIds</span></span>|<span data-ttu-id="03c78-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="03c78-198">String collection</span></span>|<span data-ttu-id="03c78-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="03c78-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="03c78-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="03c78-201">dependentAppCount</span></span>|<span data-ttu-id="03c78-202">Int32</span><span class="sxs-lookup"><span data-stu-id="03c78-202">Int32</span></span>|<span data-ttu-id="03c78-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="03c78-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="03c78-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03c78-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="03c78-205">committedContentVersion</span></span>|<span data-ttu-id="03c78-206">String</span><span class="sxs-lookup"><span data-stu-id="03c78-206">String</span></span>|<span data-ttu-id="03c78-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="03c78-207">The internal committed content version.</span></span> <span data-ttu-id="03c78-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="03c78-209">fileName</span><span class="sxs-lookup"><span data-stu-id="03c78-209">fileName</span></span>|<span data-ttu-id="03c78-210">String</span><span class="sxs-lookup"><span data-stu-id="03c78-210">String</span></span>|<span data-ttu-id="03c78-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="03c78-211">The name of the main Lob application file.</span></span> <span data-ttu-id="03c78-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="03c78-213">size</span><span class="sxs-lookup"><span data-stu-id="03c78-213">size</span></span>|<span data-ttu-id="03c78-214">Int64</span><span class="sxs-lookup"><span data-stu-id="03c78-214">Int64</span></span>|<span data-ttu-id="03c78-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="03c78-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="03c78-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="03c78-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="03c78-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="03c78-217">bundleId</span></span>|<span data-ttu-id="03c78-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="03c78-218">String</span></span>|<span data-ttu-id="03c78-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="03c78-219">The Identity Name.</span></span>|
|<span data-ttu-id="03c78-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="03c78-220">applicableDeviceType</span></span>|[<span data-ttu-id="03c78-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="03c78-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="03c78-222">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="03c78-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="03c78-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="03c78-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="03c78-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="03c78-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="03c78-225">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="03c78-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="03c78-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="03c78-226">expirationDateTime</span></span>|<span data-ttu-id="03c78-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03c78-227">DateTimeOffset</span></span>|<span data-ttu-id="03c78-228">有効期限。</span><span class="sxs-lookup"><span data-stu-id="03c78-228">The expiration time.</span></span>|
|<span data-ttu-id="03c78-229">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="03c78-229">versionNumber</span></span>|<span data-ttu-id="03c78-230">String</span><span class="sxs-lookup"><span data-stu-id="03c78-230">String</span></span>|<span data-ttu-id="03c78-231">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="03c78-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="03c78-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="03c78-232">buildNumber</span></span>|<span data-ttu-id="03c78-233">String</span><span class="sxs-lookup"><span data-stu-id="03c78-233">String</span></span>|<span data-ttu-id="03c78-234">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="03c78-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="03c78-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="03c78-235">identityVersion</span></span>|<span data-ttu-id="03c78-236">String</span><span class="sxs-lookup"><span data-stu-id="03c78-236">String</span></span>|<span data-ttu-id="03c78-237">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="03c78-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="03c78-238">応答</span><span class="sxs-lookup"><span data-stu-id="03c78-238">Response</span></span>
<span data-ttu-id="03c78-239">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="03c78-239">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03c78-240">例</span><span class="sxs-lookup"><span data-stu-id="03c78-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="03c78-241">要求</span><span class="sxs-lookup"><span data-stu-id="03c78-241">Request</span></span>
<span data-ttu-id="03c78-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03c78-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="03c78-243">応答</span><span class="sxs-lookup"><span data-stu-id="03c78-243">Response</span></span>
<span data-ttu-id="03c78-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="03c78-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





