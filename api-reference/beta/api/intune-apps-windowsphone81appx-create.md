---
title: windowsPhone81AppX を作成する
description: 新しい windowsPhone81AppX オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678e21a2d3b662ed322dc26a07f2f110312a4ff1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166487"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="9fe99-103">windowsPhone81AppX を作成する</span><span class="sxs-lookup"><span data-stu-id="9fe99-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="9fe99-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fe99-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9fe99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fe99-106">新しい[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9fe99-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fe99-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9fe99-107">Prerequisites</span></span>
<span data-ttu-id="9fe99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fe99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9fe99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fe99-110">Permission type</span></span>|<span data-ttu-id="9fe99-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fe99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fe99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fe99-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe99-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fe99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fe99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe99-115">Not supported.</span></span>|
|<span data-ttu-id="9fe99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fe99-116">Application</span></span>|<span data-ttu-id="9fe99-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fe99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fe99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9fe99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe99-119">Request headers</span></span>
|<span data-ttu-id="9fe99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe99-120">Header</span></span>|<span data-ttu-id="9fe99-121">値</span><span class="sxs-lookup"><span data-stu-id="9fe99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fe99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fe99-122">Authorization</span></span>|<span data-ttu-id="9fe99-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9fe99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fe99-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9fe99-124">Accept</span></span>|<span data-ttu-id="9fe99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fe99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fe99-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9fe99-126">Request body</span></span>
<span data-ttu-id="9fe99-127">要求本文で、windowsPhone81AppX オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fe99-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="9fe99-128">次の表に、windowsPhone81AppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9fe99-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="9fe99-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fe99-129">Property</span></span>|<span data-ttu-id="9fe99-130">型</span><span class="sxs-lookup"><span data-stu-id="9fe99-130">Type</span></span>|<span data-ttu-id="9fe99-131">説明</span><span class="sxs-lookup"><span data-stu-id="9fe99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe99-132">id</span><span class="sxs-lookup"><span data-stu-id="9fe99-132">id</span></span>|<span data-ttu-id="9fe99-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9fe99-133">String</span></span>|<span data-ttu-id="9fe99-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9fe99-134">Key of the entity.</span></span> <span data-ttu-id="9fe99-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9fe99-136">displayName</span></span>|<span data-ttu-id="9fe99-137">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-137">String</span></span>|<span data-ttu-id="9fe99-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="9fe99-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9fe99-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-140">説明</span><span class="sxs-lookup"><span data-stu-id="9fe99-140">description</span></span>|<span data-ttu-id="9fe99-141">文字列</span><span class="sxs-lookup"><span data-stu-id="9fe99-141">String</span></span>|<span data-ttu-id="9fe99-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="9fe99-142">The description of the app.</span></span> <span data-ttu-id="9fe99-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9fe99-144">publisher</span></span>|<span data-ttu-id="9fe99-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9fe99-145">String</span></span>|<span data-ttu-id="9fe99-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="9fe99-146">The publisher of the app.</span></span> <span data-ttu-id="9fe99-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9fe99-148">largeIcon</span></span>|[<span data-ttu-id="9fe99-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9fe99-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9fe99-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="9fe99-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9fe99-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fe99-152">createdDateTime</span></span>|<span data-ttu-id="9fe99-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fe99-153">DateTimeOffset</span></span>|<span data-ttu-id="9fe99-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="9fe99-154">The date and time the app was created.</span></span> <span data-ttu-id="9fe99-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fe99-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9fe99-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fe99-157">DateTimeOffset</span></span>|<span data-ttu-id="9fe99-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="9fe99-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9fe99-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9fe99-160">isFeatured</span></span>|<span data-ttu-id="9fe99-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fe99-161">Boolean</span></span>|<span data-ttu-id="9fe99-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9fe99-163">privacyInformationUrl</span></span>|<span data-ttu-id="9fe99-164">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-164">String</span></span>|<span data-ttu-id="9fe99-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="9fe99-165">The privacy statement Url.</span></span> <span data-ttu-id="9fe99-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9fe99-167">informationUrl</span></span>|<span data-ttu-id="9fe99-168">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-168">String</span></span>|<span data-ttu-id="9fe99-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="9fe99-169">The more information Url.</span></span> <span data-ttu-id="9fe99-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-171">owner</span><span class="sxs-lookup"><span data-stu-id="9fe99-171">owner</span></span>|<span data-ttu-id="9fe99-172">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-172">String</span></span>|<span data-ttu-id="9fe99-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="9fe99-173">The owner of the app.</span></span> <span data-ttu-id="9fe99-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-175">developer</span><span class="sxs-lookup"><span data-stu-id="9fe99-175">developer</span></span>|<span data-ttu-id="9fe99-176">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-176">String</span></span>|<span data-ttu-id="9fe99-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="9fe99-177">The developer of the app.</span></span> <span data-ttu-id="9fe99-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-179">notes</span><span class="sxs-lookup"><span data-stu-id="9fe99-179">notes</span></span>|<span data-ttu-id="9fe99-180">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-180">String</span></span>|<span data-ttu-id="9fe99-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="9fe99-181">Notes for the app.</span></span> <span data-ttu-id="9fe99-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9fe99-183">uploadState</span></span>|<span data-ttu-id="9fe99-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9fe99-184">Int32</span></span>|<span data-ttu-id="9fe99-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="9fe99-185">The upload state.</span></span> <span data-ttu-id="9fe99-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9fe99-187">publishingState</span></span>|[<span data-ttu-id="9fe99-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9fe99-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9fe99-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="9fe99-189">The publishing state for the app.</span></span> <span data-ttu-id="9fe99-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="9fe99-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9fe99-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9fe99-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9fe99-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="9fe99-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9fe99-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9fe99-193">isAssigned</span></span>|<span data-ttu-id="9fe99-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fe99-194">Boolean</span></span>|<span data-ttu-id="9fe99-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9fe99-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9fe99-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fe99-197">roleScopeTagIds</span></span>|<span data-ttu-id="9fe99-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9fe99-198">String collection</span></span>|<span data-ttu-id="9fe99-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="9fe99-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9fe99-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fe99-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9fe99-201">committedContentVersion</span></span>|<span data-ttu-id="9fe99-202">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-202">String</span></span>|<span data-ttu-id="9fe99-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9fe99-203">The internal committed content version.</span></span> <span data-ttu-id="9fe99-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fe99-205">fileName</span><span class="sxs-lookup"><span data-stu-id="9fe99-205">fileName</span></span>|<span data-ttu-id="9fe99-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9fe99-206">String</span></span>|<span data-ttu-id="9fe99-207">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="9fe99-207">The name of the main Lob application file.</span></span> <span data-ttu-id="9fe99-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fe99-209">size</span><span class="sxs-lookup"><span data-stu-id="9fe99-209">size</span></span>|<span data-ttu-id="9fe99-210">Int64</span><span class="sxs-lookup"><span data-stu-id="9fe99-210">Int64</span></span>|<span data-ttu-id="9fe99-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="9fe99-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="9fe99-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9fe99-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fe99-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9fe99-213">applicableArchitectures</span></span>|[<span data-ttu-id="9fe99-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9fe99-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9fe99-215">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="9fe99-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9fe99-216">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="9fe99-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9fe99-217">identityName</span><span class="sxs-lookup"><span data-stu-id="9fe99-217">identityName</span></span>|<span data-ttu-id="9fe99-218">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-218">String</span></span>|<span data-ttu-id="9fe99-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="9fe99-219">The Identity Name.</span></span>|
|<span data-ttu-id="9fe99-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9fe99-220">identityPublisherHash</span></span>|<span data-ttu-id="9fe99-221">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-221">String</span></span>|<span data-ttu-id="9fe99-222">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="9fe99-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="9fe99-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fe99-223">identityResourceIdentifier</span></span>|<span data-ttu-id="9fe99-224">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-224">String</span></span>|<span data-ttu-id="9fe99-225">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="9fe99-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9fe99-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fe99-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9fe99-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fe99-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9fe99-228">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="9fe99-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9fe99-229">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fe99-229">phoneProductIdentifier</span></span>|<span data-ttu-id="9fe99-230">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-230">String</span></span>|<span data-ttu-id="9fe99-231">電話の製品識別子。</span><span class="sxs-lookup"><span data-stu-id="9fe99-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="9fe99-232">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="9fe99-232">phonePublisherId</span></span>|<span data-ttu-id="9fe99-233">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-233">String</span></span>|<span data-ttu-id="9fe99-234">電話の発行元 Id。</span><span class="sxs-lookup"><span data-stu-id="9fe99-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="9fe99-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9fe99-235">identityVersion</span></span>|<span data-ttu-id="9fe99-236">String</span><span class="sxs-lookup"><span data-stu-id="9fe99-236">String</span></span>|<span data-ttu-id="9fe99-237">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9fe99-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9fe99-238">応答</span><span class="sxs-lookup"><span data-stu-id="9fe99-238">Response</span></span>
<span data-ttu-id="9fe99-239">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9fe99-239">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fe99-240">例</span><span class="sxs-lookup"><span data-stu-id="9fe99-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fe99-241">要求</span><span class="sxs-lookup"><span data-stu-id="9fe99-241">Request</span></span>
<span data-ttu-id="9fe99-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9fe99-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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

### <a name="response"></a><span data-ttu-id="9fe99-243">応答</span><span class="sxs-lookup"><span data-stu-id="9fe99-243">Response</span></span>
<span data-ttu-id="9fe99-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9fe99-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




