---
title: windowsPhone81AppX の更新
description: windowsPhone81AppX オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7561ec83da1a835000c939c38f34e34ea0eb0ed7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780911"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="f1570-103">windowsPhone81AppX の更新</span><span class="sxs-lookup"><span data-stu-id="f1570-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="f1570-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1570-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1570-106">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1570-106">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1570-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1570-107">Prerequisites</span></span>
<span data-ttu-id="f1570-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1570-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1570-110">Permission type</span></span>|<span data-ttu-id="f1570-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1570-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1570-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1570-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1570-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1570-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1570-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1570-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1570-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1570-115">Not supported.</span></span>|
|<span data-ttu-id="f1570-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1570-116">Application</span></span>|<span data-ttu-id="f1570-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1570-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1570-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1570-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f1570-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1570-119">Request headers</span></span>
|<span data-ttu-id="f1570-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1570-120">Header</span></span>|<span data-ttu-id="f1570-121">値</span><span class="sxs-lookup"><span data-stu-id="f1570-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1570-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1570-122">Authorization</span></span>|<span data-ttu-id="f1570-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1570-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1570-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f1570-124">Accept</span></span>|<span data-ttu-id="f1570-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1570-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1570-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1570-126">Request body</span></span>
<span data-ttu-id="f1570-127">要求本文で、 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1570-127">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="f1570-128">次の表に、 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f1570-128">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="f1570-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1570-129">Property</span></span>|<span data-ttu-id="f1570-130">型</span><span class="sxs-lookup"><span data-stu-id="f1570-130">Type</span></span>|<span data-ttu-id="f1570-131">説明</span><span class="sxs-lookup"><span data-stu-id="f1570-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1570-132">id</span><span class="sxs-lookup"><span data-stu-id="f1570-132">id</span></span>|<span data-ttu-id="f1570-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1570-133">String</span></span>|<span data-ttu-id="f1570-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f1570-134">Key of the entity.</span></span> <span data-ttu-id="f1570-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f1570-136">displayName</span></span>|<span data-ttu-id="f1570-137">String</span><span class="sxs-lookup"><span data-stu-id="f1570-137">String</span></span>|<span data-ttu-id="f1570-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f1570-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f1570-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-140">説明</span><span class="sxs-lookup"><span data-stu-id="f1570-140">description</span></span>|<span data-ttu-id="f1570-141">String</span><span class="sxs-lookup"><span data-stu-id="f1570-141">String</span></span>|<span data-ttu-id="f1570-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f1570-142">The description of the app.</span></span> <span data-ttu-id="f1570-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f1570-144">publisher</span></span>|<span data-ttu-id="f1570-145">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-145">String</span></span>|<span data-ttu-id="f1570-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f1570-146">The publisher of the app.</span></span> <span data-ttu-id="f1570-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f1570-148">largeIcon</span></span>|[<span data-ttu-id="f1570-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f1570-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f1570-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="f1570-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f1570-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1570-152">createdDateTime</span></span>|<span data-ttu-id="f1570-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1570-153">DateTimeOffset</span></span>|<span data-ttu-id="f1570-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f1570-154">The date and time the app was created.</span></span> <span data-ttu-id="f1570-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1570-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f1570-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1570-157">DateTimeOffset</span></span>|<span data-ttu-id="f1570-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f1570-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f1570-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f1570-160">isFeatured</span></span>|<span data-ttu-id="f1570-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1570-161">Boolean</span></span>|<span data-ttu-id="f1570-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f1570-163">privacyInformationUrl</span></span>|<span data-ttu-id="f1570-164">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-164">String</span></span>|<span data-ttu-id="f1570-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f1570-165">The privacy statement Url.</span></span> <span data-ttu-id="f1570-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f1570-167">informationUrl</span></span>|<span data-ttu-id="f1570-168">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-168">String</span></span>|<span data-ttu-id="f1570-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f1570-169">The more information Url.</span></span> <span data-ttu-id="f1570-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-171">owner</span><span class="sxs-lookup"><span data-stu-id="f1570-171">owner</span></span>|<span data-ttu-id="f1570-172">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-172">String</span></span>|<span data-ttu-id="f1570-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f1570-173">The owner of the app.</span></span> <span data-ttu-id="f1570-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-175">developer</span><span class="sxs-lookup"><span data-stu-id="f1570-175">developer</span></span>|<span data-ttu-id="f1570-176">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-176">String</span></span>|<span data-ttu-id="f1570-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f1570-177">The developer of the app.</span></span> <span data-ttu-id="f1570-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-179">notes</span><span class="sxs-lookup"><span data-stu-id="f1570-179">notes</span></span>|<span data-ttu-id="f1570-180">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-180">String</span></span>|<span data-ttu-id="f1570-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f1570-181">Notes for the app.</span></span> <span data-ttu-id="f1570-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f1570-183">uploadState</span></span>|<span data-ttu-id="f1570-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f1570-184">Int32</span></span>|<span data-ttu-id="f1570-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="f1570-185">The upload state.</span></span> <span data-ttu-id="f1570-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f1570-187">publishingState</span></span>|[<span data-ttu-id="f1570-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f1570-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f1570-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f1570-189">The publishing state for the app.</span></span> <span data-ttu-id="f1570-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f1570-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f1570-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f1570-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f1570-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f1570-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f1570-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f1570-193">isAssigned</span></span>|<span data-ttu-id="f1570-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1570-194">Boolean</span></span>|<span data-ttu-id="f1570-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="f1570-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f1570-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1570-197">roleScopeTagIds</span></span>|<span data-ttu-id="f1570-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f1570-198">String collection</span></span>|<span data-ttu-id="f1570-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="f1570-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f1570-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="f1570-201">dependentAppCount</span></span>|<span data-ttu-id="f1570-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f1570-202">Int32</span></span>|<span data-ttu-id="f1570-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="f1570-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f1570-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1570-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f1570-205">committedContentVersion</span></span>|<span data-ttu-id="f1570-206">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-206">String</span></span>|<span data-ttu-id="f1570-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f1570-207">The internal committed content version.</span></span> <span data-ttu-id="f1570-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1570-209">fileName</span><span class="sxs-lookup"><span data-stu-id="f1570-209">fileName</span></span>|<span data-ttu-id="f1570-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1570-210">String</span></span>|<span data-ttu-id="f1570-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="f1570-211">The name of the main Lob application file.</span></span> <span data-ttu-id="f1570-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1570-213">size</span><span class="sxs-lookup"><span data-stu-id="f1570-213">size</span></span>|<span data-ttu-id="f1570-214">Int64</span><span class="sxs-lookup"><span data-stu-id="f1570-214">Int64</span></span>|<span data-ttu-id="f1570-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="f1570-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="f1570-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f1570-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1570-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f1570-217">applicableArchitectures</span></span>|[<span data-ttu-id="f1570-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f1570-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f1570-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="f1570-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f1570-220">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="f1570-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f1570-221">identityName</span><span class="sxs-lookup"><span data-stu-id="f1570-221">identityName</span></span>|<span data-ttu-id="f1570-222">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-222">String</span></span>|<span data-ttu-id="f1570-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="f1570-223">The Identity Name.</span></span>|
|<span data-ttu-id="f1570-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="f1570-224">identityPublisherHash</span></span>|<span data-ttu-id="f1570-225">String</span><span class="sxs-lookup"><span data-stu-id="f1570-225">String</span></span>|<span data-ttu-id="f1570-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="f1570-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="f1570-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f1570-227">identityResourceIdentifier</span></span>|<span data-ttu-id="f1570-228">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-228">String</span></span>|<span data-ttu-id="f1570-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="f1570-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f1570-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f1570-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f1570-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f1570-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f1570-232">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="f1570-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f1570-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="f1570-233">phoneProductIdentifier</span></span>|<span data-ttu-id="f1570-234">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-234">String</span></span>|<span data-ttu-id="f1570-235">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="f1570-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="f1570-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="f1570-236">phonePublisherId</span></span>|<span data-ttu-id="f1570-237">文字列</span><span class="sxs-lookup"><span data-stu-id="f1570-237">String</span></span>|<span data-ttu-id="f1570-238">電話の発行元 Id。</span><span class="sxs-lookup"><span data-stu-id="f1570-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="f1570-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f1570-239">identityVersion</span></span>|<span data-ttu-id="f1570-240">String</span><span class="sxs-lookup"><span data-stu-id="f1570-240">String</span></span>|<span data-ttu-id="f1570-241">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f1570-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f1570-242">応答</span><span class="sxs-lookup"><span data-stu-id="f1570-242">Response</span></span>
<span data-ttu-id="f1570-243">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1570-243">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1570-244">例</span><span class="sxs-lookup"><span data-stu-id="f1570-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1570-245">要求</span><span class="sxs-lookup"><span data-stu-id="f1570-245">Request</span></span>
<span data-ttu-id="f1570-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1570-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1467

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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f1570-247">応答</span><span class="sxs-lookup"><span data-stu-id="f1570-247">Response</span></span>
<span data-ttu-id="f1570-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1570-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1639

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
  "identityVersion": "Identity Version value"
}
```





