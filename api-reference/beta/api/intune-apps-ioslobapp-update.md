---
title: iosLobApp の更新
description: iosLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 339f09af9617f97f73d5560b26447b045c4ba532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158402"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="5c509-103">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="5c509-103">Update iosLobApp</span></span>

> <span data-ttu-id="5c509-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c509-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c509-106">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c509-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c509-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5c509-107">Prerequisites</span></span>
<span data-ttu-id="5c509-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c509-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c509-110">Permission type</span></span>|<span data-ttu-id="5c509-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c509-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c509-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c509-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c509-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c509-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c509-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c509-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c509-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c509-115">Not supported.</span></span>|
|<span data-ttu-id="5c509-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c509-116">Application</span></span>|<span data-ttu-id="5c509-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c509-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c509-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c509-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5c509-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c509-119">Request headers</span></span>
|<span data-ttu-id="5c509-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c509-120">Header</span></span>|<span data-ttu-id="5c509-121">値</span><span class="sxs-lookup"><span data-stu-id="5c509-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c509-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c509-122">Authorization</span></span>|<span data-ttu-id="5c509-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5c509-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c509-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5c509-124">Accept</span></span>|<span data-ttu-id="5c509-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c509-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c509-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c509-126">Request body</span></span>
<span data-ttu-id="5c509-127">要求本文で、[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c509-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="5c509-128">次の表に、[iosLobApp](../resources/intune-apps-ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5c509-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="5c509-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c509-129">Property</span></span>|<span data-ttu-id="5c509-130">型</span><span class="sxs-lookup"><span data-stu-id="5c509-130">Type</span></span>|<span data-ttu-id="5c509-131">説明</span><span class="sxs-lookup"><span data-stu-id="5c509-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c509-132">id</span><span class="sxs-lookup"><span data-stu-id="5c509-132">id</span></span>|<span data-ttu-id="5c509-133">文字列</span><span class="sxs-lookup"><span data-stu-id="5c509-133">String</span></span>|<span data-ttu-id="5c509-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5c509-134">Key of the entity.</span></span> <span data-ttu-id="5c509-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5c509-136">displayName</span></span>|<span data-ttu-id="5c509-137">String</span><span class="sxs-lookup"><span data-stu-id="5c509-137">String</span></span>|<span data-ttu-id="5c509-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="5c509-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c509-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-140">説明</span><span class="sxs-lookup"><span data-stu-id="5c509-140">description</span></span>|<span data-ttu-id="5c509-141">文字列</span><span class="sxs-lookup"><span data-stu-id="5c509-141">String</span></span>|<span data-ttu-id="5c509-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="5c509-142">The description of the app.</span></span> <span data-ttu-id="5c509-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5c509-144">publisher</span></span>|<span data-ttu-id="5c509-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c509-145">String</span></span>|<span data-ttu-id="5c509-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="5c509-146">The publisher of the app.</span></span> <span data-ttu-id="5c509-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c509-148">largeIcon</span></span>|[<span data-ttu-id="5c509-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c509-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c509-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="5c509-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c509-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c509-152">createdDateTime</span></span>|<span data-ttu-id="5c509-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c509-153">DateTimeOffset</span></span>|<span data-ttu-id="5c509-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5c509-154">The date and time the app was created.</span></span> <span data-ttu-id="5c509-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c509-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5c509-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c509-157">DateTimeOffset</span></span>|<span data-ttu-id="5c509-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5c509-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5c509-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c509-160">isFeatured</span></span>|<span data-ttu-id="5c509-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c509-161">Boolean</span></span>|<span data-ttu-id="5c509-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c509-163">privacyInformationUrl</span></span>|<span data-ttu-id="5c509-164">String</span><span class="sxs-lookup"><span data-stu-id="5c509-164">String</span></span>|<span data-ttu-id="5c509-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="5c509-165">The privacy statement Url.</span></span> <span data-ttu-id="5c509-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c509-167">informationUrl</span></span>|<span data-ttu-id="5c509-168">String</span><span class="sxs-lookup"><span data-stu-id="5c509-168">String</span></span>|<span data-ttu-id="5c509-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="5c509-169">The more information Url.</span></span> <span data-ttu-id="5c509-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-171">owner</span><span class="sxs-lookup"><span data-stu-id="5c509-171">owner</span></span>|<span data-ttu-id="5c509-172">String</span><span class="sxs-lookup"><span data-stu-id="5c509-172">String</span></span>|<span data-ttu-id="5c509-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="5c509-173">The owner of the app.</span></span> <span data-ttu-id="5c509-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-175">developer</span><span class="sxs-lookup"><span data-stu-id="5c509-175">developer</span></span>|<span data-ttu-id="5c509-176">String</span><span class="sxs-lookup"><span data-stu-id="5c509-176">String</span></span>|<span data-ttu-id="5c509-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="5c509-177">The developer of the app.</span></span> <span data-ttu-id="5c509-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-179">notes</span><span class="sxs-lookup"><span data-stu-id="5c509-179">notes</span></span>|<span data-ttu-id="5c509-180">String</span><span class="sxs-lookup"><span data-stu-id="5c509-180">String</span></span>|<span data-ttu-id="5c509-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="5c509-181">Notes for the app.</span></span> <span data-ttu-id="5c509-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5c509-183">uploadState</span></span>|<span data-ttu-id="5c509-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5c509-184">Int32</span></span>|<span data-ttu-id="5c509-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="5c509-185">The upload state.</span></span> <span data-ttu-id="5c509-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c509-187">publishingState</span></span>|[<span data-ttu-id="5c509-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c509-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c509-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="5c509-189">The publishing state for the app.</span></span> <span data-ttu-id="5c509-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="5c509-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c509-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5c509-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c509-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="5c509-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c509-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c509-193">isAssigned</span></span>|<span data-ttu-id="5c509-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c509-194">Boolean</span></span>|<span data-ttu-id="5c509-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="5c509-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5c509-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c509-197">roleScopeTagIds</span></span>|<span data-ttu-id="5c509-198">String collection</span><span class="sxs-lookup"><span data-stu-id="5c509-198">String collection</span></span>|<span data-ttu-id="5c509-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="5c509-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5c509-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c509-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5c509-201">committedContentVersion</span></span>|<span data-ttu-id="5c509-202">String</span><span class="sxs-lookup"><span data-stu-id="5c509-202">String</span></span>|<span data-ttu-id="5c509-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5c509-203">The internal committed content version.</span></span> <span data-ttu-id="5c509-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c509-205">fileName</span><span class="sxs-lookup"><span data-stu-id="5c509-205">fileName</span></span>|<span data-ttu-id="5c509-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c509-206">String</span></span>|<span data-ttu-id="5c509-207">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="5c509-207">The name of the main Lob application file.</span></span> <span data-ttu-id="5c509-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c509-209">size</span><span class="sxs-lookup"><span data-stu-id="5c509-209">size</span></span>|<span data-ttu-id="5c509-210">Int64</span><span class="sxs-lookup"><span data-stu-id="5c509-210">Int64</span></span>|<span data-ttu-id="5c509-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="5c509-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="5c509-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c509-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5c509-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="5c509-213">bundleId</span></span>|<span data-ttu-id="5c509-214">String</span><span class="sxs-lookup"><span data-stu-id="5c509-214">String</span></span>|<span data-ttu-id="5c509-215">ID 名。</span><span class="sxs-lookup"><span data-stu-id="5c509-215">The Identity Name.</span></span>|
|<span data-ttu-id="5c509-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c509-216">applicableDeviceType</span></span>|[<span data-ttu-id="5c509-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c509-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5c509-218">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="5c509-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5c509-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c509-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5c509-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c509-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5c509-221">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="5c509-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5c509-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5c509-222">expirationDateTime</span></span>|<span data-ttu-id="5c509-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c509-223">DateTimeOffset</span></span>|<span data-ttu-id="5c509-224">有効期限。</span><span class="sxs-lookup"><span data-stu-id="5c509-224">The expiration time.</span></span>|
|<span data-ttu-id="5c509-225">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="5c509-225">versionNumber</span></span>|<span data-ttu-id="5c509-226">String</span><span class="sxs-lookup"><span data-stu-id="5c509-226">String</span></span>|<span data-ttu-id="5c509-227">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="5c509-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5c509-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5c509-228">buildNumber</span></span>|<span data-ttu-id="5c509-229">String</span><span class="sxs-lookup"><span data-stu-id="5c509-229">String</span></span>|<span data-ttu-id="5c509-230">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="5c509-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5c509-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5c509-231">identityVersion</span></span>|<span data-ttu-id="5c509-232">String</span><span class="sxs-lookup"><span data-stu-id="5c509-232">String</span></span>|<span data-ttu-id="5c509-233">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5c509-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5c509-234">応答</span><span class="sxs-lookup"><span data-stu-id="5c509-234">Response</span></span>
<span data-ttu-id="5c509-235">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="5c509-235">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c509-236">例</span><span class="sxs-lookup"><span data-stu-id="5c509-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c509-237">要求</span><span class="sxs-lookup"><span data-stu-id="5c509-237">Request</span></span>
<span data-ttu-id="5c509-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c509-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1364

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

### <a name="response"></a><span data-ttu-id="5c509-239">応答</span><span class="sxs-lookup"><span data-stu-id="5c509-239">Response</span></span>
<span data-ttu-id="5c509-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c509-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

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




