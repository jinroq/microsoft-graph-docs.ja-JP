---
title: MacOsVppApp を作成します。
description: 新しい macOsVppApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 64ab6fcec54beab2de2da6a5ac44f0a6b49d8ea6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430408"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="98e2f-103">MacOsVppApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="98e2f-103">Create macOsVppApp</span></span>

> <span data-ttu-id="98e2f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98e2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98e2f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98e2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98e2f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98e2f-107">新しい[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="98e2f-107">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98e2f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="98e2f-108">Prerequisites</span></span>
<span data-ttu-id="98e2f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98e2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98e2f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98e2f-111">Permission type</span></span>|<span data-ttu-id="98e2f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="98e2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98e2f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98e2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98e2f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98e2f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98e2f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98e2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98e2f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98e2f-116">Not supported.</span></span>|
|<span data-ttu-id="98e2f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98e2f-117">Application</span></span>|<span data-ttu-id="98e2f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98e2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98e2f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98e2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="98e2f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98e2f-120">Request headers</span></span>
|<span data-ttu-id="98e2f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98e2f-121">Header</span></span>|<span data-ttu-id="98e2f-122">値</span><span class="sxs-lookup"><span data-stu-id="98e2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98e2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98e2f-123">Authorization</span></span>|<span data-ttu-id="98e2f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="98e2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98e2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98e2f-125">Accept</span></span>|<span data-ttu-id="98e2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98e2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98e2f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="98e2f-127">Request body</span></span>
<span data-ttu-id="98e2f-128">要求の本文に macOsVppApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="98e2f-128">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="98e2f-129">次の表は、macOsVppApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="98e2f-129">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="98e2f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98e2f-130">Property</span></span>|<span data-ttu-id="98e2f-131">型</span><span class="sxs-lookup"><span data-stu-id="98e2f-131">Type</span></span>|<span data-ttu-id="98e2f-132">説明</span><span class="sxs-lookup"><span data-stu-id="98e2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e2f-133">id</span><span class="sxs-lookup"><span data-stu-id="98e2f-133">id</span></span>|<span data-ttu-id="98e2f-134">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-134">String</span></span>|<span data-ttu-id="98e2f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="98e2f-135">Key of the entity.</span></span> <span data-ttu-id="98e2f-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="98e2f-137">displayName</span></span>|<span data-ttu-id="98e2f-138">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-138">String</span></span>|<span data-ttu-id="98e2f-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="98e2f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="98e2f-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-141">説明</span><span class="sxs-lookup"><span data-stu-id="98e2f-141">description</span></span>|<span data-ttu-id="98e2f-142">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-142">String</span></span>|<span data-ttu-id="98e2f-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="98e2f-143">The description of the app.</span></span> <span data-ttu-id="98e2f-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="98e2f-145">publisher</span></span>|<span data-ttu-id="98e2f-146">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-146">String</span></span>|<span data-ttu-id="98e2f-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="98e2f-147">The publisher of the app.</span></span> <span data-ttu-id="98e2f-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="98e2f-149">largeIcon</span></span>|[<span data-ttu-id="98e2f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="98e2f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="98e2f-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="98e2f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="98e2f-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98e2f-153">createdDateTime</span></span>|<span data-ttu-id="98e2f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e2f-154">DateTimeOffset</span></span>|<span data-ttu-id="98e2f-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="98e2f-155">The date and time the app was created.</span></span> <span data-ttu-id="98e2f-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98e2f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="98e2f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e2f-158">DateTimeOffset</span></span>|<span data-ttu-id="98e2f-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="98e2f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="98e2f-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="98e2f-161">isFeatured</span></span>|<span data-ttu-id="98e2f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e2f-162">Boolean</span></span>|<span data-ttu-id="98e2f-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="98e2f-164">privacyInformationUrl</span></span>|<span data-ttu-id="98e2f-165">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-165">String</span></span>|<span data-ttu-id="98e2f-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="98e2f-166">The privacy statement Url.</span></span> <span data-ttu-id="98e2f-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="98e2f-168">informationUrl</span></span>|<span data-ttu-id="98e2f-169">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-169">String</span></span>|<span data-ttu-id="98e2f-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="98e2f-170">The more information Url.</span></span> <span data-ttu-id="98e2f-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-172">owner</span><span class="sxs-lookup"><span data-stu-id="98e2f-172">owner</span></span>|<span data-ttu-id="98e2f-173">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-173">String</span></span>|<span data-ttu-id="98e2f-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="98e2f-174">The owner of the app.</span></span> <span data-ttu-id="98e2f-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-176">developer</span><span class="sxs-lookup"><span data-stu-id="98e2f-176">developer</span></span>|<span data-ttu-id="98e2f-177">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-177">String</span></span>|<span data-ttu-id="98e2f-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="98e2f-178">The developer of the app.</span></span> <span data-ttu-id="98e2f-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-180">notes</span><span class="sxs-lookup"><span data-stu-id="98e2f-180">notes</span></span>|<span data-ttu-id="98e2f-181">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-181">String</span></span>|<span data-ttu-id="98e2f-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="98e2f-182">Notes for the app.</span></span> <span data-ttu-id="98e2f-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="98e2f-184">uploadState</span></span>|<span data-ttu-id="98e2f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="98e2f-185">Int32</span></span>|<span data-ttu-id="98e2f-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-186">The upload state.</span></span> <span data-ttu-id="98e2f-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="98e2f-188">publishingState</span></span>|[<span data-ttu-id="98e2f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="98e2f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="98e2f-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="98e2f-190">The publishing state for the app.</span></span> <span data-ttu-id="98e2f-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="98e2f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="98e2f-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="98e2f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="98e2f-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="98e2f-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="98e2f-194">isAssigned</span></span>|<span data-ttu-id="98e2f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e2f-195">Boolean</span></span>|<span data-ttu-id="98e2f-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="98e2f-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98e2f-198">roleScopeTagIds</span></span>|<span data-ttu-id="98e2f-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="98e2f-199">String collection</span></span>|<span data-ttu-id="98e2f-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="98e2f-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98e2f-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98e2f-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="98e2f-202">usedLicenseCount</span></span>|<span data-ttu-id="98e2f-203">Int32</span><span class="sxs-lookup"><span data-stu-id="98e2f-203">Int32</span></span>|<span data-ttu-id="98e2f-204">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="98e2f-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="98e2f-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="98e2f-205">totalLicenseCount</span></span>|<span data-ttu-id="98e2f-206">Int32</span><span class="sxs-lookup"><span data-stu-id="98e2f-206">Int32</span></span>|<span data-ttu-id="98e2f-207">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="98e2f-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="98e2f-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="98e2f-208">releaseDateTime</span></span>|<span data-ttu-id="98e2f-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e2f-209">DateTimeOffset</span></span>|<span data-ttu-id="98e2f-210">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="98e2f-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="98e2f-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="98e2f-211">appStoreUrl</span></span>|<span data-ttu-id="98e2f-212">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-212">String</span></span>|<span data-ttu-id="98e2f-213">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="98e2f-213">The store URL.</span></span>|
|<span data-ttu-id="98e2f-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="98e2f-214">licensingType</span></span>|[<span data-ttu-id="98e2f-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="98e2f-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="98e2f-216">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="98e2f-216">The supported License Type.</span></span>|
|<span data-ttu-id="98e2f-217">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="98e2f-217">vppTokenOrganizationName</span></span>|<span data-ttu-id="98e2f-218">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-218">String</span></span>|<span data-ttu-id="98e2f-219">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="98e2f-219">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="98e2f-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="98e2f-220">vppTokenAccountType</span></span>|[<span data-ttu-id="98e2f-221">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="98e2f-221">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="98e2f-222">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="98e2f-222">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="98e2f-223">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-223">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="98e2f-224">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-224">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="98e2f-225">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="98e2f-225">vppTokenAppleId</span></span>|<span data-ttu-id="98e2f-226">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-226">String</span></span>|<span data-ttu-id="98e2f-227">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="98e2f-227">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="98e2f-228">bundleId</span><span class="sxs-lookup"><span data-stu-id="98e2f-228">bundleId</span></span>|<span data-ttu-id="98e2f-229">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-229">String</span></span>|<span data-ttu-id="98e2f-230">ID 名。</span><span class="sxs-lookup"><span data-stu-id="98e2f-230">The Identity Name.</span></span>|
|<span data-ttu-id="98e2f-231">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="98e2f-231">vppTokenId</span></span>|<span data-ttu-id="98e2f-232">String</span><span class="sxs-lookup"><span data-stu-id="98e2f-232">String</span></span>|<span data-ttu-id="98e2f-233">このアプリケーションに関連付けられている VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-233">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="98e2f-234">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="98e2f-234">revokeLicenseActionResults</span></span>|<span data-ttu-id="98e2f-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="98e2f-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="98e2f-236">結果は、このアプリケーションについてのライセンスを失効します。</span><span class="sxs-lookup"><span data-stu-id="98e2f-236">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="98e2f-237">応答</span><span class="sxs-lookup"><span data-stu-id="98e2f-237">Response</span></span>
<span data-ttu-id="98e2f-238">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="98e2f-238">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98e2f-239">例</span><span class="sxs-lookup"><span data-stu-id="98e2f-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="98e2f-240">要求</span><span class="sxs-lookup"><span data-stu-id="98e2f-240">Request</span></span>
<span data-ttu-id="98e2f-241">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98e2f-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="98e2f-242">応答</span><span class="sxs-lookup"><span data-stu-id="98e2f-242">Response</span></span>
<span data-ttu-id="98e2f-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98e2f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




