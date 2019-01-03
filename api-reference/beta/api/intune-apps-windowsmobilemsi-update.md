---
title: windowsMobileMSI の更新
description: windowsMobileMSI オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 859d32fbf053ba22c0bd59afe8ad24d6b05c84a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310746"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="5f89e-103">windowsMobileMSI の更新</span><span class="sxs-lookup"><span data-stu-id="5f89e-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="5f89e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f89e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f89e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f89e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f89e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f89e-107">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f89e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f89e-108">Prerequisites</span></span>
<span data-ttu-id="5f89e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f89e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f89e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f89e-111">Permission type</span></span>|<span data-ttu-id="5f89e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f89e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f89e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f89e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f89e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f89e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f89e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f89e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f89e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-116">Not supported.</span></span>|
|<span data-ttu-id="5f89e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f89e-117">Application</span></span>|<span data-ttu-id="5f89e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f89e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f89e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5f89e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f89e-120">Request headers</span></span>
|<span data-ttu-id="5f89e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f89e-121">Header</span></span>|<span data-ttu-id="5f89e-122">値</span><span class="sxs-lookup"><span data-stu-id="5f89e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f89e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f89e-123">Authorization</span></span>|<span data-ttu-id="5f89e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5f89e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f89e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f89e-125">Accept</span></span>|<span data-ttu-id="5f89e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f89e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f89e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f89e-127">Request body</span></span>
<span data-ttu-id="5f89e-128">要求本文で、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="5f89e-129">次の表に、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="5f89e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f89e-130">Property</span></span>|<span data-ttu-id="5f89e-131">種類</span><span class="sxs-lookup"><span data-stu-id="5f89e-131">Type</span></span>|<span data-ttu-id="5f89e-132">説明</span><span class="sxs-lookup"><span data-stu-id="5f89e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f89e-133">ID</span><span class="sxs-lookup"><span data-stu-id="5f89e-133">id</span></span>|<span data-ttu-id="5f89e-134">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-134">String</span></span>|<span data-ttu-id="5f89e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5f89e-135">Key of the entity.</span></span> <span data-ttu-id="5f89e-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5f89e-137">displayName</span></span>|<span data-ttu-id="5f89e-138">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-138">String</span></span>|<span data-ttu-id="5f89e-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="5f89e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5f89e-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-141">説明</span><span class="sxs-lookup"><span data-stu-id="5f89e-141">description</span></span>|<span data-ttu-id="5f89e-142">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-142">String</span></span>|<span data-ttu-id="5f89e-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="5f89e-143">The description of the app.</span></span> <span data-ttu-id="5f89e-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5f89e-145">publisher</span></span>|<span data-ttu-id="5f89e-146">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-146">String</span></span>|<span data-ttu-id="5f89e-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="5f89e-147">The publisher of the app.</span></span> <span data-ttu-id="5f89e-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5f89e-149">largeIcon</span></span>|[<span data-ttu-id="5f89e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5f89e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5f89e-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="5f89e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5f89e-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f89e-153">createdDateTime</span></span>|<span data-ttu-id="5f89e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f89e-154">DateTimeOffset</span></span>|<span data-ttu-id="5f89e-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5f89e-155">The date and time the app was created.</span></span> <span data-ttu-id="5f89e-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f89e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5f89e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f89e-158">DateTimeOffset</span></span>|<span data-ttu-id="5f89e-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5f89e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5f89e-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5f89e-161">isFeatured</span></span>|<span data-ttu-id="5f89e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f89e-162">Boolean</span></span>|<span data-ttu-id="5f89e-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5f89e-164">privacyInformationUrl</span></span>|<span data-ttu-id="5f89e-165">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-165">String</span></span>|<span data-ttu-id="5f89e-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="5f89e-166">The privacy statement Url.</span></span> <span data-ttu-id="5f89e-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5f89e-168">informationUrl</span></span>|<span data-ttu-id="5f89e-169">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-169">String</span></span>|<span data-ttu-id="5f89e-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="5f89e-170">The more information Url.</span></span> <span data-ttu-id="5f89e-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-172">owner</span><span class="sxs-lookup"><span data-stu-id="5f89e-172">owner</span></span>|<span data-ttu-id="5f89e-173">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-173">String</span></span>|<span data-ttu-id="5f89e-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="5f89e-174">The owner of the app.</span></span> <span data-ttu-id="5f89e-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-176">developer</span><span class="sxs-lookup"><span data-stu-id="5f89e-176">developer</span></span>|<span data-ttu-id="5f89e-177">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-177">String</span></span>|<span data-ttu-id="5f89e-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="5f89e-178">The developer of the app.</span></span> <span data-ttu-id="5f89e-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-180">notes</span><span class="sxs-lookup"><span data-stu-id="5f89e-180">notes</span></span>|<span data-ttu-id="5f89e-181">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-181">String</span></span>|<span data-ttu-id="5f89e-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="5f89e-182">Notes for the app.</span></span> <span data-ttu-id="5f89e-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5f89e-184">uploadState</span></span>|<span data-ttu-id="5f89e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5f89e-185">Int32</span></span>|<span data-ttu-id="5f89e-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="5f89e-186">The upload state.</span></span> <span data-ttu-id="5f89e-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5f89e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5f89e-188">publishingState</span></span>|[<span data-ttu-id="5f89e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5f89e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5f89e-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="5f89e-190">The publishing state for the app.</span></span> <span data-ttu-id="5f89e-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5f89e-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5f89e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5f89e-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="5f89e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5f89e-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5f89e-194">committedContentVersion</span></span>|<span data-ttu-id="5f89e-195">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-195">String</span></span>|<span data-ttu-id="5f89e-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5f89e-196">The internal committed content version.</span></span> <span data-ttu-id="5f89e-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5f89e-198">fileName</span><span class="sxs-lookup"><span data-stu-id="5f89e-198">fileName</span></span>|<span data-ttu-id="5f89e-199">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-199">String</span></span>|<span data-ttu-id="5f89e-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="5f89e-200">The name of the main Lob application file.</span></span> <span data-ttu-id="5f89e-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5f89e-202">size</span><span class="sxs-lookup"><span data-stu-id="5f89e-202">size</span></span>|<span data-ttu-id="5f89e-203">Int64</span><span class="sxs-lookup"><span data-stu-id="5f89e-203">Int64</span></span>|<span data-ttu-id="5f89e-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="5f89e-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="5f89e-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5f89e-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5f89e-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="5f89e-206">commandLine</span></span>|<span data-ttu-id="5f89e-207">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-207">String</span></span>|<span data-ttu-id="5f89e-208">コマンド ライン。</span><span class="sxs-lookup"><span data-stu-id="5f89e-208">The command line.</span></span>|
|<span data-ttu-id="5f89e-209">productCode</span><span class="sxs-lookup"><span data-stu-id="5f89e-209">productCode</span></span>|<span data-ttu-id="5f89e-210">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-210">String</span></span>|<span data-ttu-id="5f89e-211">製品コード。</span><span class="sxs-lookup"><span data-stu-id="5f89e-211">The product code.</span></span>|
|<span data-ttu-id="5f89e-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="5f89e-212">productVersion</span></span>|<span data-ttu-id="5f89e-213">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-213">String</span></span>|<span data-ttu-id="5f89e-214">Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5f89e-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5f89e-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="5f89e-215">ignoreVersionDetection</span></span>|<span data-ttu-id="5f89e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f89e-216">Boolean</span></span>|<span data-ttu-id="5f89e-217">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="5f89e-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="5f89e-218">自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="5f89e-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5f89e-219">identityVersion</span></span>|<span data-ttu-id="5f89e-220">String</span><span class="sxs-lookup"><span data-stu-id="5f89e-220">String</span></span>|<span data-ttu-id="5f89e-221">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5f89e-221">The identity version.</span></span>|
|<span data-ttu-id="5f89e-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="5f89e-222">useDeviceContext</span></span>|<span data-ttu-id="5f89e-223">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="5f89e-223">Boolean</span></span>|<span data-ttu-id="5f89e-224">デバイス コンテキストのデュアル モードの MSI をインストールするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="5f89e-225">True の場合、すべてのユーザーに対してアプリケーションがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="5f89e-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="5f89e-226">False の場合、アプリケーションはユーザーごとのインストールになります。</span><span class="sxs-lookup"><span data-stu-id="5f89e-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="5f89e-227">Null の場合、サービスは、MSI パッケージの既定のインストールのコンテキストを使用します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="5f89e-228">デュアル モードの MSI が発生した場合は、ユーザーがこの既定値になります。</span><span class="sxs-lookup"><span data-stu-id="5f89e-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="5f89e-229">非デュアル モードのアプリケーション用に設定できません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="5f89e-230">アプリケーションの初期作成後は変更できません。</span><span class="sxs-lookup"><span data-stu-id="5f89e-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="5f89e-231">応答</span><span class="sxs-lookup"><span data-stu-id="5f89e-231">Response</span></span>
<span data-ttu-id="5f89e-232">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="5f89e-232">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f89e-233">例</span><span class="sxs-lookup"><span data-stu-id="5f89e-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f89e-234">要求</span><span class="sxs-lookup"><span data-stu-id="5f89e-234">Request</span></span>
<span data-ttu-id="5f89e-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f89e-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 963

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="5f89e-236">応答</span><span class="sxs-lookup"><span data-stu-id="5f89e-236">Response</span></span>
<span data-ttu-id="5f89e-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f89e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




