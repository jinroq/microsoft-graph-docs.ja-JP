---
title: androidStoreApp の作成
description: 新しい androidStoreApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa67da6ecbf1a2d0b508c228265998b69b86c4f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401937"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="c8e78-103">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="c8e78-103">Create androidStoreApp</span></span>

> <span data-ttu-id="c8e78-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8e78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8e78-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8e78-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e78-107">新しい [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8e78-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8e78-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8e78-108">Prerequisites</span></span>
<span data-ttu-id="c8e78-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8e78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8e78-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8e78-111">Permission type</span></span>|<span data-ttu-id="c8e78-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8e78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8e78-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8e78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8e78-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e78-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8e78-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8e78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8e78-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8e78-116">Not supported.</span></span>|
|<span data-ttu-id="c8e78-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8e78-117">Application</span></span>|<span data-ttu-id="c8e78-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8e78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e78-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8e78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c8e78-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8e78-120">Request headers</span></span>
|<span data-ttu-id="c8e78-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8e78-121">Header</span></span>|<span data-ttu-id="c8e78-122">値</span><span class="sxs-lookup"><span data-stu-id="c8e78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8e78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8e78-123">Authorization</span></span>|<span data-ttu-id="c8e78-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8e78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8e78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8e78-125">Accept</span></span>|<span data-ttu-id="c8e78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e78-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8e78-127">Request body</span></span>
<span data-ttu-id="c8e78-128">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8e78-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="c8e78-129">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8e78-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="c8e78-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8e78-130">Property</span></span>|<span data-ttu-id="c8e78-131">型</span><span class="sxs-lookup"><span data-stu-id="c8e78-131">Type</span></span>|<span data-ttu-id="c8e78-132">説明</span><span class="sxs-lookup"><span data-stu-id="c8e78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e78-133">id</span><span class="sxs-lookup"><span data-stu-id="c8e78-133">id</span></span>|<span data-ttu-id="c8e78-134">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-134">String</span></span>|<span data-ttu-id="c8e78-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8e78-135">Key of the entity.</span></span> <span data-ttu-id="c8e78-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c8e78-137">displayName</span></span>|<span data-ttu-id="c8e78-138">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-138">String</span></span>|<span data-ttu-id="c8e78-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c8e78-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c8e78-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-141">説明</span><span class="sxs-lookup"><span data-stu-id="c8e78-141">description</span></span>|<span data-ttu-id="c8e78-142">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-142">String</span></span>|<span data-ttu-id="c8e78-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c8e78-143">The description of the app.</span></span> <span data-ttu-id="c8e78-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c8e78-145">publisher</span></span>|<span data-ttu-id="c8e78-146">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-146">String</span></span>|<span data-ttu-id="c8e78-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c8e78-147">The publisher of the app.</span></span> <span data-ttu-id="c8e78-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c8e78-149">largeIcon</span></span>|[<span data-ttu-id="c8e78-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c8e78-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c8e78-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="c8e78-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c8e78-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8e78-153">createdDateTime</span></span>|<span data-ttu-id="c8e78-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e78-154">DateTimeOffset</span></span>|<span data-ttu-id="c8e78-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c8e78-155">The date and time the app was created.</span></span> <span data-ttu-id="c8e78-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8e78-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c8e78-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e78-158">DateTimeOffset</span></span>|<span data-ttu-id="c8e78-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c8e78-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c8e78-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c8e78-161">isFeatured</span></span>|<span data-ttu-id="c8e78-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8e78-162">Boolean</span></span>|<span data-ttu-id="c8e78-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c8e78-164">privacyInformationUrl</span></span>|<span data-ttu-id="c8e78-165">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-165">String</span></span>|<span data-ttu-id="c8e78-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c8e78-166">The privacy statement Url.</span></span> <span data-ttu-id="c8e78-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c8e78-168">informationUrl</span></span>|<span data-ttu-id="c8e78-169">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-169">String</span></span>|<span data-ttu-id="c8e78-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c8e78-170">The more information Url.</span></span> <span data-ttu-id="c8e78-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-172">owner</span><span class="sxs-lookup"><span data-stu-id="c8e78-172">owner</span></span>|<span data-ttu-id="c8e78-173">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-173">String</span></span>|<span data-ttu-id="c8e78-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c8e78-174">The owner of the app.</span></span> <span data-ttu-id="c8e78-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-176">developer</span><span class="sxs-lookup"><span data-stu-id="c8e78-176">developer</span></span>|<span data-ttu-id="c8e78-177">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-177">String</span></span>|<span data-ttu-id="c8e78-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c8e78-178">The developer of the app.</span></span> <span data-ttu-id="c8e78-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-180">notes</span><span class="sxs-lookup"><span data-stu-id="c8e78-180">notes</span></span>|<span data-ttu-id="c8e78-181">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-181">String</span></span>|<span data-ttu-id="c8e78-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c8e78-182">Notes for the app.</span></span> <span data-ttu-id="c8e78-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c8e78-184">uploadState</span></span>|<span data-ttu-id="c8e78-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c8e78-185">Int32</span></span>|<span data-ttu-id="c8e78-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-186">The upload state.</span></span> <span data-ttu-id="c8e78-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c8e78-188">publishingState</span></span>|[<span data-ttu-id="c8e78-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c8e78-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c8e78-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c8e78-190">The publishing state for the app.</span></span> <span data-ttu-id="c8e78-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c8e78-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c8e78-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c8e78-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c8e78-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c8e78-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c8e78-194">isAssigned</span></span>|<span data-ttu-id="c8e78-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8e78-195">Boolean</span></span>|<span data-ttu-id="c8e78-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c8e78-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8e78-198">roleScopeTagIds</span></span>|<span data-ttu-id="c8e78-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c8e78-199">String collection</span></span>|<span data-ttu-id="c8e78-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c8e78-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8e78-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8e78-202">packageId</span><span class="sxs-lookup"><span data-stu-id="c8e78-202">packageId</span></span>|<span data-ttu-id="c8e78-203">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-203">String</span></span>|<span data-ttu-id="c8e78-204">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="c8e78-204">The package identifier.</span></span>|
|<span data-ttu-id="c8e78-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8e78-205">appIdentifier</span></span>|<span data-ttu-id="c8e78-206">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-206">String</span></span>|<span data-ttu-id="c8e78-207">ID 名。</span><span class="sxs-lookup"><span data-stu-id="c8e78-207">The Identity Name.</span></span>|
|<span data-ttu-id="c8e78-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c8e78-208">appStoreUrl</span></span>|<span data-ttu-id="c8e78-209">String</span><span class="sxs-lookup"><span data-stu-id="c8e78-209">String</span></span>|<span data-ttu-id="c8e78-210">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="c8e78-210">The Android app store URL.</span></span>|
|<span data-ttu-id="c8e78-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c8e78-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c8e78-212">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c8e78-212">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c8e78-213">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-213">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c8e78-214">応答</span><span class="sxs-lookup"><span data-stu-id="c8e78-214">Response</span></span>
<span data-ttu-id="c8e78-215">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8e78-215">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e78-216">例</span><span class="sxs-lookup"><span data-stu-id="c8e78-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8e78-217">要求</span><span class="sxs-lookup"><span data-stu-id="c8e78-217">Request</span></span>
<span data-ttu-id="c8e78-218">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8e78-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1203

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c8e78-219">応答</span><span class="sxs-lookup"><span data-stu-id="c8e78-219">Response</span></span>
<span data-ttu-id="c8e78-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8e78-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1375

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




