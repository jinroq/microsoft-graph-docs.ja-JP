---
title: termsAndConditions の作成
description: 新しい termsAndConditions オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff711b887c012d795b5c2f5757ba22f2d8a79de5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251721"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="829e6-103">termsAndConditions の作成</span><span class="sxs-lookup"><span data-stu-id="829e6-103">Create termsAndConditions</span></span>

> <span data-ttu-id="829e6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="829e6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="829e6-105">新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="829e6-105">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="829e6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="829e6-106">Prerequisites</span></span>
<span data-ttu-id="829e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="829e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="829e6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="829e6-109">Permission type</span></span>|<span data-ttu-id="829e6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="829e6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="829e6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="829e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="829e6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="829e6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="829e6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="829e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="829e6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="829e6-114">Not supported.</span></span>|
|<span data-ttu-id="829e6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="829e6-115">Application</span></span>|<span data-ttu-id="829e6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="829e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="829e6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="829e6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="829e6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="829e6-118">Request headers</span></span>
|<span data-ttu-id="829e6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="829e6-119">Header</span></span>|<span data-ttu-id="829e6-120">値</span><span class="sxs-lookup"><span data-stu-id="829e6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="829e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="829e6-121">Authorization</span></span>|<span data-ttu-id="829e6-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="829e6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="829e6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="829e6-123">Accept</span></span>|<span data-ttu-id="829e6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="829e6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="829e6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="829e6-125">Request body</span></span>
<span data-ttu-id="829e6-126">要求本文において、termsAndConditions オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="829e6-126">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="829e6-127">次の表に、termsAndConditions の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="829e6-127">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="829e6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="829e6-128">Property</span></span>|<span data-ttu-id="829e6-129">型</span><span class="sxs-lookup"><span data-stu-id="829e6-129">Type</span></span>|<span data-ttu-id="829e6-130">説明</span><span class="sxs-lookup"><span data-stu-id="829e6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="829e6-131">id</span><span class="sxs-lookup"><span data-stu-id="829e6-131">id</span></span>|<span data-ttu-id="829e6-132">文字列</span><span class="sxs-lookup"><span data-stu-id="829e6-132">String</span></span>|<span data-ttu-id="829e6-133">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="829e6-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="829e6-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="829e6-134">createdDateTime</span></span>|<span data-ttu-id="829e6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="829e6-135">DateTimeOffset</span></span>|<span data-ttu-id="829e6-136">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="829e6-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="829e6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="829e6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="829e6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="829e6-138">DateTimeOffset</span></span>|<span data-ttu-id="829e6-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="829e6-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="829e6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="829e6-140">displayName</span></span>|<span data-ttu-id="829e6-141">String</span><span class="sxs-lookup"><span data-stu-id="829e6-141">String</span></span>|<span data-ttu-id="829e6-142">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="829e6-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="829e6-143">説明</span><span class="sxs-lookup"><span data-stu-id="829e6-143">description</span></span>|<span data-ttu-id="829e6-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="829e6-144">String</span></span>|<span data-ttu-id="829e6-145">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="829e6-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="829e6-146">タイトル</span><span class="sxs-lookup"><span data-stu-id="829e6-146">title</span></span>|<span data-ttu-id="829e6-147">String</span><span class="sxs-lookup"><span data-stu-id="829e6-147">String</span></span>|<span data-ttu-id="829e6-148">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="829e6-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="829e6-149">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="829e6-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="829e6-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="829e6-150">bodyText</span></span>|<span data-ttu-id="829e6-151">String</span><span class="sxs-lookup"><span data-stu-id="829e6-151">String</span></span>|<span data-ttu-id="829e6-152">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="829e6-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="829e6-153">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="829e6-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="829e6-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="829e6-154">acceptanceStatement</span></span>|<span data-ttu-id="829e6-155">String</span><span class="sxs-lookup"><span data-stu-id="829e6-155">String</span></span>|<span data-ttu-id="829e6-156">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="829e6-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="829e6-157">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="829e6-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="829e6-158">version</span><span class="sxs-lookup"><span data-stu-id="829e6-158">version</span></span>|<span data-ttu-id="829e6-159">Int32</span><span class="sxs-lookup"><span data-stu-id="829e6-159">Int32</span></span>|<span data-ttu-id="829e6-160">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="829e6-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="829e6-161">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="829e6-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="829e6-162">応答</span><span class="sxs-lookup"><span data-stu-id="829e6-162">Response</span></span>
<span data-ttu-id="829e6-163">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="829e6-163">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="829e6-164">例</span><span class="sxs-lookup"><span data-stu-id="829e6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="829e6-165">要求</span><span class="sxs-lookup"><span data-stu-id="829e6-165">Request</span></span>
<span data-ttu-id="829e6-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="829e6-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="829e6-167">応答</span><span class="sxs-lookup"><span data-stu-id="829e6-167">Response</span></span>
<span data-ttu-id="829e6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="829e6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



