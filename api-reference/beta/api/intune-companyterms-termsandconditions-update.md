---
title: Update termsAndConditions
description: termsAndConditions オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5d7f951aefe0124d0576277587ddcf48dbb0fd5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933880"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="3c380-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3c380-103">Update termsAndConditions</span></span>

> <span data-ttu-id="3c380-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c380-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c380-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c380-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c380-106">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3c380-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c380-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c380-107">Prerequisites</span></span>
<span data-ttu-id="3c380-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c380-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c380-110">Permission type</span></span>|<span data-ttu-id="3c380-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c380-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c380-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c380-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c380-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c380-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3c380-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c380-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c380-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c380-115">Not supported.</span></span>|
|<span data-ttu-id="3c380-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c380-116">Application</span></span>|<span data-ttu-id="3c380-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c380-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c380-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c380-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="3c380-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c380-119">Request headers</span></span>
|<span data-ttu-id="3c380-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c380-120">Header</span></span>|<span data-ttu-id="3c380-121">値</span><span class="sxs-lookup"><span data-stu-id="3c380-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c380-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c380-122">Authorization</span></span>|<span data-ttu-id="3c380-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c380-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c380-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3c380-124">Accept</span></span>|<span data-ttu-id="3c380-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c380-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c380-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c380-126">Request body</span></span>
<span data-ttu-id="3c380-127">要求本文で、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c380-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="3c380-128">次の表に、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3c380-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="3c380-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c380-129">Property</span></span>|<span data-ttu-id="3c380-130">型</span><span class="sxs-lookup"><span data-stu-id="3c380-130">Type</span></span>|<span data-ttu-id="3c380-131">説明</span><span class="sxs-lookup"><span data-stu-id="3c380-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c380-132">id</span><span class="sxs-lookup"><span data-stu-id="3c380-132">id</span></span>|<span data-ttu-id="3c380-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3c380-133">String</span></span>|<span data-ttu-id="3c380-134">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3c380-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="3c380-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c380-135">createdDateTime</span></span>|<span data-ttu-id="3c380-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c380-136">DateTimeOffset</span></span>|<span data-ttu-id="3c380-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3c380-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="3c380-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c380-138">modifiedDateTime</span></span>|<span data-ttu-id="3c380-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c380-139">DateTimeOffset</span></span>|<span data-ttu-id="3c380-140">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3c380-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3c380-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c380-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3c380-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c380-142">DateTimeOffset</span></span>|<span data-ttu-id="3c380-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3c380-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3c380-144">displayName</span><span class="sxs-lookup"><span data-stu-id="3c380-144">displayName</span></span>|<span data-ttu-id="3c380-145">文字列</span><span class="sxs-lookup"><span data-stu-id="3c380-145">String</span></span>|<span data-ttu-id="3c380-146">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="3c380-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="3c380-147">description</span><span class="sxs-lookup"><span data-stu-id="3c380-147">description</span></span>|<span data-ttu-id="3c380-148">String</span><span class="sxs-lookup"><span data-stu-id="3c380-148">String</span></span>|<span data-ttu-id="3c380-149">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="3c380-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="3c380-150">title</span><span class="sxs-lookup"><span data-stu-id="3c380-150">title</span></span>|<span data-ttu-id="3c380-151">String</span><span class="sxs-lookup"><span data-stu-id="3c380-151">String</span></span>|<span data-ttu-id="3c380-152">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="3c380-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="3c380-153">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3c380-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3c380-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="3c380-154">bodyText</span></span>|<span data-ttu-id="3c380-155">String</span><span class="sxs-lookup"><span data-stu-id="3c380-155">String</span></span>|<span data-ttu-id="3c380-156">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="3c380-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="3c380-157">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3c380-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3c380-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="3c380-158">acceptanceStatement</span></span>|<span data-ttu-id="3c380-159">String</span><span class="sxs-lookup"><span data-stu-id="3c380-159">String</span></span>|<span data-ttu-id="3c380-160">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="3c380-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="3c380-161">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3c380-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3c380-162">version</span><span class="sxs-lookup"><span data-stu-id="3c380-162">version</span></span>|<span data-ttu-id="3c380-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3c380-163">Int32</span></span>|<span data-ttu-id="3c380-164">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="3c380-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="3c380-165">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="3c380-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3c380-166">応答</span><span class="sxs-lookup"><span data-stu-id="3c380-166">Response</span></span>
<span data-ttu-id="3c380-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3c380-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c380-168">例</span><span class="sxs-lookup"><span data-stu-id="3c380-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c380-169">要求</span><span class="sxs-lookup"><span data-stu-id="3c380-169">Request</span></span>
<span data-ttu-id="3c380-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c380-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="3c380-171">応答</span><span class="sxs-lookup"><span data-stu-id="3c380-171">Response</span></span>
<span data-ttu-id="3c380-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c380-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




