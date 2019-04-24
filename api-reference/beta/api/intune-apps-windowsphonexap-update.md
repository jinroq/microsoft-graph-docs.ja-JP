---
title: windowsPhoneXAP の更新
description: windowsPhoneXAP オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c701527a2dea9a194ba201ef7bd1c83beec9bfbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32486105"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="43f00-103">windowsPhoneXAP の更新</span><span class="sxs-lookup"><span data-stu-id="43f00-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="43f00-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43f00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43f00-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43f00-106">[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="43f00-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43f00-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="43f00-107">Prerequisites</span></span>
<span data-ttu-id="43f00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43f00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43f00-110">Permission type</span></span>|<span data-ttu-id="43f00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43f00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43f00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43f00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43f00-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f00-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43f00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43f00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43f00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43f00-115">Not supported.</span></span>|
|<span data-ttu-id="43f00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43f00-116">Application</span></span>|<span data-ttu-id="43f00-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43f00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43f00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43f00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="43f00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43f00-119">Request headers</span></span>
|<span data-ttu-id="43f00-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43f00-120">Header</span></span>|<span data-ttu-id="43f00-121">値</span><span class="sxs-lookup"><span data-stu-id="43f00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43f00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43f00-122">Authorization</span></span>|<span data-ttu-id="43f00-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="43f00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43f00-124">承諾</span><span class="sxs-lookup"><span data-stu-id="43f00-124">Accept</span></span>|<span data-ttu-id="43f00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43f00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43f00-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="43f00-126">Request body</span></span>
<span data-ttu-id="43f00-127">要求本文で、 [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43f00-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="43f00-128">次の表に、 [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="43f00-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="43f00-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43f00-129">Property</span></span>|<span data-ttu-id="43f00-130">型</span><span class="sxs-lookup"><span data-stu-id="43f00-130">Type</span></span>|<span data-ttu-id="43f00-131">説明</span><span class="sxs-lookup"><span data-stu-id="43f00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f00-132">id</span><span class="sxs-lookup"><span data-stu-id="43f00-132">id</span></span>|<span data-ttu-id="43f00-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="43f00-133">String</span></span>|<span data-ttu-id="43f00-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="43f00-134">Key of the entity.</span></span> <span data-ttu-id="43f00-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-136">displayName</span><span class="sxs-lookup"><span data-stu-id="43f00-136">displayName</span></span>|<span data-ttu-id="43f00-137">String</span><span class="sxs-lookup"><span data-stu-id="43f00-137">String</span></span>|<span data-ttu-id="43f00-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="43f00-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="43f00-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-140">説明</span><span class="sxs-lookup"><span data-stu-id="43f00-140">description</span></span>|<span data-ttu-id="43f00-141">String</span><span class="sxs-lookup"><span data-stu-id="43f00-141">String</span></span>|<span data-ttu-id="43f00-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="43f00-142">The description of the app.</span></span> <span data-ttu-id="43f00-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-144">publisher</span><span class="sxs-lookup"><span data-stu-id="43f00-144">publisher</span></span>|<span data-ttu-id="43f00-145">String</span><span class="sxs-lookup"><span data-stu-id="43f00-145">String</span></span>|<span data-ttu-id="43f00-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="43f00-146">The publisher of the app.</span></span> <span data-ttu-id="43f00-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="43f00-148">largeIcon</span></span>|[<span data-ttu-id="43f00-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="43f00-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="43f00-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="43f00-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="43f00-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43f00-152">createdDateTime</span></span>|<span data-ttu-id="43f00-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43f00-153">DateTimeOffset</span></span>|<span data-ttu-id="43f00-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="43f00-154">The date and time the app was created.</span></span> <span data-ttu-id="43f00-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43f00-156">lastModifiedDateTime</span></span>|<span data-ttu-id="43f00-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43f00-157">DateTimeOffset</span></span>|<span data-ttu-id="43f00-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="43f00-158">The date and time the app was last modified.</span></span> <span data-ttu-id="43f00-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="43f00-160">isFeatured</span></span>|<span data-ttu-id="43f00-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f00-161">Boolean</span></span>|<span data-ttu-id="43f00-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="43f00-163">privacyInformationUrl</span></span>|<span data-ttu-id="43f00-164">String</span><span class="sxs-lookup"><span data-stu-id="43f00-164">String</span></span>|<span data-ttu-id="43f00-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="43f00-165">The privacy statement Url.</span></span> <span data-ttu-id="43f00-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="43f00-167">informationUrl</span></span>|<span data-ttu-id="43f00-168">String</span><span class="sxs-lookup"><span data-stu-id="43f00-168">String</span></span>|<span data-ttu-id="43f00-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="43f00-169">The more information Url.</span></span> <span data-ttu-id="43f00-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-171">owner</span><span class="sxs-lookup"><span data-stu-id="43f00-171">owner</span></span>|<span data-ttu-id="43f00-172">String</span><span class="sxs-lookup"><span data-stu-id="43f00-172">String</span></span>|<span data-ttu-id="43f00-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="43f00-173">The owner of the app.</span></span> <span data-ttu-id="43f00-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-175">developer</span><span class="sxs-lookup"><span data-stu-id="43f00-175">developer</span></span>|<span data-ttu-id="43f00-176">String</span><span class="sxs-lookup"><span data-stu-id="43f00-176">String</span></span>|<span data-ttu-id="43f00-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="43f00-177">The developer of the app.</span></span> <span data-ttu-id="43f00-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-179">notes</span><span class="sxs-lookup"><span data-stu-id="43f00-179">notes</span></span>|<span data-ttu-id="43f00-180">String</span><span class="sxs-lookup"><span data-stu-id="43f00-180">String</span></span>|<span data-ttu-id="43f00-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="43f00-181">Notes for the app.</span></span> <span data-ttu-id="43f00-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="43f00-183">uploadState</span></span>|<span data-ttu-id="43f00-184">Int32</span><span class="sxs-lookup"><span data-stu-id="43f00-184">Int32</span></span>|<span data-ttu-id="43f00-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="43f00-185">The upload state.</span></span> <span data-ttu-id="43f00-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="43f00-187">publishingState</span></span>|[<span data-ttu-id="43f00-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="43f00-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="43f00-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="43f00-189">The publishing state for the app.</span></span> <span data-ttu-id="43f00-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="43f00-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="43f00-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="43f00-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="43f00-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="43f00-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="43f00-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="43f00-193">isAssigned</span></span>|<span data-ttu-id="43f00-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f00-194">Boolean</span></span>|<span data-ttu-id="43f00-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="43f00-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="43f00-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43f00-197">roleScopeTagIds</span></span>|<span data-ttu-id="43f00-198">String collection</span><span class="sxs-lookup"><span data-stu-id="43f00-198">String collection</span></span>|<span data-ttu-id="43f00-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="43f00-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="43f00-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-201">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="43f00-201">dependentAppCount</span></span>|<span data-ttu-id="43f00-202">Int32</span><span class="sxs-lookup"><span data-stu-id="43f00-202">Int32</span></span>|<span data-ttu-id="43f00-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="43f00-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="43f00-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43f00-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="43f00-205">committedContentVersion</span></span>|<span data-ttu-id="43f00-206">String</span><span class="sxs-lookup"><span data-stu-id="43f00-206">String</span></span>|<span data-ttu-id="43f00-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="43f00-207">The internal committed content version.</span></span> <span data-ttu-id="43f00-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="43f00-209">fileName</span><span class="sxs-lookup"><span data-stu-id="43f00-209">fileName</span></span>|<span data-ttu-id="43f00-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="43f00-210">String</span></span>|<span data-ttu-id="43f00-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="43f00-211">The name of the main Lob application file.</span></span> <span data-ttu-id="43f00-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="43f00-213">size</span><span class="sxs-lookup"><span data-stu-id="43f00-213">size</span></span>|<span data-ttu-id="43f00-214">Int64</span><span class="sxs-lookup"><span data-stu-id="43f00-214">Int64</span></span>|<span data-ttu-id="43f00-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="43f00-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="43f00-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43f00-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="43f00-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="43f00-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="43f00-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="43f00-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="43f00-219">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="43f00-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="43f00-220">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="43f00-220">productIdentifier</span></span>|<span data-ttu-id="43f00-221">String</span><span class="sxs-lookup"><span data-stu-id="43f00-221">String</span></span>|<span data-ttu-id="43f00-222">製品識別子。</span><span class="sxs-lookup"><span data-stu-id="43f00-222">The Product Identifier.</span></span>|
|<span data-ttu-id="43f00-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="43f00-223">identityVersion</span></span>|<span data-ttu-id="43f00-224">String</span><span class="sxs-lookup"><span data-stu-id="43f00-224">String</span></span>|<span data-ttu-id="43f00-225">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="43f00-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="43f00-226">応答</span><span class="sxs-lookup"><span data-stu-id="43f00-226">Response</span></span>
<span data-ttu-id="43f00-227">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43f00-227">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f00-228">例</span><span class="sxs-lookup"><span data-stu-id="43f00-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="43f00-229">要求</span><span class="sxs-lookup"><span data-stu-id="43f00-229">Request</span></span>
<span data-ttu-id="43f00-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43f00-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="43f00-231">応答</span><span class="sxs-lookup"><span data-stu-id="43f00-231">Response</span></span>
<span data-ttu-id="43f00-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43f00-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





