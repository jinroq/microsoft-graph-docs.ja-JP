---
title: WindowsAppX の更新
description: WindowsAppX オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3182cb6e5e74b64431f848eaab12f1f0ecdcda
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973202"
---
# <a name="update-windowsappx"></a><span data-ttu-id="3b66b-103">WindowsAppX の更新</span><span class="sxs-lookup"><span data-stu-id="3b66b-103">Update windowsAppX</span></span>

> <span data-ttu-id="3b66b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b66b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b66b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b66b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b66b-106">[Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b66b-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b66b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b66b-107">Prerequisites</span></span>
<span data-ttu-id="3b66b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b66b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b66b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b66b-110">Permission type</span></span>|<span data-ttu-id="3b66b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b66b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b66b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b66b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b66b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b66b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b66b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b66b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b66b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b66b-115">Not supported.</span></span>|
|<span data-ttu-id="3b66b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b66b-116">Application</span></span>|<span data-ttu-id="3b66b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b66b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b66b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b66b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3b66b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b66b-119">Request headers</span></span>
|<span data-ttu-id="3b66b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b66b-120">Header</span></span>|<span data-ttu-id="3b66b-121">値</span><span class="sxs-lookup"><span data-stu-id="3b66b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b66b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b66b-122">Authorization</span></span>|<span data-ttu-id="3b66b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b66b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b66b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3b66b-124">Accept</span></span>|<span data-ttu-id="3b66b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b66b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b66b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b66b-126">Request body</span></span>
<span data-ttu-id="3b66b-127">要求本文で、 [Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3b66b-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="3b66b-128">次の表に、 [Windowsappx](../resources/intune-apps-windowsappx.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3b66b-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="3b66b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b66b-129">Property</span></span>|<span data-ttu-id="3b66b-130">型</span><span class="sxs-lookup"><span data-stu-id="3b66b-130">Type</span></span>|<span data-ttu-id="3b66b-131">説明</span><span class="sxs-lookup"><span data-stu-id="3b66b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b66b-132">id</span><span class="sxs-lookup"><span data-stu-id="3b66b-132">id</span></span>|<span data-ttu-id="3b66b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3b66b-133">String</span></span>|<span data-ttu-id="3b66b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3b66b-134">Key of the entity.</span></span> <span data-ttu-id="3b66b-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3b66b-136">displayName</span></span>|<span data-ttu-id="3b66b-137">文字列</span><span class="sxs-lookup"><span data-stu-id="3b66b-137">String</span></span>|<span data-ttu-id="3b66b-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="3b66b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b66b-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-140">description</span><span class="sxs-lookup"><span data-stu-id="3b66b-140">description</span></span>|<span data-ttu-id="3b66b-141">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-141">String</span></span>|<span data-ttu-id="3b66b-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="3b66b-142">The description of the app.</span></span> <span data-ttu-id="3b66b-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3b66b-144">publisher</span></span>|<span data-ttu-id="3b66b-145">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-145">String</span></span>|<span data-ttu-id="3b66b-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="3b66b-146">The publisher of the app.</span></span> <span data-ttu-id="3b66b-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b66b-148">largeIcon</span></span>|[<span data-ttu-id="3b66b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b66b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b66b-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="3b66b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b66b-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b66b-152">createdDateTime</span></span>|<span data-ttu-id="3b66b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b66b-153">DateTimeOffset</span></span>|<span data-ttu-id="3b66b-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="3b66b-154">The date and time the app was created.</span></span> <span data-ttu-id="3b66b-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b66b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3b66b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b66b-157">DateTimeOffset</span></span>|<span data-ttu-id="3b66b-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="3b66b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3b66b-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b66b-160">isFeatured</span></span>|<span data-ttu-id="3b66b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b66b-161">Boolean</span></span>|<span data-ttu-id="3b66b-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b66b-163">privacyInformationUrl</span></span>|<span data-ttu-id="3b66b-164">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-164">String</span></span>|<span data-ttu-id="3b66b-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="3b66b-165">The privacy statement Url.</span></span> <span data-ttu-id="3b66b-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b66b-167">informationUrl</span></span>|<span data-ttu-id="3b66b-168">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-168">String</span></span>|<span data-ttu-id="3b66b-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="3b66b-169">The more information Url.</span></span> <span data-ttu-id="3b66b-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-171">owner</span><span class="sxs-lookup"><span data-stu-id="3b66b-171">owner</span></span>|<span data-ttu-id="3b66b-172">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-172">String</span></span>|<span data-ttu-id="3b66b-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="3b66b-173">The owner of the app.</span></span> <span data-ttu-id="3b66b-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-175">developer</span><span class="sxs-lookup"><span data-stu-id="3b66b-175">developer</span></span>|<span data-ttu-id="3b66b-176">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-176">String</span></span>|<span data-ttu-id="3b66b-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="3b66b-177">The developer of the app.</span></span> <span data-ttu-id="3b66b-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-179">notes</span><span class="sxs-lookup"><span data-stu-id="3b66b-179">notes</span></span>|<span data-ttu-id="3b66b-180">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-180">String</span></span>|<span data-ttu-id="3b66b-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="3b66b-181">Notes for the app.</span></span> <span data-ttu-id="3b66b-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3b66b-183">uploadState</span></span>|<span data-ttu-id="3b66b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66b-184">Int32</span></span>|<span data-ttu-id="3b66b-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="3b66b-185">The upload state.</span></span> <span data-ttu-id="3b66b-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b66b-187">publishingState</span></span>|[<span data-ttu-id="3b66b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3b66b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3b66b-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="3b66b-189">The publishing state for the app.</span></span> <span data-ttu-id="3b66b-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="3b66b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b66b-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3b66b-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3b66b-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="3b66b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3b66b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3b66b-193">isAssigned</span></span>|<span data-ttu-id="3b66b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b66b-194">Boolean</span></span>|<span data-ttu-id="3b66b-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="3b66b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3b66b-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b66b-197">roleScopeTagIds</span></span>|<span data-ttu-id="3b66b-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3b66b-198">String collection</span></span>|<span data-ttu-id="3b66b-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="3b66b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3b66b-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="3b66b-201">dependentAppCount</span></span>|<span data-ttu-id="3b66b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66b-202">Int32</span></span>|<span data-ttu-id="3b66b-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="3b66b-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3b66b-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b66b-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3b66b-205">committedContentVersion</span></span>|<span data-ttu-id="3b66b-206">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-206">String</span></span>|<span data-ttu-id="3b66b-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3b66b-207">The internal committed content version.</span></span> <span data-ttu-id="3b66b-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3b66b-209">fileName</span><span class="sxs-lookup"><span data-stu-id="3b66b-209">fileName</span></span>|<span data-ttu-id="3b66b-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3b66b-210">String</span></span>|<span data-ttu-id="3b66b-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="3b66b-211">The name of the main Lob application file.</span></span> <span data-ttu-id="3b66b-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3b66b-213">size</span><span class="sxs-lookup"><span data-stu-id="3b66b-213">size</span></span>|<span data-ttu-id="3b66b-214">Int64</span><span class="sxs-lookup"><span data-stu-id="3b66b-214">Int64</span></span>|<span data-ttu-id="3b66b-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="3b66b-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="3b66b-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3b66b-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3b66b-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="3b66b-217">applicableArchitectures</span></span>|[<span data-ttu-id="3b66b-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="3b66b-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="3b66b-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="3b66b-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="3b66b-220">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="3b66b-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="3b66b-221">identityName</span><span class="sxs-lookup"><span data-stu-id="3b66b-221">identityName</span></span>|<span data-ttu-id="3b66b-222">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-222">String</span></span>|<span data-ttu-id="3b66b-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="3b66b-223">The Identity Name.</span></span>|
|<span data-ttu-id="3b66b-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="3b66b-224">identityPublisherHash</span></span>|<span data-ttu-id="3b66b-225">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-225">String</span></span>|<span data-ttu-id="3b66b-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="3b66b-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="3b66b-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3b66b-227">identityResourceIdentifier</span></span>|<span data-ttu-id="3b66b-228">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-228">String</span></span>|<span data-ttu-id="3b66b-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="3b66b-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="3b66b-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="3b66b-230">isBundle</span></span>|<span data-ttu-id="3b66b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b66b-231">Boolean</span></span>|<span data-ttu-id="3b66b-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3b66b-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="3b66b-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b66b-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3b66b-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b66b-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="3b66b-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="3b66b-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3b66b-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3b66b-236">identityVersion</span></span>|<span data-ttu-id="3b66b-237">String</span><span class="sxs-lookup"><span data-stu-id="3b66b-237">String</span></span>|<span data-ttu-id="3b66b-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3b66b-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3b66b-239">応答</span><span class="sxs-lookup"><span data-stu-id="3b66b-239">Response</span></span>
<span data-ttu-id="3b66b-240">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b66b-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b66b-241">例</span><span class="sxs-lookup"><span data-stu-id="3b66b-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b66b-242">要求</span><span class="sxs-lookup"><span data-stu-id="3b66b-242">Request</span></span>
<span data-ttu-id="3b66b-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b66b-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="3b66b-244">応答</span><span class="sxs-lookup"><span data-stu-id="3b66b-244">Response</span></span>
<span data-ttu-id="3b66b-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b66b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```





