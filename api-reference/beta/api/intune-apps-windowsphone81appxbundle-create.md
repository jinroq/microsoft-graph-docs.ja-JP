---
title: windowsPhone81AppXBundle を作成する
description: 新しい windowsPhone81AppXBundle オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e0c59bcfc3a976ea0ec077444f28e854e2da465
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32487848"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="7ebc9-103">windowsPhone81AppXBundle を作成する</span><span class="sxs-lookup"><span data-stu-id="7ebc9-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="7ebc9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ebc9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ebc9-106">新しい[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ebc9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7ebc9-107">Prerequisites</span></span>
<span data-ttu-id="7ebc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ebc9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ebc9-110">Permission type</span></span>|<span data-ttu-id="7ebc9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ebc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ebc9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ebc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ebc9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebc9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ebc9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ebc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ebc9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-115">Not supported.</span></span>|
|<span data-ttu-id="7ebc9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ebc9-116">Application</span></span>|<span data-ttu-id="7ebc9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ebc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ebc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7ebc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ebc9-119">Request headers</span></span>
|<span data-ttu-id="7ebc9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ebc9-120">Header</span></span>|<span data-ttu-id="7ebc9-121">値</span><span class="sxs-lookup"><span data-stu-id="7ebc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ebc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ebc9-122">Authorization</span></span>|<span data-ttu-id="7ebc9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ebc9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7ebc9-124">Accept</span></span>|<span data-ttu-id="7ebc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ebc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ebc9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ebc9-126">Request body</span></span>
<span data-ttu-id="7ebc9-127">要求本文で、windowsPhone81AppXBundle オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="7ebc9-128">次の表に、windowsPhone81AppXBundle の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="7ebc9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ebc9-129">Property</span></span>|<span data-ttu-id="7ebc9-130">型</span><span class="sxs-lookup"><span data-stu-id="7ebc9-130">Type</span></span>|<span data-ttu-id="7ebc9-131">説明</span><span class="sxs-lookup"><span data-stu-id="7ebc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ebc9-132">id</span><span class="sxs-lookup"><span data-stu-id="7ebc9-132">id</span></span>|<span data-ttu-id="7ebc9-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7ebc9-133">String</span></span>|<span data-ttu-id="7ebc9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-134">Key of the entity.</span></span> <span data-ttu-id="7ebc9-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ebc9-136">displayName</span></span>|<span data-ttu-id="7ebc9-137">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-137">String</span></span>|<span data-ttu-id="7ebc9-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7ebc9-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-140">説明</span><span class="sxs-lookup"><span data-stu-id="7ebc9-140">description</span></span>|<span data-ttu-id="7ebc9-141">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-141">String</span></span>|<span data-ttu-id="7ebc9-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-142">The description of the app.</span></span> <span data-ttu-id="7ebc9-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7ebc9-144">publisher</span></span>|<span data-ttu-id="7ebc9-145">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-145">String</span></span>|<span data-ttu-id="7ebc9-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-146">The publisher of the app.</span></span> <span data-ttu-id="7ebc9-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7ebc9-148">largeIcon</span></span>|[<span data-ttu-id="7ebc9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ebc9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ebc9-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7ebc9-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ebc9-152">createdDateTime</span></span>|<span data-ttu-id="7ebc9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ebc9-153">DateTimeOffset</span></span>|<span data-ttu-id="7ebc9-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-154">The date and time the app was created.</span></span> <span data-ttu-id="7ebc9-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ebc9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7ebc9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ebc9-157">DateTimeOffset</span></span>|<span data-ttu-id="7ebc9-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7ebc9-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7ebc9-160">isFeatured</span></span>|<span data-ttu-id="7ebc9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ebc9-161">Boolean</span></span>|<span data-ttu-id="7ebc9-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7ebc9-163">privacyInformationUrl</span></span>|<span data-ttu-id="7ebc9-164">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-164">String</span></span>|<span data-ttu-id="7ebc9-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-165">The privacy statement Url.</span></span> <span data-ttu-id="7ebc9-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7ebc9-167">informationUrl</span></span>|<span data-ttu-id="7ebc9-168">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-168">String</span></span>|<span data-ttu-id="7ebc9-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-169">The more information Url.</span></span> <span data-ttu-id="7ebc9-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-171">owner</span><span class="sxs-lookup"><span data-stu-id="7ebc9-171">owner</span></span>|<span data-ttu-id="7ebc9-172">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-172">String</span></span>|<span data-ttu-id="7ebc9-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-173">The owner of the app.</span></span> <span data-ttu-id="7ebc9-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-175">developer</span><span class="sxs-lookup"><span data-stu-id="7ebc9-175">developer</span></span>|<span data-ttu-id="7ebc9-176">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-176">String</span></span>|<span data-ttu-id="7ebc9-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-177">The developer of the app.</span></span> <span data-ttu-id="7ebc9-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-179">notes</span><span class="sxs-lookup"><span data-stu-id="7ebc9-179">notes</span></span>|<span data-ttu-id="7ebc9-180">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-180">String</span></span>|<span data-ttu-id="7ebc9-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-181">Notes for the app.</span></span> <span data-ttu-id="7ebc9-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7ebc9-183">uploadState</span></span>|<span data-ttu-id="7ebc9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7ebc9-184">Int32</span></span>|<span data-ttu-id="7ebc9-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-185">The upload state.</span></span> <span data-ttu-id="7ebc9-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7ebc9-187">publishingState</span></span>|[<span data-ttu-id="7ebc9-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7ebc9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7ebc9-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-189">The publishing state for the app.</span></span> <span data-ttu-id="7ebc9-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7ebc9-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7ebc9-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7ebc9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7ebc9-193">isAssigned</span></span>|<span data-ttu-id="7ebc9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ebc9-194">Boolean</span></span>|<span data-ttu-id="7ebc9-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7ebc9-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ebc9-197">roleScopeTagIds</span></span>|<span data-ttu-id="7ebc9-198">String collection</span><span class="sxs-lookup"><span data-stu-id="7ebc9-198">String collection</span></span>|<span data-ttu-id="7ebc9-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7ebc9-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="7ebc9-201">dependentAppCount</span></span>|<span data-ttu-id="7ebc9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7ebc9-202">Int32</span></span>|<span data-ttu-id="7ebc9-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7ebc9-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ebc9-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7ebc9-205">committedContentVersion</span></span>|<span data-ttu-id="7ebc9-206">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-206">String</span></span>|<span data-ttu-id="7ebc9-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-207">The internal committed content version.</span></span> <span data-ttu-id="7ebc9-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ebc9-209">fileName</span><span class="sxs-lookup"><span data-stu-id="7ebc9-209">fileName</span></span>|<span data-ttu-id="7ebc9-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7ebc9-210">String</span></span>|<span data-ttu-id="7ebc9-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-211">The name of the main Lob application file.</span></span> <span data-ttu-id="7ebc9-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ebc9-213">size</span><span class="sxs-lookup"><span data-stu-id="7ebc9-213">size</span></span>|<span data-ttu-id="7ebc9-214">Int64</span><span class="sxs-lookup"><span data-stu-id="7ebc9-214">Int64</span></span>|<span data-ttu-id="7ebc9-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="7ebc9-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ebc9-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ebc9-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7ebc9-217">applicableArchitectures</span></span>|[<span data-ttu-id="7ebc9-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7ebc9-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7ebc9-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7ebc9-220">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="7ebc9-221">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7ebc9-222">identityName</span><span class="sxs-lookup"><span data-stu-id="7ebc9-222">identityName</span></span>|<span data-ttu-id="7ebc9-223">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-223">String</span></span>|<span data-ttu-id="7ebc9-224">ID 名。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-224">The Identity Name.</span></span> <span data-ttu-id="7ebc9-225">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7ebc9-226">identityPublisherHash</span></span>|<span data-ttu-id="7ebc9-227">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-227">String</span></span>|<span data-ttu-id="7ebc9-228">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="7ebc9-229">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7ebc9-230">identityResourceIdentifier</span></span>|<span data-ttu-id="7ebc9-231">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-231">String</span></span>|<span data-ttu-id="7ebc9-232">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="7ebc9-233">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ebc9-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7ebc9-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ebc9-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7ebc9-236">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="7ebc9-237">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="7ebc9-238">phoneProductIdentifier</span></span>|<span data-ttu-id="7ebc9-239">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-239">String</span></span>|<span data-ttu-id="7ebc9-240">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-240">The Phone Product Identifier.</span></span> <span data-ttu-id="7ebc9-241">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="7ebc9-242">phonePublisherId</span></span>|<span data-ttu-id="7ebc9-243">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-243">String</span></span>|<span data-ttu-id="7ebc9-244">電話の発行元 Id。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7ebc9-245">identityVersion</span></span>|<span data-ttu-id="7ebc9-246">String</span><span class="sxs-lookup"><span data-stu-id="7ebc9-246">String</span></span>|<span data-ttu-id="7ebc9-247">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-247">The identity version.</span></span> <span data-ttu-id="7ebc9-248">[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ebc9-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="7ebc9-249">appXPackageInformationList</span></span>|<span data-ttu-id="7ebc9-250">[windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ebc9-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="7ebc9-251">AppX パッケージ情報のリスト。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="7ebc9-252">応答</span><span class="sxs-lookup"><span data-stu-id="7ebc9-252">Response</span></span>
<span data-ttu-id="7ebc9-253">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ebc9-254">例</span><span class="sxs-lookup"><span data-stu-id="7ebc9-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ebc9-255">要求</span><span class="sxs-lookup"><span data-stu-id="7ebc9-255">Request</span></span>
<span data-ttu-id="7ebc9-256">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="7ebc9-257">応答</span><span class="sxs-lookup"><span data-stu-id="7ebc9-257">Response</span></span>
<span data-ttu-id="7ebc9-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ebc9-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





