---
title: WindowsPhoneXAP を作成します。
description: 新しい windowsPhoneXAP オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7ff4f085a79cf16ae724df045cd6140161945a57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939792"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="1652c-103">WindowsPhoneXAP を作成します。</span><span class="sxs-lookup"><span data-stu-id="1652c-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="1652c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1652c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1652c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1652c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1652c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1652c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1652c-107">新しい[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1652c-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1652c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1652c-108">Prerequisites</span></span>
<span data-ttu-id="1652c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1652c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1652c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1652c-111">Permission type</span></span>|<span data-ttu-id="1652c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1652c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1652c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1652c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1652c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1652c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1652c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1652c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1652c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1652c-116">Not supported.</span></span>|
|<span data-ttu-id="1652c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1652c-117">Application</span></span>|<span data-ttu-id="1652c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1652c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1652c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1652c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1652c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1652c-120">Request headers</span></span>
|<span data-ttu-id="1652c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1652c-121">Header</span></span>|<span data-ttu-id="1652c-122">値</span><span class="sxs-lookup"><span data-stu-id="1652c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1652c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1652c-123">Authorization</span></span>|<span data-ttu-id="1652c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1652c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1652c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1652c-125">Accept</span></span>|<span data-ttu-id="1652c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1652c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1652c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1652c-127">Request body</span></span>
<span data-ttu-id="1652c-128">要求の本文に windowsPhoneXAP オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1652c-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="1652c-129">次の表は、windowsPhoneXAP を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1652c-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="1652c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1652c-130">Property</span></span>|<span data-ttu-id="1652c-131">種類</span><span class="sxs-lookup"><span data-stu-id="1652c-131">Type</span></span>|<span data-ttu-id="1652c-132">説明</span><span class="sxs-lookup"><span data-stu-id="1652c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1652c-133">ID</span><span class="sxs-lookup"><span data-stu-id="1652c-133">id</span></span>|<span data-ttu-id="1652c-134">String</span><span class="sxs-lookup"><span data-stu-id="1652c-134">String</span></span>|<span data-ttu-id="1652c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1652c-135">Key of the entity.</span></span> <span data-ttu-id="1652c-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1652c-137">displayName</span></span>|<span data-ttu-id="1652c-138">String</span><span class="sxs-lookup"><span data-stu-id="1652c-138">String</span></span>|<span data-ttu-id="1652c-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1652c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1652c-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-141">説明</span><span class="sxs-lookup"><span data-stu-id="1652c-141">description</span></span>|<span data-ttu-id="1652c-142">String</span><span class="sxs-lookup"><span data-stu-id="1652c-142">String</span></span>|<span data-ttu-id="1652c-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1652c-143">The description of the app.</span></span> <span data-ttu-id="1652c-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1652c-145">publisher</span></span>|<span data-ttu-id="1652c-146">String</span><span class="sxs-lookup"><span data-stu-id="1652c-146">String</span></span>|<span data-ttu-id="1652c-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1652c-147">The publisher of the app.</span></span> <span data-ttu-id="1652c-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1652c-149">largeIcon</span></span>|[<span data-ttu-id="1652c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1652c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1652c-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="1652c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1652c-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1652c-153">createdDateTime</span></span>|<span data-ttu-id="1652c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1652c-154">DateTimeOffset</span></span>|<span data-ttu-id="1652c-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1652c-155">The date and time the app was created.</span></span> <span data-ttu-id="1652c-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1652c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1652c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1652c-158">DateTimeOffset</span></span>|<span data-ttu-id="1652c-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1652c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1652c-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1652c-161">isFeatured</span></span>|<span data-ttu-id="1652c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1652c-162">Boolean</span></span>|<span data-ttu-id="1652c-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1652c-164">privacyInformationUrl</span></span>|<span data-ttu-id="1652c-165">String</span><span class="sxs-lookup"><span data-stu-id="1652c-165">String</span></span>|<span data-ttu-id="1652c-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1652c-166">The privacy statement Url.</span></span> <span data-ttu-id="1652c-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1652c-168">informationUrl</span></span>|<span data-ttu-id="1652c-169">String</span><span class="sxs-lookup"><span data-stu-id="1652c-169">String</span></span>|<span data-ttu-id="1652c-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1652c-170">The more information Url.</span></span> <span data-ttu-id="1652c-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-172">owner</span><span class="sxs-lookup"><span data-stu-id="1652c-172">owner</span></span>|<span data-ttu-id="1652c-173">String</span><span class="sxs-lookup"><span data-stu-id="1652c-173">String</span></span>|<span data-ttu-id="1652c-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1652c-174">The owner of the app.</span></span> <span data-ttu-id="1652c-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-176">developer</span><span class="sxs-lookup"><span data-stu-id="1652c-176">developer</span></span>|<span data-ttu-id="1652c-177">String</span><span class="sxs-lookup"><span data-stu-id="1652c-177">String</span></span>|<span data-ttu-id="1652c-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1652c-178">The developer of the app.</span></span> <span data-ttu-id="1652c-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-180">notes</span><span class="sxs-lookup"><span data-stu-id="1652c-180">notes</span></span>|<span data-ttu-id="1652c-181">String</span><span class="sxs-lookup"><span data-stu-id="1652c-181">String</span></span>|<span data-ttu-id="1652c-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1652c-182">Notes for the app.</span></span> <span data-ttu-id="1652c-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1652c-184">uploadState</span></span>|<span data-ttu-id="1652c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1652c-185">Int32</span></span>|<span data-ttu-id="1652c-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="1652c-186">The upload state.</span></span> <span data-ttu-id="1652c-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1652c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1652c-188">publishingState</span></span>|[<span data-ttu-id="1652c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1652c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1652c-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1652c-190">The publishing state for the app.</span></span> <span data-ttu-id="1652c-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1652c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1652c-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1652c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1652c-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1652c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1652c-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1652c-194">committedContentVersion</span></span>|<span data-ttu-id="1652c-195">String</span><span class="sxs-lookup"><span data-stu-id="1652c-195">String</span></span>|<span data-ttu-id="1652c-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1652c-196">The internal committed content version.</span></span> <span data-ttu-id="1652c-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1652c-198">fileName</span><span class="sxs-lookup"><span data-stu-id="1652c-198">fileName</span></span>|<span data-ttu-id="1652c-199">String</span><span class="sxs-lookup"><span data-stu-id="1652c-199">String</span></span>|<span data-ttu-id="1652c-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1652c-200">The name of the main Lob application file.</span></span> <span data-ttu-id="1652c-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1652c-202">size</span><span class="sxs-lookup"><span data-stu-id="1652c-202">size</span></span>|<span data-ttu-id="1652c-203">Int64</span><span class="sxs-lookup"><span data-stu-id="1652c-203">Int64</span></span>|<span data-ttu-id="1652c-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1652c-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="1652c-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1652c-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1652c-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1652c-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1652c-207">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1652c-207">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1652c-208">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="1652c-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1652c-209">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="1652c-209">productIdentifier</span></span>|<span data-ttu-id="1652c-210">String</span><span class="sxs-lookup"><span data-stu-id="1652c-210">String</span></span>|<span data-ttu-id="1652c-211">製品の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1652c-211">The Product Identifier.</span></span>|
|<span data-ttu-id="1652c-212">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1652c-212">identityVersion</span></span>|<span data-ttu-id="1652c-213">String</span><span class="sxs-lookup"><span data-stu-id="1652c-213">String</span></span>|<span data-ttu-id="1652c-214">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1652c-214">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1652c-215">応答</span><span class="sxs-lookup"><span data-stu-id="1652c-215">Response</span></span>
<span data-ttu-id="1652c-216">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1652c-216">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1652c-217">例</span><span class="sxs-lookup"><span data-stu-id="1652c-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="1652c-218">要求</span><span class="sxs-lookup"><span data-stu-id="1652c-218">Request</span></span>
<span data-ttu-id="1652c-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1652c-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1143

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

### <a name="response"></a><span data-ttu-id="1652c-220">応答</span><span class="sxs-lookup"><span data-stu-id="1652c-220">Response</span></span>
<span data-ttu-id="1652c-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1652c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1251

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





