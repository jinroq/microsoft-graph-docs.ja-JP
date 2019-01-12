---
title: Create windowsUniversalAppX
description: 新しい windowsUniversalAppX オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c652a0cbd7a5472663d5e748ec7c738838e55d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949851"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="79d51-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="79d51-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="79d51-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79d51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79d51-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79d51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79d51-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79d51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79d51-107">新しい [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="79d51-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79d51-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="79d51-108">Prerequisites</span></span>
<span data-ttu-id="79d51-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79d51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d51-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79d51-111">Permission type</span></span>|<span data-ttu-id="79d51-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79d51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79d51-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79d51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79d51-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d51-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79d51-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79d51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79d51-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79d51-116">Not supported.</span></span>|
|<span data-ttu-id="79d51-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79d51-117">Application</span></span>|<span data-ttu-id="79d51-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79d51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79d51-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79d51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="79d51-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79d51-120">Request headers</span></span>
|<span data-ttu-id="79d51-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79d51-121">Header</span></span>|<span data-ttu-id="79d51-122">値</span><span class="sxs-lookup"><span data-stu-id="79d51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79d51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79d51-123">Authorization</span></span>|<span data-ttu-id="79d51-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79d51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79d51-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79d51-125">Accept</span></span>|<span data-ttu-id="79d51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79d51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79d51-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79d51-127">Request body</span></span>
<span data-ttu-id="79d51-128">要求本文で、windowsUniversalAppX オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="79d51-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="79d51-129">次の表に、windowsUniversalAppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79d51-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="79d51-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79d51-130">Property</span></span>|<span data-ttu-id="79d51-131">種類</span><span class="sxs-lookup"><span data-stu-id="79d51-131">Type</span></span>|<span data-ttu-id="79d51-132">説明</span><span class="sxs-lookup"><span data-stu-id="79d51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d51-133">ID</span><span class="sxs-lookup"><span data-stu-id="79d51-133">id</span></span>|<span data-ttu-id="79d51-134">String</span><span class="sxs-lookup"><span data-stu-id="79d51-134">String</span></span>|<span data-ttu-id="79d51-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="79d51-135">Key of the entity.</span></span> <span data-ttu-id="79d51-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-137">displayName</span><span class="sxs-lookup"><span data-stu-id="79d51-137">displayName</span></span>|<span data-ttu-id="79d51-138">String</span><span class="sxs-lookup"><span data-stu-id="79d51-138">String</span></span>|<span data-ttu-id="79d51-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="79d51-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="79d51-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-141">説明</span><span class="sxs-lookup"><span data-stu-id="79d51-141">description</span></span>|<span data-ttu-id="79d51-142">String</span><span class="sxs-lookup"><span data-stu-id="79d51-142">String</span></span>|<span data-ttu-id="79d51-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="79d51-143">The description of the app.</span></span> <span data-ttu-id="79d51-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-145">publisher</span><span class="sxs-lookup"><span data-stu-id="79d51-145">publisher</span></span>|<span data-ttu-id="79d51-146">String</span><span class="sxs-lookup"><span data-stu-id="79d51-146">String</span></span>|<span data-ttu-id="79d51-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="79d51-147">The publisher of the app.</span></span> <span data-ttu-id="79d51-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="79d51-149">largeIcon</span></span>|[<span data-ttu-id="79d51-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79d51-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79d51-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="79d51-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="79d51-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79d51-153">createdDateTime</span></span>|<span data-ttu-id="79d51-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d51-154">DateTimeOffset</span></span>|<span data-ttu-id="79d51-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="79d51-155">The date and time the app was created.</span></span> <span data-ttu-id="79d51-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79d51-157">lastModifiedDateTime</span></span>|<span data-ttu-id="79d51-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d51-158">DateTimeOffset</span></span>|<span data-ttu-id="79d51-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="79d51-159">The date and time the app was last modified.</span></span> <span data-ttu-id="79d51-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="79d51-161">isFeatured</span></span>|<span data-ttu-id="79d51-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d51-162">Boolean</span></span>|<span data-ttu-id="79d51-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="79d51-164">privacyInformationUrl</span></span>|<span data-ttu-id="79d51-165">String</span><span class="sxs-lookup"><span data-stu-id="79d51-165">String</span></span>|<span data-ttu-id="79d51-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="79d51-166">The privacy statement Url.</span></span> <span data-ttu-id="79d51-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="79d51-168">informationUrl</span></span>|<span data-ttu-id="79d51-169">String</span><span class="sxs-lookup"><span data-stu-id="79d51-169">String</span></span>|<span data-ttu-id="79d51-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="79d51-170">The more information Url.</span></span> <span data-ttu-id="79d51-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-172">owner</span><span class="sxs-lookup"><span data-stu-id="79d51-172">owner</span></span>|<span data-ttu-id="79d51-173">String</span><span class="sxs-lookup"><span data-stu-id="79d51-173">String</span></span>|<span data-ttu-id="79d51-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="79d51-174">The owner of the app.</span></span> <span data-ttu-id="79d51-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-176">developer</span><span class="sxs-lookup"><span data-stu-id="79d51-176">developer</span></span>|<span data-ttu-id="79d51-177">String</span><span class="sxs-lookup"><span data-stu-id="79d51-177">String</span></span>|<span data-ttu-id="79d51-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="79d51-178">The developer of the app.</span></span> <span data-ttu-id="79d51-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-180">notes</span><span class="sxs-lookup"><span data-stu-id="79d51-180">notes</span></span>|<span data-ttu-id="79d51-181">String</span><span class="sxs-lookup"><span data-stu-id="79d51-181">String</span></span>|<span data-ttu-id="79d51-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="79d51-182">Notes for the app.</span></span> <span data-ttu-id="79d51-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="79d51-184">uploadState</span></span>|<span data-ttu-id="79d51-185">Int32</span><span class="sxs-lookup"><span data-stu-id="79d51-185">Int32</span></span>|<span data-ttu-id="79d51-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="79d51-186">The upload state.</span></span> <span data-ttu-id="79d51-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d51-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="79d51-188">publishingState</span></span>|[<span data-ttu-id="79d51-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="79d51-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="79d51-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="79d51-190">The publishing state for the app.</span></span> <span data-ttu-id="79d51-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="79d51-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="79d51-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="79d51-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="79d51-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="79d51-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="79d51-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="79d51-194">committedContentVersion</span></span>|<span data-ttu-id="79d51-195">String</span><span class="sxs-lookup"><span data-stu-id="79d51-195">String</span></span>|<span data-ttu-id="79d51-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="79d51-196">The internal committed content version.</span></span> <span data-ttu-id="79d51-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79d51-198">fileName</span><span class="sxs-lookup"><span data-stu-id="79d51-198">fileName</span></span>|<span data-ttu-id="79d51-199">String</span><span class="sxs-lookup"><span data-stu-id="79d51-199">String</span></span>|<span data-ttu-id="79d51-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="79d51-200">The name of the main Lob application file.</span></span> <span data-ttu-id="79d51-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79d51-202">size</span><span class="sxs-lookup"><span data-stu-id="79d51-202">size</span></span>|<span data-ttu-id="79d51-203">Int64</span><span class="sxs-lookup"><span data-stu-id="79d51-203">Int64</span></span>|<span data-ttu-id="79d51-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="79d51-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="79d51-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79d51-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79d51-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="79d51-206">applicableArchitectures</span></span>|[<span data-ttu-id="79d51-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="79d51-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="79d51-208">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="79d51-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="79d51-209">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="79d51-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="79d51-210">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="79d51-210">applicableDeviceTypes</span></span>|[<span data-ttu-id="79d51-211">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="79d51-211">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="79d51-212">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="79d51-212">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="79d51-213">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="79d51-213">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="79d51-214">identityName</span><span class="sxs-lookup"><span data-stu-id="79d51-214">identityName</span></span>|<span data-ttu-id="79d51-215">String</span><span class="sxs-lookup"><span data-stu-id="79d51-215">String</span></span>|<span data-ttu-id="79d51-216">ID 名。</span><span class="sxs-lookup"><span data-stu-id="79d51-216">The Identity Name.</span></span>|
|<span data-ttu-id="79d51-217">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="79d51-217">identityPublisherHash</span></span>|<span data-ttu-id="79d51-218">String</span><span class="sxs-lookup"><span data-stu-id="79d51-218">String</span></span>|<span data-ttu-id="79d51-219">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="79d51-219">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="79d51-220">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="79d51-220">identityResourceIdentifier</span></span>|<span data-ttu-id="79d51-221">String</span><span class="sxs-lookup"><span data-stu-id="79d51-221">String</span></span>|<span data-ttu-id="79d51-222">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="79d51-222">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="79d51-223">isBundle</span><span class="sxs-lookup"><span data-stu-id="79d51-223">isBundle</span></span>|<span data-ttu-id="79d51-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d51-224">Boolean</span></span>|<span data-ttu-id="79d51-225">アプリがバンドルかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79d51-225">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="79d51-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79d51-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="79d51-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79d51-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="79d51-228">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="79d51-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="79d51-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="79d51-229">identityVersion</span></span>|<span data-ttu-id="79d51-230">String</span><span class="sxs-lookup"><span data-stu-id="79d51-230">String</span></span>|<span data-ttu-id="79d51-231">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="79d51-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="79d51-232">応答</span><span class="sxs-lookup"><span data-stu-id="79d51-232">Response</span></span>
<span data-ttu-id="79d51-233">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79d51-233">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79d51-234">例</span><span class="sxs-lookup"><span data-stu-id="79d51-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="79d51-235">要求</span><span class="sxs-lookup"><span data-stu-id="79d51-235">Request</span></span>
<span data-ttu-id="79d51-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79d51-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1367

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

### <a name="response"></a><span data-ttu-id="79d51-237">応答</span><span class="sxs-lookup"><span data-stu-id="79d51-237">Response</span></span>
<span data-ttu-id="79d51-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79d51-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





