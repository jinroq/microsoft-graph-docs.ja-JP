---
title: WindowsAppX を更新します。
description: WindowsAppX オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: f708d15a262eb6bd6efb36f6713021b33d9527b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316031"
---
# <a name="update-windowsappx"></a><span data-ttu-id="620d7-103">WindowsAppX を更新します。</span><span class="sxs-lookup"><span data-stu-id="620d7-103">Update windowsAppX</span></span>

> <span data-ttu-id="620d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="620d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="620d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="620d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="620d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="620d7-107">[WindowsAppX](../resources/intune-apps-windowsappx.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="620d7-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="620d7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="620d7-108">Prerequisites</span></span>
<span data-ttu-id="620d7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="620d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="620d7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="620d7-111">Permission type</span></span>|<span data-ttu-id="620d7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="620d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="620d7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="620d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="620d7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="620d7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="620d7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="620d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="620d7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d7-116">Not supported.</span></span>|
|<span data-ttu-id="620d7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="620d7-117">Application</span></span>|<span data-ttu-id="620d7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="620d7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="620d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="620d7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="620d7-120">Request headers</span></span>
|<span data-ttu-id="620d7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="620d7-121">Header</span></span>|<span data-ttu-id="620d7-122">値</span><span class="sxs-lookup"><span data-stu-id="620d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="620d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="620d7-123">Authorization</span></span>|<span data-ttu-id="620d7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="620d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="620d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="620d7-125">Accept</span></span>|<span data-ttu-id="620d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="620d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="620d7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="620d7-127">Request body</span></span>
<span data-ttu-id="620d7-128">要求の本文に[windowsAppX](../resources/intune-apps-windowsappx.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="620d7-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="620d7-129">[WindowsAppX](../resources/intune-apps-windowsappx.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="620d7-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="620d7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="620d7-130">Property</span></span>|<span data-ttu-id="620d7-131">種類</span><span class="sxs-lookup"><span data-stu-id="620d7-131">Type</span></span>|<span data-ttu-id="620d7-132">説明</span><span class="sxs-lookup"><span data-stu-id="620d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="620d7-133">ID</span><span class="sxs-lookup"><span data-stu-id="620d7-133">id</span></span>|<span data-ttu-id="620d7-134">String</span><span class="sxs-lookup"><span data-stu-id="620d7-134">String</span></span>|<span data-ttu-id="620d7-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="620d7-135">Key of the entity.</span></span> <span data-ttu-id="620d7-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="620d7-137">displayName</span></span>|<span data-ttu-id="620d7-138">String</span><span class="sxs-lookup"><span data-stu-id="620d7-138">String</span></span>|<span data-ttu-id="620d7-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="620d7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="620d7-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-141">説明</span><span class="sxs-lookup"><span data-stu-id="620d7-141">description</span></span>|<span data-ttu-id="620d7-142">String</span><span class="sxs-lookup"><span data-stu-id="620d7-142">String</span></span>|<span data-ttu-id="620d7-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="620d7-143">The description of the app.</span></span> <span data-ttu-id="620d7-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="620d7-145">publisher</span></span>|<span data-ttu-id="620d7-146">String</span><span class="sxs-lookup"><span data-stu-id="620d7-146">String</span></span>|<span data-ttu-id="620d7-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="620d7-147">The publisher of the app.</span></span> <span data-ttu-id="620d7-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="620d7-149">largeIcon</span></span>|[<span data-ttu-id="620d7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="620d7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="620d7-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="620d7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="620d7-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="620d7-153">createdDateTime</span></span>|<span data-ttu-id="620d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="620d7-154">DateTimeOffset</span></span>|<span data-ttu-id="620d7-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="620d7-155">The date and time the app was created.</span></span> <span data-ttu-id="620d7-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="620d7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="620d7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="620d7-158">DateTimeOffset</span></span>|<span data-ttu-id="620d7-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="620d7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="620d7-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="620d7-161">isFeatured</span></span>|<span data-ttu-id="620d7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="620d7-162">Boolean</span></span>|<span data-ttu-id="620d7-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="620d7-164">privacyInformationUrl</span></span>|<span data-ttu-id="620d7-165">String</span><span class="sxs-lookup"><span data-stu-id="620d7-165">String</span></span>|<span data-ttu-id="620d7-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="620d7-166">The privacy statement Url.</span></span> <span data-ttu-id="620d7-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="620d7-168">informationUrl</span></span>|<span data-ttu-id="620d7-169">String</span><span class="sxs-lookup"><span data-stu-id="620d7-169">String</span></span>|<span data-ttu-id="620d7-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="620d7-170">The more information Url.</span></span> <span data-ttu-id="620d7-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-172">owner</span><span class="sxs-lookup"><span data-stu-id="620d7-172">owner</span></span>|<span data-ttu-id="620d7-173">String</span><span class="sxs-lookup"><span data-stu-id="620d7-173">String</span></span>|<span data-ttu-id="620d7-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="620d7-174">The owner of the app.</span></span> <span data-ttu-id="620d7-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-176">developer</span><span class="sxs-lookup"><span data-stu-id="620d7-176">developer</span></span>|<span data-ttu-id="620d7-177">String</span><span class="sxs-lookup"><span data-stu-id="620d7-177">String</span></span>|<span data-ttu-id="620d7-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="620d7-178">The developer of the app.</span></span> <span data-ttu-id="620d7-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-180">notes</span><span class="sxs-lookup"><span data-stu-id="620d7-180">notes</span></span>|<span data-ttu-id="620d7-181">String</span><span class="sxs-lookup"><span data-stu-id="620d7-181">String</span></span>|<span data-ttu-id="620d7-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="620d7-182">Notes for the app.</span></span> <span data-ttu-id="620d7-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="620d7-184">uploadState</span></span>|<span data-ttu-id="620d7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="620d7-185">Int32</span></span>|<span data-ttu-id="620d7-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="620d7-186">The upload state.</span></span> <span data-ttu-id="620d7-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="620d7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="620d7-188">publishingState</span></span>|[<span data-ttu-id="620d7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="620d7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="620d7-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="620d7-190">The publishing state for the app.</span></span> <span data-ttu-id="620d7-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="620d7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="620d7-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="620d7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="620d7-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="620d7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="620d7-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="620d7-194">committedContentVersion</span></span>|<span data-ttu-id="620d7-195">String</span><span class="sxs-lookup"><span data-stu-id="620d7-195">String</span></span>|<span data-ttu-id="620d7-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="620d7-196">The internal committed content version.</span></span> <span data-ttu-id="620d7-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="620d7-198">fileName</span><span class="sxs-lookup"><span data-stu-id="620d7-198">fileName</span></span>|<span data-ttu-id="620d7-199">String</span><span class="sxs-lookup"><span data-stu-id="620d7-199">String</span></span>|<span data-ttu-id="620d7-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="620d7-200">The name of the main Lob application file.</span></span> <span data-ttu-id="620d7-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="620d7-202">size</span><span class="sxs-lookup"><span data-stu-id="620d7-202">size</span></span>|<span data-ttu-id="620d7-203">Int64</span><span class="sxs-lookup"><span data-stu-id="620d7-203">Int64</span></span>|<span data-ttu-id="620d7-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="620d7-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="620d7-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="620d7-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="620d7-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="620d7-206">applicableArchitectures</span></span>|[<span data-ttu-id="620d7-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="620d7-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="620d7-208">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="620d7-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="620d7-209">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="620d7-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="620d7-210">identityName</span><span class="sxs-lookup"><span data-stu-id="620d7-210">identityName</span></span>|<span data-ttu-id="620d7-211">String</span><span class="sxs-lookup"><span data-stu-id="620d7-211">String</span></span>|<span data-ttu-id="620d7-212">ID 名。</span><span class="sxs-lookup"><span data-stu-id="620d7-212">The Identity Name.</span></span>|
|<span data-ttu-id="620d7-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="620d7-213">identityPublisherHash</span></span>|<span data-ttu-id="620d7-214">String</span><span class="sxs-lookup"><span data-stu-id="620d7-214">String</span></span>|<span data-ttu-id="620d7-215">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="620d7-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="620d7-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="620d7-216">identityResourceIdentifier</span></span>|<span data-ttu-id="620d7-217">String</span><span class="sxs-lookup"><span data-stu-id="620d7-217">String</span></span>|<span data-ttu-id="620d7-218">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="620d7-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="620d7-219">isBundle</span><span class="sxs-lookup"><span data-stu-id="620d7-219">isBundle</span></span>|<span data-ttu-id="620d7-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="620d7-220">Boolean</span></span>|<span data-ttu-id="620d7-221">アプリがバンドルかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="620d7-221">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="620d7-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="620d7-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="620d7-223">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="620d7-223">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="620d7-224">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="620d7-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="620d7-225">identityVersion</span><span class="sxs-lookup"><span data-stu-id="620d7-225">identityVersion</span></span>|<span data-ttu-id="620d7-226">String</span><span class="sxs-lookup"><span data-stu-id="620d7-226">String</span></span>|<span data-ttu-id="620d7-227">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="620d7-227">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="620d7-228">応答</span><span class="sxs-lookup"><span data-stu-id="620d7-228">Response</span></span>
<span data-ttu-id="620d7-229">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAppX](../resources/intune-apps-windowsappx.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="620d7-229">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="620d7-230">例</span><span class="sxs-lookup"><span data-stu-id="620d7-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="620d7-231">要求</span><span class="sxs-lookup"><span data-stu-id="620d7-231">Request</span></span>
<span data-ttu-id="620d7-232">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="620d7-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1269

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

### <a name="response"></a><span data-ttu-id="620d7-233">応答</span><span class="sxs-lookup"><span data-stu-id="620d7-233">Response</span></span>
<span data-ttu-id="620d7-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="620d7-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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





