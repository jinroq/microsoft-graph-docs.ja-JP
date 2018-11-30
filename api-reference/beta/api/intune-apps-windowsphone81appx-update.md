---
title: WindowsPhone81AppX を更新します。
description: WindowsPhone81AppX オブジェクトのプロパティを更新します。
ms.openlocfilehash: 3f3f17be9ba4df2b214b6167f7d54972c2f3994d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072767"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="16eea-103">WindowsPhone81AppX を更新します。</span><span class="sxs-lookup"><span data-stu-id="16eea-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="16eea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16eea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16eea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16eea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16eea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16eea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16eea-107">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16eea-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16eea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16eea-108">Prerequisites</span></span>
<span data-ttu-id="16eea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16eea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16eea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16eea-111">Permission type</span></span>|<span data-ttu-id="16eea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16eea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16eea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16eea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16eea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16eea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16eea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16eea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16eea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16eea-116">Not supported.</span></span>|
|<span data-ttu-id="16eea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16eea-117">Application</span></span>|<span data-ttu-id="16eea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16eea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16eea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16eea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="16eea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16eea-120">Request headers</span></span>
|<span data-ttu-id="16eea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16eea-121">Header</span></span>|<span data-ttu-id="16eea-122">値</span><span class="sxs-lookup"><span data-stu-id="16eea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16eea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16eea-123">Authorization</span></span>|<span data-ttu-id="16eea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16eea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16eea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16eea-125">Accept</span></span>|<span data-ttu-id="16eea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16eea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16eea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16eea-127">Request body</span></span>
<span data-ttu-id="16eea-128">要求の本文に[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="16eea-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="16eea-129">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="16eea-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="16eea-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16eea-130">Property</span></span>|<span data-ttu-id="16eea-131">型</span><span class="sxs-lookup"><span data-stu-id="16eea-131">Type</span></span>|<span data-ttu-id="16eea-132">説明</span><span class="sxs-lookup"><span data-stu-id="16eea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16eea-133">id</span><span class="sxs-lookup"><span data-stu-id="16eea-133">id</span></span>|<span data-ttu-id="16eea-134">String</span><span class="sxs-lookup"><span data-stu-id="16eea-134">String</span></span>|<span data-ttu-id="16eea-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="16eea-135">Key of the entity.</span></span> <span data-ttu-id="16eea-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-137">displayName</span><span class="sxs-lookup"><span data-stu-id="16eea-137">displayName</span></span>|<span data-ttu-id="16eea-138">String</span><span class="sxs-lookup"><span data-stu-id="16eea-138">String</span></span>|<span data-ttu-id="16eea-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="16eea-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="16eea-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-141">説明</span><span class="sxs-lookup"><span data-stu-id="16eea-141">description</span></span>|<span data-ttu-id="16eea-142">String</span><span class="sxs-lookup"><span data-stu-id="16eea-142">String</span></span>|<span data-ttu-id="16eea-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="16eea-143">The description of the app.</span></span> <span data-ttu-id="16eea-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-145">publisher</span><span class="sxs-lookup"><span data-stu-id="16eea-145">publisher</span></span>|<span data-ttu-id="16eea-146">String</span><span class="sxs-lookup"><span data-stu-id="16eea-146">String</span></span>|<span data-ttu-id="16eea-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="16eea-147">The publisher of the app.</span></span> <span data-ttu-id="16eea-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="16eea-149">largeIcon</span></span>|[<span data-ttu-id="16eea-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="16eea-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="16eea-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="16eea-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="16eea-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16eea-153">createdDateTime</span></span>|<span data-ttu-id="16eea-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16eea-154">DateTimeOffset</span></span>|<span data-ttu-id="16eea-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="16eea-155">The date and time the app was created.</span></span> <span data-ttu-id="16eea-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16eea-157">lastModifiedDateTime</span></span>|<span data-ttu-id="16eea-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16eea-158">DateTimeOffset</span></span>|<span data-ttu-id="16eea-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="16eea-159">The date and time the app was last modified.</span></span> <span data-ttu-id="16eea-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="16eea-161">isFeatured</span></span>|<span data-ttu-id="16eea-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="16eea-162">Boolean</span></span>|<span data-ttu-id="16eea-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="16eea-164">privacyInformationUrl</span></span>|<span data-ttu-id="16eea-165">String</span><span class="sxs-lookup"><span data-stu-id="16eea-165">String</span></span>|<span data-ttu-id="16eea-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="16eea-166">The privacy statement Url.</span></span> <span data-ttu-id="16eea-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="16eea-168">informationUrl</span></span>|<span data-ttu-id="16eea-169">String</span><span class="sxs-lookup"><span data-stu-id="16eea-169">String</span></span>|<span data-ttu-id="16eea-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="16eea-170">The more information Url.</span></span> <span data-ttu-id="16eea-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-172">owner</span><span class="sxs-lookup"><span data-stu-id="16eea-172">owner</span></span>|<span data-ttu-id="16eea-173">String</span><span class="sxs-lookup"><span data-stu-id="16eea-173">String</span></span>|<span data-ttu-id="16eea-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="16eea-174">The owner of the app.</span></span> <span data-ttu-id="16eea-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-176">developer</span><span class="sxs-lookup"><span data-stu-id="16eea-176">developer</span></span>|<span data-ttu-id="16eea-177">String</span><span class="sxs-lookup"><span data-stu-id="16eea-177">String</span></span>|<span data-ttu-id="16eea-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="16eea-178">The developer of the app.</span></span> <span data-ttu-id="16eea-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-180">notes</span><span class="sxs-lookup"><span data-stu-id="16eea-180">notes</span></span>|<span data-ttu-id="16eea-181">String</span><span class="sxs-lookup"><span data-stu-id="16eea-181">String</span></span>|<span data-ttu-id="16eea-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="16eea-182">Notes for the app.</span></span> <span data-ttu-id="16eea-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="16eea-184">uploadState</span></span>|<span data-ttu-id="16eea-185">Int32</span><span class="sxs-lookup"><span data-stu-id="16eea-185">Int32</span></span>|<span data-ttu-id="16eea-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="16eea-186">The upload state.</span></span> <span data-ttu-id="16eea-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="16eea-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="16eea-188">publishingState</span></span>|[<span data-ttu-id="16eea-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="16eea-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="16eea-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="16eea-190">The publishing state for the app.</span></span> <span data-ttu-id="16eea-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="16eea-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="16eea-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="16eea-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="16eea-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="16eea-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="16eea-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="16eea-194">committedContentVersion</span></span>|<span data-ttu-id="16eea-195">String</span><span class="sxs-lookup"><span data-stu-id="16eea-195">String</span></span>|<span data-ttu-id="16eea-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="16eea-196">The internal committed content version.</span></span> <span data-ttu-id="16eea-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16eea-198">fileName</span><span class="sxs-lookup"><span data-stu-id="16eea-198">fileName</span></span>|<span data-ttu-id="16eea-199">String</span><span class="sxs-lookup"><span data-stu-id="16eea-199">String</span></span>|<span data-ttu-id="16eea-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="16eea-200">The name of the main Lob application file.</span></span> <span data-ttu-id="16eea-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16eea-202">size</span><span class="sxs-lookup"><span data-stu-id="16eea-202">size</span></span>|<span data-ttu-id="16eea-203">Int64</span><span class="sxs-lookup"><span data-stu-id="16eea-203">Int64</span></span>|<span data-ttu-id="16eea-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="16eea-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="16eea-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16eea-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="16eea-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="16eea-206">applicableArchitectures</span></span>|[<span data-ttu-id="16eea-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="16eea-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="16eea-208">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="16eea-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="16eea-209">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="16eea-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="16eea-210">identityName</span><span class="sxs-lookup"><span data-stu-id="16eea-210">identityName</span></span>|<span data-ttu-id="16eea-211">String</span><span class="sxs-lookup"><span data-stu-id="16eea-211">String</span></span>|<span data-ttu-id="16eea-212">ID 名。</span><span class="sxs-lookup"><span data-stu-id="16eea-212">The Identity Name.</span></span>|
|<span data-ttu-id="16eea-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="16eea-213">identityPublisherHash</span></span>|<span data-ttu-id="16eea-214">String</span><span class="sxs-lookup"><span data-stu-id="16eea-214">String</span></span>|<span data-ttu-id="16eea-215">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="16eea-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="16eea-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="16eea-216">identityResourceIdentifier</span></span>|<span data-ttu-id="16eea-217">String</span><span class="sxs-lookup"><span data-stu-id="16eea-217">String</span></span>|<span data-ttu-id="16eea-218">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="16eea-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="16eea-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="16eea-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="16eea-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="16eea-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="16eea-221">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="16eea-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="16eea-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="16eea-222">phoneProductIdentifier</span></span>|<span data-ttu-id="16eea-223">String</span><span class="sxs-lookup"><span data-stu-id="16eea-223">String</span></span>|<span data-ttu-id="16eea-224">電話の製品識別子です。</span><span class="sxs-lookup"><span data-stu-id="16eea-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="16eea-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="16eea-225">phonePublisherId</span></span>|<span data-ttu-id="16eea-226">String</span><span class="sxs-lookup"><span data-stu-id="16eea-226">String</span></span>|<span data-ttu-id="16eea-227">電話の発行元の id。</span><span class="sxs-lookup"><span data-stu-id="16eea-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="16eea-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="16eea-228">identityVersion</span></span>|<span data-ttu-id="16eea-229">String</span><span class="sxs-lookup"><span data-stu-id="16eea-229">String</span></span>|<span data-ttu-id="16eea-230">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="16eea-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="16eea-231">応答</span><span class="sxs-lookup"><span data-stu-id="16eea-231">Response</span></span>
<span data-ttu-id="16eea-232">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="16eea-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16eea-233">例</span><span class="sxs-lookup"><span data-stu-id="16eea-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="16eea-234">要求</span><span class="sxs-lookup"><span data-stu-id="16eea-234">Request</span></span>
<span data-ttu-id="16eea-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16eea-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1362

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

### <a name="response"></a><span data-ttu-id="16eea-236">応答</span><span class="sxs-lookup"><span data-stu-id="16eea-236">Response</span></span>
<span data-ttu-id="16eea-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16eea-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1527

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





