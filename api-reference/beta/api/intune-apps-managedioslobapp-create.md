---
title: Create managedIOSLobApp
description: 新しい managedIOSLobApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9178692b0918a099fbb5aae9271ddc244c1a60ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147300"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="338ea-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="338ea-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="338ea-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="338ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="338ea-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="338ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="338ea-106">新しい [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="338ea-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="338ea-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="338ea-107">Prerequisites</span></span>
<span data-ttu-id="338ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="338ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="338ea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="338ea-110">Permission type</span></span>|<span data-ttu-id="338ea-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="338ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="338ea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="338ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="338ea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="338ea-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="338ea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="338ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="338ea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="338ea-115">Not supported.</span></span>|
|<span data-ttu-id="338ea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="338ea-116">Application</span></span>|<span data-ttu-id="338ea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="338ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="338ea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="338ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="338ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="338ea-119">Request headers</span></span>
|<span data-ttu-id="338ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="338ea-120">Header</span></span>|<span data-ttu-id="338ea-121">値</span><span class="sxs-lookup"><span data-stu-id="338ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="338ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="338ea-122">Authorization</span></span>|<span data-ttu-id="338ea-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="338ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="338ea-124">承諾</span><span class="sxs-lookup"><span data-stu-id="338ea-124">Accept</span></span>|<span data-ttu-id="338ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="338ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="338ea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="338ea-126">Request body</span></span>
<span data-ttu-id="338ea-127">要求本文で、managedIOSLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="338ea-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="338ea-128">次の表に、managedDeviceOverview の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="338ea-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="338ea-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="338ea-129">Property</span></span>|<span data-ttu-id="338ea-130">型</span><span class="sxs-lookup"><span data-stu-id="338ea-130">Type</span></span>|<span data-ttu-id="338ea-131">説明</span><span class="sxs-lookup"><span data-stu-id="338ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="338ea-132">id</span><span class="sxs-lookup"><span data-stu-id="338ea-132">id</span></span>|<span data-ttu-id="338ea-133">文字列</span><span class="sxs-lookup"><span data-stu-id="338ea-133">String</span></span>|<span data-ttu-id="338ea-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="338ea-134">Key of the entity.</span></span> <span data-ttu-id="338ea-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="338ea-136">displayName</span></span>|<span data-ttu-id="338ea-137">String</span><span class="sxs-lookup"><span data-stu-id="338ea-137">String</span></span>|<span data-ttu-id="338ea-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="338ea-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="338ea-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-140">説明</span><span class="sxs-lookup"><span data-stu-id="338ea-140">description</span></span>|<span data-ttu-id="338ea-141">文字列</span><span class="sxs-lookup"><span data-stu-id="338ea-141">String</span></span>|<span data-ttu-id="338ea-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="338ea-142">The description of the app.</span></span> <span data-ttu-id="338ea-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-144">publisher</span><span class="sxs-lookup"><span data-stu-id="338ea-144">publisher</span></span>|<span data-ttu-id="338ea-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="338ea-145">String</span></span>|<span data-ttu-id="338ea-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="338ea-146">The publisher of the app.</span></span> <span data-ttu-id="338ea-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="338ea-148">largeIcon</span></span>|[<span data-ttu-id="338ea-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="338ea-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="338ea-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="338ea-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="338ea-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="338ea-152">createdDateTime</span></span>|<span data-ttu-id="338ea-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="338ea-153">DateTimeOffset</span></span>|<span data-ttu-id="338ea-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="338ea-154">The date and time the app was created.</span></span> <span data-ttu-id="338ea-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="338ea-156">lastModifiedDateTime</span></span>|<span data-ttu-id="338ea-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="338ea-157">DateTimeOffset</span></span>|<span data-ttu-id="338ea-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="338ea-158">The date and time the app was last modified.</span></span> <span data-ttu-id="338ea-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="338ea-160">isFeatured</span></span>|<span data-ttu-id="338ea-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="338ea-161">Boolean</span></span>|<span data-ttu-id="338ea-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="338ea-163">privacyInformationUrl</span></span>|<span data-ttu-id="338ea-164">String</span><span class="sxs-lookup"><span data-stu-id="338ea-164">String</span></span>|<span data-ttu-id="338ea-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="338ea-165">The privacy statement Url.</span></span> <span data-ttu-id="338ea-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="338ea-167">informationUrl</span></span>|<span data-ttu-id="338ea-168">String</span><span class="sxs-lookup"><span data-stu-id="338ea-168">String</span></span>|<span data-ttu-id="338ea-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="338ea-169">The more information Url.</span></span> <span data-ttu-id="338ea-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-171">owner</span><span class="sxs-lookup"><span data-stu-id="338ea-171">owner</span></span>|<span data-ttu-id="338ea-172">String</span><span class="sxs-lookup"><span data-stu-id="338ea-172">String</span></span>|<span data-ttu-id="338ea-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="338ea-173">The owner of the app.</span></span> <span data-ttu-id="338ea-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-175">developer</span><span class="sxs-lookup"><span data-stu-id="338ea-175">developer</span></span>|<span data-ttu-id="338ea-176">String</span><span class="sxs-lookup"><span data-stu-id="338ea-176">String</span></span>|<span data-ttu-id="338ea-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="338ea-177">The developer of the app.</span></span> <span data-ttu-id="338ea-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-179">notes</span><span class="sxs-lookup"><span data-stu-id="338ea-179">notes</span></span>|<span data-ttu-id="338ea-180">String</span><span class="sxs-lookup"><span data-stu-id="338ea-180">String</span></span>|<span data-ttu-id="338ea-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="338ea-181">Notes for the app.</span></span> <span data-ttu-id="338ea-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="338ea-183">uploadState</span></span>|<span data-ttu-id="338ea-184">Int32</span><span class="sxs-lookup"><span data-stu-id="338ea-184">Int32</span></span>|<span data-ttu-id="338ea-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="338ea-185">The upload state.</span></span> <span data-ttu-id="338ea-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="338ea-187">publishingState</span></span>|[<span data-ttu-id="338ea-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="338ea-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="338ea-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="338ea-189">The publishing state for the app.</span></span> <span data-ttu-id="338ea-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="338ea-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="338ea-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="338ea-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="338ea-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="338ea-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="338ea-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="338ea-193">isAssigned</span></span>|<span data-ttu-id="338ea-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="338ea-194">Boolean</span></span>|<span data-ttu-id="338ea-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="338ea-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="338ea-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="338ea-197">roleScopeTagIds</span></span>|<span data-ttu-id="338ea-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="338ea-198">String collection</span></span>|<span data-ttu-id="338ea-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="338ea-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="338ea-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="338ea-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="338ea-201">appAvailability</span></span>|[<span data-ttu-id="338ea-202">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="338ea-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="338ea-203">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="338ea-203">The Application's availability.</span></span> <span data-ttu-id="338ea-204">[managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="338ea-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="338ea-205">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="338ea-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="338ea-206">version</span><span class="sxs-lookup"><span data-stu-id="338ea-206">version</span></span>|<span data-ttu-id="338ea-207">String</span><span class="sxs-lookup"><span data-stu-id="338ea-207">String</span></span>|<span data-ttu-id="338ea-208">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="338ea-208">The Application's version.</span></span> <span data-ttu-id="338ea-209">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="338ea-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="338ea-210">committedContentVersion</span></span>|<span data-ttu-id="338ea-211">String</span><span class="sxs-lookup"><span data-stu-id="338ea-211">String</span></span>|<span data-ttu-id="338ea-212">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="338ea-212">The internal committed content version.</span></span> <span data-ttu-id="338ea-213">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="338ea-214">fileName</span><span class="sxs-lookup"><span data-stu-id="338ea-214">fileName</span></span>|<span data-ttu-id="338ea-215">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="338ea-215">String</span></span>|<span data-ttu-id="338ea-216">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="338ea-216">The name of the main Lob application file.</span></span> <span data-ttu-id="338ea-217">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="338ea-218">size</span><span class="sxs-lookup"><span data-stu-id="338ea-218">size</span></span>|<span data-ttu-id="338ea-219">Int64</span><span class="sxs-lookup"><span data-stu-id="338ea-219">Int64</span></span>|<span data-ttu-id="338ea-220">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="338ea-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="338ea-221">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="338ea-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="338ea-222">bundleId</span><span class="sxs-lookup"><span data-stu-id="338ea-222">bundleId</span></span>|<span data-ttu-id="338ea-223">String</span><span class="sxs-lookup"><span data-stu-id="338ea-223">String</span></span>|<span data-ttu-id="338ea-224">ID 名。</span><span class="sxs-lookup"><span data-stu-id="338ea-224">The Identity Name.</span></span>|
|<span data-ttu-id="338ea-225">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="338ea-225">applicableDeviceType</span></span>|[<span data-ttu-id="338ea-226">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="338ea-226">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="338ea-227">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="338ea-227">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="338ea-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="338ea-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="338ea-229">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="338ea-229">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="338ea-230">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="338ea-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="338ea-231">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="338ea-231">expirationDateTime</span></span>|<span data-ttu-id="338ea-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="338ea-232">DateTimeOffset</span></span>|<span data-ttu-id="338ea-233">有効期限。</span><span class="sxs-lookup"><span data-stu-id="338ea-233">The expiration time.</span></span>|
|<span data-ttu-id="338ea-234">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="338ea-234">versionNumber</span></span>|<span data-ttu-id="338ea-235">String</span><span class="sxs-lookup"><span data-stu-id="338ea-235">String</span></span>|<span data-ttu-id="338ea-236">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="338ea-236">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="338ea-237">buildNumber</span><span class="sxs-lookup"><span data-stu-id="338ea-237">buildNumber</span></span>|<span data-ttu-id="338ea-238">String</span><span class="sxs-lookup"><span data-stu-id="338ea-238">String</span></span>|<span data-ttu-id="338ea-239">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="338ea-239">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="338ea-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="338ea-240">identityVersion</span></span>|<span data-ttu-id="338ea-241">String</span><span class="sxs-lookup"><span data-stu-id="338ea-241">String</span></span>|<span data-ttu-id="338ea-242">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="338ea-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="338ea-243">応答</span><span class="sxs-lookup"><span data-stu-id="338ea-243">Response</span></span>
<span data-ttu-id="338ea-244">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="338ea-244">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="338ea-245">例</span><span class="sxs-lookup"><span data-stu-id="338ea-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="338ea-246">要求</span><span class="sxs-lookup"><span data-stu-id="338ea-246">Request</span></span>
<span data-ttu-id="338ea-247">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="338ea-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="338ea-248">応答</span><span class="sxs-lookup"><span data-stu-id="338ea-248">Response</span></span>
<span data-ttu-id="338ea-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="338ea-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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




