---
title: Create managedAndroidLobApp
description: 新しい managedAndroidLobApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56e8a68a817bbca8e575d34f69d55f5bd3dccba5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930036"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="31bad-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="31bad-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="31bad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31bad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31bad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31bad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31bad-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31bad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31bad-107">新しい [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31bad-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31bad-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="31bad-108">Prerequisites</span></span>
<span data-ttu-id="31bad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31bad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31bad-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31bad-111">Permission type</span></span>|<span data-ttu-id="31bad-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31bad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31bad-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31bad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31bad-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31bad-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31bad-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31bad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31bad-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31bad-116">Not supported.</span></span>|
|<span data-ttu-id="31bad-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31bad-117">Application</span></span>|<span data-ttu-id="31bad-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31bad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31bad-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31bad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="31bad-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31bad-120">Request headers</span></span>
|<span data-ttu-id="31bad-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31bad-121">Header</span></span>|<span data-ttu-id="31bad-122">値</span><span class="sxs-lookup"><span data-stu-id="31bad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31bad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31bad-123">Authorization</span></span>|<span data-ttu-id="31bad-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="31bad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31bad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31bad-125">Accept</span></span>|<span data-ttu-id="31bad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31bad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31bad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="31bad-127">Request body</span></span>
<span data-ttu-id="31bad-128">要求本文で、managedAndroidLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31bad-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="31bad-129">次の表に、managedAndroidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31bad-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="31bad-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31bad-130">Property</span></span>|<span data-ttu-id="31bad-131">種類</span><span class="sxs-lookup"><span data-stu-id="31bad-131">Type</span></span>|<span data-ttu-id="31bad-132">説明</span><span class="sxs-lookup"><span data-stu-id="31bad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31bad-133">ID</span><span class="sxs-lookup"><span data-stu-id="31bad-133">id</span></span>|<span data-ttu-id="31bad-134">String</span><span class="sxs-lookup"><span data-stu-id="31bad-134">String</span></span>|<span data-ttu-id="31bad-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31bad-135">Key of the entity.</span></span> <span data-ttu-id="31bad-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-137">displayName</span><span class="sxs-lookup"><span data-stu-id="31bad-137">displayName</span></span>|<span data-ttu-id="31bad-138">String</span><span class="sxs-lookup"><span data-stu-id="31bad-138">String</span></span>|<span data-ttu-id="31bad-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="31bad-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="31bad-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-141">説明</span><span class="sxs-lookup"><span data-stu-id="31bad-141">description</span></span>|<span data-ttu-id="31bad-142">String</span><span class="sxs-lookup"><span data-stu-id="31bad-142">String</span></span>|<span data-ttu-id="31bad-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="31bad-143">The description of the app.</span></span> <span data-ttu-id="31bad-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-145">publisher</span><span class="sxs-lookup"><span data-stu-id="31bad-145">publisher</span></span>|<span data-ttu-id="31bad-146">String</span><span class="sxs-lookup"><span data-stu-id="31bad-146">String</span></span>|<span data-ttu-id="31bad-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="31bad-147">The publisher of the app.</span></span> <span data-ttu-id="31bad-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="31bad-149">largeIcon</span></span>|[<span data-ttu-id="31bad-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="31bad-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="31bad-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="31bad-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="31bad-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31bad-153">createdDateTime</span></span>|<span data-ttu-id="31bad-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31bad-154">DateTimeOffset</span></span>|<span data-ttu-id="31bad-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="31bad-155">The date and time the app was created.</span></span> <span data-ttu-id="31bad-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31bad-157">lastModifiedDateTime</span></span>|<span data-ttu-id="31bad-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31bad-158">DateTimeOffset</span></span>|<span data-ttu-id="31bad-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="31bad-159">The date and time the app was last modified.</span></span> <span data-ttu-id="31bad-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="31bad-161">isFeatured</span></span>|<span data-ttu-id="31bad-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="31bad-162">Boolean</span></span>|<span data-ttu-id="31bad-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="31bad-164">privacyInformationUrl</span></span>|<span data-ttu-id="31bad-165">String</span><span class="sxs-lookup"><span data-stu-id="31bad-165">String</span></span>|<span data-ttu-id="31bad-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="31bad-166">The privacy statement Url.</span></span> <span data-ttu-id="31bad-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="31bad-168">informationUrl</span></span>|<span data-ttu-id="31bad-169">String</span><span class="sxs-lookup"><span data-stu-id="31bad-169">String</span></span>|<span data-ttu-id="31bad-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="31bad-170">The more information Url.</span></span> <span data-ttu-id="31bad-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-172">owner</span><span class="sxs-lookup"><span data-stu-id="31bad-172">owner</span></span>|<span data-ttu-id="31bad-173">String</span><span class="sxs-lookup"><span data-stu-id="31bad-173">String</span></span>|<span data-ttu-id="31bad-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="31bad-174">The owner of the app.</span></span> <span data-ttu-id="31bad-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-176">developer</span><span class="sxs-lookup"><span data-stu-id="31bad-176">developer</span></span>|<span data-ttu-id="31bad-177">String</span><span class="sxs-lookup"><span data-stu-id="31bad-177">String</span></span>|<span data-ttu-id="31bad-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="31bad-178">The developer of the app.</span></span> <span data-ttu-id="31bad-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-180">notes</span><span class="sxs-lookup"><span data-stu-id="31bad-180">notes</span></span>|<span data-ttu-id="31bad-181">String</span><span class="sxs-lookup"><span data-stu-id="31bad-181">String</span></span>|<span data-ttu-id="31bad-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="31bad-182">Notes for the app.</span></span> <span data-ttu-id="31bad-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="31bad-184">uploadState</span></span>|<span data-ttu-id="31bad-185">Int32</span><span class="sxs-lookup"><span data-stu-id="31bad-185">Int32</span></span>|<span data-ttu-id="31bad-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="31bad-186">The upload state.</span></span> <span data-ttu-id="31bad-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31bad-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="31bad-188">publishingState</span></span>|[<span data-ttu-id="31bad-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="31bad-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="31bad-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="31bad-190">The publishing state for the app.</span></span> <span data-ttu-id="31bad-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="31bad-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="31bad-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="31bad-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="31bad-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="31bad-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="31bad-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="31bad-194">appAvailability</span></span>|[<span data-ttu-id="31bad-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="31bad-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="31bad-196">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="31bad-196">The Application's availability.</span></span> <span data-ttu-id="31bad-197">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="31bad-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="31bad-198">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="31bad-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="31bad-199">version</span><span class="sxs-lookup"><span data-stu-id="31bad-199">version</span></span>|<span data-ttu-id="31bad-200">String</span><span class="sxs-lookup"><span data-stu-id="31bad-200">String</span></span>|<span data-ttu-id="31bad-201">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="31bad-201">The Application's version.</span></span> <span data-ttu-id="31bad-202">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="31bad-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="31bad-203">committedContentVersion</span></span>|<span data-ttu-id="31bad-204">String</span><span class="sxs-lookup"><span data-stu-id="31bad-204">String</span></span>|<span data-ttu-id="31bad-205">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="31bad-205">The internal committed content version.</span></span> <span data-ttu-id="31bad-206">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="31bad-207">fileName</span><span class="sxs-lookup"><span data-stu-id="31bad-207">fileName</span></span>|<span data-ttu-id="31bad-208">String</span><span class="sxs-lookup"><span data-stu-id="31bad-208">String</span></span>|<span data-ttu-id="31bad-209">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="31bad-209">The name of the main Lob application file.</span></span> <span data-ttu-id="31bad-210">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="31bad-211">size</span><span class="sxs-lookup"><span data-stu-id="31bad-211">size</span></span>|<span data-ttu-id="31bad-212">Int64</span><span class="sxs-lookup"><span data-stu-id="31bad-212">Int64</span></span>|<span data-ttu-id="31bad-213">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="31bad-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="31bad-214">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31bad-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="31bad-215">packageId</span><span class="sxs-lookup"><span data-stu-id="31bad-215">packageId</span></span>|<span data-ttu-id="31bad-216">String</span><span class="sxs-lookup"><span data-stu-id="31bad-216">String</span></span>|<span data-ttu-id="31bad-217">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="31bad-217">The package identifier.</span></span>|
|<span data-ttu-id="31bad-218">identityName</span><span class="sxs-lookup"><span data-stu-id="31bad-218">identityName</span></span>|<span data-ttu-id="31bad-219">String</span><span class="sxs-lookup"><span data-stu-id="31bad-219">String</span></span>|<span data-ttu-id="31bad-220">ID 名。</span><span class="sxs-lookup"><span data-stu-id="31bad-220">The Identity Name.</span></span>|
|<span data-ttu-id="31bad-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="31bad-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="31bad-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="31bad-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="31bad-223">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="31bad-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="31bad-224">versionName</span><span class="sxs-lookup"><span data-stu-id="31bad-224">versionName</span></span>|<span data-ttu-id="31bad-225">String</span><span class="sxs-lookup"><span data-stu-id="31bad-225">String</span></span>|<span data-ttu-id="31bad-226">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="31bad-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="31bad-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="31bad-227">versionCode</span></span>|<span data-ttu-id="31bad-228">String</span><span class="sxs-lookup"><span data-stu-id="31bad-228">String</span></span>|<span data-ttu-id="31bad-229">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="31bad-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="31bad-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="31bad-230">identityVersion</span></span>|<span data-ttu-id="31bad-231">String</span><span class="sxs-lookup"><span data-stu-id="31bad-231">String</span></span>|<span data-ttu-id="31bad-232">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="31bad-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="31bad-233">応答</span><span class="sxs-lookup"><span data-stu-id="31bad-233">Response</span></span>
<span data-ttu-id="31bad-234">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31bad-234">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31bad-235">例</span><span class="sxs-lookup"><span data-stu-id="31bad-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="31bad-236">要求</span><span class="sxs-lookup"><span data-stu-id="31bad-236">Request</span></span>
<span data-ttu-id="31bad-237">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31bad-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1443

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="31bad-238">応答</span><span class="sxs-lookup"><span data-stu-id="31bad-238">Response</span></span>
<span data-ttu-id="31bad-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31bad-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1551

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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





