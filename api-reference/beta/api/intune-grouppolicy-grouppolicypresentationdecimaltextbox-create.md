---
title: GroupPolicyPresentationDecimalTextBox を作成する
description: 新しい groupPolicyPresentationDecimalTextBox オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88cf550c335ad690518be1cb4a112688e921a3d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357867"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="d51d4-103">GroupPolicyPresentationDecimalTextBox を作成する</span><span class="sxs-lookup"><span data-stu-id="d51d4-103">Create groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="d51d4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d51d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d51d4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d51d4-106">新しい[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-106">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d51d4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d51d4-107">Prerequisites</span></span>
<span data-ttu-id="d51d4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d51d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d51d4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d51d4-110">Permission type</span></span>|<span data-ttu-id="d51d4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d51d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d51d4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d51d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d51d4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d51d4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d51d4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d51d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d51d4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d51d4-115">Not supported.</span></span>|
|<span data-ttu-id="d51d4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d51d4-116">Application</span></span>|<span data-ttu-id="d51d4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d51d4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d51d4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d51d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="d51d4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d51d4-119">Request headers</span></span>
|<span data-ttu-id="d51d4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d51d4-120">Header</span></span>|<span data-ttu-id="d51d4-121">値</span><span class="sxs-lookup"><span data-stu-id="d51d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d51d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d51d4-122">Authorization</span></span>|<span data-ttu-id="d51d4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d51d4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d51d4-124">Accept</span></span>|<span data-ttu-id="d51d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d51d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d51d4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d51d4-126">Request body</span></span>
<span data-ttu-id="d51d4-127">要求本文で、groupPolicyPresentationDecimalTextBox オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-127">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="d51d4-128">次の表に、groupPolicyPresentationDecimalTextBox の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-128">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="d51d4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d51d4-129">Property</span></span>|<span data-ttu-id="d51d4-130">型</span><span class="sxs-lookup"><span data-stu-id="d51d4-130">Type</span></span>|<span data-ttu-id="d51d4-131">説明</span><span class="sxs-lookup"><span data-stu-id="d51d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d51d4-132">label</span><span class="sxs-lookup"><span data-stu-id="d51d4-132">label</span></span>|<span data-ttu-id="d51d4-133">String</span><span class="sxs-lookup"><span data-stu-id="d51d4-133">String</span></span>|<span data-ttu-id="d51d4-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="d51d4-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d51d4-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-135">The default value is empty.</span></span> <span data-ttu-id="d51d4-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d51d4-137">id</span><span class="sxs-lookup"><span data-stu-id="d51d4-137">id</span></span>|<span data-ttu-id="d51d4-138">String</span><span class="sxs-lookup"><span data-stu-id="d51d4-138">String</span></span>|<span data-ttu-id="d51d4-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d51d4-139">Key of the entity.</span></span> <span data-ttu-id="d51d4-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d51d4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d51d4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d51d4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d51d4-142">DateTimeOffset</span></span>|<span data-ttu-id="d51d4-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="d51d4-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="d51d4-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d51d4-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="d51d4-145">defaultValue</span></span>|<span data-ttu-id="d51d4-146">Int64</span><span class="sxs-lookup"><span data-stu-id="d51d4-146">Int64</span></span>|<span data-ttu-id="d51d4-147">小数点のテキストボックスの初期値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="d51d4-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="d51d4-148">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-148">The default value is 1.</span></span>|
|<span data-ttu-id="d51d4-149">スピン</span><span class="sxs-lookup"><span data-stu-id="d51d4-149">spin</span></span>|<span data-ttu-id="d51d4-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d51d4-150">Boolean</span></span>|<span data-ttu-id="d51d4-151">True の場合はスピンコントロールを作成します。それ以外の場合は、数値を入力するためのテキストボックスを作成します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="d51d4-152">既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-152">The default value is true.</span></span>|
|<span data-ttu-id="d51d4-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="d51d4-153">spinStep</span></span>|<span data-ttu-id="d51d4-154">Int64</span><span class="sxs-lookup"><span data-stu-id="d51d4-154">Int64</span></span>|<span data-ttu-id="d51d4-155">スピンコントロールの変更のインクリメントを指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="d51d4-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="d51d4-156">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-156">The default value is 1.</span></span>|
|<span data-ttu-id="d51d4-157">必須</span><span class="sxs-lookup"><span data-stu-id="d51d4-157">required</span></span>|<span data-ttu-id="d51d4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d51d4-158">Boolean</span></span>|<span data-ttu-id="d51d4-159">[パラメーター] ボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d51d4-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="d51d4-160">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-160">The default value is false.</span></span>|
|<span data-ttu-id="d51d4-161">minValue</span><span class="sxs-lookup"><span data-stu-id="d51d4-161">minValue</span></span>|<span data-ttu-id="d51d4-162">Int64</span><span class="sxs-lookup"><span data-stu-id="d51d4-162">Int64</span></span>|<span data-ttu-id="d51d4-163">最小許容値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="d51d4-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="d51d4-164">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-164">The default value is 0.</span></span>|
|<span data-ttu-id="d51d4-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="d51d4-165">maxValue</span></span>|<span data-ttu-id="d51d4-166">Int64</span><span class="sxs-lookup"><span data-stu-id="d51d4-166">Int64</span></span>|<span data-ttu-id="d51d4-167">最大許容値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="d51d4-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="d51d4-168">既定値は9999です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="d51d4-169">応答</span><span class="sxs-lookup"><span data-stu-id="d51d4-169">Response</span></span>
<span data-ttu-id="d51d4-170">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d51d4-170">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d51d4-171">例</span><span class="sxs-lookup"><span data-stu-id="d51d4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d51d4-172">要求</span><span class="sxs-lookup"><span data-stu-id="d51d4-172">Request</span></span>
<span data-ttu-id="d51d4-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d51d4-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="d51d4-174">応答</span><span class="sxs-lookup"><span data-stu-id="d51d4-174">Response</span></span>
<span data-ttu-id="d51d4-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d51d4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```






