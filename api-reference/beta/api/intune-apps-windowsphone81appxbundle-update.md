---
title: WindowsPhone81AppXBundle の更新
description: WindowsPhone81AppXBundle オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69fd1b46a7eb1b308189153c707d3e9f834b03dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934573"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="0c8e6-103">WindowsPhone81AppXBundle の更新</span><span class="sxs-lookup"><span data-stu-id="0c8e6-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="0c8e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c8e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c8e6-106">[WindowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c8e6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c8e6-107">Prerequisites</span></span>
<span data-ttu-id="0c8e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8e6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c8e6-110">Permission type</span></span>|<span data-ttu-id="0c8e6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c8e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c8e6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c8e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c8e6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8e6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c8e6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c8e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c8e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-115">Not supported.</span></span>|
|<span data-ttu-id="0c8e6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c8e6-116">Application</span></span>|<span data-ttu-id="0c8e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c8e6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0c8e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c8e6-119">Request headers</span></span>
|<span data-ttu-id="0c8e6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c8e6-120">Header</span></span>|<span data-ttu-id="0c8e6-121">値</span><span class="sxs-lookup"><span data-stu-id="0c8e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c8e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c8e6-122">Authorization</span></span>|<span data-ttu-id="0c8e6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c8e6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0c8e6-124">Accept</span></span>|<span data-ttu-id="0c8e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c8e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c8e6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c8e6-126">Request body</span></span>
<span data-ttu-id="0c8e6-127">要求本文で、 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="0c8e6-128">次の表に、 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="0c8e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c8e6-129">Property</span></span>|<span data-ttu-id="0c8e6-130">型</span><span class="sxs-lookup"><span data-stu-id="0c8e6-130">Type</span></span>|<span data-ttu-id="0c8e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="0c8e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c8e6-132">id</span><span class="sxs-lookup"><span data-stu-id="0c8e6-132">id</span></span>|<span data-ttu-id="0c8e6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0c8e6-133">String</span></span>|<span data-ttu-id="0c8e6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-134">Key of the entity.</span></span> <span data-ttu-id="0c8e6-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c8e6-136">displayName</span></span>|<span data-ttu-id="0c8e6-137">文字列</span><span class="sxs-lookup"><span data-stu-id="0c8e6-137">String</span></span>|<span data-ttu-id="0c8e6-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0c8e6-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-140">description</span><span class="sxs-lookup"><span data-stu-id="0c8e6-140">description</span></span>|<span data-ttu-id="0c8e6-141">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-141">String</span></span>|<span data-ttu-id="0c8e6-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-142">The description of the app.</span></span> <span data-ttu-id="0c8e6-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0c8e6-144">publisher</span></span>|<span data-ttu-id="0c8e6-145">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-145">String</span></span>|<span data-ttu-id="0c8e6-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-146">The publisher of the app.</span></span> <span data-ttu-id="0c8e6-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0c8e6-148">largeIcon</span></span>|[<span data-ttu-id="0c8e6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0c8e6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0c8e6-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0c8e6-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c8e6-152">createdDateTime</span></span>|<span data-ttu-id="0c8e6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c8e6-153">DateTimeOffset</span></span>|<span data-ttu-id="0c8e6-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-154">The date and time the app was created.</span></span> <span data-ttu-id="0c8e6-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c8e6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0c8e6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c8e6-157">DateTimeOffset</span></span>|<span data-ttu-id="0c8e6-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0c8e6-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0c8e6-160">isFeatured</span></span>|<span data-ttu-id="0c8e6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c8e6-161">Boolean</span></span>|<span data-ttu-id="0c8e6-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0c8e6-163">privacyInformationUrl</span></span>|<span data-ttu-id="0c8e6-164">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-164">String</span></span>|<span data-ttu-id="0c8e6-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-165">The privacy statement Url.</span></span> <span data-ttu-id="0c8e6-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0c8e6-167">informationUrl</span></span>|<span data-ttu-id="0c8e6-168">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-168">String</span></span>|<span data-ttu-id="0c8e6-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-169">The more information Url.</span></span> <span data-ttu-id="0c8e6-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-171">owner</span><span class="sxs-lookup"><span data-stu-id="0c8e6-171">owner</span></span>|<span data-ttu-id="0c8e6-172">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-172">String</span></span>|<span data-ttu-id="0c8e6-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-173">The owner of the app.</span></span> <span data-ttu-id="0c8e6-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-175">developer</span><span class="sxs-lookup"><span data-stu-id="0c8e6-175">developer</span></span>|<span data-ttu-id="0c8e6-176">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-176">String</span></span>|<span data-ttu-id="0c8e6-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-177">The developer of the app.</span></span> <span data-ttu-id="0c8e6-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-179">notes</span><span class="sxs-lookup"><span data-stu-id="0c8e6-179">notes</span></span>|<span data-ttu-id="0c8e6-180">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-180">String</span></span>|<span data-ttu-id="0c8e6-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-181">Notes for the app.</span></span> <span data-ttu-id="0c8e6-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0c8e6-183">uploadState</span></span>|<span data-ttu-id="0c8e6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0c8e6-184">Int32</span></span>|<span data-ttu-id="0c8e6-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-185">The upload state.</span></span> <span data-ttu-id="0c8e6-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0c8e6-187">publishingState</span></span>|[<span data-ttu-id="0c8e6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0c8e6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0c8e6-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-189">The publishing state for the app.</span></span> <span data-ttu-id="0c8e6-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0c8e6-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0c8e6-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0c8e6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0c8e6-193">isAssigned</span></span>|<span data-ttu-id="0c8e6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c8e6-194">Boolean</span></span>|<span data-ttu-id="0c8e6-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0c8e6-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c8e6-197">roleScopeTagIds</span></span>|<span data-ttu-id="0c8e6-198">String collection</span><span class="sxs-lookup"><span data-stu-id="0c8e6-198">String collection</span></span>|<span data-ttu-id="0c8e6-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0c8e6-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0c8e6-201">dependentAppCount</span></span>|<span data-ttu-id="0c8e6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0c8e6-202">Int32</span></span>|<span data-ttu-id="0c8e6-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0c8e6-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c8e6-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0c8e6-205">committedContentVersion</span></span>|<span data-ttu-id="0c8e6-206">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-206">String</span></span>|<span data-ttu-id="0c8e6-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-207">The internal committed content version.</span></span> <span data-ttu-id="0c8e6-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0c8e6-209">fileName</span><span class="sxs-lookup"><span data-stu-id="0c8e6-209">fileName</span></span>|<span data-ttu-id="0c8e6-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0c8e6-210">String</span></span>|<span data-ttu-id="0c8e6-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-211">The name of the main Lob application file.</span></span> <span data-ttu-id="0c8e6-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0c8e6-213">size</span><span class="sxs-lookup"><span data-stu-id="0c8e6-213">size</span></span>|<span data-ttu-id="0c8e6-214">Int64</span><span class="sxs-lookup"><span data-stu-id="0c8e6-214">Int64</span></span>|<span data-ttu-id="0c8e6-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="0c8e6-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c8e6-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0c8e6-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="0c8e6-217">applicableArchitectures</span></span>|[<span data-ttu-id="0c8e6-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0c8e6-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0c8e6-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="0c8e6-220">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="0c8e6-221">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="0c8e6-222">identityName</span><span class="sxs-lookup"><span data-stu-id="0c8e6-222">identityName</span></span>|<span data-ttu-id="0c8e6-223">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-223">String</span></span>|<span data-ttu-id="0c8e6-224">ID 名。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-224">The Identity Name.</span></span> <span data-ttu-id="0c8e6-225">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="0c8e6-226">identityPublisherHash</span></span>|<span data-ttu-id="0c8e6-227">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-227">String</span></span>|<span data-ttu-id="0c8e6-228">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="0c8e6-229">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c8e6-230">identityResourceIdentifier</span></span>|<span data-ttu-id="0c8e6-231">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-231">String</span></span>|<span data-ttu-id="0c8e6-232">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="0c8e6-233">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c8e6-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0c8e6-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c8e6-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0c8e6-236">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="0c8e6-237">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c8e6-238">phoneProductIdentifier</span></span>|<span data-ttu-id="0c8e6-239">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-239">String</span></span>|<span data-ttu-id="0c8e6-240">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-240">The Phone Product Identifier.</span></span> <span data-ttu-id="0c8e6-241">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="0c8e6-242">phonePublisherId</span></span>|<span data-ttu-id="0c8e6-243">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-243">String</span></span>|<span data-ttu-id="0c8e6-244">電話の発行元 Id。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0c8e6-245">identityVersion</span></span>|<span data-ttu-id="0c8e6-246">String</span><span class="sxs-lookup"><span data-stu-id="0c8e6-246">String</span></span>|<span data-ttu-id="0c8e6-247">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-247">The identity version.</span></span> <span data-ttu-id="0c8e6-248">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0c8e6-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="0c8e6-249">appXPackageInformationList</span></span>|<span data-ttu-id="0c8e6-250">[Windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c8e6-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="0c8e6-251">AppX パッケージ情報のリスト。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="0c8e6-252">応答</span><span class="sxs-lookup"><span data-stu-id="0c8e6-252">Response</span></span>
<span data-ttu-id="0c8e6-253">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c8e6-254">例</span><span class="sxs-lookup"><span data-stu-id="0c8e6-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c8e6-255">要求</span><span class="sxs-lookup"><span data-stu-id="0c8e6-255">Request</span></span>
<span data-ttu-id="0c8e6-256">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2211

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0c8e6-257">応答</span><span class="sxs-lookup"><span data-stu-id="0c8e6-257">Response</span></span>
<span data-ttu-id="0c8e6-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c8e6-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2383

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```




