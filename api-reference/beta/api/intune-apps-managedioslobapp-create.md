---
title: Create managedIOSLobApp
description: 新しい managedIOSLobApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e51887909019e6c42767e03cf44e275a364b60b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32493210"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="04bc2-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="04bc2-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="04bc2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04bc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04bc2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04bc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04bc2-106">新しい [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04bc2-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04bc2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="04bc2-107">Prerequisites</span></span>
<span data-ttu-id="04bc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04bc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04bc2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04bc2-110">Permission type</span></span>|<span data-ttu-id="04bc2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04bc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04bc2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04bc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04bc2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04bc2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04bc2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04bc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04bc2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04bc2-115">Not supported.</span></span>|
|<span data-ttu-id="04bc2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04bc2-116">Application</span></span>|<span data-ttu-id="04bc2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04bc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04bc2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04bc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="04bc2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04bc2-119">Request headers</span></span>
|<span data-ttu-id="04bc2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04bc2-120">Header</span></span>|<span data-ttu-id="04bc2-121">値</span><span class="sxs-lookup"><span data-stu-id="04bc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04bc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04bc2-122">Authorization</span></span>|<span data-ttu-id="04bc2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="04bc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04bc2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="04bc2-124">Accept</span></span>|<span data-ttu-id="04bc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04bc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04bc2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04bc2-126">Request body</span></span>
<span data-ttu-id="04bc2-127">要求本文で、managedIOSLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04bc2-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="04bc2-128">次の表に、managedDeviceOverview の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04bc2-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="04bc2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04bc2-129">Property</span></span>|<span data-ttu-id="04bc2-130">型</span><span class="sxs-lookup"><span data-stu-id="04bc2-130">Type</span></span>|<span data-ttu-id="04bc2-131">説明</span><span class="sxs-lookup"><span data-stu-id="04bc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04bc2-132">id</span><span class="sxs-lookup"><span data-stu-id="04bc2-132">id</span></span>|<span data-ttu-id="04bc2-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="04bc2-133">String</span></span>|<span data-ttu-id="04bc2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04bc2-134">Key of the entity.</span></span> <span data-ttu-id="04bc2-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="04bc2-136">displayName</span></span>|<span data-ttu-id="04bc2-137">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-137">String</span></span>|<span data-ttu-id="04bc2-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="04bc2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="04bc2-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-140">説明</span><span class="sxs-lookup"><span data-stu-id="04bc2-140">description</span></span>|<span data-ttu-id="04bc2-141">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-141">String</span></span>|<span data-ttu-id="04bc2-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="04bc2-142">The description of the app.</span></span> <span data-ttu-id="04bc2-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="04bc2-144">publisher</span></span>|<span data-ttu-id="04bc2-145">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-145">String</span></span>|<span data-ttu-id="04bc2-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="04bc2-146">The publisher of the app.</span></span> <span data-ttu-id="04bc2-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="04bc2-148">largeIcon</span></span>|[<span data-ttu-id="04bc2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="04bc2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="04bc2-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="04bc2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="04bc2-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04bc2-152">createdDateTime</span></span>|<span data-ttu-id="04bc2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04bc2-153">DateTimeOffset</span></span>|<span data-ttu-id="04bc2-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="04bc2-154">The date and time the app was created.</span></span> <span data-ttu-id="04bc2-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04bc2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="04bc2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04bc2-157">DateTimeOffset</span></span>|<span data-ttu-id="04bc2-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="04bc2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="04bc2-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="04bc2-160">isFeatured</span></span>|<span data-ttu-id="04bc2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="04bc2-161">Boolean</span></span>|<span data-ttu-id="04bc2-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="04bc2-163">privacyInformationUrl</span></span>|<span data-ttu-id="04bc2-164">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-164">String</span></span>|<span data-ttu-id="04bc2-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="04bc2-165">The privacy statement Url.</span></span> <span data-ttu-id="04bc2-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="04bc2-167">informationUrl</span></span>|<span data-ttu-id="04bc2-168">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-168">String</span></span>|<span data-ttu-id="04bc2-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="04bc2-169">The more information Url.</span></span> <span data-ttu-id="04bc2-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-171">owner</span><span class="sxs-lookup"><span data-stu-id="04bc2-171">owner</span></span>|<span data-ttu-id="04bc2-172">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-172">String</span></span>|<span data-ttu-id="04bc2-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="04bc2-173">The owner of the app.</span></span> <span data-ttu-id="04bc2-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-175">developer</span><span class="sxs-lookup"><span data-stu-id="04bc2-175">developer</span></span>|<span data-ttu-id="04bc2-176">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-176">String</span></span>|<span data-ttu-id="04bc2-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="04bc2-177">The developer of the app.</span></span> <span data-ttu-id="04bc2-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-179">notes</span><span class="sxs-lookup"><span data-stu-id="04bc2-179">notes</span></span>|<span data-ttu-id="04bc2-180">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-180">String</span></span>|<span data-ttu-id="04bc2-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="04bc2-181">Notes for the app.</span></span> <span data-ttu-id="04bc2-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="04bc2-183">uploadState</span></span>|<span data-ttu-id="04bc2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="04bc2-184">Int32</span></span>|<span data-ttu-id="04bc2-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="04bc2-185">The upload state.</span></span> <span data-ttu-id="04bc2-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="04bc2-187">publishingState</span></span>|[<span data-ttu-id="04bc2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="04bc2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="04bc2-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="04bc2-189">The publishing state for the app.</span></span> <span data-ttu-id="04bc2-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="04bc2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="04bc2-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04bc2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="04bc2-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="04bc2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="04bc2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="04bc2-193">isAssigned</span></span>|<span data-ttu-id="04bc2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="04bc2-194">Boolean</span></span>|<span data-ttu-id="04bc2-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="04bc2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="04bc2-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04bc2-197">roleScopeTagIds</span></span>|<span data-ttu-id="04bc2-198">String collection</span><span class="sxs-lookup"><span data-stu-id="04bc2-198">String collection</span></span>|<span data-ttu-id="04bc2-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="04bc2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="04bc2-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="04bc2-201">dependentAppCount</span></span>|<span data-ttu-id="04bc2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="04bc2-202">Int32</span></span>|<span data-ttu-id="04bc2-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="04bc2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="04bc2-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="04bc2-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="04bc2-205">appAvailability</span></span>|[<span data-ttu-id="04bc2-206">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="04bc2-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="04bc2-207">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="04bc2-207">The Application's availability.</span></span> <span data-ttu-id="04bc2-208">[managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04bc2-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="04bc2-209">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="04bc2-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="04bc2-210">version</span><span class="sxs-lookup"><span data-stu-id="04bc2-210">version</span></span>|<span data-ttu-id="04bc2-211">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-211">String</span></span>|<span data-ttu-id="04bc2-212">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="04bc2-212">The Application's version.</span></span> <span data-ttu-id="04bc2-213">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="04bc2-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="04bc2-214">committedContentVersion</span></span>|<span data-ttu-id="04bc2-215">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-215">String</span></span>|<span data-ttu-id="04bc2-216">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="04bc2-216">The internal committed content version.</span></span> <span data-ttu-id="04bc2-217">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="04bc2-218">fileName</span><span class="sxs-lookup"><span data-stu-id="04bc2-218">fileName</span></span>|<span data-ttu-id="04bc2-219">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-219">String</span></span>|<span data-ttu-id="04bc2-220">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="04bc2-220">The name of the main Lob application file.</span></span> <span data-ttu-id="04bc2-221">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="04bc2-222">size</span><span class="sxs-lookup"><span data-stu-id="04bc2-222">size</span></span>|<span data-ttu-id="04bc2-223">Int64</span><span class="sxs-lookup"><span data-stu-id="04bc2-223">Int64</span></span>|<span data-ttu-id="04bc2-224">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="04bc2-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="04bc2-225">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04bc2-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="04bc2-226">bundleId</span><span class="sxs-lookup"><span data-stu-id="04bc2-226">bundleId</span></span>|<span data-ttu-id="04bc2-227">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="04bc2-227">String</span></span>|<span data-ttu-id="04bc2-228">ID 名。</span><span class="sxs-lookup"><span data-stu-id="04bc2-228">The Identity Name.</span></span>|
|<span data-ttu-id="04bc2-229">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="04bc2-229">applicableDeviceType</span></span>|[<span data-ttu-id="04bc2-230">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="04bc2-230">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="04bc2-231">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="04bc2-231">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="04bc2-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04bc2-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="04bc2-233">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04bc2-233">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="04bc2-234">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="04bc2-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="04bc2-235">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="04bc2-235">expirationDateTime</span></span>|<span data-ttu-id="04bc2-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04bc2-236">DateTimeOffset</span></span>|<span data-ttu-id="04bc2-237">有効期限。</span><span class="sxs-lookup"><span data-stu-id="04bc2-237">The expiration time.</span></span>|
|<span data-ttu-id="04bc2-238">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="04bc2-238">versionNumber</span></span>|<span data-ttu-id="04bc2-239">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-239">String</span></span>|<span data-ttu-id="04bc2-240">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="04bc2-240">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04bc2-241">buildNumber</span><span class="sxs-lookup"><span data-stu-id="04bc2-241">buildNumber</span></span>|<span data-ttu-id="04bc2-242">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-242">String</span></span>|<span data-ttu-id="04bc2-243">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="04bc2-243">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04bc2-244">identityVersion</span><span class="sxs-lookup"><span data-stu-id="04bc2-244">identityVersion</span></span>|<span data-ttu-id="04bc2-245">String</span><span class="sxs-lookup"><span data-stu-id="04bc2-245">String</span></span>|<span data-ttu-id="04bc2-246">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="04bc2-246">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="04bc2-247">応答</span><span class="sxs-lookup"><span data-stu-id="04bc2-247">Response</span></span>
<span data-ttu-id="04bc2-248">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04bc2-248">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04bc2-249">例</span><span class="sxs-lookup"><span data-stu-id="04bc2-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="04bc2-250">要求</span><span class="sxs-lookup"><span data-stu-id="04bc2-250">Request</span></span>
<span data-ttu-id="04bc2-251">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04bc2-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1469

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="04bc2-252">応答</span><span class="sxs-lookup"><span data-stu-id="04bc2-252">Response</span></span>
<span data-ttu-id="04bc2-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04bc2-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1641

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
  "dependentAppCount": 1,
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





