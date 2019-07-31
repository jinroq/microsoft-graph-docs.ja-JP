---
title: Update webApp
description: webApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbe07f822ea9617e4c509795bfe9abdad9a554ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960329"
---
# <a name="update-webapp"></a><span data-ttu-id="7f4e7-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="7f4e7-103">Update webApp</span></span>

> <span data-ttu-id="7f4e7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f4e7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f4e7-106">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f4e7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f4e7-107">Prerequisites</span></span>
<span data-ttu-id="7f4e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4e7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f4e7-110">Permission type</span></span>|<span data-ttu-id="7f4e7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f4e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f4e7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f4e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f4e7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f4e7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f4e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f4e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-115">Not supported.</span></span>|
|<span data-ttu-id="7f4e7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f4e7-116">Application</span></span>|<span data-ttu-id="7f4e7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f4e7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f4e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7f4e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f4e7-119">Request headers</span></span>
|<span data-ttu-id="7f4e7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f4e7-120">Header</span></span>|<span data-ttu-id="7f4e7-121">値</span><span class="sxs-lookup"><span data-stu-id="7f4e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f4e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4e7-122">Authorization</span></span>|<span data-ttu-id="7f4e7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f4e7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f4e7-124">Accept</span></span>|<span data-ttu-id="7f4e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f4e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f4e7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f4e7-126">Request body</span></span>
<span data-ttu-id="7f4e7-127">要求本文で、[webApp](../resources/intune-apps-webapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="7f4e7-128">次の表に、[webApp](../resources/intune-apps-webapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="7f4e7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f4e7-129">Property</span></span>|<span data-ttu-id="7f4e7-130">型</span><span class="sxs-lookup"><span data-stu-id="7f4e7-130">Type</span></span>|<span data-ttu-id="7f4e7-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f4e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f4e7-132">id</span><span class="sxs-lookup"><span data-stu-id="7f4e7-132">id</span></span>|<span data-ttu-id="7f4e7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7f4e7-133">String</span></span>|<span data-ttu-id="7f4e7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-134">Key of the entity.</span></span> <span data-ttu-id="7f4e7-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7f4e7-136">displayName</span></span>|<span data-ttu-id="7f4e7-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7f4e7-137">String</span></span>|<span data-ttu-id="7f4e7-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7f4e7-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-140">description</span><span class="sxs-lookup"><span data-stu-id="7f4e7-140">description</span></span>|<span data-ttu-id="7f4e7-141">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-141">String</span></span>|<span data-ttu-id="7f4e7-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-142">The description of the app.</span></span> <span data-ttu-id="7f4e7-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7f4e7-144">publisher</span></span>|<span data-ttu-id="7f4e7-145">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-145">String</span></span>|<span data-ttu-id="7f4e7-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-146">The publisher of the app.</span></span> <span data-ttu-id="7f4e7-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7f4e7-148">largeIcon</span></span>|[<span data-ttu-id="7f4e7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7f4e7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7f4e7-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7f4e7-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f4e7-152">createdDateTime</span></span>|<span data-ttu-id="7f4e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f4e7-153">DateTimeOffset</span></span>|<span data-ttu-id="7f4e7-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-154">The date and time the app was created.</span></span> <span data-ttu-id="7f4e7-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f4e7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7f4e7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f4e7-157">DateTimeOffset</span></span>|<span data-ttu-id="7f4e7-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7f4e7-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7f4e7-160">isFeatured</span></span>|<span data-ttu-id="7f4e7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f4e7-161">Boolean</span></span>|<span data-ttu-id="7f4e7-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7f4e7-163">privacyInformationUrl</span></span>|<span data-ttu-id="7f4e7-164">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-164">String</span></span>|<span data-ttu-id="7f4e7-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-165">The privacy statement Url.</span></span> <span data-ttu-id="7f4e7-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7f4e7-167">informationUrl</span></span>|<span data-ttu-id="7f4e7-168">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-168">String</span></span>|<span data-ttu-id="7f4e7-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-169">The more information Url.</span></span> <span data-ttu-id="7f4e7-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-171">owner</span><span class="sxs-lookup"><span data-stu-id="7f4e7-171">owner</span></span>|<span data-ttu-id="7f4e7-172">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-172">String</span></span>|<span data-ttu-id="7f4e7-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-173">The owner of the app.</span></span> <span data-ttu-id="7f4e7-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-175">developer</span><span class="sxs-lookup"><span data-stu-id="7f4e7-175">developer</span></span>|<span data-ttu-id="7f4e7-176">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-176">String</span></span>|<span data-ttu-id="7f4e7-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-177">The developer of the app.</span></span> <span data-ttu-id="7f4e7-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-179">notes</span><span class="sxs-lookup"><span data-stu-id="7f4e7-179">notes</span></span>|<span data-ttu-id="7f4e7-180">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-180">String</span></span>|<span data-ttu-id="7f4e7-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-181">Notes for the app.</span></span> <span data-ttu-id="7f4e7-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7f4e7-183">uploadState</span></span>|<span data-ttu-id="7f4e7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7f4e7-184">Int32</span></span>|<span data-ttu-id="7f4e7-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-185">The upload state.</span></span> <span data-ttu-id="7f4e7-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7f4e7-187">publishingState</span></span>|[<span data-ttu-id="7f4e7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7f4e7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7f4e7-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-189">The publishing state for the app.</span></span> <span data-ttu-id="7f4e7-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7f4e7-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7f4e7-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7f4e7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7f4e7-193">isAssigned</span></span>|<span data-ttu-id="7f4e7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f4e7-194">Boolean</span></span>|<span data-ttu-id="7f4e7-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7f4e7-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f4e7-197">roleScopeTagIds</span></span>|<span data-ttu-id="7f4e7-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f4e7-198">String collection</span></span>|<span data-ttu-id="7f4e7-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7f4e7-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7f4e7-201">dependentAppCount</span></span>|<span data-ttu-id="7f4e7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7f4e7-202">Int32</span></span>|<span data-ttu-id="7f4e7-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7f4e7-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f4e7-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f4e7-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="7f4e7-205">appUrl</span></span>|<span data-ttu-id="7f4e7-206">String</span><span class="sxs-lookup"><span data-stu-id="7f4e7-206">String</span></span>|<span data-ttu-id="7f4e7-207">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-207">The web app URL.</span></span>|
|<span data-ttu-id="7f4e7-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="7f4e7-208">useManagedBrowser</span></span>|<span data-ttu-id="7f4e7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f4e7-209">Boolean</span></span>|<span data-ttu-id="7f4e7-210">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="7f4e7-211">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="7f4e7-212">応答</span><span class="sxs-lookup"><span data-stu-id="7f4e7-212">Response</span></span>
<span data-ttu-id="7f4e7-213">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [webApp](../resources/intune-apps-webapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f4e7-214">例</span><span class="sxs-lookup"><span data-stu-id="7f4e7-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f4e7-215">要求</span><span class="sxs-lookup"><span data-stu-id="7f4e7-215">Request</span></span>
<span data-ttu-id="7f4e7-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="7f4e7-217">応答</span><span class="sxs-lookup"><span data-stu-id="7f4e7-217">Response</span></span>
<span data-ttu-id="7f4e7-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f4e7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





