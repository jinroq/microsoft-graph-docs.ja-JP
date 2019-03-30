---
title: windowsPhone81AppXBundle の更新
description: windowsPhone81AppXBundle オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5908c8fad99a93305f6f3662339e1799bdd6e11
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988183"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="24b42-103">windowsPhone81AppXBundle の更新</span><span class="sxs-lookup"><span data-stu-id="24b42-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="24b42-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b42-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24b42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b42-106">[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="24b42-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b42-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="24b42-107">Prerequisites</span></span>
<span data-ttu-id="24b42-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b42-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24b42-110">Permission type</span></span>|<span data-ttu-id="24b42-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24b42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b42-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24b42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24b42-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b42-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24b42-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24b42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b42-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b42-115">Not supported.</span></span>|
|<span data-ttu-id="24b42-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24b42-116">Application</span></span>|<span data-ttu-id="24b42-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24b42-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24b42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="24b42-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b42-119">Request headers</span></span>
|<span data-ttu-id="24b42-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b42-120">Header</span></span>|<span data-ttu-id="24b42-121">値</span><span class="sxs-lookup"><span data-stu-id="24b42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24b42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b42-122">Authorization</span></span>|<span data-ttu-id="24b42-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="24b42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24b42-124">承諾</span><span class="sxs-lookup"><span data-stu-id="24b42-124">Accept</span></span>|<span data-ttu-id="24b42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24b42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b42-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="24b42-126">Request body</span></span>
<span data-ttu-id="24b42-127">要求本文で、 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24b42-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="24b42-128">次の表に、 [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24b42-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="24b42-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24b42-129">Property</span></span>|<span data-ttu-id="24b42-130">型</span><span class="sxs-lookup"><span data-stu-id="24b42-130">Type</span></span>|<span data-ttu-id="24b42-131">説明</span><span class="sxs-lookup"><span data-stu-id="24b42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b42-132">id</span><span class="sxs-lookup"><span data-stu-id="24b42-132">id</span></span>|<span data-ttu-id="24b42-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="24b42-133">String</span></span>|<span data-ttu-id="24b42-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="24b42-134">Key of the entity.</span></span> <span data-ttu-id="24b42-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-136">displayName</span><span class="sxs-lookup"><span data-stu-id="24b42-136">displayName</span></span>|<span data-ttu-id="24b42-137">String</span><span class="sxs-lookup"><span data-stu-id="24b42-137">String</span></span>|<span data-ttu-id="24b42-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="24b42-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="24b42-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-140">description</span><span class="sxs-lookup"><span data-stu-id="24b42-140">description</span></span>|<span data-ttu-id="24b42-141">String</span><span class="sxs-lookup"><span data-stu-id="24b42-141">String</span></span>|<span data-ttu-id="24b42-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="24b42-142">The description of the app.</span></span> <span data-ttu-id="24b42-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-144">publisher</span><span class="sxs-lookup"><span data-stu-id="24b42-144">publisher</span></span>|<span data-ttu-id="24b42-145">String</span><span class="sxs-lookup"><span data-stu-id="24b42-145">String</span></span>|<span data-ttu-id="24b42-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="24b42-146">The publisher of the app.</span></span> <span data-ttu-id="24b42-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="24b42-148">largeIcon</span></span>|[<span data-ttu-id="24b42-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="24b42-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="24b42-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="24b42-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="24b42-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24b42-152">createdDateTime</span></span>|<span data-ttu-id="24b42-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b42-153">DateTimeOffset</span></span>|<span data-ttu-id="24b42-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="24b42-154">The date and time the app was created.</span></span> <span data-ttu-id="24b42-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24b42-156">lastModifiedDateTime</span></span>|<span data-ttu-id="24b42-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b42-157">DateTimeOffset</span></span>|<span data-ttu-id="24b42-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="24b42-158">The date and time the app was last modified.</span></span> <span data-ttu-id="24b42-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="24b42-160">isFeatured</span></span>|<span data-ttu-id="24b42-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="24b42-161">Boolean</span></span>|<span data-ttu-id="24b42-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="24b42-163">privacyInformationUrl</span></span>|<span data-ttu-id="24b42-164">String</span><span class="sxs-lookup"><span data-stu-id="24b42-164">String</span></span>|<span data-ttu-id="24b42-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="24b42-165">The privacy statement Url.</span></span> <span data-ttu-id="24b42-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="24b42-167">informationUrl</span></span>|<span data-ttu-id="24b42-168">String</span><span class="sxs-lookup"><span data-stu-id="24b42-168">String</span></span>|<span data-ttu-id="24b42-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="24b42-169">The more information Url.</span></span> <span data-ttu-id="24b42-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-171">owner</span><span class="sxs-lookup"><span data-stu-id="24b42-171">owner</span></span>|<span data-ttu-id="24b42-172">String</span><span class="sxs-lookup"><span data-stu-id="24b42-172">String</span></span>|<span data-ttu-id="24b42-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="24b42-173">The owner of the app.</span></span> <span data-ttu-id="24b42-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-175">developer</span><span class="sxs-lookup"><span data-stu-id="24b42-175">developer</span></span>|<span data-ttu-id="24b42-176">String</span><span class="sxs-lookup"><span data-stu-id="24b42-176">String</span></span>|<span data-ttu-id="24b42-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="24b42-177">The developer of the app.</span></span> <span data-ttu-id="24b42-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-179">notes</span><span class="sxs-lookup"><span data-stu-id="24b42-179">notes</span></span>|<span data-ttu-id="24b42-180">String</span><span class="sxs-lookup"><span data-stu-id="24b42-180">String</span></span>|<span data-ttu-id="24b42-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="24b42-181">Notes for the app.</span></span> <span data-ttu-id="24b42-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="24b42-183">uploadState</span></span>|<span data-ttu-id="24b42-184">Int32</span><span class="sxs-lookup"><span data-stu-id="24b42-184">Int32</span></span>|<span data-ttu-id="24b42-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="24b42-185">The upload state.</span></span> <span data-ttu-id="24b42-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="24b42-187">publishingState</span></span>|[<span data-ttu-id="24b42-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="24b42-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="24b42-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="24b42-189">The publishing state for the app.</span></span> <span data-ttu-id="24b42-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="24b42-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="24b42-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="24b42-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="24b42-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="24b42-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="24b42-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="24b42-193">isAssigned</span></span>|<span data-ttu-id="24b42-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="24b42-194">Boolean</span></span>|<span data-ttu-id="24b42-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="24b42-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="24b42-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24b42-197">roleScopeTagIds</span></span>|<span data-ttu-id="24b42-198">String collection</span><span class="sxs-lookup"><span data-stu-id="24b42-198">String collection</span></span>|<span data-ttu-id="24b42-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="24b42-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="24b42-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="24b42-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="24b42-201">committedContentVersion</span></span>|<span data-ttu-id="24b42-202">String</span><span class="sxs-lookup"><span data-stu-id="24b42-202">String</span></span>|<span data-ttu-id="24b42-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="24b42-203">The internal committed content version.</span></span> <span data-ttu-id="24b42-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24b42-205">fileName</span><span class="sxs-lookup"><span data-stu-id="24b42-205">fileName</span></span>|<span data-ttu-id="24b42-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="24b42-206">String</span></span>|<span data-ttu-id="24b42-207">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="24b42-207">The name of the main Lob application file.</span></span> <span data-ttu-id="24b42-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24b42-209">size</span><span class="sxs-lookup"><span data-stu-id="24b42-209">size</span></span>|<span data-ttu-id="24b42-210">Int64</span><span class="sxs-lookup"><span data-stu-id="24b42-210">Int64</span></span>|<span data-ttu-id="24b42-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="24b42-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="24b42-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="24b42-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24b42-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="24b42-213">applicableArchitectures</span></span>|[<span data-ttu-id="24b42-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="24b42-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="24b42-215">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="24b42-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="24b42-216">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="24b42-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="24b42-217">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="24b42-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="24b42-218">identityName</span><span class="sxs-lookup"><span data-stu-id="24b42-218">identityName</span></span>|<span data-ttu-id="24b42-219">String</span><span class="sxs-lookup"><span data-stu-id="24b42-219">String</span></span>|<span data-ttu-id="24b42-220">ID 名。</span><span class="sxs-lookup"><span data-stu-id="24b42-220">The Identity Name.</span></span> <span data-ttu-id="24b42-221">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="24b42-222">identityPublisherHash</span></span>|<span data-ttu-id="24b42-223">String</span><span class="sxs-lookup"><span data-stu-id="24b42-223">String</span></span>|<span data-ttu-id="24b42-224">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="24b42-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="24b42-225">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="24b42-226">identityResourceIdentifier</span></span>|<span data-ttu-id="24b42-227">String</span><span class="sxs-lookup"><span data-stu-id="24b42-227">String</span></span>|<span data-ttu-id="24b42-228">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="24b42-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="24b42-229">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="24b42-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="24b42-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="24b42-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="24b42-232">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="24b42-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="24b42-233">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-234">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="24b42-234">phoneProductIdentifier</span></span>|<span data-ttu-id="24b42-235">String</span><span class="sxs-lookup"><span data-stu-id="24b42-235">String</span></span>|<span data-ttu-id="24b42-236">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="24b42-236">The Phone Product Identifier.</span></span> <span data-ttu-id="24b42-237">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-238">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="24b42-238">phonePublisherId</span></span>|<span data-ttu-id="24b42-239">String</span><span class="sxs-lookup"><span data-stu-id="24b42-239">String</span></span>|<span data-ttu-id="24b42-240">電話の発行元 Id。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="24b42-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="24b42-241">identityVersion</span></span>|<span data-ttu-id="24b42-242">String</span><span class="sxs-lookup"><span data-stu-id="24b42-242">String</span></span>|<span data-ttu-id="24b42-243">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="24b42-243">The identity version.</span></span> <span data-ttu-id="24b42-244">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="24b42-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="24b42-245">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="24b42-245">appXPackageInformationList</span></span>|<span data-ttu-id="24b42-246">[windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="24b42-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="24b42-247">AppX パッケージ情報のリスト。</span><span class="sxs-lookup"><span data-stu-id="24b42-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="24b42-248">応答</span><span class="sxs-lookup"><span data-stu-id="24b42-248">Response</span></span>
<span data-ttu-id="24b42-249">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24b42-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24b42-250">例</span><span class="sxs-lookup"><span data-stu-id="24b42-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="24b42-251">要求</span><span class="sxs-lookup"><span data-stu-id="24b42-251">Request</span></span>
<span data-ttu-id="24b42-252">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24b42-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2184

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

### <a name="response"></a><span data-ttu-id="24b42-253">応答</span><span class="sxs-lookup"><span data-stu-id="24b42-253">Response</span></span>
<span data-ttu-id="24b42-p128">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24b42-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2356

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




