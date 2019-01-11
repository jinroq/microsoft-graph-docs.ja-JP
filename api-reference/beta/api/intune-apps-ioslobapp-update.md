---
title: iosLobApp の更新
description: iosLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a556f521465c94366bdf1418eba69c73e9abe1f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870134"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="862dd-103">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="862dd-103">Update iosLobApp</span></span>

> <span data-ttu-id="862dd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="862dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="862dd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="862dd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="862dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="862dd-107">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="862dd-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="862dd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="862dd-108">Prerequisites</span></span>
<span data-ttu-id="862dd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="862dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="862dd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="862dd-111">Permission type</span></span>|<span data-ttu-id="862dd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="862dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="862dd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="862dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="862dd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="862dd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="862dd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="862dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="862dd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862dd-116">Not supported.</span></span>|
|<span data-ttu-id="862dd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="862dd-117">Application</span></span>|<span data-ttu-id="862dd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="862dd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="862dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="862dd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="862dd-120">Request headers</span></span>
|<span data-ttu-id="862dd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="862dd-121">Header</span></span>|<span data-ttu-id="862dd-122">値</span><span class="sxs-lookup"><span data-stu-id="862dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="862dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="862dd-123">Authorization</span></span>|<span data-ttu-id="862dd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="862dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="862dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="862dd-125">Accept</span></span>|<span data-ttu-id="862dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="862dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="862dd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="862dd-127">Request body</span></span>
<span data-ttu-id="862dd-128">要求本文で、[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="862dd-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="862dd-129">次の表に、[iosLobApp](../resources/intune-apps-ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="862dd-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="862dd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="862dd-130">Property</span></span>|<span data-ttu-id="862dd-131">種類</span><span class="sxs-lookup"><span data-stu-id="862dd-131">Type</span></span>|<span data-ttu-id="862dd-132">説明</span><span class="sxs-lookup"><span data-stu-id="862dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="862dd-133">ID</span><span class="sxs-lookup"><span data-stu-id="862dd-133">id</span></span>|<span data-ttu-id="862dd-134">String</span><span class="sxs-lookup"><span data-stu-id="862dd-134">String</span></span>|<span data-ttu-id="862dd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="862dd-135">Key of the entity.</span></span> <span data-ttu-id="862dd-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="862dd-137">displayName</span></span>|<span data-ttu-id="862dd-138">String</span><span class="sxs-lookup"><span data-stu-id="862dd-138">String</span></span>|<span data-ttu-id="862dd-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="862dd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="862dd-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-141">説明</span><span class="sxs-lookup"><span data-stu-id="862dd-141">description</span></span>|<span data-ttu-id="862dd-142">String</span><span class="sxs-lookup"><span data-stu-id="862dd-142">String</span></span>|<span data-ttu-id="862dd-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="862dd-143">The description of the app.</span></span> <span data-ttu-id="862dd-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="862dd-145">publisher</span></span>|<span data-ttu-id="862dd-146">String</span><span class="sxs-lookup"><span data-stu-id="862dd-146">String</span></span>|<span data-ttu-id="862dd-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="862dd-147">The publisher of the app.</span></span> <span data-ttu-id="862dd-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="862dd-149">largeIcon</span></span>|[<span data-ttu-id="862dd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="862dd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="862dd-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="862dd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="862dd-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="862dd-153">createdDateTime</span></span>|<span data-ttu-id="862dd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862dd-154">DateTimeOffset</span></span>|<span data-ttu-id="862dd-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="862dd-155">The date and time the app was created.</span></span> <span data-ttu-id="862dd-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="862dd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="862dd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862dd-158">DateTimeOffset</span></span>|<span data-ttu-id="862dd-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="862dd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="862dd-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="862dd-161">isFeatured</span></span>|<span data-ttu-id="862dd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="862dd-162">Boolean</span></span>|<span data-ttu-id="862dd-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="862dd-164">privacyInformationUrl</span></span>|<span data-ttu-id="862dd-165">String</span><span class="sxs-lookup"><span data-stu-id="862dd-165">String</span></span>|<span data-ttu-id="862dd-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="862dd-166">The privacy statement Url.</span></span> <span data-ttu-id="862dd-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="862dd-168">informationUrl</span></span>|<span data-ttu-id="862dd-169">String</span><span class="sxs-lookup"><span data-stu-id="862dd-169">String</span></span>|<span data-ttu-id="862dd-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="862dd-170">The more information Url.</span></span> <span data-ttu-id="862dd-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-172">owner</span><span class="sxs-lookup"><span data-stu-id="862dd-172">owner</span></span>|<span data-ttu-id="862dd-173">String</span><span class="sxs-lookup"><span data-stu-id="862dd-173">String</span></span>|<span data-ttu-id="862dd-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="862dd-174">The owner of the app.</span></span> <span data-ttu-id="862dd-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-176">developer</span><span class="sxs-lookup"><span data-stu-id="862dd-176">developer</span></span>|<span data-ttu-id="862dd-177">String</span><span class="sxs-lookup"><span data-stu-id="862dd-177">String</span></span>|<span data-ttu-id="862dd-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="862dd-178">The developer of the app.</span></span> <span data-ttu-id="862dd-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-180">notes</span><span class="sxs-lookup"><span data-stu-id="862dd-180">notes</span></span>|<span data-ttu-id="862dd-181">String</span><span class="sxs-lookup"><span data-stu-id="862dd-181">String</span></span>|<span data-ttu-id="862dd-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="862dd-182">Notes for the app.</span></span> <span data-ttu-id="862dd-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="862dd-184">uploadState</span></span>|<span data-ttu-id="862dd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="862dd-185">Int32</span></span>|<span data-ttu-id="862dd-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="862dd-186">The upload state.</span></span> <span data-ttu-id="862dd-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="862dd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="862dd-188">publishingState</span></span>|[<span data-ttu-id="862dd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="862dd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="862dd-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="862dd-190">The publishing state for the app.</span></span> <span data-ttu-id="862dd-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="862dd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="862dd-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="862dd-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="862dd-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="862dd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="862dd-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="862dd-194">committedContentVersion</span></span>|<span data-ttu-id="862dd-195">String</span><span class="sxs-lookup"><span data-stu-id="862dd-195">String</span></span>|<span data-ttu-id="862dd-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="862dd-196">The internal committed content version.</span></span> <span data-ttu-id="862dd-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="862dd-198">fileName</span><span class="sxs-lookup"><span data-stu-id="862dd-198">fileName</span></span>|<span data-ttu-id="862dd-199">String</span><span class="sxs-lookup"><span data-stu-id="862dd-199">String</span></span>|<span data-ttu-id="862dd-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="862dd-200">The name of the main Lob application file.</span></span> <span data-ttu-id="862dd-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="862dd-202">size</span><span class="sxs-lookup"><span data-stu-id="862dd-202">size</span></span>|<span data-ttu-id="862dd-203">Int64</span><span class="sxs-lookup"><span data-stu-id="862dd-203">Int64</span></span>|<span data-ttu-id="862dd-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="862dd-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="862dd-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="862dd-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="862dd-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="862dd-206">bundleId</span></span>|<span data-ttu-id="862dd-207">String</span><span class="sxs-lookup"><span data-stu-id="862dd-207">String</span></span>|<span data-ttu-id="862dd-208">ID 名。</span><span class="sxs-lookup"><span data-stu-id="862dd-208">The Identity Name.</span></span>|
|<span data-ttu-id="862dd-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="862dd-209">applicableDeviceType</span></span>|[<span data-ttu-id="862dd-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="862dd-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="862dd-211">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="862dd-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="862dd-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="862dd-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="862dd-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="862dd-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="862dd-214">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="862dd-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="862dd-215">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="862dd-215">expirationDateTime</span></span>|<span data-ttu-id="862dd-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862dd-216">DateTimeOffset</span></span>|<span data-ttu-id="862dd-217">有効期限。</span><span class="sxs-lookup"><span data-stu-id="862dd-217">The expiration time.</span></span>|
|<span data-ttu-id="862dd-218">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="862dd-218">versionNumber</span></span>|<span data-ttu-id="862dd-219">String</span><span class="sxs-lookup"><span data-stu-id="862dd-219">String</span></span>|<span data-ttu-id="862dd-220">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="862dd-220">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="862dd-221">buildNumber</span><span class="sxs-lookup"><span data-stu-id="862dd-221">buildNumber</span></span>|<span data-ttu-id="862dd-222">String</span><span class="sxs-lookup"><span data-stu-id="862dd-222">String</span></span>|<span data-ttu-id="862dd-223">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="862dd-223">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="862dd-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="862dd-224">identityVersion</span></span>|<span data-ttu-id="862dd-225">String</span><span class="sxs-lookup"><span data-stu-id="862dd-225">String</span></span>|<span data-ttu-id="862dd-226">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="862dd-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="862dd-227">応答</span><span class="sxs-lookup"><span data-stu-id="862dd-227">Response</span></span>
<span data-ttu-id="862dd-228">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="862dd-228">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="862dd-229">例</span><span class="sxs-lookup"><span data-stu-id="862dd-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="862dd-230">要求</span><span class="sxs-lookup"><span data-stu-id="862dd-230">Request</span></span>
<span data-ttu-id="862dd-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="862dd-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1295

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="862dd-232">応答</span><span class="sxs-lookup"><span data-stu-id="862dd-232">Response</span></span>
<span data-ttu-id="862dd-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="862dd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1451

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





