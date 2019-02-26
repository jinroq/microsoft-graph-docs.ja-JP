---
title: macoslobapp の作成
description: 新しい macoslobapp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74f700af2f4e748b44b265bb040c6529e882e84a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140804"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="4c131-103">macoslobapp の作成</span><span class="sxs-lookup"><span data-stu-id="4c131-103">Create macOSLobApp</span></span>

> <span data-ttu-id="4c131-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c131-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c131-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c131-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c131-106">新しい[macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c131-106">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c131-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c131-107">Prerequisites</span></span>
<span data-ttu-id="4c131-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c131-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c131-110">Permission type</span></span>|<span data-ttu-id="4c131-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c131-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c131-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c131-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c131-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c131-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c131-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c131-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c131-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c131-115">Not supported.</span></span>|
|<span data-ttu-id="4c131-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c131-116">Application</span></span>|<span data-ttu-id="4c131-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c131-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c131-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c131-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4c131-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c131-119">Request headers</span></span>
|<span data-ttu-id="4c131-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c131-120">Header</span></span>|<span data-ttu-id="4c131-121">値</span><span class="sxs-lookup"><span data-stu-id="4c131-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c131-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c131-122">Authorization</span></span>|<span data-ttu-id="4c131-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4c131-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c131-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c131-124">Accept</span></span>|<span data-ttu-id="4c131-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c131-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c131-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c131-126">Request body</span></span>
<span data-ttu-id="4c131-127">要求本文で、macoslobapp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c131-127">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="4c131-128">次の表に、macoslobapp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c131-128">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="4c131-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c131-129">Property</span></span>|<span data-ttu-id="4c131-130">型</span><span class="sxs-lookup"><span data-stu-id="4c131-130">Type</span></span>|<span data-ttu-id="4c131-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c131-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c131-132">id</span><span class="sxs-lookup"><span data-stu-id="4c131-132">id</span></span>|<span data-ttu-id="4c131-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4c131-133">String</span></span>|<span data-ttu-id="4c131-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c131-134">Key of the entity.</span></span> <span data-ttu-id="4c131-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4c131-136">displayName</span></span>|<span data-ttu-id="4c131-137">String</span><span class="sxs-lookup"><span data-stu-id="4c131-137">String</span></span>|<span data-ttu-id="4c131-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="4c131-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4c131-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-140">説明</span><span class="sxs-lookup"><span data-stu-id="4c131-140">description</span></span>|<span data-ttu-id="4c131-141">文字列</span><span class="sxs-lookup"><span data-stu-id="4c131-141">String</span></span>|<span data-ttu-id="4c131-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="4c131-142">The description of the app.</span></span> <span data-ttu-id="4c131-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4c131-144">publisher</span></span>|<span data-ttu-id="4c131-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4c131-145">String</span></span>|<span data-ttu-id="4c131-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="4c131-146">The publisher of the app.</span></span> <span data-ttu-id="4c131-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4c131-148">largeIcon</span></span>|[<span data-ttu-id="4c131-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4c131-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4c131-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="4c131-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4c131-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c131-152">createdDateTime</span></span>|<span data-ttu-id="4c131-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c131-153">DateTimeOffset</span></span>|<span data-ttu-id="4c131-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4c131-154">The date and time the app was created.</span></span> <span data-ttu-id="4c131-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c131-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4c131-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c131-157">DateTimeOffset</span></span>|<span data-ttu-id="4c131-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4c131-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4c131-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4c131-160">isFeatured</span></span>|<span data-ttu-id="4c131-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c131-161">Boolean</span></span>|<span data-ttu-id="4c131-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4c131-163">privacyInformationUrl</span></span>|<span data-ttu-id="4c131-164">String</span><span class="sxs-lookup"><span data-stu-id="4c131-164">String</span></span>|<span data-ttu-id="4c131-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="4c131-165">The privacy statement Url.</span></span> <span data-ttu-id="4c131-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4c131-167">informationUrl</span></span>|<span data-ttu-id="4c131-168">String</span><span class="sxs-lookup"><span data-stu-id="4c131-168">String</span></span>|<span data-ttu-id="4c131-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="4c131-169">The more information Url.</span></span> <span data-ttu-id="4c131-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-171">owner</span><span class="sxs-lookup"><span data-stu-id="4c131-171">owner</span></span>|<span data-ttu-id="4c131-172">String</span><span class="sxs-lookup"><span data-stu-id="4c131-172">String</span></span>|<span data-ttu-id="4c131-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="4c131-173">The owner of the app.</span></span> <span data-ttu-id="4c131-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-175">developer</span><span class="sxs-lookup"><span data-stu-id="4c131-175">developer</span></span>|<span data-ttu-id="4c131-176">String</span><span class="sxs-lookup"><span data-stu-id="4c131-176">String</span></span>|<span data-ttu-id="4c131-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="4c131-177">The developer of the app.</span></span> <span data-ttu-id="4c131-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-179">notes</span><span class="sxs-lookup"><span data-stu-id="4c131-179">notes</span></span>|<span data-ttu-id="4c131-180">String</span><span class="sxs-lookup"><span data-stu-id="4c131-180">String</span></span>|<span data-ttu-id="4c131-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="4c131-181">Notes for the app.</span></span> <span data-ttu-id="4c131-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4c131-183">uploadState</span></span>|<span data-ttu-id="4c131-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4c131-184">Int32</span></span>|<span data-ttu-id="4c131-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="4c131-185">The upload state.</span></span> <span data-ttu-id="4c131-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4c131-187">publishingState</span></span>|[<span data-ttu-id="4c131-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4c131-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4c131-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="4c131-189">The publishing state for the app.</span></span> <span data-ttu-id="4c131-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="4c131-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4c131-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c131-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4c131-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="4c131-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4c131-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4c131-193">isAssigned</span></span>|<span data-ttu-id="4c131-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c131-194">Boolean</span></span>|<span data-ttu-id="4c131-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="4c131-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4c131-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c131-197">roleScopeTagIds</span></span>|<span data-ttu-id="4c131-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4c131-198">String collection</span></span>|<span data-ttu-id="4c131-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="4c131-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4c131-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c131-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4c131-201">committedContentVersion</span></span>|<span data-ttu-id="4c131-202">String</span><span class="sxs-lookup"><span data-stu-id="4c131-202">String</span></span>|<span data-ttu-id="4c131-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4c131-203">The internal committed content version.</span></span> <span data-ttu-id="4c131-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4c131-205">fileName</span><span class="sxs-lookup"><span data-stu-id="4c131-205">fileName</span></span>|<span data-ttu-id="4c131-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4c131-206">String</span></span>|<span data-ttu-id="4c131-207">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="4c131-207">The name of the main Lob application file.</span></span> <span data-ttu-id="4c131-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4c131-209">size</span><span class="sxs-lookup"><span data-stu-id="4c131-209">size</span></span>|<span data-ttu-id="4c131-210">Int64</span><span class="sxs-lookup"><span data-stu-id="4c131-210">Int64</span></span>|<span data-ttu-id="4c131-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="4c131-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="4c131-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c131-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4c131-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="4c131-213">bundleId</span></span>|<span data-ttu-id="4c131-214">String</span><span class="sxs-lookup"><span data-stu-id="4c131-214">String</span></span>|<span data-ttu-id="4c131-215">バンドル id。</span><span class="sxs-lookup"><span data-stu-id="4c131-215">The bundle id.</span></span>|
|<span data-ttu-id="4c131-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c131-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4c131-217">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c131-217">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="4c131-218">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="4c131-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4c131-219">buildNumber</span><span class="sxs-lookup"><span data-stu-id="4c131-219">buildNumber</span></span>|<span data-ttu-id="4c131-220">String</span><span class="sxs-lookup"><span data-stu-id="4c131-220">String</span></span>|<span data-ttu-id="4c131-221">MacOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="4c131-221">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4c131-222">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="4c131-222">versionNumber</span></span>|<span data-ttu-id="4c131-223">String</span><span class="sxs-lookup"><span data-stu-id="4c131-223">String</span></span>|<span data-ttu-id="4c131-224">MacOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="4c131-224">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4c131-225">childapps</span><span class="sxs-lookup"><span data-stu-id="4c131-225">childApps</span></span>|<span data-ttu-id="4c131-226">[macoslobchildapp](../resources/intune-apps-macoslobchildapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c131-226">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="4c131-227">このバンドルパッケージのアプリリスト</span><span class="sxs-lookup"><span data-stu-id="4c131-227">The app list in this bundle package</span></span>|
|<span data-ttu-id="4c131-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4c131-228">identityVersion</span></span>|<span data-ttu-id="4c131-229">String</span><span class="sxs-lookup"><span data-stu-id="4c131-229">String</span></span>|<span data-ttu-id="4c131-230">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4c131-230">The identity version.</span></span>|
|<span data-ttu-id="4c131-231">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="4c131-231">md5HashChunkSize</span></span>|<span data-ttu-id="4c131-232">Int32</span><span class="sxs-lookup"><span data-stu-id="4c131-232">Int32</span></span>|<span data-ttu-id="4c131-233">MD5 ハッシュのチャンクサイズ</span><span class="sxs-lookup"><span data-stu-id="4c131-233">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="4c131-234">md5Hash</span><span class="sxs-lookup"><span data-stu-id="4c131-234">md5Hash</span></span>|<span data-ttu-id="4c131-235">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4c131-235">String collection</span></span>|<span data-ttu-id="4c131-236">MD5 ハッシュコード</span><span class="sxs-lookup"><span data-stu-id="4c131-236">The MD5 hash codes</span></span>|
|<span data-ttu-id="4c131-237">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="4c131-237">ignoreVersionDetection</span></span>|<span data-ttu-id="4c131-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c131-238">Boolean</span></span>|<span data-ttu-id="4c131-239">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="4c131-239">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="4c131-240">自己更新機能を使用する macOS 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c131-240">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="4c131-241">応答</span><span class="sxs-lookup"><span data-stu-id="4c131-241">Response</span></span>
<span data-ttu-id="4c131-242">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c131-242">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c131-243">例</span><span class="sxs-lookup"><span data-stu-id="4c131-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c131-244">要求</span><span class="sxs-lookup"><span data-stu-id="4c131-244">Request</span></span>
<span data-ttu-id="4c131-245">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c131-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1547

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="4c131-246">応答</span><span class="sxs-lookup"><span data-stu-id="4c131-246">Response</span></span>
<span data-ttu-id="4c131-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c131-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1719

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```




