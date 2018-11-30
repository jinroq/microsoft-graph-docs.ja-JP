---
title: termsAndConditions の作成
description: 新しい termsAndConditions オブジェクトを作成します。
ms.openlocfilehash: 1947a41ddfe108d8f44c899786d0b0b129ac6939
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072622"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="e089b-103">termsAndConditions の作成</span><span class="sxs-lookup"><span data-stu-id="e089b-103">Create termsAndConditions</span></span>

> <span data-ttu-id="e089b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e089b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e089b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e089b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e089b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e089b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e089b-107">新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e089b-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e089b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e089b-108">Prerequisites</span></span>
<span data-ttu-id="e089b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e089b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e089b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e089b-111">Permission type</span></span>|<span data-ttu-id="e089b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e089b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e089b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e089b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e089b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e089b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e089b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e089b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e089b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e089b-116">Not supported.</span></span>|
|<span data-ttu-id="e089b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e089b-117">Application</span></span>|<span data-ttu-id="e089b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e089b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e089b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e089b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="e089b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e089b-120">Request headers</span></span>
|<span data-ttu-id="e089b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e089b-121">Header</span></span>|<span data-ttu-id="e089b-122">値</span><span class="sxs-lookup"><span data-stu-id="e089b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e089b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e089b-123">Authorization</span></span>|<span data-ttu-id="e089b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e089b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e089b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e089b-125">Accept</span></span>|<span data-ttu-id="e089b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e089b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e089b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e089b-127">Request body</span></span>
<span data-ttu-id="e089b-128">要求本文において、termsAndConditions オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e089b-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="e089b-129">次の表に、termsAndConditions の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e089b-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="e089b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e089b-130">Property</span></span>|<span data-ttu-id="e089b-131">型</span><span class="sxs-lookup"><span data-stu-id="e089b-131">Type</span></span>|<span data-ttu-id="e089b-132">説明</span><span class="sxs-lookup"><span data-stu-id="e089b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e089b-133">id</span><span class="sxs-lookup"><span data-stu-id="e089b-133">id</span></span>|<span data-ttu-id="e089b-134">String</span><span class="sxs-lookup"><span data-stu-id="e089b-134">String</span></span>|<span data-ttu-id="e089b-135">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e089b-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="e089b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e089b-136">createdDateTime</span></span>|<span data-ttu-id="e089b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e089b-137">DateTimeOffset</span></span>|<span data-ttu-id="e089b-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e089b-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="e089b-139">変更された日時</span><span class="sxs-lookup"><span data-stu-id="e089b-139">modifiedDateTime</span></span>|<span data-ttu-id="e089b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e089b-140">DateTimeOffset</span></span>|<span data-ttu-id="e089b-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e089b-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e089b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e089b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e089b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e089b-143">DateTimeOffset</span></span>|<span data-ttu-id="e089b-144">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e089b-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e089b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e089b-145">displayName</span></span>|<span data-ttu-id="e089b-146">String</span><span class="sxs-lookup"><span data-stu-id="e089b-146">String</span></span>|<span data-ttu-id="e089b-147">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="e089b-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="e089b-148">説明</span><span class="sxs-lookup"><span data-stu-id="e089b-148">description</span></span>|<span data-ttu-id="e089b-149">String</span><span class="sxs-lookup"><span data-stu-id="e089b-149">String</span></span>|<span data-ttu-id="e089b-150">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e089b-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="e089b-151">タイトル</span><span class="sxs-lookup"><span data-stu-id="e089b-151">title</span></span>|<span data-ttu-id="e089b-152">String</span><span class="sxs-lookup"><span data-stu-id="e089b-152">String</span></span>|<span data-ttu-id="e089b-153">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="e089b-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="e089b-154">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e089b-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e089b-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="e089b-155">bodyText</span></span>|<span data-ttu-id="e089b-156">String</span><span class="sxs-lookup"><span data-stu-id="e089b-156">String</span></span>|<span data-ttu-id="e089b-157">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="e089b-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="e089b-158">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e089b-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e089b-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="e089b-159">acceptanceStatement</span></span>|<span data-ttu-id="e089b-160">String</span><span class="sxs-lookup"><span data-stu-id="e089b-160">String</span></span>|<span data-ttu-id="e089b-161">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="e089b-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="e089b-162">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e089b-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e089b-163">version</span><span class="sxs-lookup"><span data-stu-id="e089b-163">version</span></span>|<span data-ttu-id="e089b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e089b-164">Int32</span></span>|<span data-ttu-id="e089b-165">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="e089b-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="e089b-166">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="e089b-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e089b-167">応答</span><span class="sxs-lookup"><span data-stu-id="e089b-167">Response</span></span>
<span data-ttu-id="e089b-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e089b-168">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e089b-169">例</span><span class="sxs-lookup"><span data-stu-id="e089b-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="e089b-170">要求</span><span class="sxs-lookup"><span data-stu-id="e089b-170">Request</span></span>
<span data-ttu-id="e089b-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e089b-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="e089b-172">応答</span><span class="sxs-lookup"><span data-stu-id="e089b-172">Response</span></span>
<span data-ttu-id="e089b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e089b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```





