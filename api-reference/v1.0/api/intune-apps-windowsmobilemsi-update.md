---
title: windowsMobileMSI の更新
description: windowsMobileMSI オブジェクトのプロパティを更新します。
ms.openlocfilehash: a87c76413080b6c5daae828e5ed22e99be1d6bcf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023201"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="054c1-103">windowsMobileMSI の更新</span><span class="sxs-lookup"><span data-stu-id="054c1-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="054c1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="054c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="054c1-105">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="054c1-105">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="054c1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="054c1-106">Prerequisites</span></span>
<span data-ttu-id="054c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="054c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="054c1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="054c1-109">Permission type</span></span>|<span data-ttu-id="054c1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="054c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="054c1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="054c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="054c1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="054c1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="054c1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="054c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="054c1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="054c1-114">Not supported.</span></span>|
|<span data-ttu-id="054c1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="054c1-115">Application</span></span>|<span data-ttu-id="054c1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="054c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="054c1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="054c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="054c1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="054c1-118">Request headers</span></span>
|<span data-ttu-id="054c1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="054c1-119">Header</span></span>|<span data-ttu-id="054c1-120">値</span><span class="sxs-lookup"><span data-stu-id="054c1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="054c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="054c1-121">Authorization</span></span>|<span data-ttu-id="054c1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="054c1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="054c1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="054c1-123">Accept</span></span>|<span data-ttu-id="054c1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="054c1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="054c1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="054c1-125">Request body</span></span>
<span data-ttu-id="054c1-126">要求本文で、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="054c1-126">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="054c1-127">次の表に、[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="054c1-127">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="054c1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="054c1-128">Property</span></span>|<span data-ttu-id="054c1-129">型</span><span class="sxs-lookup"><span data-stu-id="054c1-129">Type</span></span>|<span data-ttu-id="054c1-130">説明</span><span class="sxs-lookup"><span data-stu-id="054c1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="054c1-131">id</span><span class="sxs-lookup"><span data-stu-id="054c1-131">id</span></span>|<span data-ttu-id="054c1-132">String</span><span class="sxs-lookup"><span data-stu-id="054c1-132">String</span></span>|<span data-ttu-id="054c1-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="054c1-133">Key of the entity.</span></span> <span data-ttu-id="054c1-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="054c1-135">displayName</span></span>|<span data-ttu-id="054c1-136">String</span><span class="sxs-lookup"><span data-stu-id="054c1-136">String</span></span>|<span data-ttu-id="054c1-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="054c1-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="054c1-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-139">説明</span><span class="sxs-lookup"><span data-stu-id="054c1-139">description</span></span>|<span data-ttu-id="054c1-140">String</span><span class="sxs-lookup"><span data-stu-id="054c1-140">String</span></span>|<span data-ttu-id="054c1-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="054c1-141">The description of the app.</span></span> <span data-ttu-id="054c1-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-143">publisher</span><span class="sxs-lookup"><span data-stu-id="054c1-143">publisher</span></span>|<span data-ttu-id="054c1-144">String</span><span class="sxs-lookup"><span data-stu-id="054c1-144">String</span></span>|<span data-ttu-id="054c1-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="054c1-145">The publisher of the app.</span></span> <span data-ttu-id="054c1-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="054c1-147">largeIcon</span></span>|[<span data-ttu-id="054c1-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="054c1-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="054c1-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="054c1-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="054c1-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="054c1-151">createdDateTime</span></span>|<span data-ttu-id="054c1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="054c1-152">DateTimeOffset</span></span>|<span data-ttu-id="054c1-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="054c1-153">The date and time the app was created.</span></span> <span data-ttu-id="054c1-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="054c1-155">lastModifiedDateTime</span></span>|<span data-ttu-id="054c1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="054c1-156">DateTimeOffset</span></span>|<span data-ttu-id="054c1-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="054c1-157">The date and time the app was last modified.</span></span> <span data-ttu-id="054c1-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="054c1-159">isFeatured</span></span>|<span data-ttu-id="054c1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="054c1-160">Boolean</span></span>|<span data-ttu-id="054c1-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="054c1-162">privacyInformationUrl</span></span>|<span data-ttu-id="054c1-163">String</span><span class="sxs-lookup"><span data-stu-id="054c1-163">String</span></span>|<span data-ttu-id="054c1-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="054c1-164">The privacy statement Url.</span></span> <span data-ttu-id="054c1-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="054c1-166">informationUrl</span></span>|<span data-ttu-id="054c1-167">String</span><span class="sxs-lookup"><span data-stu-id="054c1-167">String</span></span>|<span data-ttu-id="054c1-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="054c1-168">The more information Url.</span></span> <span data-ttu-id="054c1-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-170">owner</span><span class="sxs-lookup"><span data-stu-id="054c1-170">owner</span></span>|<span data-ttu-id="054c1-171">String</span><span class="sxs-lookup"><span data-stu-id="054c1-171">String</span></span>|<span data-ttu-id="054c1-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="054c1-172">The owner of the app.</span></span> <span data-ttu-id="054c1-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-174">developer</span><span class="sxs-lookup"><span data-stu-id="054c1-174">developer</span></span>|<span data-ttu-id="054c1-175">String</span><span class="sxs-lookup"><span data-stu-id="054c1-175">String</span></span>|<span data-ttu-id="054c1-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="054c1-176">The developer of the app.</span></span> <span data-ttu-id="054c1-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-178">notes</span><span class="sxs-lookup"><span data-stu-id="054c1-178">notes</span></span>|<span data-ttu-id="054c1-179">String</span><span class="sxs-lookup"><span data-stu-id="054c1-179">String</span></span>|<span data-ttu-id="054c1-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="054c1-180">Notes for the app.</span></span> <span data-ttu-id="054c1-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="054c1-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="054c1-182">publishingState</span></span>|[<span data-ttu-id="054c1-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="054c1-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="054c1-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="054c1-184">The publishing state for the app.</span></span> <span data-ttu-id="054c1-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="054c1-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="054c1-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="054c1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="054c1-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="054c1-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="054c1-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="054c1-188">committedContentVersion</span></span>|<span data-ttu-id="054c1-189">String</span><span class="sxs-lookup"><span data-stu-id="054c1-189">String</span></span>|<span data-ttu-id="054c1-190">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="054c1-190">The internal committed content version.</span></span> <span data-ttu-id="054c1-191">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="054c1-192">fileName</span><span class="sxs-lookup"><span data-stu-id="054c1-192">fileName</span></span>|<span data-ttu-id="054c1-193">String</span><span class="sxs-lookup"><span data-stu-id="054c1-193">String</span></span>|<span data-ttu-id="054c1-194">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="054c1-194">The name of the main Lob application file.</span></span> <span data-ttu-id="054c1-195">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="054c1-196">size</span><span class="sxs-lookup"><span data-stu-id="054c1-196">size</span></span>|<span data-ttu-id="054c1-197">Int64</span><span class="sxs-lookup"><span data-stu-id="054c1-197">Int64</span></span>|<span data-ttu-id="054c1-198">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="054c1-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="054c1-199">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="054c1-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="054c1-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="054c1-200">commandLine</span></span>|<span data-ttu-id="054c1-201">String</span><span class="sxs-lookup"><span data-stu-id="054c1-201">String</span></span>|<span data-ttu-id="054c1-202">コマンド ライン。</span><span class="sxs-lookup"><span data-stu-id="054c1-202">The command line.</span></span>|
|<span data-ttu-id="054c1-203">productCode</span><span class="sxs-lookup"><span data-stu-id="054c1-203">productCode</span></span>|<span data-ttu-id="054c1-204">String</span><span class="sxs-lookup"><span data-stu-id="054c1-204">String</span></span>|<span data-ttu-id="054c1-205">製品コード。</span><span class="sxs-lookup"><span data-stu-id="054c1-205">The product code.</span></span>|
|<span data-ttu-id="054c1-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="054c1-206">productVersion</span></span>|<span data-ttu-id="054c1-207">String</span><span class="sxs-lookup"><span data-stu-id="054c1-207">String</span></span>|<span data-ttu-id="054c1-208">Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。</span><span class="sxs-lookup"><span data-stu-id="054c1-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="054c1-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="054c1-209">ignoreVersionDetection</span></span>|<span data-ttu-id="054c1-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="054c1-210">Boolean</span></span>|<span data-ttu-id="054c1-211">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="054c1-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="054c1-212">自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="054c1-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="054c1-213">応答</span><span class="sxs-lookup"><span data-stu-id="054c1-213">Response</span></span>
<span data-ttu-id="054c1-214">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="054c1-214">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="054c1-215">例</span><span class="sxs-lookup"><span data-stu-id="054c1-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="054c1-216">要求</span><span class="sxs-lookup"><span data-stu-id="054c1-216">Request</span></span>
<span data-ttu-id="054c1-217">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="054c1-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="054c1-218">応答</span><span class="sxs-lookup"><span data-stu-id="054c1-218">Response</span></span>
<span data-ttu-id="054c1-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="054c1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```


