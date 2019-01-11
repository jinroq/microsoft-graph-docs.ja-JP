---
title: windowsUniversalAppX の更新
description: windowsUniversalAppX オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b47da8672b980b30471f87bbbe4d9cee14eb5089
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892520"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="813c8-103">windowsUniversalAppX の更新</span><span class="sxs-lookup"><span data-stu-id="813c8-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="813c8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="813c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="813c8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="813c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="813c8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="813c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="813c8-107">[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="813c8-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="813c8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="813c8-108">Prerequisites</span></span>
<span data-ttu-id="813c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="813c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="813c8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="813c8-111">Permission type</span></span>|<span data-ttu-id="813c8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="813c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="813c8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="813c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="813c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="813c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="813c8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="813c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="813c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="813c8-116">Not supported.</span></span>|
|<span data-ttu-id="813c8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="813c8-117">Application</span></span>|<span data-ttu-id="813c8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="813c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="813c8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="813c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="813c8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="813c8-120">Request headers</span></span>
|<span data-ttu-id="813c8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="813c8-121">Header</span></span>|<span data-ttu-id="813c8-122">値</span><span class="sxs-lookup"><span data-stu-id="813c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="813c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="813c8-123">Authorization</span></span>|<span data-ttu-id="813c8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="813c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="813c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="813c8-125">Accept</span></span>|<span data-ttu-id="813c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="813c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="813c8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="813c8-127">Request body</span></span>
<span data-ttu-id="813c8-128">要求本文で、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="813c8-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="813c8-129">次の表に、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="813c8-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="813c8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="813c8-130">Property</span></span>|<span data-ttu-id="813c8-131">種類</span><span class="sxs-lookup"><span data-stu-id="813c8-131">Type</span></span>|<span data-ttu-id="813c8-132">説明</span><span class="sxs-lookup"><span data-stu-id="813c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="813c8-133">ID</span><span class="sxs-lookup"><span data-stu-id="813c8-133">id</span></span>|<span data-ttu-id="813c8-134">String</span><span class="sxs-lookup"><span data-stu-id="813c8-134">String</span></span>|<span data-ttu-id="813c8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="813c8-135">Key of the entity.</span></span> <span data-ttu-id="813c8-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="813c8-137">displayName</span></span>|<span data-ttu-id="813c8-138">String</span><span class="sxs-lookup"><span data-stu-id="813c8-138">String</span></span>|<span data-ttu-id="813c8-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="813c8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="813c8-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-141">説明</span><span class="sxs-lookup"><span data-stu-id="813c8-141">description</span></span>|<span data-ttu-id="813c8-142">String</span><span class="sxs-lookup"><span data-stu-id="813c8-142">String</span></span>|<span data-ttu-id="813c8-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="813c8-143">The description of the app.</span></span> <span data-ttu-id="813c8-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="813c8-145">publisher</span></span>|<span data-ttu-id="813c8-146">String</span><span class="sxs-lookup"><span data-stu-id="813c8-146">String</span></span>|<span data-ttu-id="813c8-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="813c8-147">The publisher of the app.</span></span> <span data-ttu-id="813c8-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="813c8-149">largeIcon</span></span>|[<span data-ttu-id="813c8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="813c8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="813c8-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="813c8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="813c8-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="813c8-153">createdDateTime</span></span>|<span data-ttu-id="813c8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="813c8-154">DateTimeOffset</span></span>|<span data-ttu-id="813c8-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="813c8-155">The date and time the app was created.</span></span> <span data-ttu-id="813c8-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="813c8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="813c8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="813c8-158">DateTimeOffset</span></span>|<span data-ttu-id="813c8-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="813c8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="813c8-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="813c8-161">isFeatured</span></span>|<span data-ttu-id="813c8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="813c8-162">Boolean</span></span>|<span data-ttu-id="813c8-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="813c8-164">privacyInformationUrl</span></span>|<span data-ttu-id="813c8-165">String</span><span class="sxs-lookup"><span data-stu-id="813c8-165">String</span></span>|<span data-ttu-id="813c8-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="813c8-166">The privacy statement Url.</span></span> <span data-ttu-id="813c8-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="813c8-168">informationUrl</span></span>|<span data-ttu-id="813c8-169">String</span><span class="sxs-lookup"><span data-stu-id="813c8-169">String</span></span>|<span data-ttu-id="813c8-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="813c8-170">The more information Url.</span></span> <span data-ttu-id="813c8-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-172">owner</span><span class="sxs-lookup"><span data-stu-id="813c8-172">owner</span></span>|<span data-ttu-id="813c8-173">String</span><span class="sxs-lookup"><span data-stu-id="813c8-173">String</span></span>|<span data-ttu-id="813c8-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="813c8-174">The owner of the app.</span></span> <span data-ttu-id="813c8-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-176">developer</span><span class="sxs-lookup"><span data-stu-id="813c8-176">developer</span></span>|<span data-ttu-id="813c8-177">String</span><span class="sxs-lookup"><span data-stu-id="813c8-177">String</span></span>|<span data-ttu-id="813c8-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="813c8-178">The developer of the app.</span></span> <span data-ttu-id="813c8-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-180">notes</span><span class="sxs-lookup"><span data-stu-id="813c8-180">notes</span></span>|<span data-ttu-id="813c8-181">String</span><span class="sxs-lookup"><span data-stu-id="813c8-181">String</span></span>|<span data-ttu-id="813c8-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="813c8-182">Notes for the app.</span></span> <span data-ttu-id="813c8-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="813c8-184">uploadState</span></span>|<span data-ttu-id="813c8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="813c8-185">Int32</span></span>|<span data-ttu-id="813c8-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="813c8-186">The upload state.</span></span> <span data-ttu-id="813c8-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="813c8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="813c8-188">publishingState</span></span>|[<span data-ttu-id="813c8-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="813c8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="813c8-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="813c8-190">The publishing state for the app.</span></span> <span data-ttu-id="813c8-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="813c8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="813c8-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="813c8-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="813c8-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="813c8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="813c8-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="813c8-194">committedContentVersion</span></span>|<span data-ttu-id="813c8-195">String</span><span class="sxs-lookup"><span data-stu-id="813c8-195">String</span></span>|<span data-ttu-id="813c8-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="813c8-196">The internal committed content version.</span></span> <span data-ttu-id="813c8-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="813c8-198">fileName</span><span class="sxs-lookup"><span data-stu-id="813c8-198">fileName</span></span>|<span data-ttu-id="813c8-199">String</span><span class="sxs-lookup"><span data-stu-id="813c8-199">String</span></span>|<span data-ttu-id="813c8-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="813c8-200">The name of the main Lob application file.</span></span> <span data-ttu-id="813c8-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="813c8-202">size</span><span class="sxs-lookup"><span data-stu-id="813c8-202">size</span></span>|<span data-ttu-id="813c8-203">Int64</span><span class="sxs-lookup"><span data-stu-id="813c8-203">Int64</span></span>|<span data-ttu-id="813c8-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="813c8-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="813c8-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="813c8-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="813c8-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="813c8-206">applicableArchitectures</span></span>|[<span data-ttu-id="813c8-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="813c8-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="813c8-208">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="813c8-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="813c8-209">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="813c8-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="813c8-210">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="813c8-210">applicableDeviceTypes</span></span>|[<span data-ttu-id="813c8-211">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="813c8-211">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="813c8-212">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="813c8-212">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="813c8-213">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="813c8-213">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="813c8-214">identityName</span><span class="sxs-lookup"><span data-stu-id="813c8-214">identityName</span></span>|<span data-ttu-id="813c8-215">String</span><span class="sxs-lookup"><span data-stu-id="813c8-215">String</span></span>|<span data-ttu-id="813c8-216">ID 名。</span><span class="sxs-lookup"><span data-stu-id="813c8-216">The Identity Name.</span></span>|
|<span data-ttu-id="813c8-217">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="813c8-217">identityPublisherHash</span></span>|<span data-ttu-id="813c8-218">String</span><span class="sxs-lookup"><span data-stu-id="813c8-218">String</span></span>|<span data-ttu-id="813c8-219">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="813c8-219">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="813c8-220">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="813c8-220">identityResourceIdentifier</span></span>|<span data-ttu-id="813c8-221">String</span><span class="sxs-lookup"><span data-stu-id="813c8-221">String</span></span>|<span data-ttu-id="813c8-222">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="813c8-222">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="813c8-223">isBundle</span><span class="sxs-lookup"><span data-stu-id="813c8-223">isBundle</span></span>|<span data-ttu-id="813c8-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="813c8-224">Boolean</span></span>|<span data-ttu-id="813c8-225">アプリがバンドルかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="813c8-225">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="813c8-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="813c8-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="813c8-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="813c8-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="813c8-228">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="813c8-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="813c8-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="813c8-229">identityVersion</span></span>|<span data-ttu-id="813c8-230">String</span><span class="sxs-lookup"><span data-stu-id="813c8-230">String</span></span>|<span data-ttu-id="813c8-231">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="813c8-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="813c8-232">応答</span><span class="sxs-lookup"><span data-stu-id="813c8-232">Response</span></span>
<span data-ttu-id="813c8-233">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="813c8-233">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="813c8-234">例</span><span class="sxs-lookup"><span data-stu-id="813c8-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="813c8-235">要求</span><span class="sxs-lookup"><span data-stu-id="813c8-235">Request</span></span>
<span data-ttu-id="813c8-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="813c8-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1308

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="813c8-237">応答</span><span class="sxs-lookup"><span data-stu-id="813c8-237">Response</span></span>
<span data-ttu-id="813c8-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="813c8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1475

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





