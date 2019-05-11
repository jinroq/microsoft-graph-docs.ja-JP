---
title: GroupPolicyPresentationDecimalTextBox の更新
description: GroupPolicyPresentationDecimalTextBox オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83ef5a7acfb16607719a5bc1a064d3f841c139a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904903"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="0074a-103">GroupPolicyPresentationDecimalTextBox の更新</span><span class="sxs-lookup"><span data-stu-id="0074a-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="0074a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0074a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0074a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0074a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0074a-106">[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0074a-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0074a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0074a-107">Prerequisites</span></span>
<span data-ttu-id="0074a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0074a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0074a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0074a-110">Permission type</span></span>|<span data-ttu-id="0074a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0074a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0074a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0074a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0074a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0074a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0074a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0074a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0074a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0074a-115">Not supported.</span></span>|
|<span data-ttu-id="0074a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0074a-116">Application</span></span>|<span data-ttu-id="0074a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0074a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0074a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0074a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="0074a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0074a-119">Request headers</span></span>
|<span data-ttu-id="0074a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0074a-120">Header</span></span>|<span data-ttu-id="0074a-121">値</span><span class="sxs-lookup"><span data-stu-id="0074a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0074a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0074a-122">Authorization</span></span>|<span data-ttu-id="0074a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0074a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0074a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0074a-124">Accept</span></span>|<span data-ttu-id="0074a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0074a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0074a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0074a-126">Request body</span></span>
<span data-ttu-id="0074a-127">要求本文で、 [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0074a-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="0074a-128">次の表に、 [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0074a-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="0074a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0074a-129">Property</span></span>|<span data-ttu-id="0074a-130">型</span><span class="sxs-lookup"><span data-stu-id="0074a-130">Type</span></span>|<span data-ttu-id="0074a-131">説明</span><span class="sxs-lookup"><span data-stu-id="0074a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0074a-132">label</span><span class="sxs-lookup"><span data-stu-id="0074a-132">label</span></span>|<span data-ttu-id="0074a-133">String</span><span class="sxs-lookup"><span data-stu-id="0074a-133">String</span></span>|<span data-ttu-id="0074a-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="0074a-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0074a-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="0074a-135">The default value is empty.</span></span> <span data-ttu-id="0074a-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0074a-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0074a-137">id</span><span class="sxs-lookup"><span data-stu-id="0074a-137">id</span></span>|<span data-ttu-id="0074a-138">String</span><span class="sxs-lookup"><span data-stu-id="0074a-138">String</span></span>|<span data-ttu-id="0074a-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0074a-139">Key of the entity.</span></span> <span data-ttu-id="0074a-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0074a-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0074a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0074a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0074a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0074a-142">DateTimeOffset</span></span>|<span data-ttu-id="0074a-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="0074a-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="0074a-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0074a-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0074a-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0074a-145">defaultValue</span></span>|<span data-ttu-id="0074a-146">Int64</span><span class="sxs-lookup"><span data-stu-id="0074a-146">Int64</span></span>|<span data-ttu-id="0074a-147">小数点のテキストボックスの初期値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="0074a-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="0074a-148">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="0074a-148">The default value is 1.</span></span>|
|<span data-ttu-id="0074a-149">スピン</span><span class="sxs-lookup"><span data-stu-id="0074a-149">spin</span></span>|<span data-ttu-id="0074a-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="0074a-150">Boolean</span></span>|<span data-ttu-id="0074a-151">True の場合はスピンコントロールを作成します。それ以外の場合は、数値を入力するためのテキストボックスを作成します。</span><span class="sxs-lookup"><span data-stu-id="0074a-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="0074a-152">既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="0074a-152">The default value is true.</span></span>|
|<span data-ttu-id="0074a-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="0074a-153">spinStep</span></span>|<span data-ttu-id="0074a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="0074a-154">Int64</span></span>|<span data-ttu-id="0074a-155">スピンコントロールの変更のインクリメントを指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="0074a-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="0074a-156">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="0074a-156">The default value is 1.</span></span>|
|<span data-ttu-id="0074a-157">必須</span><span class="sxs-lookup"><span data-stu-id="0074a-157">required</span></span>|<span data-ttu-id="0074a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0074a-158">Boolean</span></span>|<span data-ttu-id="0074a-159">[パラメーター] ボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0074a-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="0074a-160">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="0074a-160">The default value is false.</span></span>|
|<span data-ttu-id="0074a-161">minValue</span><span class="sxs-lookup"><span data-stu-id="0074a-161">minValue</span></span>|<span data-ttu-id="0074a-162">Int64</span><span class="sxs-lookup"><span data-stu-id="0074a-162">Int64</span></span>|<span data-ttu-id="0074a-163">最小許容値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="0074a-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="0074a-164">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="0074a-164">The default value is 0.</span></span>|
|<span data-ttu-id="0074a-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="0074a-165">maxValue</span></span>|<span data-ttu-id="0074a-166">Int64</span><span class="sxs-lookup"><span data-stu-id="0074a-166">Int64</span></span>|<span data-ttu-id="0074a-167">最大許容値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="0074a-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="0074a-168">既定値は9999です。</span><span class="sxs-lookup"><span data-stu-id="0074a-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="0074a-169">応答</span><span class="sxs-lookup"><span data-stu-id="0074a-169">Response</span></span>
<span data-ttu-id="0074a-170">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0074a-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0074a-171">例</span><span class="sxs-lookup"><span data-stu-id="0074a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="0074a-172">要求</span><span class="sxs-lookup"><span data-stu-id="0074a-172">Request</span></span>
<span data-ttu-id="0074a-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0074a-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="0074a-174">応答</span><span class="sxs-lookup"><span data-stu-id="0074a-174">Response</span></span>
<span data-ttu-id="0074a-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0074a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




