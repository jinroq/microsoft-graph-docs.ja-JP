---
title: Update termsAndConditions
description: termsAndConditions オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3eca58812eb4032113e968ad054a7a11bf110b81
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409490"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="4cfa2-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4cfa2-103">Update termsAndConditions</span></span>

> <span data-ttu-id="4cfa2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4cfa2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cfa2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfa2-107">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cfa2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4cfa2-108">Prerequisites</span></span>
<span data-ttu-id="4cfa2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4cfa2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4cfa2-111">Permission type</span></span>|<span data-ttu-id="4cfa2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4cfa2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cfa2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4cfa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cfa2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfa2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4cfa2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4cfa2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cfa2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-116">Not supported.</span></span>|
|<span data-ttu-id="4cfa2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4cfa2-117">Application</span></span>|<span data-ttu-id="4cfa2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cfa2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4cfa2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="4cfa2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cfa2-120">Request headers</span></span>
|<span data-ttu-id="4cfa2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cfa2-121">Header</span></span>|<span data-ttu-id="4cfa2-122">値</span><span class="sxs-lookup"><span data-stu-id="4cfa2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cfa2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cfa2-123">Authorization</span></span>|<span data-ttu-id="4cfa2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cfa2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cfa2-125">Accept</span></span>|<span data-ttu-id="4cfa2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cfa2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cfa2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4cfa2-127">Request body</span></span>
<span data-ttu-id="4cfa2-128">要求本文で、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="4cfa2-129">次の表に、[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="4cfa2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cfa2-130">Property</span></span>|<span data-ttu-id="4cfa2-131">型</span><span class="sxs-lookup"><span data-stu-id="4cfa2-131">Type</span></span>|<span data-ttu-id="4cfa2-132">説明</span><span class="sxs-lookup"><span data-stu-id="4cfa2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cfa2-133">id</span><span class="sxs-lookup"><span data-stu-id="4cfa2-133">id</span></span>|<span data-ttu-id="4cfa2-134">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-134">String</span></span>|<span data-ttu-id="4cfa2-135">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="4cfa2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cfa2-136">createdDateTime</span></span>|<span data-ttu-id="4cfa2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cfa2-137">DateTimeOffset</span></span>|<span data-ttu-id="4cfa2-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="4cfa2-139">変更された日時</span><span class="sxs-lookup"><span data-stu-id="4cfa2-139">modifiedDateTime</span></span>|<span data-ttu-id="4cfa2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cfa2-140">DateTimeOffset</span></span>|<span data-ttu-id="4cfa2-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4cfa2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cfa2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="4cfa2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cfa2-143">DateTimeOffset</span></span>|<span data-ttu-id="4cfa2-144">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4cfa2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4cfa2-145">displayName</span></span>|<span data-ttu-id="4cfa2-146">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-146">String</span></span>|<span data-ttu-id="4cfa2-147">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="4cfa2-148">説明</span><span class="sxs-lookup"><span data-stu-id="4cfa2-148">description</span></span>|<span data-ttu-id="4cfa2-149">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-149">String</span></span>|<span data-ttu-id="4cfa2-150">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="4cfa2-151">タイトル</span><span class="sxs-lookup"><span data-stu-id="4cfa2-151">title</span></span>|<span data-ttu-id="4cfa2-152">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-152">String</span></span>|<span data-ttu-id="4cfa2-153">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="4cfa2-154">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4cfa2-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="4cfa2-155">bodyText</span></span>|<span data-ttu-id="4cfa2-156">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-156">String</span></span>|<span data-ttu-id="4cfa2-157">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="4cfa2-158">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4cfa2-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="4cfa2-159">acceptanceStatement</span></span>|<span data-ttu-id="4cfa2-160">String</span><span class="sxs-lookup"><span data-stu-id="4cfa2-160">String</span></span>|<span data-ttu-id="4cfa2-161">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="4cfa2-162">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4cfa2-163">version</span><span class="sxs-lookup"><span data-stu-id="4cfa2-163">version</span></span>|<span data-ttu-id="4cfa2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfa2-164">Int32</span></span>|<span data-ttu-id="4cfa2-165">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="4cfa2-166">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4cfa2-167">応答</span><span class="sxs-lookup"><span data-stu-id="4cfa2-167">Response</span></span>
<span data-ttu-id="4cfa2-168">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-168">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cfa2-169">例</span><span class="sxs-lookup"><span data-stu-id="4cfa2-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cfa2-170">要求</span><span class="sxs-lookup"><span data-stu-id="4cfa2-170">Request</span></span>
<span data-ttu-id="4cfa2-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cfa2-172">応答</span><span class="sxs-lookup"><span data-stu-id="4cfa2-172">Response</span></span>
<span data-ttu-id="4cfa2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4cfa2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




