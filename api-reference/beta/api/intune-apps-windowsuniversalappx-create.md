---
title: Create windowsUniversalAppX
description: 新しい windowsUniversalAppX オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc6678b950ca5894b5fd480e74f8a4ab4ed371dd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971564"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="7d8f6-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="7d8f6-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="7d8f6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d8f6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d8f6-106">新しい [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d8f6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d8f6-107">Prerequisites</span></span>
<span data-ttu-id="7d8f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d8f6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d8f6-110">Permission type</span></span>|<span data-ttu-id="7d8f6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d8f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d8f6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d8f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d8f6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8f6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d8f6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d8f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d8f6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-115">Not supported.</span></span>|
|<span data-ttu-id="7d8f6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d8f6-116">Application</span></span>|<span data-ttu-id="7d8f6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d8f6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d8f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7d8f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d8f6-119">Request headers</span></span>
|<span data-ttu-id="7d8f6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d8f6-120">Header</span></span>|<span data-ttu-id="7d8f6-121">値</span><span class="sxs-lookup"><span data-stu-id="7d8f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d8f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8f6-122">Authorization</span></span>|<span data-ttu-id="7d8f6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d8f6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7d8f6-124">Accept</span></span>|<span data-ttu-id="7d8f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d8f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d8f6-126">Request body</span></span>
<span data-ttu-id="7d8f6-127">要求本文で、windowsUniversalAppX オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="7d8f6-128">次の表に、windowsUniversalAppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="7d8f6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d8f6-129">Property</span></span>|<span data-ttu-id="7d8f6-130">型</span><span class="sxs-lookup"><span data-stu-id="7d8f6-130">Type</span></span>|<span data-ttu-id="7d8f6-131">説明</span><span class="sxs-lookup"><span data-stu-id="7d8f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d8f6-132">id</span><span class="sxs-lookup"><span data-stu-id="7d8f6-132">id</span></span>|<span data-ttu-id="7d8f6-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d8f6-133">String</span></span>|<span data-ttu-id="7d8f6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-134">Key of the entity.</span></span> <span data-ttu-id="7d8f6-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7d8f6-136">displayName</span></span>|<span data-ttu-id="7d8f6-137">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-137">String</span></span>|<span data-ttu-id="7d8f6-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7d8f6-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-140">description</span><span class="sxs-lookup"><span data-stu-id="7d8f6-140">description</span></span>|<span data-ttu-id="7d8f6-141">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-141">String</span></span>|<span data-ttu-id="7d8f6-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-142">The description of the app.</span></span> <span data-ttu-id="7d8f6-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7d8f6-144">publisher</span></span>|<span data-ttu-id="7d8f6-145">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-145">String</span></span>|<span data-ttu-id="7d8f6-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-146">The publisher of the app.</span></span> <span data-ttu-id="7d8f6-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7d8f6-148">largeIcon</span></span>|[<span data-ttu-id="7d8f6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7d8f6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7d8f6-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7d8f6-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d8f6-152">createdDateTime</span></span>|<span data-ttu-id="7d8f6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d8f6-153">DateTimeOffset</span></span>|<span data-ttu-id="7d8f6-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-154">The date and time the app was created.</span></span> <span data-ttu-id="7d8f6-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d8f6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7d8f6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d8f6-157">DateTimeOffset</span></span>|<span data-ttu-id="7d8f6-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7d8f6-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7d8f6-160">isFeatured</span></span>|<span data-ttu-id="7d8f6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d8f6-161">Boolean</span></span>|<span data-ttu-id="7d8f6-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7d8f6-163">privacyInformationUrl</span></span>|<span data-ttu-id="7d8f6-164">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-164">String</span></span>|<span data-ttu-id="7d8f6-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-165">The privacy statement Url.</span></span> <span data-ttu-id="7d8f6-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7d8f6-167">informationUrl</span></span>|<span data-ttu-id="7d8f6-168">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-168">String</span></span>|<span data-ttu-id="7d8f6-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-169">The more information Url.</span></span> <span data-ttu-id="7d8f6-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-171">owner</span><span class="sxs-lookup"><span data-stu-id="7d8f6-171">owner</span></span>|<span data-ttu-id="7d8f6-172">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-172">String</span></span>|<span data-ttu-id="7d8f6-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-173">The owner of the app.</span></span> <span data-ttu-id="7d8f6-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-175">developer</span><span class="sxs-lookup"><span data-stu-id="7d8f6-175">developer</span></span>|<span data-ttu-id="7d8f6-176">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-176">String</span></span>|<span data-ttu-id="7d8f6-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-177">The developer of the app.</span></span> <span data-ttu-id="7d8f6-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-179">notes</span><span class="sxs-lookup"><span data-stu-id="7d8f6-179">notes</span></span>|<span data-ttu-id="7d8f6-180">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-180">String</span></span>|<span data-ttu-id="7d8f6-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-181">Notes for the app.</span></span> <span data-ttu-id="7d8f6-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7d8f6-183">uploadState</span></span>|<span data-ttu-id="7d8f6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7d8f6-184">Int32</span></span>|<span data-ttu-id="7d8f6-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-185">The upload state.</span></span> <span data-ttu-id="7d8f6-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7d8f6-187">publishingState</span></span>|[<span data-ttu-id="7d8f6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7d8f6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7d8f6-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-189">The publishing state for the app.</span></span> <span data-ttu-id="7d8f6-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7d8f6-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7d8f6-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7d8f6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7d8f6-193">isAssigned</span></span>|<span data-ttu-id="7d8f6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d8f6-194">Boolean</span></span>|<span data-ttu-id="7d8f6-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7d8f6-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d8f6-197">roleScopeTagIds</span></span>|<span data-ttu-id="7d8f6-198">String collection</span><span class="sxs-lookup"><span data-stu-id="7d8f6-198">String collection</span></span>|<span data-ttu-id="7d8f6-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7d8f6-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7d8f6-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7d8f6-201">committedContentVersion</span></span>|<span data-ttu-id="7d8f6-202">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-202">String</span></span>|<span data-ttu-id="7d8f6-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-203">The internal committed content version.</span></span> <span data-ttu-id="7d8f6-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7d8f6-205">fileName</span><span class="sxs-lookup"><span data-stu-id="7d8f6-205">fileName</span></span>|<span data-ttu-id="7d8f6-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d8f6-206">String</span></span>|<span data-ttu-id="7d8f6-207">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-207">The name of the main Lob application file.</span></span> <span data-ttu-id="7d8f6-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7d8f6-209">size</span><span class="sxs-lookup"><span data-stu-id="7d8f6-209">size</span></span>|<span data-ttu-id="7d8f6-210">Int64</span><span class="sxs-lookup"><span data-stu-id="7d8f6-210">Int64</span></span>|<span data-ttu-id="7d8f6-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="7d8f6-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7d8f6-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7d8f6-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7d8f6-213">applicableArchitectures</span></span>|[<span data-ttu-id="7d8f6-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7d8f6-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7d8f6-215">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7d8f6-216">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7d8f6-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="7d8f6-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="7d8f6-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="7d8f6-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="7d8f6-219">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="7d8f6-220">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="7d8f6-221">identityName</span><span class="sxs-lookup"><span data-stu-id="7d8f6-221">identityName</span></span>|<span data-ttu-id="7d8f6-222">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-222">String</span></span>|<span data-ttu-id="7d8f6-223">ID 名。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-223">The Identity Name.</span></span>|
|<span data-ttu-id="7d8f6-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7d8f6-224">identityPublisherHash</span></span>|<span data-ttu-id="7d8f6-225">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-225">String</span></span>|<span data-ttu-id="7d8f6-226">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="7d8f6-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d8f6-227">identityResourceIdentifier</span></span>|<span data-ttu-id="7d8f6-228">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-228">String</span></span>|<span data-ttu-id="7d8f6-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7d8f6-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="7d8f6-230">isBundle</span></span>|<span data-ttu-id="7d8f6-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d8f6-231">Boolean</span></span>|<span data-ttu-id="7d8f6-232">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="7d8f6-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7d8f6-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7d8f6-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7d8f6-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7d8f6-235">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7d8f6-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7d8f6-236">identityVersion</span></span>|<span data-ttu-id="7d8f6-237">String</span><span class="sxs-lookup"><span data-stu-id="7d8f6-237">String</span></span>|<span data-ttu-id="7d8f6-238">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7d8f6-239">応答</span><span class="sxs-lookup"><span data-stu-id="7d8f6-239">Response</span></span>
<span data-ttu-id="7d8f6-240">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-240">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8f6-241">例</span><span class="sxs-lookup"><span data-stu-id="7d8f6-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d8f6-242">要求</span><span class="sxs-lookup"><span data-stu-id="7d8f6-242">Request</span></span>
<span data-ttu-id="7d8f6-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1388

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="7d8f6-244">応答</span><span class="sxs-lookup"><span data-stu-id="7d8f6-244">Response</span></span>
<span data-ttu-id="7d8f6-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d8f6-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1560

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




