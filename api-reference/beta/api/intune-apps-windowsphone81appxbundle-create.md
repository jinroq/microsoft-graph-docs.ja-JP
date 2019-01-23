---
title: WindowsPhone81AppXBundle を作成します。
description: 新しい windowsPhone81AppXBundle オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c660e7a211fae6ea4f1a180b4b1db75af644f9a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401944"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="b6567-103">WindowsPhone81AppXBundle を作成します。</span><span class="sxs-lookup"><span data-stu-id="b6567-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="b6567-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6567-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6567-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6567-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6567-107">新しい[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6567-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6567-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6567-108">Prerequisites</span></span>
<span data-ttu-id="b6567-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6567-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6567-111">Permission type</span></span>|<span data-ttu-id="b6567-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6567-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6567-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6567-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6567-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6567-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6567-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6567-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6567-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6567-116">Not supported.</span></span>|
|<span data-ttu-id="b6567-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6567-117">Application</span></span>|<span data-ttu-id="b6567-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6567-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6567-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6567-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b6567-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6567-120">Request headers</span></span>
|<span data-ttu-id="b6567-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6567-121">Header</span></span>|<span data-ttu-id="b6567-122">値</span><span class="sxs-lookup"><span data-stu-id="b6567-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6567-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6567-123">Authorization</span></span>|<span data-ttu-id="b6567-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b6567-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6567-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6567-125">Accept</span></span>|<span data-ttu-id="b6567-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6567-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6567-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6567-127">Request body</span></span>
<span data-ttu-id="b6567-128">要求の本文に windowsPhone81AppXBundle オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6567-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="b6567-129">次の表は、windowsPhone81AppXBundle を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b6567-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="b6567-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6567-130">Property</span></span>|<span data-ttu-id="b6567-131">型</span><span class="sxs-lookup"><span data-stu-id="b6567-131">Type</span></span>|<span data-ttu-id="b6567-132">説明</span><span class="sxs-lookup"><span data-stu-id="b6567-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6567-133">id</span><span class="sxs-lookup"><span data-stu-id="b6567-133">id</span></span>|<span data-ttu-id="b6567-134">String</span><span class="sxs-lookup"><span data-stu-id="b6567-134">String</span></span>|<span data-ttu-id="b6567-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b6567-135">Key of the entity.</span></span> <span data-ttu-id="b6567-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b6567-137">displayName</span></span>|<span data-ttu-id="b6567-138">String</span><span class="sxs-lookup"><span data-stu-id="b6567-138">String</span></span>|<span data-ttu-id="b6567-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b6567-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b6567-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-141">説明</span><span class="sxs-lookup"><span data-stu-id="b6567-141">description</span></span>|<span data-ttu-id="b6567-142">String</span><span class="sxs-lookup"><span data-stu-id="b6567-142">String</span></span>|<span data-ttu-id="b6567-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b6567-143">The description of the app.</span></span> <span data-ttu-id="b6567-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b6567-145">publisher</span></span>|<span data-ttu-id="b6567-146">String</span><span class="sxs-lookup"><span data-stu-id="b6567-146">String</span></span>|<span data-ttu-id="b6567-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b6567-147">The publisher of the app.</span></span> <span data-ttu-id="b6567-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b6567-149">largeIcon</span></span>|[<span data-ttu-id="b6567-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b6567-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b6567-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="b6567-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b6567-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6567-153">createdDateTime</span></span>|<span data-ttu-id="b6567-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6567-154">DateTimeOffset</span></span>|<span data-ttu-id="b6567-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b6567-155">The date and time the app was created.</span></span> <span data-ttu-id="b6567-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6567-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b6567-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6567-158">DateTimeOffset</span></span>|<span data-ttu-id="b6567-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b6567-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b6567-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b6567-161">isFeatured</span></span>|<span data-ttu-id="b6567-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6567-162">Boolean</span></span>|<span data-ttu-id="b6567-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b6567-164">privacyInformationUrl</span></span>|<span data-ttu-id="b6567-165">String</span><span class="sxs-lookup"><span data-stu-id="b6567-165">String</span></span>|<span data-ttu-id="b6567-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b6567-166">The privacy statement Url.</span></span> <span data-ttu-id="b6567-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b6567-168">informationUrl</span></span>|<span data-ttu-id="b6567-169">String</span><span class="sxs-lookup"><span data-stu-id="b6567-169">String</span></span>|<span data-ttu-id="b6567-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b6567-170">The more information Url.</span></span> <span data-ttu-id="b6567-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-172">owner</span><span class="sxs-lookup"><span data-stu-id="b6567-172">owner</span></span>|<span data-ttu-id="b6567-173">String</span><span class="sxs-lookup"><span data-stu-id="b6567-173">String</span></span>|<span data-ttu-id="b6567-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b6567-174">The owner of the app.</span></span> <span data-ttu-id="b6567-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-176">developer</span><span class="sxs-lookup"><span data-stu-id="b6567-176">developer</span></span>|<span data-ttu-id="b6567-177">String</span><span class="sxs-lookup"><span data-stu-id="b6567-177">String</span></span>|<span data-ttu-id="b6567-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b6567-178">The developer of the app.</span></span> <span data-ttu-id="b6567-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-180">notes</span><span class="sxs-lookup"><span data-stu-id="b6567-180">notes</span></span>|<span data-ttu-id="b6567-181">String</span><span class="sxs-lookup"><span data-stu-id="b6567-181">String</span></span>|<span data-ttu-id="b6567-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b6567-182">Notes for the app.</span></span> <span data-ttu-id="b6567-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b6567-184">uploadState</span></span>|<span data-ttu-id="b6567-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b6567-185">Int32</span></span>|<span data-ttu-id="b6567-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="b6567-186">The upload state.</span></span> <span data-ttu-id="b6567-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b6567-188">publishingState</span></span>|[<span data-ttu-id="b6567-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b6567-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b6567-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b6567-190">The publishing state for the app.</span></span> <span data-ttu-id="b6567-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b6567-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b6567-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b6567-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b6567-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b6567-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b6567-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b6567-194">isAssigned</span></span>|<span data-ttu-id="b6567-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6567-195">Boolean</span></span>|<span data-ttu-id="b6567-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="b6567-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b6567-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6567-198">roleScopeTagIds</span></span>|<span data-ttu-id="b6567-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b6567-199">String collection</span></span>|<span data-ttu-id="b6567-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b6567-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b6567-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6567-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b6567-202">committedContentVersion</span></span>|<span data-ttu-id="b6567-203">String</span><span class="sxs-lookup"><span data-stu-id="b6567-203">String</span></span>|<span data-ttu-id="b6567-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6567-204">The internal committed content version.</span></span> <span data-ttu-id="b6567-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6567-206">fileName</span><span class="sxs-lookup"><span data-stu-id="b6567-206">fileName</span></span>|<span data-ttu-id="b6567-207">String</span><span class="sxs-lookup"><span data-stu-id="b6567-207">String</span></span>|<span data-ttu-id="b6567-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="b6567-208">The name of the main Lob application file.</span></span> <span data-ttu-id="b6567-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6567-210">size</span><span class="sxs-lookup"><span data-stu-id="b6567-210">size</span></span>|<span data-ttu-id="b6567-211">Int64</span><span class="sxs-lookup"><span data-stu-id="b6567-211">Int64</span></span>|<span data-ttu-id="b6567-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="b6567-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="b6567-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6567-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b6567-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b6567-214">applicableArchitectures</span></span>|[<span data-ttu-id="b6567-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b6567-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b6567-216">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="b6567-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b6567-217">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b6567-217">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="b6567-218">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b6567-218">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b6567-219">identityName</span><span class="sxs-lookup"><span data-stu-id="b6567-219">identityName</span></span>|<span data-ttu-id="b6567-220">String</span><span class="sxs-lookup"><span data-stu-id="b6567-220">String</span></span>|<span data-ttu-id="b6567-221">ID 名。</span><span class="sxs-lookup"><span data-stu-id="b6567-221">The Identity Name.</span></span> <span data-ttu-id="b6567-222">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-223">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b6567-223">identityPublisherHash</span></span>|<span data-ttu-id="b6567-224">String</span><span class="sxs-lookup"><span data-stu-id="b6567-224">String</span></span>|<span data-ttu-id="b6567-225">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="b6567-225">The Identity Publisher Hash.</span></span> <span data-ttu-id="b6567-226">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6567-227">identityResourceIdentifier</span></span>|<span data-ttu-id="b6567-228">String</span><span class="sxs-lookup"><span data-stu-id="b6567-228">String</span></span>|<span data-ttu-id="b6567-229">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="b6567-229">The Identity Resource Identifier.</span></span> <span data-ttu-id="b6567-230">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6567-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b6567-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6567-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b6567-233">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="b6567-233">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="b6567-234">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-235">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6567-235">phoneProductIdentifier</span></span>|<span data-ttu-id="b6567-236">String</span><span class="sxs-lookup"><span data-stu-id="b6567-236">String</span></span>|<span data-ttu-id="b6567-237">電話の製品識別子です。</span><span class="sxs-lookup"><span data-stu-id="b6567-237">The Phone Product Identifier.</span></span> <span data-ttu-id="b6567-238">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-239">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="b6567-239">phonePublisherId</span></span>|<span data-ttu-id="b6567-240">String</span><span class="sxs-lookup"><span data-stu-id="b6567-240">String</span></span>|<span data-ttu-id="b6567-241">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承した電話のパブリッシャー id。</span><span class="sxs-lookup"><span data-stu-id="b6567-241">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b6567-242">identityVersion</span></span>|<span data-ttu-id="b6567-243">String</span><span class="sxs-lookup"><span data-stu-id="b6567-243">String</span></span>|<span data-ttu-id="b6567-244">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6567-244">The identity version.</span></span> <span data-ttu-id="b6567-245">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b6567-245">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b6567-246">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="b6567-246">appXPackageInformationList</span></span>|<span data-ttu-id="b6567-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6567-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="b6567-248">AppX パッケージ情報の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b6567-248">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="b6567-249">応答</span><span class="sxs-lookup"><span data-stu-id="b6567-249">Response</span></span>
<span data-ttu-id="b6567-250">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b6567-250">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6567-251">例</span><span class="sxs-lookup"><span data-stu-id="b6567-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6567-252">要求</span><span class="sxs-lookup"><span data-stu-id="b6567-252">Request</span></span>
<span data-ttu-id="b6567-253">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6567-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2184

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
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b6567-254">応答</span><span class="sxs-lookup"><span data-stu-id="b6567-254">Response</span></span>
<span data-ttu-id="b6567-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6567-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2356

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
        "v10_1803": true
      }
    }
  ]
}
```




