---
title: windowsPhone81AppX を作成する
description: 新しい windowsPhone81AppX オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eae471c839a8ad69d444d458c2fd2b1b32e9f23c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32487764"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="62a9a-103">windowsPhone81AppX を作成する</span><span class="sxs-lookup"><span data-stu-id="62a9a-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="62a9a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62a9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62a9a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62a9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a9a-106">新しい[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="62a9a-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a9a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62a9a-107">Prerequisites</span></span>
<span data-ttu-id="62a9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62a9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a9a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62a9a-110">Permission type</span></span>|<span data-ttu-id="62a9a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62a9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a9a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62a9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62a9a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a9a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62a9a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62a9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a9a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62a9a-115">Not supported.</span></span>|
|<span data-ttu-id="62a9a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62a9a-116">Application</span></span>|<span data-ttu-id="62a9a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62a9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a9a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62a9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="62a9a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62a9a-119">Request headers</span></span>
|<span data-ttu-id="62a9a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62a9a-120">Header</span></span>|<span data-ttu-id="62a9a-121">値</span><span class="sxs-lookup"><span data-stu-id="62a9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a9a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62a9a-122">Authorization</span></span>|<span data-ttu-id="62a9a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62a9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a9a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62a9a-124">Accept</span></span>|<span data-ttu-id="62a9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62a9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a9a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62a9a-126">Request body</span></span>
<span data-ttu-id="62a9a-127">要求本文で、windowsPhone81AppX オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62a9a-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="62a9a-128">次の表に、windowsPhone81AppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62a9a-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="62a9a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62a9a-129">Property</span></span>|<span data-ttu-id="62a9a-130">型</span><span class="sxs-lookup"><span data-stu-id="62a9a-130">Type</span></span>|<span data-ttu-id="62a9a-131">説明</span><span class="sxs-lookup"><span data-stu-id="62a9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a9a-132">id</span><span class="sxs-lookup"><span data-stu-id="62a9a-132">id</span></span>|<span data-ttu-id="62a9a-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="62a9a-133">String</span></span>|<span data-ttu-id="62a9a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62a9a-134">Key of the entity.</span></span> <span data-ttu-id="62a9a-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="62a9a-136">displayName</span></span>|<span data-ttu-id="62a9a-137">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-137">String</span></span>|<span data-ttu-id="62a9a-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="62a9a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="62a9a-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-140">説明</span><span class="sxs-lookup"><span data-stu-id="62a9a-140">description</span></span>|<span data-ttu-id="62a9a-141">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-141">String</span></span>|<span data-ttu-id="62a9a-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="62a9a-142">The description of the app.</span></span> <span data-ttu-id="62a9a-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="62a9a-144">publisher</span></span>|<span data-ttu-id="62a9a-145">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-145">String</span></span>|<span data-ttu-id="62a9a-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="62a9a-146">The publisher of the app.</span></span> <span data-ttu-id="62a9a-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="62a9a-148">largeIcon</span></span>|[<span data-ttu-id="62a9a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62a9a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62a9a-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="62a9a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="62a9a-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62a9a-152">createdDateTime</span></span>|<span data-ttu-id="62a9a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a9a-153">DateTimeOffset</span></span>|<span data-ttu-id="62a9a-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="62a9a-154">The date and time the app was created.</span></span> <span data-ttu-id="62a9a-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62a9a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="62a9a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a9a-157">DateTimeOffset</span></span>|<span data-ttu-id="62a9a-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="62a9a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="62a9a-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="62a9a-160">isFeatured</span></span>|<span data-ttu-id="62a9a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="62a9a-161">Boolean</span></span>|<span data-ttu-id="62a9a-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="62a9a-163">privacyInformationUrl</span></span>|<span data-ttu-id="62a9a-164">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-164">String</span></span>|<span data-ttu-id="62a9a-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="62a9a-165">The privacy statement Url.</span></span> <span data-ttu-id="62a9a-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="62a9a-167">informationUrl</span></span>|<span data-ttu-id="62a9a-168">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-168">String</span></span>|<span data-ttu-id="62a9a-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="62a9a-169">The more information Url.</span></span> <span data-ttu-id="62a9a-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-171">owner</span><span class="sxs-lookup"><span data-stu-id="62a9a-171">owner</span></span>|<span data-ttu-id="62a9a-172">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-172">String</span></span>|<span data-ttu-id="62a9a-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="62a9a-173">The owner of the app.</span></span> <span data-ttu-id="62a9a-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-175">developer</span><span class="sxs-lookup"><span data-stu-id="62a9a-175">developer</span></span>|<span data-ttu-id="62a9a-176">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-176">String</span></span>|<span data-ttu-id="62a9a-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="62a9a-177">The developer of the app.</span></span> <span data-ttu-id="62a9a-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-179">notes</span><span class="sxs-lookup"><span data-stu-id="62a9a-179">notes</span></span>|<span data-ttu-id="62a9a-180">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-180">String</span></span>|<span data-ttu-id="62a9a-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="62a9a-181">Notes for the app.</span></span> <span data-ttu-id="62a9a-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="62a9a-183">uploadState</span></span>|<span data-ttu-id="62a9a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="62a9a-184">Int32</span></span>|<span data-ttu-id="62a9a-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="62a9a-185">The upload state.</span></span> <span data-ttu-id="62a9a-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="62a9a-187">publishingState</span></span>|[<span data-ttu-id="62a9a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="62a9a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="62a9a-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="62a9a-189">The publishing state for the app.</span></span> <span data-ttu-id="62a9a-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="62a9a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="62a9a-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62a9a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="62a9a-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="62a9a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="62a9a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="62a9a-193">isAssigned</span></span>|<span data-ttu-id="62a9a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="62a9a-194">Boolean</span></span>|<span data-ttu-id="62a9a-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="62a9a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="62a9a-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62a9a-197">roleScopeTagIds</span></span>|<span data-ttu-id="62a9a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="62a9a-198">String collection</span></span>|<span data-ttu-id="62a9a-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="62a9a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="62a9a-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="62a9a-201">dependentAppCount</span></span>|<span data-ttu-id="62a9a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="62a9a-202">Int32</span></span>|<span data-ttu-id="62a9a-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="62a9a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="62a9a-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="62a9a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="62a9a-205">committedContentVersion</span></span>|<span data-ttu-id="62a9a-206">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-206">String</span></span>|<span data-ttu-id="62a9a-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="62a9a-207">The internal committed content version.</span></span> <span data-ttu-id="62a9a-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="62a9a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="62a9a-209">fileName</span></span>|<span data-ttu-id="62a9a-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="62a9a-210">String</span></span>|<span data-ttu-id="62a9a-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="62a9a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="62a9a-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="62a9a-213">size</span><span class="sxs-lookup"><span data-stu-id="62a9a-213">size</span></span>|<span data-ttu-id="62a9a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="62a9a-214">Int64</span></span>|<span data-ttu-id="62a9a-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="62a9a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="62a9a-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="62a9a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="62a9a-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="62a9a-217">applicableArchitectures</span></span>|[<span data-ttu-id="62a9a-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="62a9a-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="62a9a-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="62a9a-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="62a9a-220">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="62a9a-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="62a9a-221">identityName</span><span class="sxs-lookup"><span data-stu-id="62a9a-221">identityName</span></span>|<span data-ttu-id="62a9a-222">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-222">String</span></span>|<span data-ttu-id="62a9a-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="62a9a-223">The Identity Name.</span></span>|
|<span data-ttu-id="62a9a-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="62a9a-224">identityPublisherHash</span></span>|<span data-ttu-id="62a9a-225">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-225">String</span></span>|<span data-ttu-id="62a9a-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="62a9a-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="62a9a-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="62a9a-227">identityResourceIdentifier</span></span>|<span data-ttu-id="62a9a-228">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-228">String</span></span>|<span data-ttu-id="62a9a-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="62a9a-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="62a9a-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="62a9a-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="62a9a-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="62a9a-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="62a9a-232">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="62a9a-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="62a9a-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="62a9a-233">phoneProductIdentifier</span></span>|<span data-ttu-id="62a9a-234">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-234">String</span></span>|<span data-ttu-id="62a9a-235">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="62a9a-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="62a9a-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="62a9a-236">phonePublisherId</span></span>|<span data-ttu-id="62a9a-237">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-237">String</span></span>|<span data-ttu-id="62a9a-238">電話の発行元 Id。</span><span class="sxs-lookup"><span data-stu-id="62a9a-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="62a9a-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="62a9a-239">identityVersion</span></span>|<span data-ttu-id="62a9a-240">String</span><span class="sxs-lookup"><span data-stu-id="62a9a-240">String</span></span>|<span data-ttu-id="62a9a-241">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="62a9a-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="62a9a-242">応答</span><span class="sxs-lookup"><span data-stu-id="62a9a-242">Response</span></span>
<span data-ttu-id="62a9a-243">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62a9a-243">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a9a-244">例</span><span class="sxs-lookup"><span data-stu-id="62a9a-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a9a-245">要求</span><span class="sxs-lookup"><span data-stu-id="62a9a-245">Request</span></span>
<span data-ttu-id="62a9a-246">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62a9a-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="62a9a-247">応答</span><span class="sxs-lookup"><span data-stu-id="62a9a-247">Response</span></span>
<span data-ttu-id="62a9a-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62a9a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





