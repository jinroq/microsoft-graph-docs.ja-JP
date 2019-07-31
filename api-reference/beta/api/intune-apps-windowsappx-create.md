---
title: WindowsAppX を作成する
description: 新しい windowsAppX オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 957776f9617003f333d05fed7d310fd8258298a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960174"
---
# <a name="create-windowsappx"></a><span data-ttu-id="b6ff0-103">WindowsAppX を作成する</span><span class="sxs-lookup"><span data-stu-id="b6ff0-103">Create windowsAppX</span></span>

> <span data-ttu-id="b6ff0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6ff0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6ff0-106">新しい[Windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6ff0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6ff0-107">Prerequisites</span></span>
<span data-ttu-id="b6ff0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6ff0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6ff0-110">Permission type</span></span>|<span data-ttu-id="b6ff0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6ff0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6ff0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6ff0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6ff0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6ff0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6ff0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6ff0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6ff0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-115">Not supported.</span></span>|
|<span data-ttu-id="b6ff0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6ff0-116">Application</span></span>|<span data-ttu-id="b6ff0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6ff0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6ff0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b6ff0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6ff0-119">Request headers</span></span>
|<span data-ttu-id="b6ff0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6ff0-120">Header</span></span>|<span data-ttu-id="b6ff0-121">値</span><span class="sxs-lookup"><span data-stu-id="b6ff0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6ff0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6ff0-122">Authorization</span></span>|<span data-ttu-id="b6ff0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6ff0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b6ff0-124">Accept</span></span>|<span data-ttu-id="b6ff0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6ff0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6ff0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6ff0-126">Request body</span></span>
<span data-ttu-id="b6ff0-127">要求本文で、windowsAppX オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="b6ff0-128">次の表に、windowsAppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="b6ff0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6ff0-129">Property</span></span>|<span data-ttu-id="b6ff0-130">型</span><span class="sxs-lookup"><span data-stu-id="b6ff0-130">Type</span></span>|<span data-ttu-id="b6ff0-131">説明</span><span class="sxs-lookup"><span data-stu-id="b6ff0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6ff0-132">id</span><span class="sxs-lookup"><span data-stu-id="b6ff0-132">id</span></span>|<span data-ttu-id="b6ff0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b6ff0-133">String</span></span>|<span data-ttu-id="b6ff0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-134">Key of the entity.</span></span> <span data-ttu-id="b6ff0-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b6ff0-136">displayName</span></span>|<span data-ttu-id="b6ff0-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b6ff0-137">String</span></span>|<span data-ttu-id="b6ff0-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b6ff0-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-140">description</span><span class="sxs-lookup"><span data-stu-id="b6ff0-140">description</span></span>|<span data-ttu-id="b6ff0-141">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-141">String</span></span>|<span data-ttu-id="b6ff0-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-142">The description of the app.</span></span> <span data-ttu-id="b6ff0-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b6ff0-144">publisher</span></span>|<span data-ttu-id="b6ff0-145">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-145">String</span></span>|<span data-ttu-id="b6ff0-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-146">The publisher of the app.</span></span> <span data-ttu-id="b6ff0-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b6ff0-148">largeIcon</span></span>|[<span data-ttu-id="b6ff0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b6ff0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b6ff0-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b6ff0-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6ff0-152">createdDateTime</span></span>|<span data-ttu-id="b6ff0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6ff0-153">DateTimeOffset</span></span>|<span data-ttu-id="b6ff0-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-154">The date and time the app was created.</span></span> <span data-ttu-id="b6ff0-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6ff0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b6ff0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6ff0-157">DateTimeOffset</span></span>|<span data-ttu-id="b6ff0-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b6ff0-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b6ff0-160">isFeatured</span></span>|<span data-ttu-id="b6ff0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6ff0-161">Boolean</span></span>|<span data-ttu-id="b6ff0-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b6ff0-163">privacyInformationUrl</span></span>|<span data-ttu-id="b6ff0-164">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-164">String</span></span>|<span data-ttu-id="b6ff0-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-165">The privacy statement Url.</span></span> <span data-ttu-id="b6ff0-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b6ff0-167">informationUrl</span></span>|<span data-ttu-id="b6ff0-168">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-168">String</span></span>|<span data-ttu-id="b6ff0-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-169">The more information Url.</span></span> <span data-ttu-id="b6ff0-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-171">owner</span><span class="sxs-lookup"><span data-stu-id="b6ff0-171">owner</span></span>|<span data-ttu-id="b6ff0-172">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-172">String</span></span>|<span data-ttu-id="b6ff0-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-173">The owner of the app.</span></span> <span data-ttu-id="b6ff0-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-175">developer</span><span class="sxs-lookup"><span data-stu-id="b6ff0-175">developer</span></span>|<span data-ttu-id="b6ff0-176">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-176">String</span></span>|<span data-ttu-id="b6ff0-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-177">The developer of the app.</span></span> <span data-ttu-id="b6ff0-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-179">notes</span><span class="sxs-lookup"><span data-stu-id="b6ff0-179">notes</span></span>|<span data-ttu-id="b6ff0-180">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-180">String</span></span>|<span data-ttu-id="b6ff0-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-181">Notes for the app.</span></span> <span data-ttu-id="b6ff0-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b6ff0-183">uploadState</span></span>|<span data-ttu-id="b6ff0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ff0-184">Int32</span></span>|<span data-ttu-id="b6ff0-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-185">The upload state.</span></span> <span data-ttu-id="b6ff0-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b6ff0-187">publishingState</span></span>|[<span data-ttu-id="b6ff0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b6ff0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b6ff0-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-189">The publishing state for the app.</span></span> <span data-ttu-id="b6ff0-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b6ff0-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b6ff0-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b6ff0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b6ff0-193">isAssigned</span></span>|<span data-ttu-id="b6ff0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6ff0-194">Boolean</span></span>|<span data-ttu-id="b6ff0-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b6ff0-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6ff0-197">roleScopeTagIds</span></span>|<span data-ttu-id="b6ff0-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b6ff0-198">String collection</span></span>|<span data-ttu-id="b6ff0-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b6ff0-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b6ff0-201">dependentAppCount</span></span>|<span data-ttu-id="b6ff0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ff0-202">Int32</span></span>|<span data-ttu-id="b6ff0-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b6ff0-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6ff0-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b6ff0-205">committedContentVersion</span></span>|<span data-ttu-id="b6ff0-206">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-206">String</span></span>|<span data-ttu-id="b6ff0-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-207">The internal committed content version.</span></span> <span data-ttu-id="b6ff0-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6ff0-209">fileName</span><span class="sxs-lookup"><span data-stu-id="b6ff0-209">fileName</span></span>|<span data-ttu-id="b6ff0-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b6ff0-210">String</span></span>|<span data-ttu-id="b6ff0-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-211">The name of the main Lob application file.</span></span> <span data-ttu-id="b6ff0-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6ff0-213">size</span><span class="sxs-lookup"><span data-stu-id="b6ff0-213">size</span></span>|<span data-ttu-id="b6ff0-214">Int64</span><span class="sxs-lookup"><span data-stu-id="b6ff0-214">Int64</span></span>|<span data-ttu-id="b6ff0-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="b6ff0-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6ff0-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6ff0-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b6ff0-217">applicableArchitectures</span></span>|[<span data-ttu-id="b6ff0-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b6ff0-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b6ff0-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b6ff0-220">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b6ff0-221">identityName</span><span class="sxs-lookup"><span data-stu-id="b6ff0-221">identityName</span></span>|<span data-ttu-id="b6ff0-222">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-222">String</span></span>|<span data-ttu-id="b6ff0-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-223">The Identity Name.</span></span>|
|<span data-ttu-id="b6ff0-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b6ff0-224">identityPublisherHash</span></span>|<span data-ttu-id="b6ff0-225">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-225">String</span></span>|<span data-ttu-id="b6ff0-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="b6ff0-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6ff0-227">identityResourceIdentifier</span></span>|<span data-ttu-id="b6ff0-228">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-228">String</span></span>|<span data-ttu-id="b6ff0-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b6ff0-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="b6ff0-230">isBundle</span></span>|<span data-ttu-id="b6ff0-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6ff0-231">Boolean</span></span>|<span data-ttu-id="b6ff0-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="b6ff0-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6ff0-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b6ff0-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6ff0-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b6ff0-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b6ff0-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b6ff0-236">identityVersion</span></span>|<span data-ttu-id="b6ff0-237">String</span><span class="sxs-lookup"><span data-stu-id="b6ff0-237">String</span></span>|<span data-ttu-id="b6ff0-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b6ff0-239">応答</span><span class="sxs-lookup"><span data-stu-id="b6ff0-239">Response</span></span>
<span data-ttu-id="b6ff0-240">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-240">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6ff0-241">例</span><span class="sxs-lookup"><span data-stu-id="b6ff0-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6ff0-242">要求</span><span class="sxs-lookup"><span data-stu-id="b6ff0-242">Request</span></span>
<span data-ttu-id="b6ff0-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6ff0-244">応答</span><span class="sxs-lookup"><span data-stu-id="b6ff0-244">Response</span></span>
<span data-ttu-id="b6ff0-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6ff0-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





