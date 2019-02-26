---
title: windowsPhone81AppX の更新
description: windowsPhone81AppX オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ab6a96eb4fe9892a07be764a32309ee2d52b73
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151766"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="454db-103">windowsPhone81AppX の更新</span><span class="sxs-lookup"><span data-stu-id="454db-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="454db-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="454db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="454db-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="454db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="454db-106">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="454db-106">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="454db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="454db-107">Prerequisites</span></span>
<span data-ttu-id="454db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="454db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="454db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="454db-110">Permission type</span></span>|<span data-ttu-id="454db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="454db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="454db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="454db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="454db-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="454db-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="454db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="454db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="454db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="454db-115">Not supported.</span></span>|
|<span data-ttu-id="454db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="454db-116">Application</span></span>|<span data-ttu-id="454db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="454db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="454db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="454db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="454db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="454db-119">Request headers</span></span>
|<span data-ttu-id="454db-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="454db-120">Header</span></span>|<span data-ttu-id="454db-121">値</span><span class="sxs-lookup"><span data-stu-id="454db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="454db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="454db-122">Authorization</span></span>|<span data-ttu-id="454db-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="454db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="454db-124">承諾</span><span class="sxs-lookup"><span data-stu-id="454db-124">Accept</span></span>|<span data-ttu-id="454db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="454db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="454db-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="454db-126">Request body</span></span>
<span data-ttu-id="454db-127">要求本文で、 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="454db-127">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="454db-128">次の表に、 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="454db-128">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="454db-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="454db-129">Property</span></span>|<span data-ttu-id="454db-130">型</span><span class="sxs-lookup"><span data-stu-id="454db-130">Type</span></span>|<span data-ttu-id="454db-131">説明</span><span class="sxs-lookup"><span data-stu-id="454db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="454db-132">id</span><span class="sxs-lookup"><span data-stu-id="454db-132">id</span></span>|<span data-ttu-id="454db-133">文字列</span><span class="sxs-lookup"><span data-stu-id="454db-133">String</span></span>|<span data-ttu-id="454db-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="454db-134">Key of the entity.</span></span> <span data-ttu-id="454db-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="454db-136">displayName</span></span>|<span data-ttu-id="454db-137">String</span><span class="sxs-lookup"><span data-stu-id="454db-137">String</span></span>|<span data-ttu-id="454db-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="454db-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="454db-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-140">説明</span><span class="sxs-lookup"><span data-stu-id="454db-140">description</span></span>|<span data-ttu-id="454db-141">文字列</span><span class="sxs-lookup"><span data-stu-id="454db-141">String</span></span>|<span data-ttu-id="454db-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="454db-142">The description of the app.</span></span> <span data-ttu-id="454db-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-144">publisher</span><span class="sxs-lookup"><span data-stu-id="454db-144">publisher</span></span>|<span data-ttu-id="454db-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="454db-145">String</span></span>|<span data-ttu-id="454db-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="454db-146">The publisher of the app.</span></span> <span data-ttu-id="454db-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="454db-148">largeIcon</span></span>|[<span data-ttu-id="454db-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="454db-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="454db-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="454db-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="454db-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="454db-152">createdDateTime</span></span>|<span data-ttu-id="454db-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454db-153">DateTimeOffset</span></span>|<span data-ttu-id="454db-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="454db-154">The date and time the app was created.</span></span> <span data-ttu-id="454db-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="454db-156">lastModifiedDateTime</span></span>|<span data-ttu-id="454db-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454db-157">DateTimeOffset</span></span>|<span data-ttu-id="454db-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="454db-158">The date and time the app was last modified.</span></span> <span data-ttu-id="454db-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="454db-160">isFeatured</span></span>|<span data-ttu-id="454db-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="454db-161">Boolean</span></span>|<span data-ttu-id="454db-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="454db-163">privacyInformationUrl</span></span>|<span data-ttu-id="454db-164">String</span><span class="sxs-lookup"><span data-stu-id="454db-164">String</span></span>|<span data-ttu-id="454db-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="454db-165">The privacy statement Url.</span></span> <span data-ttu-id="454db-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="454db-167">informationUrl</span></span>|<span data-ttu-id="454db-168">String</span><span class="sxs-lookup"><span data-stu-id="454db-168">String</span></span>|<span data-ttu-id="454db-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="454db-169">The more information Url.</span></span> <span data-ttu-id="454db-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-171">owner</span><span class="sxs-lookup"><span data-stu-id="454db-171">owner</span></span>|<span data-ttu-id="454db-172">String</span><span class="sxs-lookup"><span data-stu-id="454db-172">String</span></span>|<span data-ttu-id="454db-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="454db-173">The owner of the app.</span></span> <span data-ttu-id="454db-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-175">developer</span><span class="sxs-lookup"><span data-stu-id="454db-175">developer</span></span>|<span data-ttu-id="454db-176">String</span><span class="sxs-lookup"><span data-stu-id="454db-176">String</span></span>|<span data-ttu-id="454db-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="454db-177">The developer of the app.</span></span> <span data-ttu-id="454db-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-179">notes</span><span class="sxs-lookup"><span data-stu-id="454db-179">notes</span></span>|<span data-ttu-id="454db-180">String</span><span class="sxs-lookup"><span data-stu-id="454db-180">String</span></span>|<span data-ttu-id="454db-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="454db-181">Notes for the app.</span></span> <span data-ttu-id="454db-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="454db-183">uploadState</span></span>|<span data-ttu-id="454db-184">Int32</span><span class="sxs-lookup"><span data-stu-id="454db-184">Int32</span></span>|<span data-ttu-id="454db-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="454db-185">The upload state.</span></span> <span data-ttu-id="454db-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="454db-187">publishingState</span></span>|[<span data-ttu-id="454db-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="454db-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="454db-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="454db-189">The publishing state for the app.</span></span> <span data-ttu-id="454db-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="454db-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="454db-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="454db-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="454db-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="454db-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="454db-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="454db-193">isAssigned</span></span>|<span data-ttu-id="454db-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="454db-194">Boolean</span></span>|<span data-ttu-id="454db-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="454db-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="454db-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="454db-197">roleScopeTagIds</span></span>|<span data-ttu-id="454db-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="454db-198">String collection</span></span>|<span data-ttu-id="454db-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="454db-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="454db-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="454db-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="454db-201">committedContentVersion</span></span>|<span data-ttu-id="454db-202">String</span><span class="sxs-lookup"><span data-stu-id="454db-202">String</span></span>|<span data-ttu-id="454db-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="454db-203">The internal committed content version.</span></span> <span data-ttu-id="454db-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="454db-205">fileName</span><span class="sxs-lookup"><span data-stu-id="454db-205">fileName</span></span>|<span data-ttu-id="454db-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="454db-206">String</span></span>|<span data-ttu-id="454db-207">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="454db-207">The name of the main Lob application file.</span></span> <span data-ttu-id="454db-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="454db-209">size</span><span class="sxs-lookup"><span data-stu-id="454db-209">size</span></span>|<span data-ttu-id="454db-210">Int64</span><span class="sxs-lookup"><span data-stu-id="454db-210">Int64</span></span>|<span data-ttu-id="454db-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="454db-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="454db-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="454db-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="454db-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="454db-213">applicableArchitectures</span></span>|[<span data-ttu-id="454db-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="454db-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="454db-215">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="454db-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="454db-216">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="454db-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="454db-217">identityName</span><span class="sxs-lookup"><span data-stu-id="454db-217">identityName</span></span>|<span data-ttu-id="454db-218">String</span><span class="sxs-lookup"><span data-stu-id="454db-218">String</span></span>|<span data-ttu-id="454db-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="454db-219">The Identity Name.</span></span>|
|<span data-ttu-id="454db-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="454db-220">identityPublisherHash</span></span>|<span data-ttu-id="454db-221">String</span><span class="sxs-lookup"><span data-stu-id="454db-221">String</span></span>|<span data-ttu-id="454db-222">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="454db-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="454db-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="454db-223">identityResourceIdentifier</span></span>|<span data-ttu-id="454db-224">String</span><span class="sxs-lookup"><span data-stu-id="454db-224">String</span></span>|<span data-ttu-id="454db-225">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="454db-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="454db-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="454db-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="454db-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="454db-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="454db-228">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="454db-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="454db-229">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="454db-229">phoneProductIdentifier</span></span>|<span data-ttu-id="454db-230">String</span><span class="sxs-lookup"><span data-stu-id="454db-230">String</span></span>|<span data-ttu-id="454db-231">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="454db-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="454db-232">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="454db-232">phonePublisherId</span></span>|<span data-ttu-id="454db-233">String</span><span class="sxs-lookup"><span data-stu-id="454db-233">String</span></span>|<span data-ttu-id="454db-234">電話の発行元 Id。</span><span class="sxs-lookup"><span data-stu-id="454db-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="454db-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="454db-235">identityVersion</span></span>|<span data-ttu-id="454db-236">String</span><span class="sxs-lookup"><span data-stu-id="454db-236">String</span></span>|<span data-ttu-id="454db-237">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="454db-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="454db-238">応答</span><span class="sxs-lookup"><span data-stu-id="454db-238">Response</span></span>
<span data-ttu-id="454db-239">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="454db-239">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="454db-240">例</span><span class="sxs-lookup"><span data-stu-id="454db-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="454db-241">要求</span><span class="sxs-lookup"><span data-stu-id="454db-241">Request</span></span>
<span data-ttu-id="454db-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="454db-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="454db-243">応答</span><span class="sxs-lookup"><span data-stu-id="454db-243">Response</span></span>
<span data-ttu-id="454db-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="454db-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1612

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "identityVersion": "Identity Version value"
}
```




