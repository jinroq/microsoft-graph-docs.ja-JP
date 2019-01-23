---
title: iosLobApp の更新
description: iosLobApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1e2b7813752cca20f2ad1a1c111a39e65f837db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414362"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="d5710-103">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="d5710-103">Update iosLobApp</span></span>

> <span data-ttu-id="d5710-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5710-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5710-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5710-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5710-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5710-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5710-107">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5710-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5710-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5710-108">Prerequisites</span></span>
<span data-ttu-id="d5710-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5710-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d5710-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5710-111">Permission type</span></span>|<span data-ttu-id="d5710-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5710-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5710-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5710-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5710-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5710-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5710-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5710-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5710-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5710-116">Not supported.</span></span>|
|<span data-ttu-id="d5710-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5710-117">Application</span></span>|<span data-ttu-id="d5710-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5710-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5710-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5710-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d5710-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5710-120">Request headers</span></span>
|<span data-ttu-id="d5710-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5710-121">Header</span></span>|<span data-ttu-id="d5710-122">値</span><span class="sxs-lookup"><span data-stu-id="d5710-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5710-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5710-123">Authorization</span></span>|<span data-ttu-id="d5710-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d5710-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5710-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5710-125">Accept</span></span>|<span data-ttu-id="d5710-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5710-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5710-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5710-127">Request body</span></span>
<span data-ttu-id="d5710-128">要求本文で、[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5710-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="d5710-129">次の表に、[iosLobApp](../resources/intune-apps-ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d5710-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="d5710-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5710-130">Property</span></span>|<span data-ttu-id="d5710-131">型</span><span class="sxs-lookup"><span data-stu-id="d5710-131">Type</span></span>|<span data-ttu-id="d5710-132">説明</span><span class="sxs-lookup"><span data-stu-id="d5710-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5710-133">id</span><span class="sxs-lookup"><span data-stu-id="d5710-133">id</span></span>|<span data-ttu-id="d5710-134">String</span><span class="sxs-lookup"><span data-stu-id="d5710-134">String</span></span>|<span data-ttu-id="d5710-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d5710-135">Key of the entity.</span></span> <span data-ttu-id="d5710-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d5710-137">displayName</span></span>|<span data-ttu-id="d5710-138">String</span><span class="sxs-lookup"><span data-stu-id="d5710-138">String</span></span>|<span data-ttu-id="d5710-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d5710-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d5710-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-141">説明</span><span class="sxs-lookup"><span data-stu-id="d5710-141">description</span></span>|<span data-ttu-id="d5710-142">String</span><span class="sxs-lookup"><span data-stu-id="d5710-142">String</span></span>|<span data-ttu-id="d5710-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d5710-143">The description of the app.</span></span> <span data-ttu-id="d5710-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d5710-145">publisher</span></span>|<span data-ttu-id="d5710-146">String</span><span class="sxs-lookup"><span data-stu-id="d5710-146">String</span></span>|<span data-ttu-id="d5710-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d5710-147">The publisher of the app.</span></span> <span data-ttu-id="d5710-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d5710-149">largeIcon</span></span>|[<span data-ttu-id="d5710-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d5710-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d5710-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="d5710-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d5710-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5710-153">createdDateTime</span></span>|<span data-ttu-id="d5710-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5710-154">DateTimeOffset</span></span>|<span data-ttu-id="d5710-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d5710-155">The date and time the app was created.</span></span> <span data-ttu-id="d5710-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5710-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d5710-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5710-158">DateTimeOffset</span></span>|<span data-ttu-id="d5710-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d5710-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d5710-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d5710-161">isFeatured</span></span>|<span data-ttu-id="d5710-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5710-162">Boolean</span></span>|<span data-ttu-id="d5710-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d5710-164">privacyInformationUrl</span></span>|<span data-ttu-id="d5710-165">String</span><span class="sxs-lookup"><span data-stu-id="d5710-165">String</span></span>|<span data-ttu-id="d5710-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d5710-166">The privacy statement Url.</span></span> <span data-ttu-id="d5710-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d5710-168">informationUrl</span></span>|<span data-ttu-id="d5710-169">String</span><span class="sxs-lookup"><span data-stu-id="d5710-169">String</span></span>|<span data-ttu-id="d5710-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d5710-170">The more information Url.</span></span> <span data-ttu-id="d5710-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-172">owner</span><span class="sxs-lookup"><span data-stu-id="d5710-172">owner</span></span>|<span data-ttu-id="d5710-173">String</span><span class="sxs-lookup"><span data-stu-id="d5710-173">String</span></span>|<span data-ttu-id="d5710-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d5710-174">The owner of the app.</span></span> <span data-ttu-id="d5710-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-176">developer</span><span class="sxs-lookup"><span data-stu-id="d5710-176">developer</span></span>|<span data-ttu-id="d5710-177">String</span><span class="sxs-lookup"><span data-stu-id="d5710-177">String</span></span>|<span data-ttu-id="d5710-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d5710-178">The developer of the app.</span></span> <span data-ttu-id="d5710-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-180">notes</span><span class="sxs-lookup"><span data-stu-id="d5710-180">notes</span></span>|<span data-ttu-id="d5710-181">String</span><span class="sxs-lookup"><span data-stu-id="d5710-181">String</span></span>|<span data-ttu-id="d5710-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d5710-182">Notes for the app.</span></span> <span data-ttu-id="d5710-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d5710-184">uploadState</span></span>|<span data-ttu-id="d5710-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d5710-185">Int32</span></span>|<span data-ttu-id="d5710-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="d5710-186">The upload state.</span></span> <span data-ttu-id="d5710-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d5710-188">publishingState</span></span>|[<span data-ttu-id="d5710-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d5710-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d5710-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d5710-190">The publishing state for the app.</span></span> <span data-ttu-id="d5710-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d5710-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d5710-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d5710-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d5710-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d5710-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d5710-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d5710-194">isAssigned</span></span>|<span data-ttu-id="d5710-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5710-195">Boolean</span></span>|<span data-ttu-id="d5710-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="d5710-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d5710-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5710-198">roleScopeTagIds</span></span>|<span data-ttu-id="d5710-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d5710-199">String collection</span></span>|<span data-ttu-id="d5710-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d5710-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d5710-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5710-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d5710-202">committedContentVersion</span></span>|<span data-ttu-id="d5710-203">String</span><span class="sxs-lookup"><span data-stu-id="d5710-203">String</span></span>|<span data-ttu-id="d5710-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d5710-204">The internal committed content version.</span></span> <span data-ttu-id="d5710-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d5710-206">fileName</span><span class="sxs-lookup"><span data-stu-id="d5710-206">fileName</span></span>|<span data-ttu-id="d5710-207">String</span><span class="sxs-lookup"><span data-stu-id="d5710-207">String</span></span>|<span data-ttu-id="d5710-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="d5710-208">The name of the main Lob application file.</span></span> <span data-ttu-id="d5710-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d5710-210">size</span><span class="sxs-lookup"><span data-stu-id="d5710-210">size</span></span>|<span data-ttu-id="d5710-211">Int64</span><span class="sxs-lookup"><span data-stu-id="d5710-211">Int64</span></span>|<span data-ttu-id="d5710-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="d5710-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="d5710-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5710-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d5710-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="d5710-214">bundleId</span></span>|<span data-ttu-id="d5710-215">String</span><span class="sxs-lookup"><span data-stu-id="d5710-215">String</span></span>|<span data-ttu-id="d5710-216">ID 名。</span><span class="sxs-lookup"><span data-stu-id="d5710-216">The Identity Name.</span></span>|
|<span data-ttu-id="d5710-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d5710-217">applicableDeviceType</span></span>|[<span data-ttu-id="d5710-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d5710-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d5710-219">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="d5710-219">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d5710-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d5710-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d5710-221">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d5710-221">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d5710-222">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="d5710-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d5710-223">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5710-223">expirationDateTime</span></span>|<span data-ttu-id="d5710-224">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5710-224">DateTimeOffset</span></span>|<span data-ttu-id="d5710-225">有効期限。</span><span class="sxs-lookup"><span data-stu-id="d5710-225">The expiration time.</span></span>|
|<span data-ttu-id="d5710-226">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="d5710-226">versionNumber</span></span>|<span data-ttu-id="d5710-227">String</span><span class="sxs-lookup"><span data-stu-id="d5710-227">String</span></span>|<span data-ttu-id="d5710-228">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="d5710-228">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d5710-229">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d5710-229">buildNumber</span></span>|<span data-ttu-id="d5710-230">String</span><span class="sxs-lookup"><span data-stu-id="d5710-230">String</span></span>|<span data-ttu-id="d5710-231">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="d5710-231">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d5710-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d5710-232">identityVersion</span></span>|<span data-ttu-id="d5710-233">String</span><span class="sxs-lookup"><span data-stu-id="d5710-233">String</span></span>|<span data-ttu-id="d5710-234">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d5710-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d5710-235">応答</span><span class="sxs-lookup"><span data-stu-id="d5710-235">Response</span></span>
<span data-ttu-id="d5710-236">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d5710-236">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5710-237">例</span><span class="sxs-lookup"><span data-stu-id="d5710-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5710-238">要求</span><span class="sxs-lookup"><span data-stu-id="d5710-238">Request</span></span>
<span data-ttu-id="d5710-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5710-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5710-240">応答</span><span class="sxs-lookup"><span data-stu-id="d5710-240">Response</span></span>
<span data-ttu-id="d5710-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5710-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




