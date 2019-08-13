---
title: Update termsAndConditions
description: termsAndConditions オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21cb17ff4787eeb5a52d3cfdd509e5c2ad5a5c82
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328173"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="d6630-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d6630-103">Update termsAndConditions</span></span>

> <span data-ttu-id="d6630-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6630-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6630-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6630-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6630-106">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6630-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6630-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6630-107">Prerequisites</span></span>
<span data-ttu-id="d6630-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6630-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6630-110">Permission type</span></span>|<span data-ttu-id="d6630-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6630-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6630-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6630-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6630-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6630-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6630-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6630-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6630-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6630-115">Not supported.</span></span>|
|<span data-ttu-id="d6630-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6630-116">Application</span></span>|<span data-ttu-id="d6630-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6630-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6630-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6630-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="d6630-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6630-119">Request headers</span></span>
|<span data-ttu-id="d6630-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6630-120">Header</span></span>|<span data-ttu-id="d6630-121">値</span><span class="sxs-lookup"><span data-stu-id="d6630-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6630-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6630-122">Authorization</span></span>|<span data-ttu-id="d6630-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6630-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6630-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d6630-124">Accept</span></span>|<span data-ttu-id="d6630-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6630-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6630-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6630-126">Request body</span></span>
<span data-ttu-id="d6630-127">要求本文で、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6630-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="d6630-128">次の表に、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d6630-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="d6630-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6630-129">Property</span></span>|<span data-ttu-id="d6630-130">型</span><span class="sxs-lookup"><span data-stu-id="d6630-130">Type</span></span>|<span data-ttu-id="d6630-131">説明</span><span class="sxs-lookup"><span data-stu-id="d6630-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6630-132">id</span><span class="sxs-lookup"><span data-stu-id="d6630-132">id</span></span>|<span data-ttu-id="d6630-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d6630-133">String</span></span>|<span data-ttu-id="d6630-134">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d6630-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="d6630-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6630-135">createdDateTime</span></span>|<span data-ttu-id="d6630-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6630-136">DateTimeOffset</span></span>|<span data-ttu-id="d6630-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6630-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="d6630-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6630-138">modifiedDateTime</span></span>|<span data-ttu-id="d6630-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6630-139">DateTimeOffset</span></span>|<span data-ttu-id="d6630-140">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6630-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d6630-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6630-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d6630-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6630-142">DateTimeOffset</span></span>|<span data-ttu-id="d6630-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6630-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d6630-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d6630-144">displayName</span></span>|<span data-ttu-id="d6630-145">文字列</span><span class="sxs-lookup"><span data-stu-id="d6630-145">String</span></span>|<span data-ttu-id="d6630-146">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="d6630-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="d6630-147">description</span><span class="sxs-lookup"><span data-stu-id="d6630-147">description</span></span>|<span data-ttu-id="d6630-148">String</span><span class="sxs-lookup"><span data-stu-id="d6630-148">String</span></span>|<span data-ttu-id="d6630-149">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="d6630-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="d6630-150">title</span><span class="sxs-lookup"><span data-stu-id="d6630-150">title</span></span>|<span data-ttu-id="d6630-151">String</span><span class="sxs-lookup"><span data-stu-id="d6630-151">String</span></span>|<span data-ttu-id="d6630-152">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="d6630-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="d6630-153">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d6630-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="d6630-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="d6630-154">bodyText</span></span>|<span data-ttu-id="d6630-155">String</span><span class="sxs-lookup"><span data-stu-id="d6630-155">String</span></span>|<span data-ttu-id="d6630-156">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="d6630-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="d6630-157">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d6630-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="d6630-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="d6630-158">acceptanceStatement</span></span>|<span data-ttu-id="d6630-159">String</span><span class="sxs-lookup"><span data-stu-id="d6630-159">String</span></span>|<span data-ttu-id="d6630-160">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="d6630-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="d6630-161">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d6630-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="d6630-162">version</span><span class="sxs-lookup"><span data-stu-id="d6630-162">version</span></span>|<span data-ttu-id="d6630-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d6630-163">Int32</span></span>|<span data-ttu-id="d6630-164">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="d6630-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="d6630-165">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="d6630-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d6630-166">応答</span><span class="sxs-lookup"><span data-stu-id="d6630-166">Response</span></span>
<span data-ttu-id="d6630-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d6630-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6630-168">例</span><span class="sxs-lookup"><span data-stu-id="d6630-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6630-169">要求</span><span class="sxs-lookup"><span data-stu-id="d6630-169">Request</span></span>
<span data-ttu-id="d6630-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6630-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6630-171">応答</span><span class="sxs-lookup"><span data-stu-id="d6630-171">Response</span></span>
<span data-ttu-id="d6630-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6630-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






