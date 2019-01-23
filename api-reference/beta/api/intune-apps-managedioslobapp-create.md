---
title: Create managedIOSLobApp
description: 新しい managedIOSLobApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ae2e7e362881731122b1a9f783d378c3f0ff5a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409056"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="78935-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="78935-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="78935-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78935-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78935-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78935-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78935-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78935-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78935-107">新しい [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="78935-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78935-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="78935-108">Prerequisites</span></span>
<span data-ttu-id="78935-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78935-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="78935-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78935-111">Permission type</span></span>|<span data-ttu-id="78935-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78935-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78935-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78935-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78935-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78935-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78935-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78935-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78935-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78935-116">Not supported.</span></span>|
|<span data-ttu-id="78935-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78935-117">Application</span></span>|<span data-ttu-id="78935-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78935-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78935-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78935-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="78935-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78935-120">Request headers</span></span>
|<span data-ttu-id="78935-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78935-121">Header</span></span>|<span data-ttu-id="78935-122">値</span><span class="sxs-lookup"><span data-stu-id="78935-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78935-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78935-123">Authorization</span></span>|<span data-ttu-id="78935-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="78935-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78935-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78935-125">Accept</span></span>|<span data-ttu-id="78935-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78935-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78935-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="78935-127">Request body</span></span>
<span data-ttu-id="78935-128">要求本文で、managedIOSLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78935-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="78935-129">次の表に、managedDeviceOverview の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78935-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="78935-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78935-130">Property</span></span>|<span data-ttu-id="78935-131">型</span><span class="sxs-lookup"><span data-stu-id="78935-131">Type</span></span>|<span data-ttu-id="78935-132">説明</span><span class="sxs-lookup"><span data-stu-id="78935-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78935-133">id</span><span class="sxs-lookup"><span data-stu-id="78935-133">id</span></span>|<span data-ttu-id="78935-134">String</span><span class="sxs-lookup"><span data-stu-id="78935-134">String</span></span>|<span data-ttu-id="78935-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78935-135">Key of the entity.</span></span> <span data-ttu-id="78935-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-137">displayName</span><span class="sxs-lookup"><span data-stu-id="78935-137">displayName</span></span>|<span data-ttu-id="78935-138">String</span><span class="sxs-lookup"><span data-stu-id="78935-138">String</span></span>|<span data-ttu-id="78935-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="78935-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="78935-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-141">説明</span><span class="sxs-lookup"><span data-stu-id="78935-141">description</span></span>|<span data-ttu-id="78935-142">String</span><span class="sxs-lookup"><span data-stu-id="78935-142">String</span></span>|<span data-ttu-id="78935-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="78935-143">The description of the app.</span></span> <span data-ttu-id="78935-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-145">publisher</span><span class="sxs-lookup"><span data-stu-id="78935-145">publisher</span></span>|<span data-ttu-id="78935-146">String</span><span class="sxs-lookup"><span data-stu-id="78935-146">String</span></span>|<span data-ttu-id="78935-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="78935-147">The publisher of the app.</span></span> <span data-ttu-id="78935-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="78935-149">largeIcon</span></span>|[<span data-ttu-id="78935-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78935-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="78935-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="78935-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="78935-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78935-153">createdDateTime</span></span>|<span data-ttu-id="78935-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78935-154">DateTimeOffset</span></span>|<span data-ttu-id="78935-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="78935-155">The date and time the app was created.</span></span> <span data-ttu-id="78935-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78935-157">lastModifiedDateTime</span></span>|<span data-ttu-id="78935-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78935-158">DateTimeOffset</span></span>|<span data-ttu-id="78935-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="78935-159">The date and time the app was last modified.</span></span> <span data-ttu-id="78935-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="78935-161">isFeatured</span></span>|<span data-ttu-id="78935-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="78935-162">Boolean</span></span>|<span data-ttu-id="78935-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="78935-164">privacyInformationUrl</span></span>|<span data-ttu-id="78935-165">String</span><span class="sxs-lookup"><span data-stu-id="78935-165">String</span></span>|<span data-ttu-id="78935-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="78935-166">The privacy statement Url.</span></span> <span data-ttu-id="78935-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="78935-168">informationUrl</span></span>|<span data-ttu-id="78935-169">String</span><span class="sxs-lookup"><span data-stu-id="78935-169">String</span></span>|<span data-ttu-id="78935-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="78935-170">The more information Url.</span></span> <span data-ttu-id="78935-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-172">owner</span><span class="sxs-lookup"><span data-stu-id="78935-172">owner</span></span>|<span data-ttu-id="78935-173">String</span><span class="sxs-lookup"><span data-stu-id="78935-173">String</span></span>|<span data-ttu-id="78935-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="78935-174">The owner of the app.</span></span> <span data-ttu-id="78935-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-176">developer</span><span class="sxs-lookup"><span data-stu-id="78935-176">developer</span></span>|<span data-ttu-id="78935-177">String</span><span class="sxs-lookup"><span data-stu-id="78935-177">String</span></span>|<span data-ttu-id="78935-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="78935-178">The developer of the app.</span></span> <span data-ttu-id="78935-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-180">notes</span><span class="sxs-lookup"><span data-stu-id="78935-180">notes</span></span>|<span data-ttu-id="78935-181">String</span><span class="sxs-lookup"><span data-stu-id="78935-181">String</span></span>|<span data-ttu-id="78935-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="78935-182">Notes for the app.</span></span> <span data-ttu-id="78935-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="78935-184">uploadState</span></span>|<span data-ttu-id="78935-185">Int32</span><span class="sxs-lookup"><span data-stu-id="78935-185">Int32</span></span>|<span data-ttu-id="78935-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="78935-186">The upload state.</span></span> <span data-ttu-id="78935-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="78935-188">publishingState</span></span>|[<span data-ttu-id="78935-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="78935-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="78935-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="78935-190">The publishing state for the app.</span></span> <span data-ttu-id="78935-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="78935-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="78935-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="78935-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="78935-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="78935-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="78935-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="78935-194">isAssigned</span></span>|<span data-ttu-id="78935-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="78935-195">Boolean</span></span>|<span data-ttu-id="78935-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="78935-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="78935-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78935-198">roleScopeTagIds</span></span>|<span data-ttu-id="78935-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="78935-199">String collection</span></span>|<span data-ttu-id="78935-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="78935-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="78935-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="78935-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="78935-202">appAvailability</span></span>|[<span data-ttu-id="78935-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="78935-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="78935-204">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="78935-204">The Application's availability.</span></span> <span data-ttu-id="78935-205">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="78935-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="78935-206">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="78935-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="78935-207">version</span><span class="sxs-lookup"><span data-stu-id="78935-207">version</span></span>|<span data-ttu-id="78935-208">String</span><span class="sxs-lookup"><span data-stu-id="78935-208">String</span></span>|<span data-ttu-id="78935-209">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="78935-209">The Application's version.</span></span> <span data-ttu-id="78935-210">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="78935-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="78935-211">committedContentVersion</span></span>|<span data-ttu-id="78935-212">String</span><span class="sxs-lookup"><span data-stu-id="78935-212">String</span></span>|<span data-ttu-id="78935-213">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="78935-213">The internal committed content version.</span></span> <span data-ttu-id="78935-214">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="78935-215">fileName</span><span class="sxs-lookup"><span data-stu-id="78935-215">fileName</span></span>|<span data-ttu-id="78935-216">String</span><span class="sxs-lookup"><span data-stu-id="78935-216">String</span></span>|<span data-ttu-id="78935-217">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="78935-217">The name of the main Lob application file.</span></span> <span data-ttu-id="78935-218">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="78935-219">size</span><span class="sxs-lookup"><span data-stu-id="78935-219">size</span></span>|<span data-ttu-id="78935-220">Int64</span><span class="sxs-lookup"><span data-stu-id="78935-220">Int64</span></span>|<span data-ttu-id="78935-221">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="78935-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="78935-222">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="78935-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="78935-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="78935-223">bundleId</span></span>|<span data-ttu-id="78935-224">String</span><span class="sxs-lookup"><span data-stu-id="78935-224">String</span></span>|<span data-ttu-id="78935-225">ID 名。</span><span class="sxs-lookup"><span data-stu-id="78935-225">The Identity Name.</span></span>|
|<span data-ttu-id="78935-226">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="78935-226">applicableDeviceType</span></span>|[<span data-ttu-id="78935-227">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="78935-227">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="78935-228">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="78935-228">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="78935-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78935-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="78935-230">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78935-230">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="78935-231">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="78935-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="78935-232">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78935-232">expirationDateTime</span></span>|<span data-ttu-id="78935-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78935-233">DateTimeOffset</span></span>|<span data-ttu-id="78935-234">有効期限。</span><span class="sxs-lookup"><span data-stu-id="78935-234">The expiration time.</span></span>|
|<span data-ttu-id="78935-235">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="78935-235">versionNumber</span></span>|<span data-ttu-id="78935-236">String</span><span class="sxs-lookup"><span data-stu-id="78935-236">String</span></span>|<span data-ttu-id="78935-237">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="78935-237">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="78935-238">buildNumber</span><span class="sxs-lookup"><span data-stu-id="78935-238">buildNumber</span></span>|<span data-ttu-id="78935-239">String</span><span class="sxs-lookup"><span data-stu-id="78935-239">String</span></span>|<span data-ttu-id="78935-240">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="78935-240">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="78935-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="78935-241">identityVersion</span></span>|<span data-ttu-id="78935-242">String</span><span class="sxs-lookup"><span data-stu-id="78935-242">String</span></span>|<span data-ttu-id="78935-243">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="78935-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="78935-244">応答</span><span class="sxs-lookup"><span data-stu-id="78935-244">Response</span></span>
<span data-ttu-id="78935-245">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78935-245">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78935-246">例</span><span class="sxs-lookup"><span data-stu-id="78935-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="78935-247">要求</span><span class="sxs-lookup"><span data-stu-id="78935-247">Request</span></span>
<span data-ttu-id="78935-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78935-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78935-249">応答</span><span class="sxs-lookup"><span data-stu-id="78935-249">Response</span></span>
<span data-ttu-id="78935-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78935-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




