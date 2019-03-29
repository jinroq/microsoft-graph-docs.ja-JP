---
title: windowsPhoneXAP の更新
description: windowsPhoneXAP オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f215feea187ec8ddf4c5a91fb529b9912e47a92a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982386"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="69126-103">windowsPhoneXAP の更新</span><span class="sxs-lookup"><span data-stu-id="69126-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="69126-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69126-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69126-106">[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="69126-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69126-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="69126-107">Prerequisites</span></span>
<span data-ttu-id="69126-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69126-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69126-110">Permission type</span></span>|<span data-ttu-id="69126-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69126-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69126-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69126-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69126-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69126-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69126-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69126-115">Not supported.</span></span>|
|<span data-ttu-id="69126-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69126-116">Application</span></span>|<span data-ttu-id="69126-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69126-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69126-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="69126-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69126-119">Request headers</span></span>
|<span data-ttu-id="69126-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69126-120">Header</span></span>|<span data-ttu-id="69126-121">値</span><span class="sxs-lookup"><span data-stu-id="69126-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69126-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69126-122">Authorization</span></span>|<span data-ttu-id="69126-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="69126-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69126-124">承諾</span><span class="sxs-lookup"><span data-stu-id="69126-124">Accept</span></span>|<span data-ttu-id="69126-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69126-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69126-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="69126-126">Request body</span></span>
<span data-ttu-id="69126-127">要求本文で、 [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69126-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="69126-128">次の表に、 [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69126-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="69126-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69126-129">Property</span></span>|<span data-ttu-id="69126-130">型</span><span class="sxs-lookup"><span data-stu-id="69126-130">Type</span></span>|<span data-ttu-id="69126-131">説明</span><span class="sxs-lookup"><span data-stu-id="69126-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69126-132">id</span><span class="sxs-lookup"><span data-stu-id="69126-132">id</span></span>|<span data-ttu-id="69126-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="69126-133">String</span></span>|<span data-ttu-id="69126-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="69126-134">Key of the entity.</span></span> <span data-ttu-id="69126-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-136">displayName</span><span class="sxs-lookup"><span data-stu-id="69126-136">displayName</span></span>|<span data-ttu-id="69126-137">String</span><span class="sxs-lookup"><span data-stu-id="69126-137">String</span></span>|<span data-ttu-id="69126-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="69126-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="69126-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-140">description</span><span class="sxs-lookup"><span data-stu-id="69126-140">description</span></span>|<span data-ttu-id="69126-141">String</span><span class="sxs-lookup"><span data-stu-id="69126-141">String</span></span>|<span data-ttu-id="69126-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="69126-142">The description of the app.</span></span> <span data-ttu-id="69126-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-144">publisher</span><span class="sxs-lookup"><span data-stu-id="69126-144">publisher</span></span>|<span data-ttu-id="69126-145">String</span><span class="sxs-lookup"><span data-stu-id="69126-145">String</span></span>|<span data-ttu-id="69126-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="69126-146">The publisher of the app.</span></span> <span data-ttu-id="69126-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="69126-148">largeIcon</span></span>|[<span data-ttu-id="69126-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69126-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="69126-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="69126-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="69126-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69126-152">createdDateTime</span></span>|<span data-ttu-id="69126-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69126-153">DateTimeOffset</span></span>|<span data-ttu-id="69126-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="69126-154">The date and time the app was created.</span></span> <span data-ttu-id="69126-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69126-156">lastModifiedDateTime</span></span>|<span data-ttu-id="69126-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69126-157">DateTimeOffset</span></span>|<span data-ttu-id="69126-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="69126-158">The date and time the app was last modified.</span></span> <span data-ttu-id="69126-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="69126-160">isFeatured</span></span>|<span data-ttu-id="69126-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="69126-161">Boolean</span></span>|<span data-ttu-id="69126-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="69126-163">privacyInformationUrl</span></span>|<span data-ttu-id="69126-164">String</span><span class="sxs-lookup"><span data-stu-id="69126-164">String</span></span>|<span data-ttu-id="69126-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="69126-165">The privacy statement Url.</span></span> <span data-ttu-id="69126-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="69126-167">informationUrl</span></span>|<span data-ttu-id="69126-168">String</span><span class="sxs-lookup"><span data-stu-id="69126-168">String</span></span>|<span data-ttu-id="69126-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="69126-169">The more information Url.</span></span> <span data-ttu-id="69126-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-171">owner</span><span class="sxs-lookup"><span data-stu-id="69126-171">owner</span></span>|<span data-ttu-id="69126-172">String</span><span class="sxs-lookup"><span data-stu-id="69126-172">String</span></span>|<span data-ttu-id="69126-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="69126-173">The owner of the app.</span></span> <span data-ttu-id="69126-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-175">developer</span><span class="sxs-lookup"><span data-stu-id="69126-175">developer</span></span>|<span data-ttu-id="69126-176">String</span><span class="sxs-lookup"><span data-stu-id="69126-176">String</span></span>|<span data-ttu-id="69126-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="69126-177">The developer of the app.</span></span> <span data-ttu-id="69126-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-179">notes</span><span class="sxs-lookup"><span data-stu-id="69126-179">notes</span></span>|<span data-ttu-id="69126-180">String</span><span class="sxs-lookup"><span data-stu-id="69126-180">String</span></span>|<span data-ttu-id="69126-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="69126-181">Notes for the app.</span></span> <span data-ttu-id="69126-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="69126-183">uploadState</span></span>|<span data-ttu-id="69126-184">Int32</span><span class="sxs-lookup"><span data-stu-id="69126-184">Int32</span></span>|<span data-ttu-id="69126-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="69126-185">The upload state.</span></span> <span data-ttu-id="69126-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="69126-187">publishingState</span></span>|[<span data-ttu-id="69126-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="69126-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="69126-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="69126-189">The publishing state for the app.</span></span> <span data-ttu-id="69126-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="69126-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="69126-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="69126-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="69126-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="69126-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="69126-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="69126-193">isAssigned</span></span>|<span data-ttu-id="69126-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="69126-194">Boolean</span></span>|<span data-ttu-id="69126-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="69126-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="69126-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69126-197">roleScopeTagIds</span></span>|<span data-ttu-id="69126-198">String collection</span><span class="sxs-lookup"><span data-stu-id="69126-198">String collection</span></span>|<span data-ttu-id="69126-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="69126-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="69126-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69126-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="69126-201">committedContentVersion</span></span>|<span data-ttu-id="69126-202">String</span><span class="sxs-lookup"><span data-stu-id="69126-202">String</span></span>|<span data-ttu-id="69126-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="69126-203">The internal committed content version.</span></span> <span data-ttu-id="69126-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="69126-205">fileName</span><span class="sxs-lookup"><span data-stu-id="69126-205">fileName</span></span>|<span data-ttu-id="69126-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="69126-206">String</span></span>|<span data-ttu-id="69126-207">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="69126-207">The name of the main Lob application file.</span></span> <span data-ttu-id="69126-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="69126-209">size</span><span class="sxs-lookup"><span data-stu-id="69126-209">size</span></span>|<span data-ttu-id="69126-210">Int64</span><span class="sxs-lookup"><span data-stu-id="69126-210">Int64</span></span>|<span data-ttu-id="69126-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="69126-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="69126-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69126-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="69126-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69126-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="69126-214">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69126-214">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="69126-215">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="69126-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="69126-216">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="69126-216">productIdentifier</span></span>|<span data-ttu-id="69126-217">String</span><span class="sxs-lookup"><span data-stu-id="69126-217">String</span></span>|<span data-ttu-id="69126-218">製品識別子。</span><span class="sxs-lookup"><span data-stu-id="69126-218">The Product Identifier.</span></span>|
|<span data-ttu-id="69126-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="69126-219">identityVersion</span></span>|<span data-ttu-id="69126-220">String</span><span class="sxs-lookup"><span data-stu-id="69126-220">String</span></span>|<span data-ttu-id="69126-221">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="69126-221">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="69126-222">応答</span><span class="sxs-lookup"><span data-stu-id="69126-222">Response</span></span>
<span data-ttu-id="69126-223">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69126-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69126-224">例</span><span class="sxs-lookup"><span data-stu-id="69126-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="69126-225">要求</span><span class="sxs-lookup"><span data-stu-id="69126-225">Request</span></span>
<span data-ttu-id="69126-226">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69126-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1164

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="69126-227">応答</span><span class="sxs-lookup"><span data-stu-id="69126-227">Response</span></span>
<span data-ttu-id="69126-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69126-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1336

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




