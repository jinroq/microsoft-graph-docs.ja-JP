---
title: WindowsPhone81AppXBundle を作成する
description: 新しい windowsPhone81AppXBundle オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c7ced679757c316485eb436808bee5f02c26fb1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973069"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="e81d5-103">WindowsPhone81AppXBundle を作成する</span><span class="sxs-lookup"><span data-stu-id="e81d5-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="e81d5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e81d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e81d5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e81d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e81d5-106">新しい[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e81d5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e81d5-107">Prerequisites</span></span>
<span data-ttu-id="e81d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e81d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e81d5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e81d5-110">Permission type</span></span>|<span data-ttu-id="e81d5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e81d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e81d5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e81d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e81d5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e81d5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e81d5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e81d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e81d5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e81d5-115">Not supported.</span></span>|
|<span data-ttu-id="e81d5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e81d5-116">Application</span></span>|<span data-ttu-id="e81d5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e81d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e81d5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e81d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e81d5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e81d5-119">Request headers</span></span>
|<span data-ttu-id="e81d5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e81d5-120">Header</span></span>|<span data-ttu-id="e81d5-121">値</span><span class="sxs-lookup"><span data-stu-id="e81d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e81d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e81d5-122">Authorization</span></span>|<span data-ttu-id="e81d5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e81d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e81d5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e81d5-124">Accept</span></span>|<span data-ttu-id="e81d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e81d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e81d5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e81d5-126">Request body</span></span>
<span data-ttu-id="e81d5-127">要求本文で、windowsPhone81AppXBundle オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="e81d5-128">次の表に、windowsPhone81AppXBundle の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="e81d5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e81d5-129">Property</span></span>|<span data-ttu-id="e81d5-130">型</span><span class="sxs-lookup"><span data-stu-id="e81d5-130">Type</span></span>|<span data-ttu-id="e81d5-131">説明</span><span class="sxs-lookup"><span data-stu-id="e81d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e81d5-132">id</span><span class="sxs-lookup"><span data-stu-id="e81d5-132">id</span></span>|<span data-ttu-id="e81d5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e81d5-133">String</span></span>|<span data-ttu-id="e81d5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e81d5-134">Key of the entity.</span></span> <span data-ttu-id="e81d5-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e81d5-136">displayName</span></span>|<span data-ttu-id="e81d5-137">文字列</span><span class="sxs-lookup"><span data-stu-id="e81d5-137">String</span></span>|<span data-ttu-id="e81d5-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e81d5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e81d5-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-140">description</span><span class="sxs-lookup"><span data-stu-id="e81d5-140">description</span></span>|<span data-ttu-id="e81d5-141">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-141">String</span></span>|<span data-ttu-id="e81d5-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e81d5-142">The description of the app.</span></span> <span data-ttu-id="e81d5-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e81d5-144">publisher</span></span>|<span data-ttu-id="e81d5-145">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-145">String</span></span>|<span data-ttu-id="e81d5-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e81d5-146">The publisher of the app.</span></span> <span data-ttu-id="e81d5-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e81d5-148">largeIcon</span></span>|[<span data-ttu-id="e81d5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e81d5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e81d5-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e81d5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e81d5-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e81d5-152">createdDateTime</span></span>|<span data-ttu-id="e81d5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81d5-153">DateTimeOffset</span></span>|<span data-ttu-id="e81d5-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e81d5-154">The date and time the app was created.</span></span> <span data-ttu-id="e81d5-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e81d5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e81d5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81d5-157">DateTimeOffset</span></span>|<span data-ttu-id="e81d5-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e81d5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e81d5-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e81d5-160">isFeatured</span></span>|<span data-ttu-id="e81d5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e81d5-161">Boolean</span></span>|<span data-ttu-id="e81d5-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e81d5-163">privacyInformationUrl</span></span>|<span data-ttu-id="e81d5-164">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-164">String</span></span>|<span data-ttu-id="e81d5-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e81d5-165">The privacy statement Url.</span></span> <span data-ttu-id="e81d5-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e81d5-167">informationUrl</span></span>|<span data-ttu-id="e81d5-168">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-168">String</span></span>|<span data-ttu-id="e81d5-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e81d5-169">The more information Url.</span></span> <span data-ttu-id="e81d5-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-171">owner</span><span class="sxs-lookup"><span data-stu-id="e81d5-171">owner</span></span>|<span data-ttu-id="e81d5-172">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-172">String</span></span>|<span data-ttu-id="e81d5-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e81d5-173">The owner of the app.</span></span> <span data-ttu-id="e81d5-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-175">developer</span><span class="sxs-lookup"><span data-stu-id="e81d5-175">developer</span></span>|<span data-ttu-id="e81d5-176">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-176">String</span></span>|<span data-ttu-id="e81d5-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e81d5-177">The developer of the app.</span></span> <span data-ttu-id="e81d5-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-179">notes</span><span class="sxs-lookup"><span data-stu-id="e81d5-179">notes</span></span>|<span data-ttu-id="e81d5-180">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-180">String</span></span>|<span data-ttu-id="e81d5-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e81d5-181">Notes for the app.</span></span> <span data-ttu-id="e81d5-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e81d5-183">uploadState</span></span>|<span data-ttu-id="e81d5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e81d5-184">Int32</span></span>|<span data-ttu-id="e81d5-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="e81d5-185">The upload state.</span></span> <span data-ttu-id="e81d5-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e81d5-187">publishingState</span></span>|[<span data-ttu-id="e81d5-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e81d5-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e81d5-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e81d5-189">The publishing state for the app.</span></span> <span data-ttu-id="e81d5-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e81d5-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e81d5-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e81d5-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e81d5-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e81d5-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e81d5-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e81d5-193">isAssigned</span></span>|<span data-ttu-id="e81d5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e81d5-194">Boolean</span></span>|<span data-ttu-id="e81d5-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e81d5-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e81d5-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e81d5-197">roleScopeTagIds</span></span>|<span data-ttu-id="e81d5-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e81d5-198">String collection</span></span>|<span data-ttu-id="e81d5-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="e81d5-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e81d5-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e81d5-201">dependentAppCount</span></span>|<span data-ttu-id="e81d5-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e81d5-202">Int32</span></span>|<span data-ttu-id="e81d5-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="e81d5-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e81d5-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81d5-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e81d5-205">committedContentVersion</span></span>|<span data-ttu-id="e81d5-206">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-206">String</span></span>|<span data-ttu-id="e81d5-207">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e81d5-207">The internal committed content version.</span></span> <span data-ttu-id="e81d5-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81d5-209">fileName</span><span class="sxs-lookup"><span data-stu-id="e81d5-209">fileName</span></span>|<span data-ttu-id="e81d5-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e81d5-210">String</span></span>|<span data-ttu-id="e81d5-211">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="e81d5-211">The name of the main Lob application file.</span></span> <span data-ttu-id="e81d5-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81d5-213">size</span><span class="sxs-lookup"><span data-stu-id="e81d5-213">size</span></span>|<span data-ttu-id="e81d5-214">Int64</span><span class="sxs-lookup"><span data-stu-id="e81d5-214">Int64</span></span>|<span data-ttu-id="e81d5-215">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="e81d5-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="e81d5-216">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e81d5-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81d5-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e81d5-217">applicableArchitectures</span></span>|[<span data-ttu-id="e81d5-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e81d5-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e81d5-219">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="e81d5-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e81d5-220">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e81d5-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="e81d5-221">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="e81d5-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e81d5-222">identityName</span><span class="sxs-lookup"><span data-stu-id="e81d5-222">identityName</span></span>|<span data-ttu-id="e81d5-223">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-223">String</span></span>|<span data-ttu-id="e81d5-224">ID 名。</span><span class="sxs-lookup"><span data-stu-id="e81d5-224">The Identity Name.</span></span> <span data-ttu-id="e81d5-225">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e81d5-226">identityPublisherHash</span></span>|<span data-ttu-id="e81d5-227">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-227">String</span></span>|<span data-ttu-id="e81d5-228">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="e81d5-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="e81d5-229">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e81d5-230">identityResourceIdentifier</span></span>|<span data-ttu-id="e81d5-231">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-231">String</span></span>|<span data-ttu-id="e81d5-232">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="e81d5-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="e81d5-233">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e81d5-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e81d5-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e81d5-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e81d5-236">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="e81d5-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="e81d5-237">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="e81d5-238">phoneProductIdentifier</span></span>|<span data-ttu-id="e81d5-239">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-239">String</span></span>|<span data-ttu-id="e81d5-240">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="e81d5-240">The Phone Product Identifier.</span></span> <span data-ttu-id="e81d5-241">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="e81d5-242">phonePublisherId</span></span>|<span data-ttu-id="e81d5-243">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-243">String</span></span>|<span data-ttu-id="e81d5-244">電話の発行元 Id。 [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e81d5-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e81d5-245">identityVersion</span></span>|<span data-ttu-id="e81d5-246">String</span><span class="sxs-lookup"><span data-stu-id="e81d5-246">String</span></span>|<span data-ttu-id="e81d5-247">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e81d5-247">The identity version.</span></span> <span data-ttu-id="e81d5-248">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81d5-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="e81d5-249">appXPackageInformationList</span></span>|<span data-ttu-id="e81d5-250">[Windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e81d5-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="e81d5-251">AppX パッケージ情報のリスト。</span><span class="sxs-lookup"><span data-stu-id="e81d5-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="e81d5-252">応答</span><span class="sxs-lookup"><span data-stu-id="e81d5-252">Response</span></span>
<span data-ttu-id="e81d5-253">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e81d5-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81d5-254">例</span><span class="sxs-lookup"><span data-stu-id="e81d5-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="e81d5-255">要求</span><span class="sxs-lookup"><span data-stu-id="e81d5-255">Request</span></span>
<span data-ttu-id="e81d5-256">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e81d5-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e81d5-257">応答</span><span class="sxs-lookup"><span data-stu-id="e81d5-257">Response</span></span>
<span data-ttu-id="e81d5-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e81d5-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```





