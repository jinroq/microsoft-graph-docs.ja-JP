---
title: androidLobApp の更新
description: androidLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 513a8d6a059cf7e86abaaeb55ddbcdff97b0dcea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332082"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="f3303-103">androidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="f3303-103">Update androidLobApp</span></span>

> <span data-ttu-id="f3303-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3303-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3303-105">[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3303-105">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3303-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3303-106">Prerequisites</span></span>
<span data-ttu-id="f3303-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3303-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3303-109">Permission type</span></span>|<span data-ttu-id="f3303-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3303-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3303-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3303-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3303-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3303-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3303-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3303-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3303-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3303-114">Not supported.</span></span>|
|<span data-ttu-id="f3303-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3303-115">Application</span></span>|<span data-ttu-id="f3303-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3303-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3303-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3303-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f3303-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3303-118">Request headers</span></span>
|<span data-ttu-id="f3303-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3303-119">Header</span></span>|<span data-ttu-id="f3303-120">値</span><span class="sxs-lookup"><span data-stu-id="f3303-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3303-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3303-121">Authorization</span></span>|<span data-ttu-id="f3303-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f3303-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3303-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3303-123">Accept</span></span>|<span data-ttu-id="f3303-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3303-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3303-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3303-125">Request body</span></span>
<span data-ttu-id="f3303-126">要求本文で、[androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3303-126">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="f3303-127">次の表に、[androidLobApp](../resources/intune-apps-androidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3303-127">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="f3303-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3303-128">Property</span></span>|<span data-ttu-id="f3303-129">種類</span><span class="sxs-lookup"><span data-stu-id="f3303-129">Type</span></span>|<span data-ttu-id="f3303-130">説明</span><span class="sxs-lookup"><span data-stu-id="f3303-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3303-131">ID</span><span class="sxs-lookup"><span data-stu-id="f3303-131">id</span></span>|<span data-ttu-id="f3303-132">String</span><span class="sxs-lookup"><span data-stu-id="f3303-132">String</span></span>|<span data-ttu-id="f3303-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3303-133">Key of the entity.</span></span> <span data-ttu-id="f3303-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f3303-135">displayName</span></span>|<span data-ttu-id="f3303-136">String</span><span class="sxs-lookup"><span data-stu-id="f3303-136">String</span></span>|<span data-ttu-id="f3303-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f3303-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3303-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-139">説明</span><span class="sxs-lookup"><span data-stu-id="f3303-139">description</span></span>|<span data-ttu-id="f3303-140">String</span><span class="sxs-lookup"><span data-stu-id="f3303-140">String</span></span>|<span data-ttu-id="f3303-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f3303-141">The description of the app.</span></span> <span data-ttu-id="f3303-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f3303-143">publisher</span></span>|<span data-ttu-id="f3303-144">String</span><span class="sxs-lookup"><span data-stu-id="f3303-144">String</span></span>|<span data-ttu-id="f3303-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f3303-145">The publisher of the app.</span></span> <span data-ttu-id="f3303-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3303-147">largeIcon</span></span>|[<span data-ttu-id="f3303-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3303-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3303-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f3303-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3303-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3303-151">createdDateTime</span></span>|<span data-ttu-id="f3303-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3303-152">DateTimeOffset</span></span>|<span data-ttu-id="f3303-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f3303-153">The date and time the app was created.</span></span> <span data-ttu-id="f3303-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3303-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f3303-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3303-156">DateTimeOffset</span></span>|<span data-ttu-id="f3303-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f3303-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f3303-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3303-159">isFeatured</span></span>|<span data-ttu-id="f3303-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3303-160">Boolean</span></span>|<span data-ttu-id="f3303-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3303-162">privacyInformationUrl</span></span>|<span data-ttu-id="f3303-163">String</span><span class="sxs-lookup"><span data-stu-id="f3303-163">String</span></span>|<span data-ttu-id="f3303-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f3303-164">The privacy statement Url.</span></span> <span data-ttu-id="f3303-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3303-166">informationUrl</span></span>|<span data-ttu-id="f3303-167">String</span><span class="sxs-lookup"><span data-stu-id="f3303-167">String</span></span>|<span data-ttu-id="f3303-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f3303-168">The more information Url.</span></span> <span data-ttu-id="f3303-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-170">owner</span><span class="sxs-lookup"><span data-stu-id="f3303-170">owner</span></span>|<span data-ttu-id="f3303-171">String</span><span class="sxs-lookup"><span data-stu-id="f3303-171">String</span></span>|<span data-ttu-id="f3303-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f3303-172">The owner of the app.</span></span> <span data-ttu-id="f3303-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-174">developer</span><span class="sxs-lookup"><span data-stu-id="f3303-174">developer</span></span>|<span data-ttu-id="f3303-175">String</span><span class="sxs-lookup"><span data-stu-id="f3303-175">String</span></span>|<span data-ttu-id="f3303-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f3303-176">The developer of the app.</span></span> <span data-ttu-id="f3303-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-178">notes</span><span class="sxs-lookup"><span data-stu-id="f3303-178">notes</span></span>|<span data-ttu-id="f3303-179">String</span><span class="sxs-lookup"><span data-stu-id="f3303-179">String</span></span>|<span data-ttu-id="f3303-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f3303-180">Notes for the app.</span></span> <span data-ttu-id="f3303-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3303-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3303-182">publishingState</span></span>|[<span data-ttu-id="f3303-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f3303-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3303-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f3303-184">The publishing state for the app.</span></span> <span data-ttu-id="f3303-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f3303-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3303-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f3303-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f3303-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f3303-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3303-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f3303-188">committedContentVersion</span></span>|<span data-ttu-id="f3303-189">String</span><span class="sxs-lookup"><span data-stu-id="f3303-189">String</span></span>|<span data-ttu-id="f3303-190">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3303-190">The internal committed content version.</span></span> <span data-ttu-id="f3303-191">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3303-192">fileName</span><span class="sxs-lookup"><span data-stu-id="f3303-192">fileName</span></span>|<span data-ttu-id="f3303-193">String</span><span class="sxs-lookup"><span data-stu-id="f3303-193">String</span></span>|<span data-ttu-id="f3303-194">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="f3303-194">The name of the main Lob application file.</span></span> <span data-ttu-id="f3303-195">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3303-196">size</span><span class="sxs-lookup"><span data-stu-id="f3303-196">size</span></span>|<span data-ttu-id="f3303-197">Int64</span><span class="sxs-lookup"><span data-stu-id="f3303-197">Int64</span></span>|<span data-ttu-id="f3303-198">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="f3303-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="f3303-199">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3303-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3303-200">packageId</span><span class="sxs-lookup"><span data-stu-id="f3303-200">packageId</span></span>|<span data-ttu-id="f3303-201">String</span><span class="sxs-lookup"><span data-stu-id="f3303-201">String</span></span>|<span data-ttu-id="f3303-202">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="f3303-202">The package identifier.</span></span>|
|<span data-ttu-id="f3303-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3303-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f3303-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3303-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f3303-205">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="f3303-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f3303-206">versionName</span><span class="sxs-lookup"><span data-stu-id="f3303-206">versionName</span></span>|<span data-ttu-id="f3303-207">String</span><span class="sxs-lookup"><span data-stu-id="f3303-207">String</span></span>|<span data-ttu-id="f3303-208">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="f3303-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f3303-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="f3303-209">versionCode</span></span>|<span data-ttu-id="f3303-210">String</span><span class="sxs-lookup"><span data-stu-id="f3303-210">String</span></span>|<span data-ttu-id="f3303-211">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="f3303-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f3303-212">応答</span><span class="sxs-lookup"><span data-stu-id="f3303-212">Response</span></span>
<span data-ttu-id="f3303-213">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidLobApp](../resources/intune-apps-androidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f3303-213">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3303-214">例</span><span class="sxs-lookup"><span data-stu-id="f3303-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3303-215">要求</span><span class="sxs-lookup"><span data-stu-id="f3303-215">Request</span></span>
<span data-ttu-id="f3303-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3303-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="f3303-217">応答</span><span class="sxs-lookup"><span data-stu-id="f3303-217">Response</span></span>
<span data-ttu-id="f3303-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3303-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



