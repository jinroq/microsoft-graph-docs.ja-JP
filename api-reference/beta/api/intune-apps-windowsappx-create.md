---
title: WindowsAppX を作成する
description: 新しい windowsAppX オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40367ab7d5a8d546694f24a8bf75cb7c0920757f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328726"
---
# <a name="create-windowsappx"></a><span data-ttu-id="94a7d-103">WindowsAppX を作成する</span><span class="sxs-lookup"><span data-stu-id="94a7d-103">Create windowsAppX</span></span>

> <span data-ttu-id="94a7d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94a7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94a7d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94a7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94a7d-106">新しい[Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="94a7d-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94a7d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="94a7d-107">Prerequisites</span></span>
<span data-ttu-id="94a7d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94a7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a7d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94a7d-110">Permission type</span></span>|<span data-ttu-id="94a7d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94a7d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94a7d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94a7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94a7d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a7d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94a7d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94a7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94a7d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94a7d-115">Not supported.</span></span>|
|<span data-ttu-id="94a7d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94a7d-116">Application</span></span>|<span data-ttu-id="94a7d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a7d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94a7d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94a7d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="94a7d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94a7d-119">Request headers</span></span>
|<span data-ttu-id="94a7d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94a7d-120">Header</span></span>|<span data-ttu-id="94a7d-121">値</span><span class="sxs-lookup"><span data-stu-id="94a7d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94a7d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a7d-122">Authorization</span></span>|<span data-ttu-id="94a7d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="94a7d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94a7d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="94a7d-124">Accept</span></span>|<span data-ttu-id="94a7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94a7d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a7d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="94a7d-126">Request body</span></span>
<span data-ttu-id="94a7d-127">要求本文で、windowsAppX オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94a7d-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="94a7d-128">次の表に、windowsAppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="94a7d-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="94a7d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94a7d-129">Property</span></span>|<span data-ttu-id="94a7d-130">型</span><span class="sxs-lookup"><span data-stu-id="94a7d-130">Type</span></span>|<span data-ttu-id="94a7d-131">説明</span><span class="sxs-lookup"><span data-stu-id="94a7d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a7d-132">id</span><span class="sxs-lookup"><span data-stu-id="94a7d-132">id</span></span>|<span data-ttu-id="94a7d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="94a7d-133">String</span></span>|<span data-ttu-id="94a7d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="94a7d-134">Key of the entity.</span></span> <span data-ttu-id="94a7d-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="94a7d-136">displayName</span></span>|<span data-ttu-id="94a7d-137">文字列</span><span class="sxs-lookup"><span data-stu-id="94a7d-137">String</span></span>|<span data-ttu-id="94a7d-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="94a7d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="94a7d-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-140">description</span><span class="sxs-lookup"><span data-stu-id="94a7d-140">description</span></span>|<span data-ttu-id="94a7d-141">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-141">String</span></span>|<span data-ttu-id="94a7d-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="94a7d-142">The description of the app.</span></span> <span data-ttu-id="94a7d-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="94a7d-144">publisher</span></span>|<span data-ttu-id="94a7d-145">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-145">String</span></span>|<span data-ttu-id="94a7d-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="94a7d-146">The publisher of the app.</span></span> <span data-ttu-id="94a7d-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="94a7d-148">largeIcon</span></span>|[<span data-ttu-id="94a7d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="94a7d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="94a7d-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="94a7d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="94a7d-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94a7d-152">createdDateTime</span></span>|<span data-ttu-id="94a7d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a7d-153">DateTimeOffset</span></span>|<span data-ttu-id="94a7d-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="94a7d-154">The date and time the app was created.</span></span> <span data-ttu-id="94a7d-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94a7d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="94a7d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a7d-157">DateTimeOffset</span></span>|<span data-ttu-id="94a7d-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="94a7d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="94a7d-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="94a7d-160">isFeatured</span></span>|<span data-ttu-id="94a7d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a7d-161">Boolean</span></span>|<span data-ttu-id="94a7d-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="94a7d-163">privacyInformationUrl</span></span>|<span data-ttu-id="94a7d-164">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-164">String</span></span>|<span data-ttu-id="94a7d-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="94a7d-165">The privacy statement Url.</span></span> <span data-ttu-id="94a7d-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="94a7d-167">informationUrl</span></span>|<span data-ttu-id="94a7d-168">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-168">String</span></span>|<span data-ttu-id="94a7d-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="94a7d-169">The more information Url.</span></span> <span data-ttu-id="94a7d-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-171">owner</span><span class="sxs-lookup"><span data-stu-id="94a7d-171">owner</span></span>|<span data-ttu-id="94a7d-172">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-172">String</span></span>|<span data-ttu-id="94a7d-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="94a7d-173">The owner of the app.</span></span> <span data-ttu-id="94a7d-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-175">developer</span><span class="sxs-lookup"><span data-stu-id="94a7d-175">developer</span></span>|<span data-ttu-id="94a7d-176">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-176">String</span></span>|<span data-ttu-id="94a7d-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="94a7d-177">The developer of the app.</span></span> <span data-ttu-id="94a7d-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-179">notes</span><span class="sxs-lookup"><span data-stu-id="94a7d-179">notes</span></span>|<span data-ttu-id="94a7d-180">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-180">String</span></span>|<span data-ttu-id="94a7d-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="94a7d-181">Notes for the app.</span></span> <span data-ttu-id="94a7d-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="94a7d-183">uploadState</span></span>|<span data-ttu-id="94a7d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="94a7d-184">Int32</span></span>|<span data-ttu-id="94a7d-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="94a7d-185">The upload state.</span></span> <span data-ttu-id="94a7d-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="94a7d-187">publishingState</span></span>|[<span data-ttu-id="94a7d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="94a7d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="94a7d-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="94a7d-189">The publishing state for the app.</span></span> <span data-ttu-id="94a7d-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="94a7d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="94a7d-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="94a7d-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="94a7d-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="94a7d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="94a7d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="94a7d-193">isAssigned</span></span>|<span data-ttu-id="94a7d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a7d-194">Boolean</span></span>|<span data-ttu-id="94a7d-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="94a7d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="94a7d-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94a7d-197">roleScopeTagIds</span></span>|<span data-ttu-id="94a7d-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="94a7d-198">String collection</span></span>|<span data-ttu-id="94a7d-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="94a7d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="94a7d-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="94a7d-201">dependentAppCount</span></span>|<span data-ttu-id="94a7d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="94a7d-202">Int32</span></span>|<span data-ttu-id="94a7d-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="94a7d-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="94a7d-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="94a7d-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="94a7d-205">committedContentVersion</span></span>|<span data-ttu-id="94a7d-206">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-206">String</span></span>|<span data-ttu-id="94a7d-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="94a7d-207">The internal committed content version.</span></span> <span data-ttu-id="94a7d-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="94a7d-209">fileName</span><span class="sxs-lookup"><span data-stu-id="94a7d-209">fileName</span></span>|<span data-ttu-id="94a7d-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="94a7d-210">String</span></span>|<span data-ttu-id="94a7d-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="94a7d-211">The name of the main Lob application file.</span></span> <span data-ttu-id="94a7d-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="94a7d-213">size</span><span class="sxs-lookup"><span data-stu-id="94a7d-213">size</span></span>|<span data-ttu-id="94a7d-214">Int64</span><span class="sxs-lookup"><span data-stu-id="94a7d-214">Int64</span></span>|<span data-ttu-id="94a7d-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="94a7d-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="94a7d-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="94a7d-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="94a7d-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="94a7d-217">applicableArchitectures</span></span>|[<span data-ttu-id="94a7d-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="94a7d-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="94a7d-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="94a7d-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="94a7d-220">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="94a7d-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="94a7d-221">identityName</span><span class="sxs-lookup"><span data-stu-id="94a7d-221">identityName</span></span>|<span data-ttu-id="94a7d-222">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-222">String</span></span>|<span data-ttu-id="94a7d-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="94a7d-223">The Identity Name.</span></span>|
|<span data-ttu-id="94a7d-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="94a7d-224">identityPublisherHash</span></span>|<span data-ttu-id="94a7d-225">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-225">String</span></span>|<span data-ttu-id="94a7d-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="94a7d-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="94a7d-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="94a7d-227">identityResourceIdentifier</span></span>|<span data-ttu-id="94a7d-228">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-228">String</span></span>|<span data-ttu-id="94a7d-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="94a7d-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="94a7d-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="94a7d-230">isBundle</span></span>|<span data-ttu-id="94a7d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="94a7d-231">Boolean</span></span>|<span data-ttu-id="94a7d-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="94a7d-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="94a7d-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="94a7d-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="94a7d-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="94a7d-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="94a7d-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="94a7d-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="94a7d-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="94a7d-236">identityVersion</span></span>|<span data-ttu-id="94a7d-237">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-237">String</span></span>|<span data-ttu-id="94a7d-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="94a7d-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="94a7d-239">応答</span><span class="sxs-lookup"><span data-stu-id="94a7d-239">Response</span></span>
<span data-ttu-id="94a7d-240">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94a7d-240">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a7d-241">例</span><span class="sxs-lookup"><span data-stu-id="94a7d-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="94a7d-242">要求</span><span class="sxs-lookup"><span data-stu-id="94a7d-242">Request</span></span>
<span data-ttu-id="94a7d-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94a7d-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="94a7d-244">応答</span><span class="sxs-lookup"><span data-stu-id="94a7d-244">Response</span></span>
<span data-ttu-id="94a7d-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94a7d-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






