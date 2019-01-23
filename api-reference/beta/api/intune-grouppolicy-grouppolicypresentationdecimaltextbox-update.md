---
title: GroupPolicyPresentationDecimalTextBox を更新します。
description: GroupPolicyPresentationDecimalTextBox オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4f91abc80fe37fe3f3677afc7d06b547df9bee4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430318"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="df706-103">GroupPolicyPresentationDecimalTextBox を更新します。</span><span class="sxs-lookup"><span data-stu-id="df706-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="df706-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df706-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df706-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df706-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df706-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df706-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df706-107">[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="df706-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df706-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="df706-108">Prerequisites</span></span>
<span data-ttu-id="df706-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df706-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df706-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df706-111">Permission type</span></span>|<span data-ttu-id="df706-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df706-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df706-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df706-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df706-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df706-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df706-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df706-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df706-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df706-116">Not supported.</span></span>|
|<span data-ttu-id="df706-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df706-117">Application</span></span>|<span data-ttu-id="df706-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df706-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df706-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df706-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="df706-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df706-120">Request headers</span></span>
|<span data-ttu-id="df706-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df706-121">Header</span></span>|<span data-ttu-id="df706-122">値</span><span class="sxs-lookup"><span data-stu-id="df706-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df706-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df706-123">Authorization</span></span>|<span data-ttu-id="df706-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="df706-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df706-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df706-125">Accept</span></span>|<span data-ttu-id="df706-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df706-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df706-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="df706-127">Request body</span></span>
<span data-ttu-id="df706-128">要求の本文に[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="df706-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="df706-129">[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="df706-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="df706-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df706-130">Property</span></span>|<span data-ttu-id="df706-131">型</span><span class="sxs-lookup"><span data-stu-id="df706-131">Type</span></span>|<span data-ttu-id="df706-132">説明</span><span class="sxs-lookup"><span data-stu-id="df706-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df706-133">label</span><span class="sxs-lookup"><span data-stu-id="df706-133">label</span></span>|<span data-ttu-id="df706-134">String</span><span class="sxs-lookup"><span data-stu-id="df706-134">String</span></span>|<span data-ttu-id="df706-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="df706-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="df706-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="df706-136">The default value is empty.</span></span> <span data-ttu-id="df706-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="df706-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df706-138">id</span><span class="sxs-lookup"><span data-stu-id="df706-138">id</span></span>|<span data-ttu-id="df706-139">String</span><span class="sxs-lookup"><span data-stu-id="df706-139">String</span></span>|<span data-ttu-id="df706-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="df706-140">Key of the entity.</span></span> <span data-ttu-id="df706-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="df706-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df706-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df706-142">lastModifiedDateTime</span></span>|<span data-ttu-id="df706-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df706-143">DateTimeOffset</span></span>|<span data-ttu-id="df706-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="df706-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="df706-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="df706-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="df706-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="df706-146">defaultValue</span></span>|<span data-ttu-id="df706-147">Int64</span><span class="sxs-lookup"><span data-stu-id="df706-147">Int64</span></span>|<span data-ttu-id="df706-148">符号なし整数を 10 進数のテキスト ボックスの初期値を指定します。</span><span class="sxs-lookup"><span data-stu-id="df706-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="df706-149">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="df706-149">The default value is 1.</span></span>|
|<span data-ttu-id="df706-150">スピン</span><span class="sxs-lookup"><span data-stu-id="df706-150">spin</span></span>|<span data-ttu-id="df706-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="df706-151">Boolean</span></span>|<span data-ttu-id="df706-152">True の場合、スピン コントロールを作成します。それ以外の場合、数値入力用のテキスト ボックスを作成します。</span><span class="sxs-lookup"><span data-stu-id="df706-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="df706-153">既定値は、true を指定します。</span><span class="sxs-lookup"><span data-stu-id="df706-153">The default value is true.</span></span>|
|<span data-ttu-id="df706-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="df706-154">spinStep</span></span>|<span data-ttu-id="df706-155">Int64</span><span class="sxs-lookup"><span data-stu-id="df706-155">Int64</span></span>|<span data-ttu-id="df706-156">スピン コントロールの変更の増分値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="df706-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="df706-157">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="df706-157">The default value is 1.</span></span>|
|<span data-ttu-id="df706-158">必須</span><span class="sxs-lookup"><span data-stu-id="df706-158">required</span></span>|<span data-ttu-id="df706-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="df706-159">Boolean</span></span>|<span data-ttu-id="df706-160">パラメーター] ボックスに値を入力するための要件です。</span><span class="sxs-lookup"><span data-stu-id="df706-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="df706-161">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="df706-161">The default value is false.</span></span>|
|<span data-ttu-id="df706-162">minValue</span><span class="sxs-lookup"><span data-stu-id="df706-162">minValue</span></span>|<span data-ttu-id="df706-163">Int64</span><span class="sxs-lookup"><span data-stu-id="df706-163">Int64</span></span>|<span data-ttu-id="df706-164">指定できる最小の値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="df706-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="df706-165">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="df706-165">The default value is 0.</span></span>|
|<span data-ttu-id="df706-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="df706-166">maxValue</span></span>|<span data-ttu-id="df706-167">Int64</span><span class="sxs-lookup"><span data-stu-id="df706-167">Int64</span></span>|<span data-ttu-id="df706-168">最大許容値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="df706-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="df706-169">既定値は、9999 です。</span><span class="sxs-lookup"><span data-stu-id="df706-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="df706-170">応答</span><span class="sxs-lookup"><span data-stu-id="df706-170">Response</span></span>
<span data-ttu-id="df706-171">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="df706-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df706-172">例</span><span class="sxs-lookup"><span data-stu-id="df706-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="df706-173">要求</span><span class="sxs-lookup"><span data-stu-id="df706-173">Request</span></span>
<span data-ttu-id="df706-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df706-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df706-175">応答</span><span class="sxs-lookup"><span data-stu-id="df706-175">Response</span></span>
<span data-ttu-id="df706-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df706-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




