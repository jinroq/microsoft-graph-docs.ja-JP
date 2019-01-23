---
title: MacOsVppApp を更新します。
description: MacOsVppApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b34a8e4ae3e179cfa8674abb08565b5fbe0c72a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431637"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="f27a5-103">MacOsVppApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="f27a5-103">Update macOsVppApp</span></span>

> <span data-ttu-id="f27a5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f27a5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f27a5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f27a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f27a5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f27a5-107">[MacOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f27a5-107">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f27a5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f27a5-108">Prerequisites</span></span>
<span data-ttu-id="f27a5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f27a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f27a5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f27a5-111">Permission type</span></span>|<span data-ttu-id="f27a5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f27a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f27a5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f27a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f27a5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f27a5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f27a5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f27a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f27a5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f27a5-116">Not supported.</span></span>|
|<span data-ttu-id="f27a5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f27a5-117">Application</span></span>|<span data-ttu-id="f27a5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f27a5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f27a5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f27a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f27a5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f27a5-120">Request headers</span></span>
|<span data-ttu-id="f27a5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f27a5-121">Header</span></span>|<span data-ttu-id="f27a5-122">値</span><span class="sxs-lookup"><span data-stu-id="f27a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f27a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f27a5-123">Authorization</span></span>|<span data-ttu-id="f27a5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f27a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f27a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f27a5-125">Accept</span></span>|<span data-ttu-id="f27a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f27a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f27a5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f27a5-127">Request body</span></span>
<span data-ttu-id="f27a5-128">要求の本文に[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f27a5-128">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="f27a5-129">[MacOsVppApp](../resources/intune-apps-macosvppapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f27a5-129">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="f27a5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f27a5-130">Property</span></span>|<span data-ttu-id="f27a5-131">型</span><span class="sxs-lookup"><span data-stu-id="f27a5-131">Type</span></span>|<span data-ttu-id="f27a5-132">説明</span><span class="sxs-lookup"><span data-stu-id="f27a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f27a5-133">id</span><span class="sxs-lookup"><span data-stu-id="f27a5-133">id</span></span>|<span data-ttu-id="f27a5-134">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-134">String</span></span>|<span data-ttu-id="f27a5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f27a5-135">Key of the entity.</span></span> <span data-ttu-id="f27a5-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f27a5-137">displayName</span></span>|<span data-ttu-id="f27a5-138">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-138">String</span></span>|<span data-ttu-id="f27a5-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f27a5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f27a5-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-141">説明</span><span class="sxs-lookup"><span data-stu-id="f27a5-141">description</span></span>|<span data-ttu-id="f27a5-142">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-142">String</span></span>|<span data-ttu-id="f27a5-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f27a5-143">The description of the app.</span></span> <span data-ttu-id="f27a5-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f27a5-145">publisher</span></span>|<span data-ttu-id="f27a5-146">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-146">String</span></span>|<span data-ttu-id="f27a5-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f27a5-147">The publisher of the app.</span></span> <span data-ttu-id="f27a5-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f27a5-149">largeIcon</span></span>|[<span data-ttu-id="f27a5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f27a5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f27a5-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f27a5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f27a5-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f27a5-153">createdDateTime</span></span>|<span data-ttu-id="f27a5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f27a5-154">DateTimeOffset</span></span>|<span data-ttu-id="f27a5-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f27a5-155">The date and time the app was created.</span></span> <span data-ttu-id="f27a5-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f27a5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f27a5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f27a5-158">DateTimeOffset</span></span>|<span data-ttu-id="f27a5-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f27a5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f27a5-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f27a5-161">isFeatured</span></span>|<span data-ttu-id="f27a5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f27a5-162">Boolean</span></span>|<span data-ttu-id="f27a5-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f27a5-164">privacyInformationUrl</span></span>|<span data-ttu-id="f27a5-165">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-165">String</span></span>|<span data-ttu-id="f27a5-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f27a5-166">The privacy statement Url.</span></span> <span data-ttu-id="f27a5-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f27a5-168">informationUrl</span></span>|<span data-ttu-id="f27a5-169">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-169">String</span></span>|<span data-ttu-id="f27a5-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f27a5-170">The more information Url.</span></span> <span data-ttu-id="f27a5-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-172">owner</span><span class="sxs-lookup"><span data-stu-id="f27a5-172">owner</span></span>|<span data-ttu-id="f27a5-173">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-173">String</span></span>|<span data-ttu-id="f27a5-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f27a5-174">The owner of the app.</span></span> <span data-ttu-id="f27a5-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-176">developer</span><span class="sxs-lookup"><span data-stu-id="f27a5-176">developer</span></span>|<span data-ttu-id="f27a5-177">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-177">String</span></span>|<span data-ttu-id="f27a5-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f27a5-178">The developer of the app.</span></span> <span data-ttu-id="f27a5-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-180">notes</span><span class="sxs-lookup"><span data-stu-id="f27a5-180">notes</span></span>|<span data-ttu-id="f27a5-181">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-181">String</span></span>|<span data-ttu-id="f27a5-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f27a5-182">Notes for the app.</span></span> <span data-ttu-id="f27a5-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f27a5-184">uploadState</span></span>|<span data-ttu-id="f27a5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f27a5-185">Int32</span></span>|<span data-ttu-id="f27a5-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-186">The upload state.</span></span> <span data-ttu-id="f27a5-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f27a5-188">publishingState</span></span>|[<span data-ttu-id="f27a5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f27a5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f27a5-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f27a5-190">The publishing state for the app.</span></span> <span data-ttu-id="f27a5-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f27a5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f27a5-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f27a5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f27a5-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f27a5-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f27a5-194">isAssigned</span></span>|<span data-ttu-id="f27a5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f27a5-195">Boolean</span></span>|<span data-ttu-id="f27a5-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f27a5-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f27a5-198">roleScopeTagIds</span></span>|<span data-ttu-id="f27a5-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f27a5-199">String collection</span></span>|<span data-ttu-id="f27a5-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f27a5-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f27a5-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f27a5-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f27a5-202">usedLicenseCount</span></span>|<span data-ttu-id="f27a5-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f27a5-203">Int32</span></span>|<span data-ttu-id="f27a5-204">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="f27a5-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="f27a5-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f27a5-205">totalLicenseCount</span></span>|<span data-ttu-id="f27a5-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f27a5-206">Int32</span></span>|<span data-ttu-id="f27a5-207">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="f27a5-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="f27a5-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f27a5-208">releaseDateTime</span></span>|<span data-ttu-id="f27a5-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f27a5-209">DateTimeOffset</span></span>|<span data-ttu-id="f27a5-210">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="f27a5-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="f27a5-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f27a5-211">appStoreUrl</span></span>|<span data-ttu-id="f27a5-212">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-212">String</span></span>|<span data-ttu-id="f27a5-213">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="f27a5-213">The store URL.</span></span>|
|<span data-ttu-id="f27a5-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="f27a5-214">licensingType</span></span>|[<span data-ttu-id="f27a5-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f27a5-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="f27a5-216">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="f27a5-216">The supported License Type.</span></span>|
|<span data-ttu-id="f27a5-217">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f27a5-217">vppTokenOrganizationName</span></span>|<span data-ttu-id="f27a5-218">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-218">String</span></span>|<span data-ttu-id="f27a5-219">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="f27a5-219">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f27a5-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f27a5-220">vppTokenAccountType</span></span>|[<span data-ttu-id="f27a5-221">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f27a5-221">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f27a5-222">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="f27a5-222">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f27a5-223">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-223">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f27a5-224">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-224">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f27a5-225">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="f27a5-225">vppTokenAppleId</span></span>|<span data-ttu-id="f27a5-226">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-226">String</span></span>|<span data-ttu-id="f27a5-227">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f27a5-227">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f27a5-228">bundleId</span><span class="sxs-lookup"><span data-stu-id="f27a5-228">bundleId</span></span>|<span data-ttu-id="f27a5-229">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-229">String</span></span>|<span data-ttu-id="f27a5-230">ID 名。</span><span class="sxs-lookup"><span data-stu-id="f27a5-230">The Identity Name.</span></span>|
|<span data-ttu-id="f27a5-231">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f27a5-231">vppTokenId</span></span>|<span data-ttu-id="f27a5-232">String</span><span class="sxs-lookup"><span data-stu-id="f27a5-232">String</span></span>|<span data-ttu-id="f27a5-233">このアプリケーションに関連付けられている VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-233">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="f27a5-234">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="f27a5-234">revokeLicenseActionResults</span></span>|<span data-ttu-id="f27a5-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f27a5-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="f27a5-236">結果は、このアプリケーションについてのライセンスを失効します。</span><span class="sxs-lookup"><span data-stu-id="f27a5-236">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="f27a5-237">応答</span><span class="sxs-lookup"><span data-stu-id="f27a5-237">Response</span></span>
<span data-ttu-id="f27a5-238">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f27a5-238">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f27a5-239">例</span><span class="sxs-lookup"><span data-stu-id="f27a5-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="f27a5-240">要求</span><span class="sxs-lookup"><span data-stu-id="f27a5-240">Request</span></span>
<span data-ttu-id="f27a5-241">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f27a5-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="f27a5-242">応答</span><span class="sxs-lookup"><span data-stu-id="f27a5-242">Response</span></span>
<span data-ttu-id="f27a5-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f27a5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




