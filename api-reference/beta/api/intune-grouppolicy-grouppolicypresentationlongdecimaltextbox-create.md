---
title: GroupPolicyPresentationLongDecimalTextBox を作成します。
description: 新しい groupPolicyPresentationLongDecimalTextBox オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1fd47d422358dd0cd4a23ff35137654787498bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430344"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="0f89b-103">GroupPolicyPresentationLongDecimalTextBox を作成します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="0f89b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f89b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f89b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f89b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f89b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f89b-107">新しい[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f89b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f89b-108">Prerequisites</span></span>
<span data-ttu-id="0f89b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f89b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f89b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f89b-111">Permission type</span></span>|<span data-ttu-id="0f89b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f89b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f89b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f89b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f89b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f89b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0f89b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f89b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f89b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f89b-116">Not supported.</span></span>|
|<span data-ttu-id="0f89b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f89b-117">Application</span></span>|<span data-ttu-id="0f89b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f89b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f89b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f89b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0f89b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f89b-120">Request headers</span></span>
|<span data-ttu-id="0f89b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f89b-121">Header</span></span>|<span data-ttu-id="0f89b-122">値</span><span class="sxs-lookup"><span data-stu-id="0f89b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f89b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f89b-123">Authorization</span></span>|<span data-ttu-id="0f89b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0f89b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f89b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f89b-125">Accept</span></span>|<span data-ttu-id="0f89b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f89b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f89b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f89b-127">Request body</span></span>
<span data-ttu-id="0f89b-128">要求の本文に groupPolicyPresentationLongDecimalTextBox オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="0f89b-129">次の表は、groupPolicyPresentationLongDecimalTextBox を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="0f89b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f89b-130">Property</span></span>|<span data-ttu-id="0f89b-131">型</span><span class="sxs-lookup"><span data-stu-id="0f89b-131">Type</span></span>|<span data-ttu-id="0f89b-132">説明</span><span class="sxs-lookup"><span data-stu-id="0f89b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f89b-133">label</span><span class="sxs-lookup"><span data-stu-id="0f89b-133">label</span></span>|<span data-ttu-id="0f89b-134">String</span><span class="sxs-lookup"><span data-stu-id="0f89b-134">String</span></span>|<span data-ttu-id="0f89b-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="0f89b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0f89b-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-136">The default value is empty.</span></span> <span data-ttu-id="0f89b-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0f89b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f89b-138">id</span><span class="sxs-lookup"><span data-stu-id="0f89b-138">id</span></span>|<span data-ttu-id="0f89b-139">String</span><span class="sxs-lookup"><span data-stu-id="0f89b-139">String</span></span>|<span data-ttu-id="0f89b-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f89b-140">Key of the entity.</span></span> <span data-ttu-id="0f89b-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0f89b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f89b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f89b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="0f89b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f89b-143">DateTimeOffset</span></span>|<span data-ttu-id="0f89b-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="0f89b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="0f89b-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0f89b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f89b-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0f89b-146">defaultValue</span></span>|<span data-ttu-id="0f89b-147">Int64</span><span class="sxs-lookup"><span data-stu-id="0f89b-147">Int64</span></span>|<span data-ttu-id="0f89b-148">符号なし整数を 10 進数のテキスト ボックスの初期値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="0f89b-149">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-149">The default value is 1.</span></span>|
|<span data-ttu-id="0f89b-150">スピン</span><span class="sxs-lookup"><span data-stu-id="0f89b-150">spin</span></span>|<span data-ttu-id="0f89b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f89b-151">Boolean</span></span>|<span data-ttu-id="0f89b-152">True の場合、スピン コントロールを作成します。それ以外の場合、数値入力用のテキスト ボックスを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="0f89b-153">既定値は、true を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-153">The default value is true.</span></span>|
|<span data-ttu-id="0f89b-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="0f89b-154">spinStep</span></span>|<span data-ttu-id="0f89b-155">Int64</span><span class="sxs-lookup"><span data-stu-id="0f89b-155">Int64</span></span>|<span data-ttu-id="0f89b-156">スピン コントロールの変更の増分値を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="0f89b-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="0f89b-157">既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-157">The default value is 1.</span></span>|
|<span data-ttu-id="0f89b-158">必須</span><span class="sxs-lookup"><span data-stu-id="0f89b-158">required</span></span>|<span data-ttu-id="0f89b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f89b-159">Boolean</span></span>|<span data-ttu-id="0f89b-160">パラメーター] ボックスに値を入力するための要件です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="0f89b-161">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f89b-161">The default value is false.</span></span>|
|<span data-ttu-id="0f89b-162">minValue</span><span class="sxs-lookup"><span data-stu-id="0f89b-162">minValue</span></span>|<span data-ttu-id="0f89b-163">Int64</span><span class="sxs-lookup"><span data-stu-id="0f89b-163">Int64</span></span>|<span data-ttu-id="0f89b-164">符号なし、許容される最小値を指定する long です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="0f89b-165">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-165">The default value is 0.</span></span>|
|<span data-ttu-id="0f89b-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="0f89b-166">maxValue</span></span>|<span data-ttu-id="0f89b-167">Int64</span><span class="sxs-lookup"><span data-stu-id="0f89b-167">Int64</span></span>|<span data-ttu-id="0f89b-168">符号なしの値の許容最大値を指定する long です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="0f89b-169">既定値は、9999 です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="0f89b-170">応答</span><span class="sxs-lookup"><span data-stu-id="0f89b-170">Response</span></span>
<span data-ttu-id="0f89b-171">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0f89b-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f89b-172">例</span><span class="sxs-lookup"><span data-stu-id="0f89b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f89b-173">要求</span><span class="sxs-lookup"><span data-stu-id="0f89b-173">Request</span></span>
<span data-ttu-id="0f89b-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f89b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="0f89b-175">応答</span><span class="sxs-lookup"><span data-stu-id="0f89b-175">Response</span></span>
<span data-ttu-id="0f89b-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f89b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




